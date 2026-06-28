# tmux-dot-config

# 🚀 My Minimal tmux Configuration

A clean and minimal **tmux** configuration focused on productivity. No plugins, no unnecessary status bar widgets—just the essentials.

---

## ✨ Features

* 🔑 Prefix key: `\`
* 🖱️ Mouse support
* 📂 Window numbering starts at **1**
* 🔄 Automatic window renumbering
* 📜 50,000 lines of scrollback history
* ⌨️ Vim-style copy mode
* 🎨 Minimal dark theme
* 📍 Status bar at the **top**
* 🔲 Easy pane management
* 📐 Quick pane resizing
* 🔄 Instant configuration reload

---
## Installing `fzf`

### Debian / Ubuntu / Kali

```bash
sudo apt update
sudo apt install -y fzf
```

### Arch Linux / Manjaro / EndeavourOS

```bash
sudo pacman -S fzf
```

### Fedora

```bash
sudo dnf install fzf
```

### RHEL / CentOS (EPEL)

```bash
sudo dnf install epel-release
sudo dnf install fzf
```

### openSUSE

```bash
sudo zypper install fzf
```

### Alpine Linux

```bash
sudo apk add fzf
```

### Void Linux

```bash
sudo xbps-install -S fzf
```

### Gentoo

```bash
sudo emerge --ask app-shells/fzf
```

### NixOS

```bash
nix-env -iA nixpkgs.fzf
```

### Verify Installation

```bash
fzf --version
```
---

# ⌨️ Keybindings

> **Leader (Prefix):** `\`

Every shortcut below starts with the **Leader** key.

Example:

```text
\ + v
```

means:

1. Press `\`
2. Release it
3. Press `v`

---

# 📂 Pane Management

| Shortcut | Action              |
| -------- | ------------------- |
| `\ v`    | Split Left / Right  |
| `\ h`    | Split Top / Bottom  |
| `\ h`    | Move to Left Pane   |
| `\ j`    | Move to Bottom Pane |
| `\ k`    | Move to Upper Pane  |
| `\ l`    | Move to Right Pane  |

---

# 📏 Resize Panes

| Shortcut | Action       |
| -------- | ------------ |
| `\ H`    | Resize Left  |
| `\ J`    | Resize Down  |
| `\ K`    | Resize Up    |
| `\ L`    | Resize Right |

*(Uppercase means hold **Shift**.)*

---

# 🪟 Layout

| Shortcut | Action                              |
| -------- | ----------------------------------- |
| `\ t`    | Arrange all panes in a tiled layout |

---

# 🔄 Reload Configuration

| Shortcut | Action                |
| -------- | --------------------- |
| `\ r`    | Reload `~/.tmux.conf` |

No need to restart tmux after making changes.

---

# Status bar toggle
| Shortcut | Action                    |
| -------- | --------------------------|
| `\ b`    | status bar enable/disable |

---
# Popup window
| Shortcut | Action                            |
| -------- | ----------------------------------|
| `\ Space`| open default shell on popup window|
|`\ w`     | show window list on popup window  |
# 🖱️ Mouse Support

Mouse support is enabled.

You can:

* Click to select panes
* Resize panes by dragging borders
* Scroll through terminal history
* Select windows using the mouse

---

# 📜 Copy Mode

Copy mode uses **Vim** keybindings.

Enter copy mode using tmux's default key:

```text
\ [
```

Useful keys inside copy mode:

| Key     | Action          |
| ------- | --------------- |
| `h`     | Left            |
| `j`     | Down            |
| `k`     | Up              |
| `l`     | Right           |
| `gg`    | Top             |
| `G`     | Bottom          |
| `/`     | Search          |
| `n`     | Next match      |
| `Space` | Start selection |
| `Enter` | Copy selection  |
| `q`     | Exit copy mode  |

---

# 🎨 Appearance

* Status bar at the top
* Minimal dark color scheme
* Highlighted active window
* Highlighted active pane border
* No clock
* No hostname
* No CPU or RAM widgets
* No unnecessary information

---

# 📚 Useful tmux Commands

Create a new session:

```bash
tmux
```

Create a named session:

```bash
tmux new -s work
```

List sessions:

```bash
tmux ls
```

Attach to a session:

```bash
tmux attach -t work
```

Detach from a session:

```text
\ d
```

Kill current session:

```bash
tmux kill-session
```

Kill tmux completely:

```bash
tmux kill-server
```

---

# 💡 Tips

* Every pane runs independently.
* Closing a pane does **not** affect the others.
* Sessions continue running after you detach.
* Perfect for SSH, development, and penetration testing.

