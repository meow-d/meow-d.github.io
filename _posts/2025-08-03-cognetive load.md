---
title: Managing cognetive load
tags: productivity
---

I am currently not diagnosed with anything, but anyone can tell I'm not exactly neurotypical. I genuinely don't know if I have autism or ADHD or anything, but I know my problems.

I'm not sure if my brain is different, but I get tired extremely easily. And when I do, my brain gets too slow to think in real-time, working memory gets significantly nerfed (as in, ram, not hard disk). I start going on autopilot and follows my instincts without thinking, causing me to overexert myself and making me even more tired.

I'm like a computer swapping important stuff just to run a video game and freezing the DE, so that you can't even close your apps. When I'm tired, I skip things like showering and journaling to prioritize the task in front of me. It's like a carrot dangling in front of head it's just hours of shortsightedness thinking the problem will go away if I just try for 5 more minutes. In the worst-case scenario, I get to a point where I keep forgetting what I'm currently doing and start moving on to different tasks.

I think seeing the problem in the lens of cognitive load theory makes sense. It's literally an indispensable part of UI/UX - non-tech-literate people tend to be inefficient with computers due to a combination of unoptimized workflows and unfamiliarity. The version of me in extreme tiredness resembles these people with how messy my technology usage is. An UX designer's whole job is to optimize cognitive load across novice and experts.

Luckily I _am_ tech literate, I can always try making my workflows more optimized to manage my cognitive load. To varying degrees of success.

## what I've already been doing
- [the meow_d note-taking/PKMS setup™]({% link _posts/2025-08-03-note taking.md %})
- [File navigation using the command line]({% link _posts/2024-09-28-How I navigate my school documents.md %})

## evaluating my existing system
### let's automate more stuff!
I've decided everything needs to be even lower in overhead. I've created scripts and systemd timers for git sync, create daily note, create weekly notes, etc. eventually I plan to configured Neovim and VSCode to open up todo.md and the daily note on startup too.

### todo
One of the benefits of having a todo system is a backup of my working memory, as a sort of... second brain (heh). My brain will still be swapping, but it's kinda cached and therefore much faster... If that makes sense.

But none of that worked in practice because I am always too tired to bother. Don't get me wrong, not utilizing your second brain is fine to me, because I don't think religiously following methodologies is a good thing. I like listening to my own body and if I feel like I'm wasting my time I'll just stop bothering organizing my notes. However, this is a case where not following the methodology harmed me in the long run.

in a broader sense, I need a rule to prioritize self care over everything, avoid blindly following instincts[^1]. I need to internalize the fact that, if I have no energy for my PKM and self-care, I probably don't have the energy for other tasks and I'll be miserable, and I'll need to rest. I need to force myself to utilize the notes as an up-to-date backup of my working memory - what am I currently doing, the current list of tasks, etc.

[^1]: I think that's what mindfulness is about but I'm not sure. I need to look into what mindfulness actually is I feel like my idea is probably very far from the actual thing.

### multitasking
The opposite problem of me over-focusing. Multitasking is inefficient, full stop. It should be avoided at all costs.

I have apps and tabs open in the background so that I get to them later. This is a form of using my computer as working memory, but unfortunately they either always end up staying there for weeks, or get distracted by it.

I think it's better to close my tabs and put tasks in todo, or save in daily note, whenever possible. It gives the tasks more purpose and gives me a change to evaluate if I really want to do it.

### workspaces
Part of why I have so much trouble with distractions is my inconsistent use of workspaces. I _really really_ don't like using alt-tab. My browser is always on the first workspace - socials pinned, plus whatever I'm doing. My VSCode is always at the second workspace. When something gets too complex I move them out to a third or forth workspace. One task can span across 3 workspaces, with stuff like socials overlapping. Essentially my workspaces are consistent but a complete mess.

That's why, for the past weeks, I've been switching to Niri. It's a pretty unorthodox window manager that can only be described as a "scrolling window manager". I thought it will take me time to get used to it, but I got used to it immediately. It turns out it's exactly my dream DE, what I wanted GNOME to be.

Just by getting rid of alt tab, I was able to clean up my use of workspaces - first workspace acts for the pinned essential stuff, like journal, socials, and music; everything else afterward for each task. It sounds messy if you say it out loud but it makes complete sense to me. Did I mention I _really really_ don't like alt tab?

### mobile
And then there's also the lack of convenience on mobile. Typing on a phone is clunky, so is opening up Termux and doing git sync, so is using Obsidian. so... I'm gonna start using google keep for notes on the go, Obsidian when I do need to access stuff. I guess.

It's not ideal but you know what? Being a purist sucks, utilizing multiple tools when they are suitable is cool. You _can_ use separate specialized tools for bookmarks, todo's, journaling, etc. You don't have to integrate every tool to Obsidian, because Obsidian is only a second brain, not your actual brain!

---
