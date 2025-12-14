# Changelog

## [Unreleased] - 2025-12-16

### Added
- Markdown code fence support for Lang3 syntax highlighting documented in README.md
- Gitignore now ignores `*.vsix` files and `VSIX Releases/` folder

### Changed
- CHANGELOG.md has content for versions 0.0.1, 0.1.0, and 1.0.0
- README.md updated to include marketplace installation link and instructions, npm steps simplified
- README.md updated to include which themes "Lang3 Dark" is based off of

### Removed
- VSIX binaries for each release (still packaged with the release, just not in the repository)

## [0.1.0] - 2025-12-10

### Added
- Syntax highlighting in Lang3 code fences in markdown files ([#1](https://github.com/FinnE145/Lang3Extension/pull/1))
- Markdown injection language in package.json ([#1](https://github.com/FinnE145/Lang3Extension/pull/1))
- Ignoring `_test/` folder in gitignore ([#1](https://github.com/FinnE145/Lang3Extension/pull/1))

## [0.0.1] - 2025-12-10

### Added
- Initial release of Lang3 Extension for Visual Studio Code
- Syntax highlighting for Lang3 files (`.lang3`, `.l3`) with a .tmLanguage.json grammar
- Custom dark theme "Lang3 Dark" based off of VS Code's "Dark Modern" theme syntax highlighting and [WarmToast](https://marketplace.visualstudio.com/items?itemName=GregPasquariello.warmtoast) editor colours
- All content in README.md
- Icon image
- License file (MIT)
- Basic repository and extension structure