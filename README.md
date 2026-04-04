# dotfiles

## Setup

```bash
stow git tmux zsh starship sheldon alacritty
```

Install list

git
stow

neovim

tmux

zsh
starship
sheldon
zoxide
delta
fzf

alacritty
JetBrainsMono Nerd Font


## Alacritty

Download catppuccin mocha theme:

```bash
curl -o ~/.config/alacritty/catppuccin-mocha.toml \
  https://raw.githubusercontent.com/catppuccin/alacritty/main/catppuccin-mocha.toml
```

## Neovim

```

```

## Notes

- **zsh** is not XDG compliant — `~/.zshenv` is unavoidable, used to set `ZDOTDIR` to redirect config into `~/.config/zsh/`
- **stow** is not XDG compliant — `.stowrc` must live in `$HOME` or the stow directory

## Future

- Consider nushell as an alternative shell
