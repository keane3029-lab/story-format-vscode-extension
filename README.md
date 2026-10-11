# .STORY Format Support

Syntax highlighting, snippets and language support for `.story` files, a plain-text format for writing day-by-day stories with narration and dialogue.

## Features

- Syntax highlighting for `.story` and `.STORY` files
- Snippets for the common building blocks
- Comment, bracket and auto-closing support through the language configuration

## The .story format

```story
day: 1
title: The First Day
scene: Classroom
mood: Chaotic
---
* The bell rings and nobody moves.
Carl: bro is the teacher even here
Kier: nope
# this is a comment

===
day: 2
title: The Next Day
---
* Everything is somehow worse.
```

- `key: value` lines at the top form the day header (`day`, `title`, `scene`, `mood`)
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

From the Marketplace: search for `.STORY Format Support` in the Extensions view.

From a `.vsix` file:

1. Run `npm install` then `npm run package` to build the `.vsix`
2. In VS Code, open the Extensions view, tap the three dots, choose `Install from VSIX...`, and pick the file

## Development

```
npm install
npm run compile
```

Press `F5` in VS Code to launch an Extension Development Host with the extension loaded. Open a file from the `samples` folder to try it.

## Links

- Issues: https://github.com/keane3029-lab/story-format-vscode-extension/issues
- Source: https://github.com/keane3029-lab/story-format-vscode-extension

## License

MIT
