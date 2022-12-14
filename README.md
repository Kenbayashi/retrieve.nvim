# retrieve.nvim
retrieve.nvim is all about "returning instantly". The plugin provides mappings to easily set a mark and return to the mark.

## Installation
Install using your favorite package manager.

### Packer
```lua
use { "Kenbayashi/retrieve.nvim" }
```

### vim-plug
```lua
Plug 'Kenbayashi/retrieve.nvim'
```

### dein
```vim
call dein#add('Kenbayashi/retrieve.nvim')
```

## Usage
Call require("retrieve") and set keymaps.
In this example, you can set a mark with "m" and return to the mark with "M".

```lua
require("retrieve").setup()
vim.keymap.set("n", "m", "<Plug>retrieve-set", {noremap = false})
vim.keymap.set("n", "M", "<Plug>retrieve-return", {noremap = false})
```
