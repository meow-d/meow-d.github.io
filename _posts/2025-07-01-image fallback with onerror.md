---
tags: site-meta computers
---

Have you ever wanted to hotlink an image but you're afraid if their site goes down? Just add a fallback with onerror!

```html
<img src="https://meow-d.github.io/assets/images/buttons/meow_d.webp" onerror="this.onerror=null; this.src=`/fallback.webp`;">
```

The onerror also overrides itself, so that when the fallback itself fails it doesn't get into an endless loop of replacing the fallback.

You could also use `<object>` for a javascript-free approach, but i don't want to overcomplicate things.
