# CLAUDE.md — surfn-plasma-flow

## Project overview

Standalone repo for the **Surfn Plasma Flow** icon theme, split out of the
`erikdubois/surfn` monolith. See [README.md](./README.md).

## Current state

Ships one theme: `usr/share/icons/Surfn-Plasma-Flow/`. Packaged as `surfn-plasma-flow-git`
(recipe in `~/KIRO-PKG-BUILD-ICONS/surfn-plasma-flow/`), `depends=('surfn-plasma-dark-icons-git')`.
The recipe also copies the theme into `/usr/share/plasma/`.

## Patterns & decisions

- Theme dir PascalCase; repo/package lowercase. `icon-theme.cache` rebuilt by the pacman
  hook on install. Theme `Inherits=breeze-dark,Surfn-Plasma-Dark,breeze,hicolor` — it does
  **not** inherit base Surfn. Bash scripts follow the canonical Kiro template.
