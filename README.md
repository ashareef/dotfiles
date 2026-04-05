# dotfiles

## Setup

First, stow the `.stowrc` config so stow uses the correct options for all subsequent commands:

```bash
stow stow
```

Then stow everything else:

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

rust (via rustup: `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`, run after stow zsh — rustup appends to `~/.zshenv`)

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
