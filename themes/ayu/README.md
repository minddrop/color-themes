# ayu

A port of [ayu](https://github.com/ayu-theme/ayu-colors) by Konstantin Pschera. MIT license, see [LICENSE](LICENSE).

| Variant | Windows Terminal |
| --- | --- |
| mirage | [ayu-mirage.json](windows-terminal/ayu-mirage.json) |

## Install

### Windows Terminal

1. Open **Settings**, then **Open JSON file**.
2. Paste the file's contents into the `"schemes": [ ... ]` list.
3. Set `"colorScheme": "Ayu Mirage"` on a profile, or under `profiles.defaults` to use it everywhere.

## Notes

- **Bright black** is upstream's `#0A0000`, which is nearly invisible on the dark background. If dim text (zsh autosuggestions, some `ls` colors) disappears, change `brightBlack` to `#6E7C8F`.
- **Background** is `#1F2430`, the classic mirage background. Use `#242936` to match the newer editor background.

<details>
<summary>Palette and source details</summary>

Colors come from the built `ayu@9.1.0` npm package (`dist/generated/mirage.js`). The upstream YAML files ([mirage.yaml](https://github.com/ayu-theme/ayu-colors/blob/master/themes/mirage.yaml)) only give base colors and rules for adjusting them, so the package has the final hex codes.

### mirage

| Role | Hex | Upstream key |
| --- | --- | --- |
| Background (UI) | `#1F2430` | `ui.bg` / `surface.base` |
| Background (editor) | `#242936` | `editor.bg` / `surface.lift` |
| Background (sunk) | `#181C26` | `surface.sunk` |
| Foreground | `#CCCAC2` | `editor.fg` |
| UI foreground | `#707A8C` | `ui.fg` |
| Accent / cursor | `#FFCC66` | `common.accent.tint` |
| Selection | `#409FFF` at 25% | `editor.selection.active` |
| Comment | `#6E7C8F` | `syntax.comment` |
| Error | `#FF6666` | `common.error` |

| ANSI | Normal | Bright |
| --- | --- | --- |
| Black | `#0A0000` | `#0A0000` |
| Red | `#F06B5C` | `#F39184` |
| Green | `#BFE76D` | `#D5FF80` |
| Yellow | `#E6B752` | `#FFCD66` |
| Blue | `#3BBBF4` | `#73D0FF` |
| Magenta | `#D09FFD` | `#DFBFFF` |
| Cyan | `#84CEB5` | `#95E6CB` |
| White | `#D2D6DC` | `#E3E6EA` |

| Syntax | Hex |
| --- | --- |
| Tag | `#5CCFE6` |
| Function | `#FFCD66` |
| Entity | `#73D0FF` |
| String | `#D5FF80` |
| Regexp | `#95E6CB` |
| Markup | `#F28779` |
| Keyword | `#FFA659` |
| Special | `#D9BE98` |
| Constant | `#DFBFFF` |
| Operator | `#F29E74` |

Windows Terminal draws the selection color semi-transparent, so solid `#409FFF` there looks like the editor's 25% blue.

</details>
