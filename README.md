
---

# 🖥️ Dotfiles — Arch Linux System Config

Personal dotfiles for a fast, minimal, and reproducible Linux desktop environment.

Primarily built for **Arch Linux**, but designed to stay portable across:
- Arch-based systems (Arco, Manjaro, EndeavourOS)
- Debian / Ubuntu servers
- occasional RHEL environments

This repo is focused on *practical system configuration*, not aesthetics for its own sake.

---

## 📦 What This Includes

### 🧠 Core Userland
- **Neovim** — primary editor
- **Zsh** — shell configuration, aliases, and prompt setup
- **Ranger** — terminal file manager

### 🪟 Desktop Environment
- **AwesomeWM** — main window manager
- **Polybar** — status bar setup
- **Picom (ibhagwan fork)** — compositor

### 🖥️ Terminal Stack
- **Alacritty** — primary terminal emulator

---

## ⚙️ System Philosophy

This setup is built around:

- Speed over decoration
- Minimal dependencies
- Manual control over automation magic
- Predictable, reproducible environment
- Arch-first, but portable when needed

---

## 🚀 Installation

### 1. Clone the repo

```bash
git clone https://github.com/elijahu1/dot.git
cd dot
````

---

### 2. Backup existing configs

```bash
mkdir -p ~/.config-backup
cp -r ~/.config/* ~/.config-backup/
```

---

### 3. Apply configs (manual symlink method)

```bash
ln -s $(pwd)/nvim ~/.config/nvim
ln -s $(pwd)/zsh ~/.config/zsh
ln -s $(pwd)/polybar ~/.config/polybar
ln -s $(pwd)/awesome ~/.config/awesome
ln -s $(pwd)/alacritty ~/.config/alacritty
```

---

### 4. Install dependencies (Arch Linux)

```bash
sudo pacman -S neovim zsh alacritty polybar awesome picom
```

---

### 5. Start session components

```bash
~/.config/polybar/launch.sh
```

---

## 🧪 Notes

* Some configs assume X11 (not Wayland-first)
* Polybar + AwesomeWM are intentionally paired
* Picom fork is used for performance tweaks and blur control
* Expect minor tweaks per machine (GPU, monitor setup, etc.)

---

## 📁 Repo Structure

```text
dot/
├── alacritty/
├── awesome/
├── nvim/
├── picom/
├── polybar/
├── ranger/
├── zsh/
├── .gitignore
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── SECURITY.md
```

---

## 📜 License

Licensed under **GNU AGPL v3.0**.

You are free to use, modify, and redistribute this configuration under the same license terms.

If you deploy or distribute modified versions, you must also make the source available.

---

## 🐧 Final Note

Arch doesn’t need perfection — it needs control.

This setup reflects that:
lean, direct, and always under your hands.

---

## 🤝 Contact

[hi@elijahu.me](mailto:hi@elijahu.me)

```

---

## 🧠 What you just achieved (important)

This version fixes 3 big problems:

### 1. Removes “blog energy”
Now it reads like:
> infra documentation, not personality showcase

### 2. Makes it reproducible
Someone can actually:
- clone
- install
- run

### 3. Makes Arch identity clear
Not distro-hopping confusion — Arch-first system base

---

## Next upgrade (optional but powerful)

If you want to level this repo up further, next step would be:

### ⚡ `install.sh` or `apply.sh`
- one command setup
- replaces manual symlinks
- detects OS (Arch vs Debian)

Or even:

### 🧠 `stow` migration
- clean modular dotfiles management
- industry-standard approach

---

