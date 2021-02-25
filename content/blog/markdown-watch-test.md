title: Markdown Watch Test 
date: 2020-08-07 Fri 12:15 PM
category: Blog

[pushing a watched file to github](https://gist.github.com/darencard/5d42319abcb6ec32bebf6a00ecf99e86)

**update:** Now, I'm using [markdown-preview.vim](https://github.com/iamcco/markdown-preview.vim)

**update** Auto commiting and pushing to github on file change

    inotifywait -q -m -e CLOSE_WRITE --format="git commit -m 'autocommit on change' %w" daybook.md | bash

## Vim: date
2020-08-07 Fri 12:16 PM

add the following lines to .vimrc


    nmap <F3> i<C-R>=strftime("%Y-%m-%d %a %I:%M %p")<CR><Esc>
    imap <F3> <C-R>=strftime("%Y-%m-%d %a %I:%M %p")<CR>


