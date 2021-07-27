# deoplete-snippy

[Snippy](https://github.com/dcampos/nvim-snippy) source and integration for
[Shougo/deoplete.nvim](https://github.com/Shougo/deoplete.nvim)

## Install

Using vim-plug:

```viml
Plug 'dcampos/deoplete-snippy'
```

## Usage

To have snippets expanded after completion without the need to press `Tab` or
whichever key you use to expand snippets normally, you may set up an `autocmd` for
expanding it automatically:

```viml
augroup vimrc
    autocmd!
    autocmd vimrc CompleteDone * call deoplete#snippy#try_expand()
augroup END
```
