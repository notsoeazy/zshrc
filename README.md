# zshrc

This repository contains my personal **Zsh configuration**, based on the [zensh](https://github.com/dreamsofautonomy/zensh) setup featured on the *Dreams of Autonomy* YouTube channel.

## Prerequisites

Before installing, make sure you have:

- `zsh`
- `fzf`

### Ubuntu
```bash
sudo apt install zsh
sudo apt install fzf
```
### Arch
```bash
sudo pacman -S zsh
sudo pacman -S fzf
```
### Make zsh default shell
```bash
sudo chsh -s $(which zsh)
```
Logout and login for it to take effect.
## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/zshrc.git
   cd zshrc
   ```
2. Move or copy the `.zshrc` file to your home directory:
    ```bash
    mv ./.zshrc ~/
    ```
3. Open a new terminal to initialize the setup.

## Post-installation

Run `p10k cofigure` to customize the look and feel.

### Features / Keybinds
1. **History Search** `CTRL+R`
2. **Tab Completion** `TAB`
3. **Go into Directory** `ALT+C`
4. **Previews** `cd` `cp` `mv`

### Transfer environment variables / PATH exports
If you have custom settings in your old ~/.bashrc or ~/.bash_profile (e.g. for Ruby, Go, MIME types, etc.), move them into your Zsh config `.zshrc`. For example:

```bash
# Ruby
export PATH="$HOME/.rbenv/bin:$PATH"
eval "$(rbenv init - zsh)"
```

## Thank you!