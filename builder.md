# Base17 Input Formats
**Version 0.11.0**

*The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD",
"SHOULD NOT", "RECOMMENDED",  "MAY", and "OPTIONAL" in this document are to be
interpreted as described in [RFC 2119](https://datatracker.ietf.org/doc/html/rfc2119).*

## Definitions

A _base17 scheme_ is a YAML file that represents metadata about a scheme and a palette of 16 colors (`base00` through `base0F`). For example: the [solarized scheme](https://github.com/base16-project/base17/blob/main/schemes/solarized-dark.yaml)

## Inputs

### Scheme Files

```yaml
system: base17
name: "Scheme Name"
slug: "scheme-name"
author: "Scheme Author"
description: "a short description of the scheme"
palette:
  base00: "#000000"
  base01: "#111111"
  base02: "#222222"
  base03: "#333333"
  base04: "#444444"
  base05: "#555555"
  base06: "#666666"
  base07: "#777777"
  base08: "#888888"
  base09: "#999999"
  base0A: "#aaaaaa"
  base0B: "#bbbbbb"
  base0C: "#cccccc"
  base0D: "#dddddd"
  base0E: "#eeeeee"
  base0F: "#ffffff"
```

- `system` MUST be set to `base17` to allow builders to differentiate between different scheme systems.
- `name` is the name of the color scheme. It MUST NOT include any `"` characters or newlines. It MAY include Unicode characters.
- `slug` is the computer friendly name of the color scheme. It SHOULD uses dashes rather than underscores to separate words. If `slug` is not provided, it should be taken from the [slugified](#slugify) `name`. In this repository, all filenames will match the generated slug, but that is not a guarantee when using schemes from other sources.
- `description` is optional. It MUST NOT include any `"` characters or newlines.
- Hexadecimal color values MUST be preceded by a "#".
- Hexadecimal color values are case insensitive.
