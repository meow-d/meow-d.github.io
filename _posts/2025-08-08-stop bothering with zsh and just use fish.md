---
title: Stop bothering with Zsh and just use Fish
tags: computers
---

You know why everyone installs Zsh in the first place? Because they want a Fish-like experience. Which you usually do with a ton of plugins. Zsh-autosuggestions in particular is Fish inspired.

A tutorial will usually first present it like the most innovative thing ever, then tell you to install Oh My Zsh. Apart from having weird vibes, OMZ is bloated tons of stuff that you will never need, with a gigantic and confusing default config file, and installing non-OMZ plugins still requires manually doing git clone. I guess they only called it a framework, not framework + plugin manager, cause it's so bad at managing plugins. I don't think there's anything wrong with it per se, I just don't feel excited about using it, and the whole point of the upgrade is to feel good about using your terminal.

Despite that, there's a reason why OMZ is still the de facto Zsh plugin manager. It gives you all the sane defaults with just one command so you can jump in and instantly feel the "oh my zsh" or something. It has a plugin for pretty much everything out there. And the competition. The competition. Is a complete mess.

Zsh has an insane amount of competing plugin managers and 80% ended up abandoned eventually. It's an [xkcd 927 (competing standards)](https://xkcd.com/927/) situation, but extreme to the point where it doesn't feel real. The readme of [zsh_unplugged](https://github.com/mattmc3/zsh_unplugged/#newspaper_roll-current-state) explains this pretty well.

### if you still want to use Zsh
urm.... I don't really have a recommendation as someone who has only tried a few and quit years ago.

In terms of alternatives to OMZ, there's [zsh-quickstart-kit](https://github.com/unixorn/zsh-quickstart-kit), which I guess is the closest thing to it.

As for plugin managers, when I was still using Zsh, [ZInit](https://github.com/zdharma-continuum/zinit) was the goat. It supports plugins from OMZ and Prezto, lightning fast performance thanks to turbo mode (async loading). The big problem is the extremely confusing documentation and syntax for something that's actually very simple underneath. If you want a reference for a config you can find [my old .zshrc here](https://github.com/meow-d/dotfiles/blob/master/.zshrc).

For a minimal elegant solution there's also [zsh_unplugged](https://github.com/mattmc3/zsh_unplugged) as mentioned just now. Just a ~20 line function you can yank into your jortz. Plug tuah.

## the part where I shill Fish
what's special about Fish? nothing. You don't have to do anything and it just works. You can use Fish just fine with zero plugin or config. And by that I mean all the autocomplete and conventional text editor keybinds. You don't even need a bazillion OMZ plugins for completion, because Fish has a `fish_update_completions` command that automatically generates them from manpages. Insane.

Okay to be fair, `ctr + backspace` is disabled by default, due to differences in terminals. So it's _nearly_ perfect.

Also, you might have heard how Fish is (intentionally) not POSIX compliant. Yes, the lack of `&&` was a huge pain point until they added it a couple of years ago. But it's not much of a problem in practice because: you can always run stuff in bash when you need it anyways, and shebangs exist.

---

## bonus
- There are more shells out there than the big 3, with pretty interesting ideas. Try them!
- Bash, or more specifically, Readline, can do more than you think - tab completion, history search, undo, etc. Most already have default keybinds, but [you can configure to feel more conventional](https://github.com/meow-d/dotfiles/blob/master/.inputrc).
  - There's also [ble.sh](https://github.com/akinomyoga/ble.sh), which replaces Readline in Bash, and provides syntax highlighting, auto suggestions and more... As glad as I am that it exists, I'm not sure why would I use this over fish.
