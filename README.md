# Dotfiles for Linux

Dotfiles managed by GNU Stow

## Installation

Warning: This will override any existing configuration you have

```sh
git clone --depth=1 https://github.com/PlatyPew/dotfiles-linux.git ~/dotfiles && \
    cd ~/dotfile && stow -v --adopt */ && git restore .
```
