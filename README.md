# less.edn

A VS Code extension for Clojure/EDN editing assistance. Remove commas, line breaks, toggle block comments, and format vectors — with Calva integration.

## Features

- **Remove Commas** — Remove all commas from selected text. If no text is selected, automatically expands selection via Calva's paredit.
- **Remove Line Breaks** — Merge selected lines into a single line.
- **Toggle Block Comment** — Toggle Clojure block comment (`#_`) or line comment (`;`) for the current form or selection, then move cursor to the next form.
- **Insert Newlines Between Vector Elements** — Split a `[...]` vector so each element is on its own line (ignores nested vectors).

## Usage

Open the command palette (`Cmd+Shift+P` / `Ctrl+Shift+P`) and search for:

| Command | Keybinding |
| --- | --- |
| Remove Commas | `Ctrl+Alt+C ,` |
| Remove Line Breaks | `Ctrl+Alt+C .` |
| Toggle Block Comment | `Cmd+Alt+/` |
| Insert Newlines Between Vector Elements | — |

## Requirements

- VS Code 1.85.0 or higher
- [Calva](https://marketplace.visualstudio.com/items?itemName=betterthantomorrow.calva) extension (required dependency for paredit integration)

## Release Notes

### 0.0.4

- Insert newlines between vector elements.
- Ignore nested vectors when inserting newlines.
- Multiple spaces are replaced with a single newline.

### 0.0.3

- Toggle block comment (`#_` / `;`) for selected text or current line.
- Add default keybindings.

### 0.0.2

- Remove line breaks from selected text.
- Auto-expand selection via paredit when no text is selected.

### 0.0.1

- Initial release with comma removal.
