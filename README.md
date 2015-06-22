# tools
Small scripts I have found useful.

## genpasswd

Use /dev/random to generate random password of arbitrary length. For example,

```
genpasswd 25
```

generates a password of 25 characters. If no number is specified, it generates 8 characters.

## man2browser

Generates a `man` page in `HTML` format and shows it in the default web browser. For example,

```
man2browser 3 printf
```

shows the page for `printf` on section 3. Section is optional.

## mkvimball

Create a [VimBall](http://vim.sourceforge.net/scripts/script.php?script_id=1502) from command line.
Useful for Vim scripts published on GitHub and ready for installation tools like [Pathogen](https://github.com/tpope/vim-pathogen) and [Vundle](https://github.com/gmarik/Vundle.vim).

Just `cd` to the git repository and execute

```
mkvimball [name]
```

If `name` is specified, that will be the name of the generated file. Otherwise, the current directory's base name will be used.

## vless

Vim-based version of `less`. It uses the script located under "`$VIMRUNTIME/macors/less.sh`", part of any standard Vim installation.
