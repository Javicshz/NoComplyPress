# Getting Started with VS Code

This guide will walk you through the basics of using **Visual Studio Code (VS Code)** for our NoComplyPress project. It’s our main editor, so knowing your way around will make everything easier.

---

## 1. Opening the Project

1. Launch **Visual Studio Code**.
2. Go to the menu bar and click:
   ```
   File → Open Folder...
   ```
3. Navigate to your local copy of the `NoComplyPress` folder and open it.

Now you'll see your project’s files and folders in the **Explorer sidebar** on the left.

---

## 2. Navigating Files in VS Code

- Click on folders to expand or collapse them
- Click on any `.md`, `.py`, `.html`, or `.css` file to open it in a tab
- You can open multiple files in split-screen by dragging tabs side by side
- Press `Cmd+P` (Mac) or `Ctrl+P` (Windows/Linux) to quickly search for files by name

---

## 3. Installing Extensions

Extensions add features like syntax highlighting, formatting, and autocomplete.

### How to Install:

1. Click the **Extensions icon** on the sidebar (or press `Cmd+Shift+X` / `Ctrl+Shift+X`)
2. In the search bar at the top, type the extension name
3. Click **Install**

---

## 4. Recommended Extensions for This Project

| Extension Name            | What It Does                                          |
|---------------------------|--------------------------------------------------------|
| **Python** (by Microsoft) | Syntax support, linting, debugging, venv detection     |
| **Flask Snippets**        | Quick snippets for Flask routes/templates              |
| **Live Server**           | Instantly preview HTML files in your browser           |
| **Prettier - Code Formatter** | Formats code consistently across HTML/CSS/JS/Python |
| **Markdown All in One**  | Adds live preview, shortcuts, TOC for Markdown files   |
| **GitLens**               | Shows Git history, blame, and change tracking          |
| **vscode-icons** (optional) | Adds colorful file icons to make the sidebar clearer |

> Tip: After installing, reload VS Code if prompted.

---

## 5. Customizing VS Code (Optional)

- **Settings** → `Cmd+,` or `Ctrl+,`
- Search for settings like:
  - Font size
  - Tab width (set to `4` spaces for this project)
  - Word wrap
- You can switch between **light/dark themes** from the command palette:
  ```
  View → Command Palette → “Color Theme”
  ```

---

## 6. Opening the Terminal

To use Git, Python, or run Flask:

- Go to:
  ```
  Terminal → New Terminal
  ```
- Or use the shortcut:
  - `Ctrl+` backtick (\`) on Windows
  - `Cmd+` backtick (\`) on Mac

This opens the terminal in the bottom panel inside your project folder.

---

## 7. Pro Tips

- You can pin frequently used files by right-clicking the tab and choosing **"Keep Open"**
- Use the **Outline view** (top of the sidebar) to jump around functions and headings
- `Cmd+Shift+F` or `Ctrl+Shift+F` lets you search *across all files* in the project

---

Now you're set up with VS Code! You’ll pick up new shortcuts and features as you work, so don’t worry about learning everything at once.
