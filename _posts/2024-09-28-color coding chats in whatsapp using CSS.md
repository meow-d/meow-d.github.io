---
layout: post
tags: computers
---

whatsapp's organization features are so lackluster. well business accounts get to tag their chats, but the rest of us will have to stick to the communities feature, which is so bad that i don't know where to start. it's like a mix of discord and whatsapp with the worst of both worlds.

i found some third-party browser extensions, but none of them are available for firefox. i guess whatsapp is the most normie chat app and therefore you only need to support the most normie web browser.

my solution? a userstyle using [CSS attribute selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/Attribute_selectors), as all WhatsApp chat names have the title attribute for accessibility purposes.

```css
/* use = for exact match */
._ak8q span[title="study group"] {
    color: #56ff5c;
}

/* ^= start with */
._ak8q span[title^="[internal]"] {
    color: #ad35d6;
}
/* *= contains */
._ak8q span[title*="study"] {
    color: #ad35d6;
}
```
