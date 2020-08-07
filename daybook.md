2020-08-07 Fri 03:13 PM

## Markdown Watch Test 
2020-08-07 Fri 12:15 PM

[pushing a watched file to github](https://gist.github.com/darencard/5d42319abcb6ec32bebf6a00ecf99e86)

**update:** Now, I'm using [markdown-preview.vim](https://github.com/iamcco/markdown-preview.vim)

**update** Auto commiting and pushing to github on file change

    inotifywait -q -m -e CLOSE_WRITE --format="git commit -m 'autocommit on change' %w" file.txt | bash

## Vim: date
2020-08-07 Fri 12:16 PM

add the following lines to .vimrc


    nmap <F3> i<C-R>=strftime("%Y-%m-%d %a %I:%M %p")<CR><Esc>
    imap <F3> <C-R>=strftime("%Y-%m-%d %a %I:%M %p")<CR>

## Daybook
2020-08-07 Fri 12:17 PM

Hi I just converted my solutions.txt file to this markdown soluion

## Bluetooth errors

https://askubuntu.com/questions/801404/bluetooth-connection-failed-blueman-bluez-errors-dbusfailederror-protocol-no

The solution from this article worked for me:

    sudo apt-get install pulseaudio-module-bluetooth pactl load-module module-bluetooth-discover

Then delete the device from bluetooth devices and pair it again.

If it works, you can consider adding the second command to your startup settings, so that you don't have to run it again after every reboot.

If it doesn't work, try restarting pulseaudio:

    pulseaudio -k
    pulseaudio -D


## Linux: kill unwanted processes
2020-08-07 Fri 12:24 PM

IDENTIFY IT WITH

    pgrep <process-name-yer-lookin-fer>

then kill it
  
    kill -9 <pid> or <name-you-grepped-above>

## JS: sliders (investigating)
2020-08-07 Fri 12:24 PM

Looking at [splidejs.com](https://www.splidejs.com)
