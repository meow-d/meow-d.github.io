---
tags: productivity computers
title: How I navigate my school documents using the command line (and why you might want to too)
---

## folder structure
first of all, have a folder for each subject/module. you can group them by semester and intake. pretty standard for anyone in uni.

folder names have to be in short form, and try to be consistent with the structure within each module's folder, for reasons i'll explain later.

```
├── school
│   ├── diploma
│   │   ├── 5
│   │   │   ├── DSF
│   │   │   │   ├── slides
│   │   │   │   ├── assignment
│   │   │   │   ├── tutorial
│   │   │   ├── IAI
│   │   │   ├── JP
│   │   │   └── SDP
│   ├── degree
│   │   ├── 2
│   │   │   ├── MAE
...
```

## command line navigation
open your terminal. since i use vscode to take notes, i can just use `ctrl + backtick` for the intergrated terminal. though i mostly prefer to open up a separate terminal window, which i bind to `win + t`.

install any of those "smarter cd" tools, like [zoxide](https://github.com/ajeetdsouza/zoxide). this is why the folder names need to be short - to avoid ambiguity when it chooses a folder from your history. after installation, remember to cd to each of the folders once to save them. you can also alias/abbevrate it to `cd`.

then, make an alias/abbreviation for `xdg-open` (i abbr'ed it to `xo`). this command opens the file using the defaults application, identical to clicking on a file in your usual file manager.

_for those who don't know, [abbreviations](https://fishshell.com/docs/current/cmds/abbr.html) are a feature in Fish. instead of replacing the command entirely like aliases, it replaces the abbreviation with the command once you press space. it's pretty much what aliases are meant to be._

## why do this?
here's how i used to open up lecture slides:
1. open up the file manager (with a shortcut)
2. use the trackpad to click "School" from the sidebar, because Dolphin doesn't allow you to navigate the sidebar with a keyboard
3. click the main ui to change the focus back to the files.
4. use the keyboard to navigate the rest (current semester, module, then the folder)

this is probably nothing to most people, but im not "most people". i'm constantly tired as hell. i cannot do all of that while i'm barely awake and listening to the lectures. the split second that you usually need to remember _what class you're in_ can escalate to me completely losing track of, urm, literally everything. yeah I have no idea how I'm even alive right now.

in comparison, nowadays i just:
1. `win + t`
2. `cd dsf sli`
3. `xo 1<tab>`. utilizing the tab completion to choose files that contain `1`.

it's entirely keyboard-only, and it only takes a couple of seconds. the only two things I need to remember are my subject and the file I want.

Hopefully this post is helpful to anyone with a similar issue (lemme know if you do because I have never seen anyone talk about this). And if anyone has any similar or better workflows, lemme know too.

## bonus: command line snippets
now that you're using the command line, you can do a lot of trickery :3. here are a few snippers i commonly use.

_these are in fish because it's what i use. if you use bash or zsh you'd have to change them a bit. just ask an LLM, idk._

_protip: fish's history autocompletion allows you to easily search for past snippets! who needs abbreviations anyways_

### move all docx files from downloads here
```sh
mv ~/Downloads/*.docx ./
```

i mean, replace the docx with whatever you want.

### unzip
```sh
mv ~/Downloads/*.zip ./ && unzip *.zip && rm *.zip
```

be careful to not unzip something you don't want in your school notes...

### unzip into a folder and delete the zip and delete the __MACOSX
```sh
for f in *.zip; set name (basename $f .zip) && mkdir -p $name && unzip -d $name $f && rm $f && rm -rd $name/__MACOSX; end
```

### convert to pdf
```sh
libreoffice --headless --invisible --convert-to pdf *.docx && mkdir -p docx && mv *.docx docx/

libreoffice --headless --invisible --convert-to pdf *.pptx && mkdir -p pptx && mv *.pptx pptx/
```

cause i don't like opening up resource-heavy office software for the documents/slides when all i need is a lightweight pdf reader.

---

[Original post from Cohost](https://cohost.org/meow-d/post/4276461-my-optimum-way-to-ac#comments)
