# Dotfiles

These are my dotfiles. I primarily use **Arch Linux**, but from time to time, I’ve been known to use **Arco**, **Manjaro**, or another Arch-based distro. **Solus** is also dope, although it doesn't need much configuration. I also run **Debian** or **Ubuntu** on a few server systems, so I ensure my dotfiles work there as well. And, on the rare occasion, I use a **MacBook**, where most of these dotfiles also work without issue.

---

## Main Things Here

- **Neovim** configuration.
- **Zsh** configuration.
- **Window manager** configuration.
- **Alacritty** configuration.
- **Polybar** configuration.
- **Ranger** configs.

---

## My Setup

Currently, my primary system is **Arch Linux** running on a **Ryzen 5 2600X (6-core)** CPU with a **GTX 1050Ti**. I use the **Awesome Window Manager** as my window manager (yes, it's paired with Polybar because I like it that way — don't judge). Though I do enjoy **DWM** and **BSPWM**, **Awesome** has my heart. For transparency effects, I use **iBhagwan's Picom Fork**.

My terminal of choice is **Alacritty** (with **kitty** or **st** as a backup), and **Neovim** is my go-to text editor. 

Here’s a quick breakdown:

- **Window Manager**: Awesome WM (with Polybar)
- **Terminal**: Alacritty (kitty or st as backup)
- **Editor**: Neovim
- **Compositor**: iBhagwan's Picom Fork
- **System**: Arch Linux (on Ryzen 5 2600X, GTX 1050Ti)
  
You can view all of my dotfiles [here](https://github.com/elijahu1/dot).

---

## Quick Start

If you want to use these dotfiles, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/elijahu1/dot.git
   cd dot
   ```

2. **Backup Your Current Configs**:
   ```bash
   mkdir ~/.config-backup
   mv ~/.config/* ~/.config-backup/
   ```

3. **Create Symlinks**:
   ```bash
   ln -s $(pwd)/polybar ~/.config/polybar
   ln -s $(pwd)/neovim ~/.config/nvim
   ln -s $(pwd)/zsh ~/.config/zsh
   ```

4. **Install Dependencies**:
   Install **Neovim**, **Zsh**, **Alacritty**, and **Polybar** if you don’t have them already.
   ```bash
   sudo pacman -S neovim zsh alacritty polybar
   ```

5. **Start Polybar**:
   ```bash
   ~/.config/polybar/launch.sh
   ```

---

## License

Feel free to use, modify, and distribute these dotfiles. Attribution is appreciated, but not required. 🚀

---

### 🌟 Stay Awesome

"Arch Linux: I break it, I fix it, and it works better each time." 😎
```
