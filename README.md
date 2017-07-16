# fi8916w-ipcamera-fix
fix your bricked fi8916w ipcamera


step one open tera term

uart to usb you ipcamera and select your com port
after that press setup and serial port baud rate 15200.
power ipcamera and press Esc fast to get in bootmode.




terminal tera term
del 6 "Enter" THEN del 7 "Enter"

fx 6 romfs.img 0x7f0e0000 0x7f0e0000 -a
and press file and transfer and 
send file xmodem in tera term

fx 7 linux.zip 0x7f020000 0x8000 -acxz

send file xmodem in tera term

fx 8 webui.bin 0x7f200000 0x7f200000 -a

send file xmodem in tera term

boot "enter"

afer that login your ipcamera webpage

webui are http://(ip)index.htm. without this ipcamera says error 404 not found
