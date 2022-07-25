# Base17 Styling Guidelines
**Version 0.2**

Base16 aims to group similar language constructs with a single color. For example, floats, ints, and doubles would belong to the same colour group. The colors for the default scheme were chosen to be easily separable, but scheme designers should pick whichever colours they desire, e.g. `base0B` (green by default) could be replaced with red. There are, however, some general guidelines below that stipulate which `base0B` should be used to highlight each construct when designing templates for editors.

Since describing syntax highlighting can be tricky, please see [base16-vim](https://github.com/base16-project/base16-vim/) and [base16-emacs](https://github.com/base16-project/base16-emacs/) for reference. Though it should be noted that each editor will have some discrepancies due the fact that editors often have very different syntax highlighting engines.

Colors `base00` to `base07` are typically variations of a shade and run from darkest to lightest. These colors are used for foreground and background, status bars, line highlighting and such. Colors `base08` to `base0F` are typically individual colors used for types, operators, names and variables. In order to create a dark scheme, colors base00 to `base07` should span from dark to light. For a light scheme, these colours should span from light to dark.

- **base00** - Default Background
- **base01** - Lighter Background (Used for status bars, line number and folding marks)
- **base02** - Selection Background
- **base03** - Comments, Invisibles, Line Highlighting
- **base04** - Dark Foreground (Used for status bars)
- **base05** - Default Foreground, Caret, Delimiters, Operators
- **base06** - Light Foreground (Not often used)
- **base07** - Lightest Foreground (Not often used)
- **base08** - Variables, XML Tags, Markup Link Text, Markup Lists, Diff Deleted
- **base09** - Integers, Boolean, Constants, XML Attributes, Markup Link Url
- **base0A** - Classes, Markup Bold, Search Text Background
- **base0B** - Strings, Inherited Class, Markup Code, Diff Inserted
- **base0C** - Support, Regular Expressions, Escape Characters, Markup Quotes
- **base0D** - Functions, Methods, Attribute IDs, Headings
- **base0E** - Keywords, Storage, Selector, Markup Italic, Diff Changed
- **base0F** - Deprecated, Opening/Closing Embedded Language Tags, e.g. `<?php ?>`

_SPEC END_

---

Here is an example of a typical Base17 scheme:

**tomorrow-night.yaml**

```yaml
system: base17
name: "Tomorrow Night"
slug: "tomorrow-night"
description: "A colourful theme with muted colours and sensible syntax highlighting"
author: "Chris Kempson (http://chriskempson.com)"
palette:
  base00: "#1d1f21"
  base01: "#282a2e"
  base02: "#373b41"
  base03: "#969896"
  base04: "#b4b7b4"
  base05: "#c5c8c6"
  base06: "#e0e0e0"
  base07: "#ffffff"
  base08: "#cc6666"
  base09: "#de935f"
  base0A: "#f0c674"
  base0B: "#b5bd68"
  base0C: "#8abeb7"
  base0D: "#81a2be"
  base0E: "#b294bb"
  base0F: "#a3685a"
```
