# 🐱 Kitty Terminal Configuration

A personal [Kitty Terminal](https://sw.kovidgoyal.net/kitty/) configuration adjusted to personal preferences.

## ✨ Features

### 🎨 **Visual & Theming**
- **Catppuccin Mocha** color scheme for beautiful, eye-friendly colors
- **VictorMono Nerd Font** with ligature support
- **Hidden tab bar** for clean, distraction-free interface
- **Optimized window sizing** and padding for better aesthetics

### ⚡ **Performance Optimizations**
- **Disabled cursor blinking** for better performance
- **Optimized repaint delays** (10ms) and input delays (3ms)
- **Monitor sync enabled** for smooth display
- **Extended scrollback** (10,000 lines) for comprehensive history

### 🛠️ **Development Integration**
- **Fish shell integration** with automatic setup
- **Tmux optimization** with remote control support
- **Neovim integration** as default editor
- **Wayland support** for modern Linux environments

### 🖱️ **Enhanced Interaction**
- **Copy-on-select** for convenient clipboard usage
- **Smart trailing space stripping**
- **Optimized URL detection** with theme-matching colors
- **Silent operation** (audio bell disabled)

## 📁 Project Structure

```
├── kitty.conf              # Main configuration file
├── catppuccin-mocha.conf   # Custom Catppuccin Mocha theme
├── diff.conf               # Diff configuration
└── README.md               # This file
```

## 🚀 Quick Start

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/MikePapaSierra/kitty.git ~/.config/kitty
   ```

2. **Install required font (optional but recommended):**
   ```bash
   # Arch/Manjaro
   sudo pacman -S ttf-victormono-nerd
   
   # Ubuntu/Debian
   sudo apt install fonts-victormono
   ```

3. **Restart Kitty** to apply the configuration

### Verification

Use the included validation tools:
```bash
# Check configuration syntax
kitty --check-config

# List available fonts
kitty +list-fonts | grep -i victor
```

## ⚙️ Configuration Highlights

### Core Optimizations
- **Font**: VictorMono NFM Medium, 12pt
- **Cursor**: Block shape, no blinking
- **Scrollback**: 10,000 lines
- **Shell Integration**: Enabled for Fish shell
- **Tab Management**: Completely disabled (Tmux-focused workflow)

### Keyboard Shortcuts
- `Ctrl+Shift+Plus/Minus` - Adjust font size
- `Ctrl+Shift+Backspace` - Reset font size
- `Ctrl+Shift+F5` - Reload configuration

### Theme Integration
The configuration uses a custom Catppuccin Mocha theme that provides:
- Consistent color palette across all UI elements
- Proper contrast ratios for accessibility
- Integration with popular development tools

## 🎯 Target Workflow

This configuration is optimized for developers using:
- **Linux** (Arch, Ubuntu, Fedora, etc.)
- **Fish Shell** for interactive usage
- **Tmux** for terminal multiplexing
- **Neovim/Vim** for text editing
- **Modern development tools** (Git, Docker, etc.)

## 📋 System Requirements

- **Kitty Terminal** 0.21.0 or newer
- **Linux** operating system (Wayland or X11)
- **Fish Shell** (optional, but recommended)
- **VictorMono Nerd Font** (optional, fallback fonts available)

## 🔧 Customization

### Changing Fonts
Edit `font_family` in `kitty.conf`:
```conf
font_family      Your Preferred Font
font_size        12.0
```

### Adjusting Colors
Modify colors in `catppuccin-mocha.conf` or create your own theme file.

### Performance Tuning
Adjust performance settings in the optimization section of `kitty.conf`:
```conf
repaint_delay 10
input_delay 3
sync_to_monitor yes
```

## 📝 License & Usage

### 📖 **License**
This project is released under the **MIT License**. See the repository for full license terms.

### 🍴 **Forking Policy**
- ✅ **Forks are welcome and encouraged!** 
- ✅ Feel free to adapt this configuration for your needs
- ✅ Share your improvements with the community
- ❌ **Contributions to this repository are not accepted**
- ❌ This is a personal configuration project

### 🙏 **Attribution**
While not required, attribution is appreciated if you use this configuration as a base for your own setup.

## 🔗 Related Projects

- [Kitty Terminal](https://sw.kovidgoyal.net/kitty/) - Fast, feature-rich terminal emulator
- [Catppuccin](https://catppuccin.com/) - Soothing pastel theme for developers
- [VictorMono](https://rubjo.github.io/victor-mono/) - Programming font with cursive italics
- [Fish Shell](https://fishshell.com/) - Smart and user-friendly command line shell
- [Tmux](https://github.com/tmux/tmux) - Terminal multiplexer

## 📞 Support

For questions about Kitty terminal itself, please refer to the [official Kitty documentation](https://sw.kovidgoyal.net/kitty/). Please note that I do not support any issues specyfic to this configuraiton.

---
