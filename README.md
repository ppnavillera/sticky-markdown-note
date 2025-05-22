# Sticky Markdown Note

A lightweight, always-on-top sticky note applicatoin with Markdown support, built with Electron. Save and manage your notes in Markdown format, complete with live preview, math rendering (KaTeX), themes, and session restore.

## Features

- **Persistent Notes**: Notes saved as `.md` files in your user data directory.
- **Live Preview**: Real-time Markdown rendering with KaTex math support.
- **Light/Dark Themes**: Toggle between light and dark modes.
- **Autosave & Session Restore**: Automatically restores open notes on startup.
- **Search & Filter**: Quickly find notes by title or content.
- **Window Memory**: Remembers last position and size of each note window.
- **Keyboard Shortcuts**: See below for a comprehensive list.

## Installation

### Prerequisites

- [Node.js](https://nodejs.org/) (>=14)
- npm (comes with Node.js)

### Development Setup

```bash
# Clone the repository
git clone https://github.com/seongmini/sticky-markdown-note.git
cd sticky-markdown

# Install dependencies
npm install

# Run in development mode
npm start
```

### Building for Windows
```bash
# Generate installer and unpacked app in the `dist` folder
npm run dist
```

After buildilng, you'll find:

- **Sticky Note Setup.exe** ─ the installer.
- **win-unpacked/** ─ the portable executable folder you can copy around.

## Usage

1. **Launch** the app. The **Memo List** window shows all your notes.
2. Click **➕ New note** or press the shortcut to create a new note.
3. Select a note in the list to open it in its own window.
4. Edit text on the left; preview appears on the right.
5. Use search or shortcuts to navigate and manage notes.

## Configuration

You can customize default font sizes and theme via a `.env` file in your user data path:

```dotenv
FONT_SIZE_DEFAULT=16
FONT_SIZE_MIN=8
FONT_SIZE_MAX=40
THEME=LIGHT # or dark
```

## Keyboard Shortcuts

### Global (any window)

| Shortcut   | Action                                                    |
| ---------- | --------------------------------------------------------- |
| **Ctrl+P** | Switch to **Both** view mode                              |
| **Ctrl+O** | Toggle between **Editor Only** and **Preview Only** modes |
| **Ctrl+M** | Open the **Memo List** window                             |

### In Note Editor Window

| Shortcut               | Action                                   |
| ---------------------- | ---------------------------------------- |
| **Ctrl+N** / **Cmd+N** | Create a **New Note**                    |
| **Ctrl+B**             | **Bold** formatting (`**text**`)         |
| **Ctrl+I**             | *Italic* formatting (`*text*`)           |
| **Ctrl+\`**            | Inline `code` formatting                 |
| **Ctrl+K**             | Insert code block (`\n code \n`)         |
| **Ctrl+Q**             | Blockquote (`> `)                        |
| **Ctrl+H**             | Heading (`# `)                           |
| **Ctrl+Shift+S**       | ~~Strikethrough~~ (`~~text~~`)           |
| **Ctrl+L**             | Create or edit **Link** (`[text](url)`)  |
| **Ctrl+Shift+L**       | Bullet list (`- item`)                   |
| **Ctrl+Shift+O**       | Numbered list (`1. item`)                |
| **Ctrl+Shift+C**       | Toggle task checkbox (`- [ ]` / `- [x]`) |
| **Tab**                | Indent line(s)                           |
| **Shift+Tab**          | Outdent line(s)                          |
| **Ctrl + Mouse Wheel** | Increase / decrease font size            |

### In Memo List Window

| Shortcut               | Action                     |
| ---------------------- | -------------------------- |
| **Ctrl+N** / **Cmd+N** | Create a **New Note**      |
| **Ctrl+F** / **Cmd+F** | Focus the **Search** input |

### Theme Toggle

| Control         | Action                                       |
| --------------- | -------------------------------------------- |
| 🌗 Theme button | Toggle between **Light** and **Dark** themes |

## Support

If you find this app useful, consider supporting its development:

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/notemad)

### License

This project is licensed under the [MIT License](LICENSE).
