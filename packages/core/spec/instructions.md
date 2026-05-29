<!-- SPDX-License-Identifier: CC-BY-4.0 -->
# L0174 Dialect Extensions

L0174 is the base dialect of Graffiticode, focused on simple interactions and visualizations.

## L0174 Functions

| Function | Signature | Description |
| :------- | :-------- | :---------- |
| `hello` | `<string: record>` | Renders a "hello, {string}!" greeting |
| `image` | `<string: record>` | Renders an image from a URL |
| `theme` | `<tag record: record>` | Sets UI theme (DARK or LIGHT) wrapping a body expression |
| `id` | `<string any: record>` | Sets an element identifier |

## L0174 Built-in Tags

- `DARK` — dark theme
- `LIGHT` — light theme

## L0174 Examples

### Hello world
```
hello "world"..
```

### Themed greeting
```
theme DARK hello "world"..
```

### Image display
```
image "https://example.com/photo.jpg"..
```

### Combining core and L0174 functions
```
let name = "world"..
theme LIGHT hello name..
```
