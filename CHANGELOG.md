# Changelog

All notable changes to the `omni-devtools` skill will be documented in this file.

## [1.0.0] - 2026-06-01

This is the initial public release of the `omni-devtools` skill.

### Added
- **CSS Custom Properties Layer**: Guidance on establishing relative variables in core theme stylesheets for responsive scaling.
- **Non-Blocking Head Preloader**: Safe preloader script in page `<head>` to parse local configurations before paint, preventing CLS and FOUT.
- **Safe Google Fonts Fallback Loader**: Progressive loader to try standard Google Font variants from v2 API cleanly without throwing 400 errors.
- **Undo/Redo Design History Stack**: Input checkpoint stack utilizing distinct slider events (`input` vs `change`) to track comparisons without performance lag.
