# Lang3 Extension

This is a Visual Studio Code extension that provides support for the [Lang3 programming language](https://github.com/FinnE145/Lang3). It includes syntax highlighting, a dark theme, and has plans for a full language server.

## Installation

Search for "Lang3" in the [Visual Studio Code Marketplace](https://marketplace.visualstudio.com/) or in the extensions sidebar in VS Code and click "Install". Alternatively, you can install the extension manually by following these steps:

1. Clone or download the extension repository
2. Open the extension folder in VS Code
3. Run `npm install` to install dependencies
4. Run `npm run compile` to build the extension
5. Press `F5` to open a new VS Code window with the extension loaded for testing
6. To package the extension as a `.vsix` file, run `vsce package`
7. Install the `.vsix` file by opening the Extensions view in VS Code, clicking the "..." menu, and selecting "Install from VSIX..."

If that doesn't work, you can place the extension folder directly in your VS Code extensions directory:
- **Windows**: `%USERPROFILE%\.vscode\extensions\`
- **macOS**: `~/.vscode/extensions/`
- **Linux**: `~/.vscode/extensions/`

## Syntax Highlighting
The extension provides a TextMate grammar for Lang3, enabling syntax highlighting for `.lang3` and `.l3` files, that works with any theme in VS Code. This includes variables, types, numbers, strings, keywords, operators, comments, and language-specific functionality like tables.

Note that there are some aspects of this grammar that are purely stylistic, as they make code much more readable and align better with common conventions. For example, functions are identified as different from variables, even though Lang3 does not semantically differentiate between the two. Additionally, many of the best practices for comments are reinforced by the grammar, such as identifying heading comments (`### ... ###`), code-blocks in comments (`# :...;`), and errors in comments (`# !Error;`). All of these aspects of the language are still tagged with their true semantic meaning (either using multiple tags or more-specific tags), so you can modify your themes to either include these stylistic choices or ignore them.

## Dark Theme
The extension includes a custom dark theme called "Lang3 Dark". To use this theme:
1. Open the Color Theme picker in VS Code (`Ctrl+K Ctrl+T` or `Cmd+K Cmd+T` on macOS)
2. Select "Lang3 Dark" from the list of available themes
This theme is designed to work well with the Lang3 syntax highlighting, but also works nicely with other languages. It has not been tested extensively with languages other than Lang3, so please [report](https://github.com/FinnE145/Lang3Extension/issues) any missing or poorly chosen colors.