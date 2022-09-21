# retrieve.nvim
retrieve.nvim is all about "returning instantly". The plugin provides mappings to easily set an anchor and return to the anchor.

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
In this example, you can set an anchor with "m" and return to the anchor with "M".

```lua
require("retrieve")
vim.keymap.set("n", "m", "<Plug>retrieve-set", {noremap = false})
vim.keymap.set("n", "M", "<Plug>retrieve-return", {noremap = false})
```
