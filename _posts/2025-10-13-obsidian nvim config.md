---
tags: computers
title: essential obsidian.nvim configs because the defaults are really really strange
---

someone please remind me to change the comment color because damn it is hard to read

```lua
-- in Lazy.nvim format because it's what i use
{
  -- install `obsidian-nvim/obsidian.nvim` instead of `epwalsh/obsidian.nvim`, the unmaintained original version, which unfortunately still outranks the activly developed fork in search results
  "obsidian-nvim/obsidian.nvim",
  version = "*",
  ft = { "markdown" },

  -- the actual config

  ---@module 'obsidian'
  ---@type obsidian.config
  opts = {
    -- disables old commands and the depercation warning
    legacy_commands = false,

    -- does not literally "disable the frontmatter", but rather disable the auto formatting on save that removes your comments and sorts everything and adds ids and stuff
    frontmatter = { enabled = false },
    -- for older versions, use this instead of `frontmatter = { enabled = false }`
    -- disable_frontmatter = true,

    checkbox = {
      -- enter on normal mode turns everything into a checkbox, this disables it
      create_new = false,
      -- five niche, non-standard checkboxes as default is strange...
      order = { " ", "x" },
    }

    -- your actual config
    -- workspaces = {
    --   {
    --     name = "notes",
    --     path = "~/path-to-your-notes",
    --   },
    -- },
  },
},
```

## copy and paste-able versions
```lua
{
  "obsidian-nvim/obsidian.nvim",
  version = "*",
  ft = { "markdown" },

  ---@module 'obsidian'
  ---@type obsidian.config
  opts = {
    legacy_commands = false,
    frontmatter = { enabled = false },
    checkbox = {
      create_new = false,
      order = { " ", "x" },
    }

    -- your actual config
    -- ...
  },
},
```

### for older versions
```lua
{
  "obsidian-nvim/obsidian.nvim",
  version = "*",
  ft = { "markdown" },

  ---@module 'obsidian'
  ---@type obsidian.config
  opts = {
    disable_frontmatter = true,

    checkbox = {
      create_new = false,
      order = { " ", "x" },
    }

    -- your actual config
    -- workspaces = {
    --   {
    --     name = "notes",
    --     path = "~/path-to-your-notes",
    --   },
    -- },
  },
},
```
