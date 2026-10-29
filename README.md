# Nothing — an Omarchy theme

True-black OLED theme inspired by Nothing OS: monochrome dot-matrix with a single orange accent (`#ff6a13`).

## Install

```
omarchy theme install https://github.com/hell0world69/omarchy-nothing-theme
```

## What's inside

- `colors.toml` — the palette; Omarchy generates every app config from it.
- `btop.theme` — hand-patched so btop's network border uses the accent
  instead of red. It does not follow `colors.toml`; update it if you change
  the accent, or delete it to let Omarchy generate one.
- `backgrounds/` — five original dot-matrix wallpapers, a plain AMOLED black one, and the Omarchy vantablack logo and wordmark on black (`omarchy theme bg next` to cycle).
- `unlock.png` / `preview-unlock.png` — dot-matrix boot-screen logo
  (`omarchy plymouth set-by-theme nothing`).
- `preview.png` — theme picker thumbnail.
- `icons.theme` — grey folder icons (`Tela-circle-grey-dark`). Install them with
  `omarchy pkg add tela-circle-icon-theme-grey`; without the package you
  get the default icons.

## Optional: dot-matrix bar font

The full look uses [Doto](https://fonts.google.com/specimen/Doto) (OFL) in the
bar only. Install the font to `~/.local/share/fonts/`, then add a fontconfig
rule matching `prgname` `quickshell` that replaces `monospace` with `Doto`.
