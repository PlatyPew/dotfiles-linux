# Dotfiles for Linux

Dotfiles managed by GNU Stow

## Installation

Warning: This will override any existing configuration you have

```bash
git clone --depth=1 https://github.com/PlatyPew/dotfiles-linux.git ~/dotfiles && \
    cd ~/dotfiles && stow -v --adopt */ && git restore . && \
    zsh -c "source ~/.zshrc && zgenom update && fast-theme CONFIG:catppuccin-mocha && bat cache --build" && \
    ~/.tmux/plugins/tpm/scripts/install_plugins.sh && \
    nvim -c "lua require('lazy').restore({wait = true})" +qa
```
