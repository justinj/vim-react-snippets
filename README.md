vim-react-snippets
==================

A set of snippets for Vim to work with Facebook's
[React](http://facebook.github.io/react/) library. This fork change the snippet
syntax to ES6. Remove semicolon and comma. I also remove snippets related to
[react-classset](https://github.com/petehunt/react-classset) as it is deprecated now.

Require [UltiSnips](https://github.com/SirVer/ultisnips).
I only update the `UltiSnips` version. Pull requests for
[vim-snipmate](https://github.com/garbas/vim-snipmate) version are welcome.


Installation
============

Use your preferred Vim plugin installation method. For me, I like
[vim-plug](https://github.com/junegunn/vim-plug). If you also using `vim-plug`,
put the following into your `.vimrc`.

````vimrc
Plug 'SirVer/ultisnips'

" Currently, es6 version of snippets is available in es6 branch only
Plug 'letientai299/vim-react-snippets', { 'branch': 'es6' }

Plug 'honza/vim-snippets' "optional
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
getDefaultProps() {
    return {

    };
},
```

Another example:

```
rcx<Tab>
```

Expanding to

```
class ClassName extends React.Component {
  render(){
    return (

    )
  }
}
```

And a bunch of others!

Check `./UltiSnips/javascript.snippets` to see the full list.
