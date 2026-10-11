# .STORY Format Support

Syntax highlighting, snippets and language support for `.story` files, a plain-text format for writing day-by-day stories with narration and dialogue.

## Features

- Syntax highlighting for `.story` and `.STORY` files
- Snippets for the common building blocks
- Comment, bracket and auto-closing support through the language configuration

## The .story format

```story
day: 1
title: The Arrival
scene: Train Station
mood: nervous
author: keane
---
# this is a comment
* the rain would not stop.
mira: you came
jonas: i almost didn't
===
day: 2
title: Morning After
---
* sunlight crept in.
mira: we need to talk
```

- `key: value` lines at the top form the day header (`day`, `title`, `scene`, `mood`, `author`)
- `---` ends the header and starts the body
- `* text` is a narration line
- `speaker: text` is a dialogue line
- `# text` is a comment
- `===` separates one day from the next

## Snippets

Type the prefix and press Tab.

| Prefix    | What it inserts                                  |
| --------- | ------------------------------------------------ |
| `day`     | Day header, separator and first body lines       |
| `nextday` | Day separator plus a new day header              |
| `nar`     | Narration line                                   |
| `say`     | Dialogue line                                    |
| `note`    | Comment line                                     |

## Install

From a `.vsix` file (download it from the Releases page):

1. In VS Code, open the Extensions view
2. Tap the three dots at the top
3. Choose `Install from VSIX...` and pick the file

## Development

```
npm install
npm run compile
npm run package
```

Press `F5` in VS Code to launch an Extension Development Host with the extension loaded. Open `samples/example.story` to try it.

## Links

- Issues: https://github.com/keane3029-lab/story-format-vscode-extension/issues
- Source: https://github.com/keane3029-lab/story-format-vscode-extension

## License

MIT
