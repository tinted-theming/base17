# Base17 Styling Guidelines
**Version 0.2**

Base17 aims to group similar language constructs with a single color. For example, floats, ints, and doubles would belong to the same colour group. The colors for the default scheme were chosen to be easily separable, but scheme designers should pick whichever colours they desire, e.g. `base0B` (green by default) could be replaced with red. There are, however, some general guidelines below that stipulate which `base0B` should be used to highlight each construct when designing templates for editors.

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


---

Here is an example of a typical Base17 scheme:

**tomorrow-night.yaml**

```yaml
system: base17
name: "Monokai"
slug: "monokai"
description: "A port of the original Monokai color scheme for TextMate"
author: "Wimer Hazenberg (http://www.monokai.nl)"
palette:
  base00: "#272822"
  base01: "#383830"
  base02: "#49483e"
  base03: "#75715e"
  base04: "#a59f85"
  base05: "#f8f8f2"
  base06: "#f5f4f1"
  base07: "#f9f8f5"
  base08: "#f92672"
  base09: "#fd971f"
  base0A: "#f4bf75"
  base0B: "#a6e22e"
  base0C: "#a1efe4"
  base0D: "#66d9ef"
  base0E: "#ae81ff"
  base0F: "#cc6633"
```
