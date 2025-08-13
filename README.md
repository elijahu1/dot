---

# 🖥️ My Dotfiles

Welcome to my personal collection of **dotfiles** — the configs that make my systems feel like *home*.

I live in **Arch Linux** land most of the time, but I occasionally roam into **Arco**, **Manjaro**, or other Arch-based distros.
On servers, I run **Debian** or **Ubuntu** (sometimes **RHEL**), keeping these configs as portable as possible.
Yes, they even run fine on laptops when I have to step away from the battle station.

---

## 📦 What’s Inside

* **Neovim** – my main text editor.
* **Zsh** – shell with custom aliases and theming.
* **AwesomeWM** – my daily driver window manager.
* **Alacritty** – terminal of choice (with Kitty and ST on standby).
* **Polybar** – status bar with my tweaks.
* **Ranger** – terminal file manager configs.

---

## 🖤 My Daily Setup

* **OS:** Arch Linux (Ryzen 5 2600X, GTX 1050Ti)
* **WM:** AwesomeWM + Polybar (yes, I run them together — fight me)
* **Terminal:** Alacritty
* **Editor:** Neovim
* **Compositor:** [iBhagwan’s Picom fork](https://github.com/ibhagwan/picom)
* **Backup WMs:** DWM, BSPWM (but Awesome always wins)

---

## 🚀 Quick Start

**1. Clone the repo**

```bash
git clone https://github.com/elijahu1/dot.git
cd dot
```

**2. Backup your current configs** *(optional but smart)*

```bash
mkdir ~/.config-backup
mv ~/.config/* ~/.config-backup/
```

**3. Symlink what you need**

```bash
ln -s $(pwd)/polybar ~/.config/polybar
ln -s $(pwd)/nvim ~/.config/nvim
ln -s $(pwd)/zsh ~/.config/zsh
```

**4. Install dependencies** *(Arch example)*

```bash
sudo pacman -S neovim zsh alacritty polybar
```

**5. Launch Polybar**

```bash
~/.config/polybar/launch.sh
```

---

## 📜 License

Use, modify, and share freely. Attribution is appreciated but not required.

---

> 🐧 *Arch BTW.*
> Configured for speed, minimalism, and a touch of personal chaos.


