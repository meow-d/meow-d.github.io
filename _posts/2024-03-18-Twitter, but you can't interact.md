---
layout: post
author: meow_d
tags: computers
---

Twitter is terrifyingly addicting - it's super easy to click on the home page and get stuck in the algorithm for hours. An easy solution was to just not have an account, but thanks to Elon you need an account to see anything on the site. Nitter worked for while but was eventually shut down.

my solution? create an account, then use a css userstyle that prevents me from interacting with anything. it's like not having an account at all.

https://userstyles.world/style/15315/twitter-but-you-cant-interact

### limitations
you can still like posts with the keyboard shortcuts though. i don't think you can change that with css, but who knows. i haven't looked into it either.

### i'm actually much smarter about it this time
look at this:

<pre style="background-color:rgb(28, 29, 33);color:rgb(192, 197, 206);position:relative;padding:0;line-height:1.2rem;margin-bottom:0"><code style="padding:0 16px;display:block;margin-bottom:9px;margin-top:9px"><span style=""><span style="color: rgb(180, 94, 164)">div</span><span style="">[aria-label=&quot;Timeline: Your Home Timeline&quot;]</span> {...}</span></span></code></pre><div style="text-align: right; font-size: min(1.87vw, 70%); opacity: 0.7; margin-bottom: 1.7142857em;">made with @nex3's <a href="https://nex3.github.io/cohost-highlight">syntax highlighter</a></div>

i mean, sure, they might actually change the wording in the future, but it has consequences. they can always change the classes and break everything, but they can't just remove accessibility features... _or can they? at this point, i don't even know what elon is willing to do._

### alternatives
- if you don't care about viewing replies, you can use https://www.sotwe.com/. unlike nitter, it's a proprietary service that probably actually pays for the api.

- there are some Nitter instances out there that are still running and functional. (these use a huge number of actual accounts, so they're much riskier to run.)

---

[original post on cohost](https://cohost.org/meow-d/post/5143158-twitter-but-you-can/)
