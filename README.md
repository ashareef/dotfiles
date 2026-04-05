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

- [git](https://git-scm.com/)
- [stow](https://www.gnu.org/software/stow/)
- [neovim](https://neovim.io/)
- [tmux](https://github.com/tmux/tmux) + [TPM](https://github.com/tmux-plugins/tpm) (plugins install automatically on first launch)
  - [tmux-resurrect](https://github.com/tmux-plugins/tmux-resurrect)
  - [tmux-continuum](https://github.com/tmux-plugins/tmux-continuum)
  - [catppuccin/tmux](https://github.com/catppuccin/tmux)
- [zsh](https://www.zsh.org/)
- [starship](https://starship.rs/)
- [zoxide](https://github.com/ajeetdsouza/zoxide)
- [delta](https://github.com/dandavison/delta)
- [fzf](https://github.com/junegunn/fzf)
- [rust](https://www.rust-lang.org/) (via [rustup](https://rustup.rs/): `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`, run after stow zsh — rustup appends to `~/.zshenv`)
- [alacritty](https://alacritty.org/) (GUI — install on host OS, not inside a remote/container environment)
- [JetBrainsMono Nerd Font](https://www.nerdfonts.com/) (install on host OS)

### zsh plugins (no plugin manager)

Clone directly into `~/.local/share/zsh/plugins/`:

```bash
git clone --depth=1 https://github.com/zsh-users/zsh-autosuggestions ~/.local/share/zsh/plugins/zsh-autosuggestions
git clone --depth=1 https://github.com/zsh-users/zsh-syntax-highlighting ~/.local/share/zsh/plugins/zsh-syntax-highlighting
```

- [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)
- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

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
