## doc-highlight.nvim

A neovim plugin for LSP Document Highlight. Automatically highlighting other references of the word 
under the cursor by LSP. 

## Demo
![doc-highlight](https://github.com/user-attachments/assets/8b74c1d0-754e-40a7-8b01-cac3165aa7bc)


## Features

- Automatically highlighting other references of the word under the cursor.
- Reduce flicker and LSP requests when move the cursor in the references.

## Installation

<details>
<summary>with <a href="https://neovim.io/doc/user/pack/#_plugin-manager">vim.pack</a></summary>

```
vim.pack.add({ "https://github.com/allworldg/doc-highlight" }, { confirm = false })
```

</details>

<details>
<summary>with <a href="https://github.com/folke/lazy.nvim">lazy.nvim</a></summary>

```
{"allworldg/doc-highlight"}
```

</details>

<details>
<summary>copy</summary>

This plugin code is very simple, and all the code is in the `lua/doc-highlight.lua`, so you can easily just copy code
and put it in your config.

</details>

**Remember to call** `require("doc-highlight").setup()` to enable it.

## Highlight Groups

### DocHighlight

Highlight group used for references.
`vim.api.nvim_set_hl(0,'DocHighlight',{bg=xxx,fg=xxx})`


## Similar plugins
- Builtin document highlight in Neovim, see `:h vim.lsp.buf.document_highlight()`
- <a href="https://github.com/RRethy/vim-illuminate">vim-illuminate</a>

