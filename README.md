vim-react-snippets
==================

A set of snippets for Vim to work with Facebook's [React](http://facebook.github.io/react/) library.

A direct port of the awesome snippets from 
[jgebhardt/sublime-react](https://github.com/jgebhardt/sublime-react).

Requires [vim-snipmate](https://github.com/garbas/vim-snipmate) or [Ultisnips](https://github.com/SirVer/ultisnips).

Installation
============

Use your preferred Vim plugin installation method.
I like [Vundle](http://github.com/gmarik/vundle), but other options like
[pathogen](https://github.com/tpope/vim-pathogen) should work fine as well.

####SnipMate

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
####Ultisnips

If you prefer to use `vim-react-snippets` with `Ultisnips`, put this in your .vimrc 
to install using Vundle

````
" vim-react-snippets:
Bundle "justinj/vim-react-snippets"

" Ultisnips
Bundle "SirVer/ultisnips"

" Other sets of snippets (optional):
Bundle "honza/vim-snippets"
````

Usage
=====

Within any Javascript or JSX file, you should be able to do the following:

(in insert mode)
```
gdp<Tab>
```

expanding to

```
getDefaultProps: function() {
    return {

    };
},
```

And a bunch of others!
Check `snippets/javascript.snippets` to see the full list.
