# Gruvbox Light theme for ARGVUS

Official ARGVUS Light theme, `gruvbox-light`, with its Sticky and Float variants.

[![CI](https://github.com/argvus/argvus-theme-gruvbox-light/actions/workflows/ci.yml/badge.svg)](https://github.com/argvus/argvus-theme-gruvbox-light/actions/workflows/ci.yml)
[![Release](https://github.com/argvus/argvus-theme-gruvbox-light/actions/workflows/release.yml/badge.svg)](https://github.com/argvus/argvus-theme-gruvbox-light/actions/workflows/release.yml)
[![License](https://img.shields.io/badge/License-GPL--3.0-blue.svg)](LICENSE)

## Theme identity

| Field | Value |
| --- | --- |
| Theme ID | `gruvbox-light` (Float variant: `gruvbox-light-float`) |
| Display name | Gruvbox Light |
| Mode | `light` |
| Default highlight | `#458588` |
| GTK color scheme | `prefer-light` |
| Calendar stylesheet | `gruvbox-light` |
| Package | `argvus-theme-gruvbox-light` |
| Wallpaper | `/usr/share/backgrounds/argvus/abstract/light/gruvbox-abstract-light.jxl` |

The values above are the ones declared in
`src/usr/share/argvus/appearance/themes.d/gruvbox-light/theme.toml`, the manifest that the
desktop reads. The manifest is the source of truth; this page describes it.

## Installing

The package depends on `argvus` and `argvus-appearance`, so pacman installs them with it.

```sh
sudo pacman -S argvus-theme-gruvbox-light
```

Select the theme in the Control Center (Appearance > Themes), or run
`argvus theme-switch gruvbox-light`.

## Files

The package installs the theme's per-component files under `/usr/share/argvus` (and the
calendar stylesheet under `/etc/argvus/taskbar/calendar/themes`). Each component that
the theme styles has its own directory, listed by `find src -type f` in this repository.

## Development

Validate with `make validate` before building. The design rules are in
[DEVELOPMENT.md](DEVELOPMENT.md); the ARGVUS documentation for themes is in
`argvus/docs/en/user-guide/appearance.md` of the `argvus` repository.

## License

GPL-3.0-only. See [LICENSE](LICENSE).
