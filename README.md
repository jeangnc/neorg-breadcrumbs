# neorg-contexts

A small Neorg external module that shows the current heading context as a single line.

Example:

```
Project > Planning > Milestones
```

## Install

Use your plugin manager to add this repo, then enable it in Neorg:

```lua
require("neorg").setup({
  load = {
    ["core.defaults"] = {},
    ["core.concealer"] = {},
    ["core.neorgcmd"] = {},
    ["external.context"] = {},
  },
})
```

## Commands

- `:Neorg context toggle`
- `:Neorg context enable`
- `:Neorg context disable`

## Notes

- Only renders in `norg` buffers.
- Context line is updated on scroll, buffer enter, window enter, and cursor move.
