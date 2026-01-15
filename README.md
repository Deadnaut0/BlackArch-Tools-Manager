# 🖤 BlackArch Tools Manager


A **fully interactive, GUI-style terminal launcher** for **BlackArch Linux tools**, built with `bash + fzf`.

Browse **hundreds of BlackArch tools by category**, view **full package descriptions**, **install / uninstall / run tools**, manage **favorites**, and launch tools in **floating terminals** — all without memorizing commands.

> Designed for **Hyprland / Wayland users**, but works on any Arch-based BlackArch setup.

## Showcase


https://github.com/user-attachments/assets/a9c8aa97-df12-47a2-ae9b-f5f21b62962e


https://www.youtube.com/watch?v=PxLzP1xjdSI




---

## ✨ Features

### 📂 Category-Based Navigation

- Automatically loads **all BlackArch categories**
- Clean, emoji-enhanced category list
- No empty or broken categories

![](assets/tool-menu.png)

### 🔍 Search All Tools

- Search **every BlackArch tool** instantly
- Fuzzy matching powered by `fzf`

![](assets/favorite-recent.png)

### ⭐ Favorites System

- Mark tools as favorites
- Favorites persist across sessions
- ⭐ icon displayed next to favorite tools
- Dedicated **Favorites** category
![](assets/recent.png)

### 🕘 Recent Tools

- Automatically tracks recently used tools
- Quick access to last executed tools

### 📦 Install / Uninstall from GUI

- Install tools directly via `pacman`
- Uninstall cleanly with dependency removal
- Installed tools detected automatically
![](assets/installing.png)
### 🧠 Full Tool Information

- Scrollable **full package descriptions**
- Uses `pacman -Si`
- Preview pane supports long descriptions

![](assets/tool-menu.png)

### 🔧 Tool Actions Menu
- After selecting a tool, choose to:
  - Run in floating terminal
  - Open pre-filled command terminal
  - Install / Uninstall
  - Open tool homepage
  - Add / Remove from favorites
![when tool is not installed](assets/action-menu1.png)
![when tool is installed](assets/action-menu2.png)
### 🚀 Run Tools in Floating Terminal

- Tools run inside a **floating Kitty terminal**
- Terminal stays open after execution
- Password prompt handled correctly

![](assets/run-directly.png)

### ⚡ Open Pre-Filled Command Terminal

- Opens terminal with:

  ```bash
  sudo toolname
  ```

- Editable before execution
- Perfect for tools with arguments

![](assets/run-tools.png)
### 🌐 Open Tool Homepage

- Automatically extracts tool URL
- Opens in default browser

---

## 🖥 UI Preview (fzf GUI)

- Full-height interface
- Scrollable previews
- ANSI colors + icons
- Keyboard-only workflow
- No mouse required

> **Feels like a GUI, runs in the terminal.**

---

## ⌨ Keybindings

| Key | Action |
|-----|--------|
| `Enter` | Select / Confirm |
| `Esc` | Go back |
| `↑` `↓` | Navigate |
| `/` | Fuzzy search |
| `Tab` | Cycle selections |

> Favorites are managed from the Action Menu.

---

## 📁 Configuration Files

All user data is stored safely in:

```
~/.config/blackarch-tools-script/
```

| File | Purpose |
|------|---------|
| `favorites.conf` | Favorite tools |
| `recent.conf` | Recently used tools |
| `installed_tools.cache` | Installed tools cache |

> No system files are modified.

---

## 📦 Requirements

- **BlackArch Linux** (Arch-based)
- `fzf`
- `pacman`
- `kitty` terminal
- `hyprctl` (for floating windows)
- `notify-send`

### Install dependencies

```bash
sudo pacman -S fzf kitty libnotify
```

---

## 🚀 Usage

Make the script executable:

```bash
chmod +x blackarch-tool-manager
```

Run it:

```bash
./blackarchtool-manager
```

**That's it.**  
No arguments. No config needed.

---

## 🧠 Why This Exists

BlackArch has thousands of tools, but:

- Names are hard to remember
- Categories are fragmented
- Descriptions are rarely read
- Running tools closes terminals
- Favorites don't exist

**This launcher fixes that.**

---

## 🛡 Safety Notes

- Uses `sudo` only when required
- No background services
- No telemetry
- No external APIs
- Fully local & transparent

---

## 🧩 Customization

You can easily:

- Change terminal (`TERM="kitty"`)
- Add/remove categories
- Modify floating window size
- Adjust preview layout

> Script is cleanly structured and modifiable.

---

## 🤝 Contributing

PRs are welcome:

- New features
- Performance improvements
- UX polish
- Compatibility fixes

---

## 🧑‍💻 Author

Created by **Deadnaut**  
Built for hackers who want speed without losing clarity.

---

## 🖤 License

**MIT License**  
Use it. Fork it. Improve it.
