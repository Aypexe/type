# Type
<p align="center">
  <img src=https://github.com/Aypexe/type/blob/main/icon_1024x1024.png width="128" >
</p>

Type is inspired by Rafal Pastuszak's Ensō -- a personal piece of software we wrote to focus on writing and _not_ editing or overthinking. Type a sentence and hit enter. As you type more sentences, previous ones will fade away, leaving only the work in front of you.

Ensō had some design limitations that I couldn't get past (like cmd+a not selecting all text), so I rewrote this in SwiftUI as a native MacOS app (working on iPhone/iPad next). In general I did not want to disturb the philosophy of write now, edit later -- but I do find not being able to back a line (especially if you are typing quickly and accidentally commit a line), so I added the ability to cmd+z to the previous line (no further). This should help UX a bit when making minor mistakes that would be more bothersome to not fix... hopefully without disrupting the ethos too much.

## Installation

### Homebrew (recommended)

```bash
brew tap Aypexe/tap
brew install --cask type
```

### Manual

1. Download the latest `Type.dmg` from [Releases](https://github.com/Aypexe/type/releases)
2. Open the DMG and drag Type to Applications
3. Right-click Type.app and select "Open" (required first time for unsigned apps)

## Keyboard Shortcuts

### Writing

| Shortcut | Action |
|----------|--------|
| `Enter` | Commit current sentence and start a new line |
| `Cmd + Z` | Edit previous sentence (current text is preserved) |
| `Cmd + Shift + Z` | Cancel edit and restore previous state |
| `Cmd + D` | Clear current sentence |

### File Management

| Shortcut | Action |
|----------|--------|
| `Cmd + N` | New window |
| `Cmd + O` | Open file |
| `Cmd + S` | Save |
| `Cmd + Shift + S` | Save As |
| `Cmd + W` | Close window |

## File Format

Type saves documents as standard Markdown files. Editing can be done in your preferred markdown editor after you leave your flow state ;)

## Requirements

- macOS Sonoma (14.0) or later
