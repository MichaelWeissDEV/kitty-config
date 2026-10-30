# Installation

This guide covers installing the **Kitty** terminal emulator, securing font requirements, and deploying this configuration.

For managed Arch installation, backups and updates, see {doc}`packages`.
The following standalone setup is a separate alternative.

---

## Prerequisites

1. **Kitty terminal emulator**: Version 0.28 or newer.
2. **Nerd Font**: `JetBrainsMono Nerd Font` for status icons, Neovim file tree symbols, and Powerline glyphs.
3. **Shell**: Configured to spawn `/usr/bin/zsh`.

---

## Installing Kitty

### Arch Linux

```bash
sudo pacman -Syu --needed kitty ttf-jetbrains-mono-nerd zsh
```

### macOS

Using Homebrew:

```bash
brew install --cask kitty font-jetbrains-mono-nerd-font
```

### Debian / Ubuntu

```bash
sudo apt-get update
sudo apt-get install -y kitty fonts-jetbrains-mono zsh
```

---

## Deploying the Configuration

### Route A: Standalone Setup

Clone the repository directly into your XDG configuration directory:

```bash
# Backup any existing configuration
[ -d ~/.config/kitty ] && mv ~/.config/kitty ~/.config/kitty.bak

# Clone kitty-config
git clone https://github.com/MichaelWeissDEV/kitty-config.git ~/.config/kitty
```

### Route B: Inside the Arch Dotfiles Hub

Kitty is distributed as the independent `arch-dotfiles-kitty` package.
See {doc}`packages` for installation and signed `pacman -Syu` updates.

---

## Verification

Launch Kitty from your terminal or desktop launcher:

```bash
kitty
```

Verify visual characteristics:
1. Terminal background renders with `0.90` opacity and Catppuccin Mocha slate tone (`#1e1e2e`).
2. An unblinking Rosewater block cursor appears.
3. Opening multiple tabs (<kbd>Ctrl+Shift+T</kbd>) renders the Catppuccin Powerline tab bar.

---

## Rollback & Uninstall

For packages, deactivate with `arch-dotfiles-config deactivate kitty` before
removal; see {doc}`packages`. For a standalone clone, review and move it aside
before restoring your own backup. Do not delete personal configuration blindly.
