# NeoVim-Config
Personal NeoVim Configuration.

## Keyboard Shortcuts
* Toggle Diagnostics (disabled by default): `<Leader>e` (by default `<Leader>` is assigned to `\`)
* NvimTree Toggle (File Explorer, enabled by default): `<C-n>`
* Telescope File Finder: `<C-p>`
* Telescope Live Grep: `<C-f>`
* Within the autocomplete functions of the selected LSP-Server:
    - **N**ext Suggestion: `<C-n>`
    - **P**revious Suggestion: `<C-p>`
    - **U**p in the Suggestion Documentation: `<C-u>`
    - **D**own in the Suggestion Documentation: `<C-d>`

## NeoVim Installation

**(I suggest you rather follow the official installation steps)**

In order to download the latest version of `neovim`:
```zsh
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim.appimage
chmod u+x nvim.appimage
./nvim.appimage
```

In order to create a shortcut as `nvim`:
```zsh
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
