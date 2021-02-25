title: Daybook
date: 2020-08-07 Fri 12:17 PM
category: misc

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



