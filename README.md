## doc-highlight.nvim
A neovim plugin for LSP Document Highlight. Automatically highlighting other references of the word 
under the cursor by LSP. 

## Demo


## Features
- Automatically highlighting other references of the word.
- Reduce flicker and lsp requests when move the cursor in the references.

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
<details>

<summary>Copy</summary>

This plugin code is very simple, and all the code is in the `lua/doc-highlight.lua`, so you can easily copy  
and put it in your config.

</details>

</details>

**Remember to call** `require("require("doc-highlight").setup())` to enable it.


## Highlight Groups

## DocHighlight
Highlight group used for references.
`vim.api.nvim_set_hl(0,'DocHighlight',{bg=xxx,fg=xxx})`


## Similar plugins
- Builtin document highlight in Neovim, see `:h vim.lsp.buf.document_highlight()`
- <a href="https://github.com/RRethy/vim-illuminate">vim-illuminate</a>

