vim-react-snippets
==================

A direct port of the awesome snippets from 
[jgebhardt/sublime-react](https://github.com/jgebhardt/sublime-react)
to work with Vim.

Requires [vim-snipmate](https://github.com/garbas/vim-snipmate).

Installation
============

Use your preferred Vim plugin installation method.
I like [Vundle](http://github.com/gmarik/vundle), but other options like
[pathogen](https://github.com/tpope/vim-pathogen) should work fine as well.

If you're using Vundle, and you don't currently have SnipMate, you will need to
add the following to your `.vimrc` (taken from the [SnipMate README](https://github.com/garbas/vim-snipmate/blob/master/README.md)):

```
" vim-react-snippets:
Bundle "justinj/vim-react-snippets"

" SnipMate and its dependencies:
Bundle "MarcWeber/vim-addon-mw-utils"
Bundle "tomtom/tlib_vim"
Bundle "garbas/vim-snipmate"

" Other sets of snippets (optional):
Bundle "honza/vim-snippets"
```
