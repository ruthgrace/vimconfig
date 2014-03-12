My Vim Configuration
====================

Initial Setup
-------------

Clone this repository to `~/.vim`

```bash
git clone https://github.com/jeffshantz/vimconfig.git ~/.vim
```

Install `vundle`:

```bash
git clone https://github.com/gmarik/vundle.git ~/.vim/bundle/vundle
```

Install all bundles:

```bash
vim +BundleInstall +qall
```

RUTH ADDITION: install neocomplcache by following instructions from
https://github.com/Shougo/neocomplcache.vim/blob/master/README.md

Link `~/.vimrc` to `~/.vim/vimrc` (if necessary)

```bash
ln -s ~/.vim/vimrc ~/.vimrc
```

Features
--------

Some of the features of this configuration include:

* Forcing one to use `hjkl` navigation

* Powerline status bar

* Tabularize
  * Use `,a=` to align by `=`
  * Use `,a:` to align by `:`
  * Tabularize is called every time you type `|`, which is great for Cucumber tables

* Comment boxes
  * An 80-character comment box is inserted when you use `,cb #`, where `#` is the comment
    character to use.

* Snippets
  * Plenty of snippets in `.vim/bundle/vim-snippets/snippets/`
  * I added a few custom Java snippets that I use in my teaching:
    * `pc` - `public class ClassName { }`
    * `psvm` - `public static void main(String[] args) { }`
    * `psvmte` - `public static void main(String[] args) throws Exception { }`
    * `sop` - `System.out.println("text");`
  * Additional snippets can be added to the `.vim/snippets` directory

RUTH ADDITION - snippets are accessed by SHIFT-TAB, TAB is now simply autocomplete.

* `Ctrl-p` file navigation
