---
title: How to get Bluetooth on virt-manager
tags: computers
---

There's no way to get Bluetooth without passing through your entire Bluetooth device on libvirt. You won't be able to use Bluetooth in your host and guest at the same time. If your device is responsible for both Bluetooth and Wifi, tough luck... maybe get a usb Bluetooth adapter?

## How
1. Open your VM > Show virtual hardware details > Add hardware
2. Find your Bluetooth device in either "USB Host Device" or "PCI Host Device". For example, mine is in USB Host Device, `003:019 Intel Corp. AX201 Bluetooth`
3. Profit

## Troubleshooting
It's supposed to work out of the box, but I had to do several extra steps.

- Driver installation. I got mine from [here](https://www.intel.com/content/www/us/en/products/sku/130293/intel-wifi-6-ax201-gig/downloads.html).

- Adding `<source guestReset='off'>`. Otherwise the driver won't load properly. For example, my XML becomes:

```xml
<hostdev mode="subsystem" type="usb" managed="yes">
  <source guestReset="off">
    <vendor id="0x8087"/>
    <product id="0x0026"/>
    <address bus="3" device="3"/>
  </source>
  <alias name="hostdev0"/>
  <address type="usb" bus="0" port="4"/>
</hostdev>
```

Note: XML editing is disabled by default. To enable, go to Menu bar > Edit > Preferences > Enable XML editing.

- Manually unbind device from driver. It's supposed to do this automatically tho?

```sh
# find usb device
lsusb | grep -i bluetooth
# Bus 003 Device 019: ID 8087:0026 Intel Corp. AX201 Bluetooth

# unbind
`echo -n '3-10:1.0' | sudo tee /sys/bus/usb/drivers/btusb/unbind`

# verify
lsusb -t

# if you suceed your device should look like this
#     |__ Port 010: Dev 019, If 0, Class=Wireless, Driver=[none], 12M
#     |__ Port 010: Dev 019, If 1, Class=Wireless, Driver=[none], 12M
```

- Remember to restart.

## resources
- https://github.com/virt-manager/virt-manager/issues/954
