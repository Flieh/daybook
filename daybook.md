** [pushing a watched file to github](https://gist.github.com/darencard/5d42319abcb6ec32bebf6a00ecf99e86) **


**vim date**

**Fri 07 Aug 2020 08:52:49 AM CEST**

add the following lines to .vimrc

```
nmap <F3> i<C-R>=strftime("%Y-%m-%d %a %I:%M %p")<CR><Esc>
imap <F3> <C-R>=strftime("%Y-%m-%d %a %I:%M %p")<CR>
```

**Daybook**

Hi I just converted my solutions.txt file to this markdown soluion

**BLUETOOTH ERRORS**

https://askubuntu.com/questions/801404/bluetooth-connection-failed-blueman-bluez-errors-dbusfailederror-protocol-no

The solution from this article worked for me:

sudo apt-get install pulseaudio-module-bluetooth
pactl load-module module-bluetooth-discover

Then delete the device from bluetooth devices and pair it again.

If it works, you can consider adding the second command to your startup settings, so that you don't have to run it again after every reboot.

If it doesn't work, try restarting pulseaudio:

pulseaudio -k
pulseaudio -D


KILL UNWANTED PROCESS

IDENTIFY IT WITH
    pgrep <process-name-yer-lookin-fer>
    kill -9 <pid> or <name-you-grepped-above>

--------------------
sliders (investigating)
--------------------
Looking at splidejs.com
