# NeoVim-Config
Personal NeoVim Configuration.

## NeoVim Installation

In order to download the latest version of `neovim`:
```
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim.appimage
chmod u+x nvim.appimage
./nvim.appimage
```

In order to create a shortcut as `nvim`:
```
sudo ln -s ./nvim.appimage /usr/bin/nvim
```

## Configuration Setup

In order to setup the current configuration, move the `init.lua` file to `~/.config/nvim/init.lua`

## Appendix A - `.zshrc` Setup

Additionaly, you can add the following lines to your `.zshrc` configuration file to enable autocompletion and *slash*-completion: 
```zsh
# Enable completion
autoload -U compinit
compinit

# Add a "/" after ".." when pressing Tab
zstyle ':completion:*' special-dirs true
export PATH="/usr/local/sbin:$PATH"
```
