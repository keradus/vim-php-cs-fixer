Vim-php-cs-fixer
================

Integrate [php-cs-fixer](https://github.com/fabpot/PHP-CS-Fixer) created by fabpot.

This plugin will execute the `php-cs-fixer` command on the directory where you launch the command. See options to know how to customize that.

**Options available**:

```viml
let g:php_cs_fixer_path = "~/php-cs-fixer.phar" " define the path to the php-cs-fixer.phar
let g:php_cs_fixer_level = "all"                " which level ?
let g:php_cs_fixer_finder = "SymfonyFinder"     " Which finder ?
let g:php_cs_fixer_php_path = "php"             " Path to PHP
let g:php_cs_fixer_default_mapping = 1          " Enable the mapping by default (<leader>pcd)
let g:php_cs_fixer_dry_run = 0                  " Call command with dry-run option
```

Default mapping is `<leader>pcd`

If you want to change it:

```viml
map <leader>pcd :call PhpCsFixerFix(expand('%:p:h'))<CR>
```

# Installation

Via **[Vundle](https://github.com/gmarik/vundle)**, add:

```viml
Bundle 'stephpy/vim-php-cs-fixer'
```

To see how to install `php-cs-fixer`, look at [php-cs-fixer](https://github.com/fabpot/PHP-CS-Fixer) repository.

If you see any improvement or question, contribute or create an issue
