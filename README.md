# zshrc

This repository contains my personal **Zsh configuration**, based on the [zensh](https://github.com/dreamsofautonomy/zensh) setup featured on the *Dreams of Autonomy* YouTube channel.

## Prerequisites

> [!NOTE]
> Before installing, make sure you have:
>
> - `zsh`
> - `fzf`
>
> ### Ubuntu
> ```bash
> sudo apt install zsh
> sudo apt install fzf
> ```
> ### Arch
> ```bash
> sudo pacman -S zsh
> sudo pacman -S fzf
> ```
### Make zsh default shell
```bash
chsh -s $(which zsh)
```

### Install Nerd Fonts
```bash
sudo apt install fonts-jetbrains-mono
```

### Run zsh
```bash
zsh
```

After Logout and login zsh will be the default terminal.

## Installation

Copy the contents of `.zshrc` from this repo or do the following:

1. Clone this repository:
   ```bash
   git clone https://github.com/notsoeazy/zshrc.git
   cd zshrc
   ```
2. Copy the `.zshrc` file to your home directory:
    ```bash
    cp ./.zshrc ~/
    ```
3. Open a new terminal to initialize the setup.

## Post-installation

1. Run `p10k configure` to customize the look and feel.
2. Copy your `.bash_history` to `zsh_history`

### Features / Keybinds
1. **History Search** `CTRL+R`
2. **Tab Completion** `TAB`
3. **Go into Directory** `ALT+C`
4. **Previews** `cd` `cp` `mv`

### Transfer environment variables / PATH exports
If you have custom settings in your old ~/.bashrc (e.g. for Ruby, Go, MIME types, etc.), move them into your Zsh config `.zshrc`. For example:

```bash
# Ruby
export PATH="$HOME/.rbenv/bin:$PATH"
eval "$(rbenv init - zsh)"
```

## Thank you!
