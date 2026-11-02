# color-themes

My color themes for terminals, editors, and anything else that takes a color scheme.

## Themes

| Theme | Variants | Apps | License |
| --- | --- | --- | --- |
| [ayu](themes/ayu/) | mirage | Windows Terminal | MIT (port) |

Open a theme's folder for the files and install steps.

## Layout

```
themes/<theme>/
  README.md              # install steps, notes, palette
  LICENSE                # only for ports of someone else's theme
  <app>/<theme>-<variant>.<ext>
```

App folders use lowercase kebab-case names, e.g. `windows-terminal`, `vscode`, `vim`. If an app needs several files or a fixed structure, they all go in its folder.

## License

- **My own themes** and everything else here: [MIT-0](LICENSE). Use them for anything; no credit needed.
- **Ports of other people's themes** keep their original license, in that theme's `LICENSE` file. The table above shows which ones.

Before porting a theme, check its license. If it has none, don't copy it in. Link to it instead.
