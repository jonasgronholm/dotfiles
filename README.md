# Dotfiles

Personal configuration files for my CachyOS Linux desktop.

## System

- **OS:** CachyOS (Arch-based)
- **WM:** Hyprland (JaKooLit dotfiles as base)
- **Bar:** Waybar
- **Terminal:** Alacritty
- **Shell:** Zsh with Powerlevel10k
- **GPU:** AMD Radeon 7900 XTX
- **CPU:** AMD Ryzen 9800 X3D

## Monitors

- 35" Ultrawide 1440p (primary)
- 27" 1440p portrait (secondary)

## Contents

- `hypr/UserConfigs/` — Hyprland personal configuration
- `waybar/` — Waybar configuration and modules
- `.zshrc` — Zsh configuration with Powerlevel10k

## Restore

1. Install CachyOS with Hyprland (JaKooLit installer)
2. Clone this repo
```bash
   git clone git@github.com:jonasgronholm/dotfiles.git
```
3. Copy Hyprland UserConfigs
```bash
   cp -r dotfiles/hypr/UserConfigs/* ~/.config/hypr/UserConfigs/
```
4. Copy Waybar config
```bash
   cp -r dotfiles/waybar/* ~/.config/waybar/
```
5. Copy zsh config
```bash
   cp dotfiles/.zshrc ~/.zshrc
```
6. Install zsh and set as default shell
```bash
   sudo pacman -S zsh
   chsh -s /usr/bin/zsh
```
7. Log out and back in

## Notes

- Hyprland config based on JaKooLit's Arch-Hyprland dotfiles
- Personal customizations in UserConfigs only
- LC_TIME set to sv_FI.UTF-8 for 24h time format
