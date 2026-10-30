# Kitty configuration

GPU-Terminal mit Catppuccin Mocha, Powerline-Tabs und Zsh.

**[Vollständige Dokumentation](https://kitty-config.readthedocs.io/en/latest/)** ·
[Arch-Paket](https://kitty-config.readthedocs.io/en/latest/packages/) ·
[Dotfiles-Handbuch](https://arch-dotfiles.readthedocs.io/en/latest/)

```bash
curl -fsSL https://raw.githubusercontent.com/MichaelWeissDEV/dotfiles/main/install.sh | bash -s -- kitty
```

Paket: `arch-dotfiles-kitty`. Einstellungen: `~/.config/kitty/kitty.conf`.
Konfiguration, Tastenkombinationen und Standalone-Installation stehen im Handbuch.
Hier unabhängig entwickeln und auf `main` pushen; nach erfolgreichem Registry-Build
mit `sudo pacman -Syu` aktualisieren. Lokale Builds: [PACKAGING.md](PACKAGING.md).

[![Package safety](https://github.com/MichaelWeissDEV/kitty-config/actions/workflows/package.yml/badge.svg)](https://github.com/MichaelWeissDEV/kitty-config/actions/workflows/package.yml)

[MIT-Lizenz](LICENSE).
