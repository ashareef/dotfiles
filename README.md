# dotfiles

## Setup

First, stow the `.stowrc` config so stow uses the correct options for all subsequent commands:

```bash
stow stow
```

Then stow everything else:

```bash
stow git tmux zsh starship alacritty
```

## Install list

- git
- stow
- neovim
- tmux + [TPM](https://github.com/tmux-plugins/tpm) (plugins install automatically on first launch)
- zsh
- starship
- zoxide
- delta
- fzf
- rust (via rustup: `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`, run after stow zsh — rustup appends to `~/.zshenv`)
- alacritty (GUI — install on host OS, not inside a remote/container environment)
- JetBrainsMono Nerd Font (install on host OS)

### zsh plugins (no plugin manager)

Clone directly into `~/.local/share/zsh/plugins/`:

```bash
git clone --depth=1 https://github.com/zsh-users/zsh-autosuggestions ~/.local/share/zsh/plugins/zsh-autosuggestions
git clone --depth=1 https://github.com/zsh-users/zsh-syntax-highlighting ~/.local/share/zsh/plugins/zsh-syntax-highlighting
```

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
