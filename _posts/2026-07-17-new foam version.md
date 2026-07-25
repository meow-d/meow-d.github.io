---
tags: computers
title: Foam (the PKM VSCode extension) got a glow-up
---

I've been using an old version of Foam since last year due to a bug I forgot, and I only recently updated. There are so many new features now. The execution is mixed, but will be very exciting to any Foam user nonetheless.

>Context but I explained like you're 5: I [write my notes in a folder of markdown text files]({% link _posts/2025-08-03-note taking.md %}), which is compatible with basically any software. I use Neovim with the [obsidian.nvim]({% link _posts/2025-10-13-obsidian nvim config.md %}) plugin, and VSCode with the [Foam extension](https://foam.md/), which brings Obsidian features to VSCode.

The new features do have hallmarks of AI coding. But there's no shame of harnessing the power of vibe coding, especially when you're a small yet important project whose main bottleneck is available developers. Despite how much I hate AI slop, I find vibe coding empowering to those with very few resources.

## The new website
There is a new home page, a new docs site, and the new foam.md domain. The new docs page is more conventional, but good. The domain must have been expensive.

The home page is obviously vibe coded. It is full of AI design and AI marketing copy - em dash, no x no x no x pattern, your x your x pattern, weird AI metaphors. Not the best look for Foam, since these websites usually scream low effort AI slop, and Foam definitely don't deserve to be associated with those.

The old pages had charm. While there is definitely a way to keep that design after the glow-up, I don't particularly care that much.

## It's now "agent ready", or so it claims
There is now a Foam CLI, with an MCP server. Actually, the Foam CLI [existed](https://www.npmjs.com/package/foam-cli?activeTab=versions) since forever, but it was only 2 months ago that it was turned into a fully fledged thing.

>Tangent: it's funny how the AI hype has unintentionally promoted the command line due to how well agents work with them. It is also funny how much hype MCP had before completely [falling off](https://tombedor.dev/mcp-is-a-fad/) and replaced by the humble bash tool. As a heavy command line user and light coding agent user, this is a win for me.

From my testing it doesn't seem "ready" though. For example, running `foam daily` returns `journals/2026-07-17.md  [does not exist]`, which is the wrong folder. I don't know if that's a bug but there's no clear indication what I should do instead. Printing the stack trace on every error by default doesn't seem very user friendly.

Speed is another major issue. Is it starting an instance of Foam on every command with nothing cached? Either way, it is definitely not as fast and human-usable compared to the Foam extension itself.

## Foam query
They finally added their own Obsidian dataview to foam. The [syntax](https://docs.foam.md/features/foam-queries/) seems to be closer to [Obsidian bases' syntax](https://obsidian.md/help/bases/syntax), being yaml based.

Speaking of bases, Foam's answer to bases seem to be [smart folders](https://docs.foam.md/features/smart-folders/). A more descriptive name would be "folder filters". They're just foam queries in yaml files, and they'll show up in your explorer sidebar as filtered version of your file tree.

I think the Foam query is in an awkward place right now. It is featureful enough to be useful, but not powerful.

I find certain limitations and inconsistencies annoying. Backlinks are a `links_from` in filter, `backlinks` in jexl, and not in displayed fields. In fact, the simple filters, structured filters, jexl fields, and displayed fields (used in select and sort), are 4 different things. I was also disappointed that you can't sort by outlink order (so my todo list use case is kinda in the wrong order).

I think they're limited by the fact that it's yaml-based rather than a real DSL, which their jexl and js support kinda makes up for in an awkward way. If we have the power of vibe coding anyways, why not just make the AI reimplement the dataview query language, or the bases syntax? Maybe I should just spend my tokens on that...

Another idea I have is turning those smart folders into a full blown bases alternative, by opening those yaml files with a bases like view. `select:` will no longer be unused in smart folders.

But enough of the negative stuff. I think I'm already giving off an impression that I'm Foam hater or something. I love Foam and use it daily. I am a actually really happy about the feature. I'm a highly statisfied customer and I would eat Foam every day. Crunch.

## some example foam queries
### orphan notes
```yaml
filter:
  and:
    - path: "/notes/notes"
    - path: ".md"
    - jexl: "resource.backlinks|length == 0"
    - jexl: "resource.outlinks|length == 0"
sort: title ASC
```

### most linked notes
```yaml
filter:
  path: ""
select: [title, backlink-count, tags]
sort: backlink-count DESC
limit: 10
```

### smart folder where you pin specific notes
```yaml
# create a note called pinned.md or smth
filter:
  links_from: "pinned"
```
