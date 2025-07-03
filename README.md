# About

This extension adds full GPC Scripting support for Visual Studio Code, offering a wide range of features and tools to enhance your development experience.

# ⚠️⚠️ WARNING ⚠️⚠️
This Extension is deprecated and will no longer receive updates or support. Please use the extension "GPC Language Support" instead.

## Features
### Language Support
- Full syntax highlighting for GPC files
- IntelliSense support with:
  - Code completion for Variables, Functions, Combos, and Built-in functions
  - Hover information

### Smart Diagnostics
- Real time error detection for:
  - Invalid function parameter counts
  - String quote validation
  - Decimal number warnings
  - Unknown character warnings
- Toriel Build System
  - https://github.com/zKiwiko/Toriel-BT

### Code Snippets
Quick templates for common GPC/C like constructs:
- For loops (`For~`)
- While loops (`While~`)
- If statements (`If~`)
- If-else statements (`Ifelse~`)
- Function definitions (`Function~`)

### Toriel Built System Intergration
Built-in support for [Toriel BT](https://github.com/zKiwiko/Toriel-BT).

Toriel BT is completely optional to use, for more information on the build process and its features, check here: https://github.com/zKiwiko/Toriel-IDE?tab=readme-ov-file#project-structuring

## Requirements
- Visual Studio Code Version 1.98.0 or higher
- GPC Knowledge

## Setup
1. Install the extension from the VS Code marketplace
2. Create or open a GPC project or file
3. For built functionality, ensure you have a valid `project.json` file in your workspace's root directory.


### Toriel Project Configuration
Create a `project.json` file in your project's root directory containing:
```JSON
{
   "project" : {
      "name": "",
      "version": "",
      "source": "",
      },
   "headers": []
}
```
### Configuration Fields
- `name`: Your project name (used for build output)
- `version`: Project version
- `source`: Main entry point file
- `headers`: Array of header files used in project
- `std`: Array of standard library files used

## Commands
- Build Project: `Ctrl+Shift+P` → "GPC: Build project with Toriel"

## Contributing
Feel free to open issues or submit pull requests on the [GitHub repository](https://github.com/zKiwiko/vscode-gpc-extension).

## License
This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
Any trademarks related to this repository are owned by their respective owners.
