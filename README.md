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
