# Changelog

## 2026.06.23 — Tela colour split

**Install docs:** the README install section now lists the meta packages (top-level `*-icons-meta`, plus the group meta where applicable) alongside the per-variant `*-icons-git` package — replacing the outdated single `pacman -S` line.

### What Changed

Initial standalone repo. The **Surfn-Tela-Red** folder icons were taken from the Tela icon theme
(`vinceliuice/Tela-icon-theme`) and surfn-ified so they ship as `surfn-tela-red-icons-git`, depending on the
base `surfn-icons-git`.

### Technical Details

- Only the `places` context is shipped (folders); everything else inherits Surfn.
- `index.theme`: `Name=Surfn Tela Red`, `Inherits=Surfn,hicolor`.
- Cross-context symlinks dereferenced so no broken links ship; `icon-theme.cache` excluded.

### Files Modified

- Initial scaffold + usr/share/icons/Surfn-Tela-Red/
