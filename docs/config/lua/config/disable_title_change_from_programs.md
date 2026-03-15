---
tags:
  - appearance
  - title
  - security
---
# `disable_title_change_from_programs = true`

When set to `true`, WezTerm will ignore OSC (Operating System Command)
escape sequences emitted by programs that attempt to change the tab or
window title. This prevents applications from modifying the GUI title
via the standard OSC sequences while still allowing titles to be changed
programmatically via WezTerm's APIs or the `wezterm cli` (for example
`wezterm cli set-window-title "hello world"`).

The default is `false` (i.e., honor title changes requested by programs).

```lua
config.disable_title_change_from_programs = true
```
