# miasma.nvim-transparent

This is a clone of the [miasma.nvim](https://github.com/xero/miasma.nvim) colorscheme for Vim/Neovim. It’s currently behind the official repo in commits, so the original might have features this fork doesn’t. The main purpose of this fork is to add a transparency feature temporarily until the official plugin implements it.

The setup is the same as the original, with one extra line to enable transparent backgrounds. Here’s how to configure it with different plugin managers:

using `lazy`

```lua
{
  "khaled-chawa/miasma.nvim-transparent",
  lazy = false,
  priority = 1000,
  config = function()
    vim.g.miasma_transparent = 1 -- Enable transparency
    vim.cmd("colorscheme miasma")
  end,
}
```

using `plug`

```vim
Plug 'khaled-chawa/miasma.nvim-transparent'
let g:miasma_transparent = 1 -- Enable transparency
colorscheme miasma
```

using `packer`

```lua
use {
  "khaled-chawa/miasma.nvim",
  config = function()
    vim.g.miasma_transparent = 1 -- Enable transparency
    vim.cmd("colorscheme miasma")
  end
}
```
