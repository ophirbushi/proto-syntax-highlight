# proto-syntax-highlight

Lightweight Visual Studio Code extension that provides improved syntax highlighting for Protocol Buffer (.proto) files.

## What it does
- Adds accurate tokenization and colors for Protocol Buffer syntax (keywords, messages, enums, fields, services, options, imports, comments, and primitive types).
- Works with files using the `.proto` extension and files recognized as the `proto` language.

## Features
- Highlighting for protobuf keywords (syntax, package, import, message, enum, service, rpc, option, repeated, optional, required).
- Distinct colors for types, message names, enum members, and field names.
- Proper handling of comments and documentation strings.
- Lightweight and fast — no background language server required.

## Usage
1. Install the extension from the VS Code Marketplace or load it from the extension development host.
2. Open any `.proto` file — syntax highlighting will be applied automatically.
3. If a file is not recognized, open the Command Palette and run "Change Language Mode" → `proto`.

## Installation
- From VS Code: Search for "proto-syntax-highlight" in Extensions and click Install.
- From source: clone the repo, open it in VS Code, and run the Extension Development Host.

## Extension Settings
This extension does not add runtime settings. Color customizations can be made via your editor theme or by overriding token colors in VS Code settings.

Example to customize colors in settings.json:
```json
// Add under "editor.tokenColorCustomizations"
{
  "textMateRules": [
    {
      "scope": "source.proto keyword",
      "settings": { "foreground": "#FF8800" }
    }
  ]
}
```

## Contributing
Contributions, bug reports, and feature requests are welcome. Please open issues or PRs in the repository.

---

For more information about developing VS Code extensions, see:
- https://code.visualstudio.com/api
