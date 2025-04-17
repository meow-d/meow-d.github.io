---
tags: linux productivity
title: How I navigate my school documents using the command line (and why you might want to too)
---

## how?
### folder structure
obviously, i have a folder for each subject. these are grouped by semester and intake. pretty standard for anyone in uni.

folder names have to be in short form, for reasons i'll explain later.

```
├── school
│   ├── diploma
│   │   ├── 5
│   │   │   ├── DSF
│   │   │   │   ├── slides
│   │   │   │   ├── assignment
│   │   │   ├── IAI
│   │   │   ├── JP
│   │   │   └── SDP
│   ├── degree
│   │   ├── 2
```

### command line
since i use vscode to take notes, i can just use ctrl + \` to open up the built-in terminal. though i mostly prefer to open up a separate window.

install any of those "smarter cd" tools. this is why the folder names need to be short - to avoid ambiguity when it chooses a folder from your history. after installation, remember to cd to each of the folders once so that the it remembers them. personally, i use [zoxide](https://github.com/ajeetdsouza/zoxide), and alias/abbevrate it to `cd`.

lastly, make an alias/abbreviation for `xdg-open`. this command opens the file using the defaults application, identical to clicking on a file in your usual file manager. i personally made it an abbreviation and set it to `xo`

_for those who don't know, [abbreviation](https://fishshell.com/docs/current/cmds/abbr.html) is a feature in Fish. instead of replacing the command entirely like aliases, it replaces the abbreviation with the command once you press space. it's pretty much what aliases are meant to be._

## why do this?
here's how i used to open up lecture slides:
1. open up the file manager (with a shortcut)
2. use the trackpad to click "School" from the sidebar, because Dolphin doesn't allow you to navigate the sidebar with a keyboard
3. click the main ui to change the focus back to the files.
4. use the keyboard to navigate the rest (current semester, module, then the folder)

this is probably nothing to most people, but im not "most people". i'm constantly tired as hell. i cannot do all of that while i'm barely awake and listening to the lectures. the split second that you usually need to remember _what class you're in_ can escalate to me completely losing track of, urm, literally everything. yeah I have no idea how I'm even alive right now.

in comparisn, here's a __complete__ example of how I do it nowadays:
1. open up terminal
2. `cd dsf slides`
3. `xo 1<tab>`. utilizing the tab completion to choose files that contain `1`.

it's entirely keyboard-only, and it only takes a couple of seconds. the only two things I need to remember are my subject and the file I want.

Hopefully this post is helpful to anyone with a similar issue (lemme know if you do because I have never seen anyone talk about this). And if anyone has any similar or better workflows, lemme know too.

---

[Original post from Cohost](https://cohost.org/meow-d/post/4276461-my-optimum-way-to-ac#comments)
