# Changelog

## 2026.06.21 — repo standardisation

### What Changed

Relocated the icon tree to `usr/share/icons/`, added the standard project docs, and
corrected the README's dependency note.

### Technical Details

- Icon theme moved from `icons/` to `usr/share/icons/Surfn-Plasma-Flow/`; the packaging
  recipe `surfn-plasma-flow-git` (in `~/KIRO-PKG-BUILD-ICONS/`) was updated to copy from
  the new path.
- README dependency note corrected: the theme `Inherits=breeze-dark,Surfn-Plasma-Dark,breeze,hicolor`,
  so the package depends on `surfn-plasma-dark-icons-git`, not `surfn-icons-git`.
- Added CLAUDE.md.

### Files Modified

- usr/share/icons/Surfn-Plasma-Flow/ (relocated)
- README.md, CHANGELOG.md, CLAUDE.md
