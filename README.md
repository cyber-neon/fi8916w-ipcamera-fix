# fi8916w-ipcamera-fix
fix your bricked fi8916w ipcamera


open tera term

uart to usb you ipcamera and select your com port
after that press setup and serial port baud rate 15200.
power ipcamera and press Esc fast to get in bootmode.

now type del 6 "Enter" and del 7 "Enter"



type" fx 6 romfs.img 0x7f0e0000 0x7f0e0000 -a
and press file and transfer and 
send file xmodem in tera term

type" fx 7 linux.zip 0x7f020000 0x8000 -acxz

send file xmodem in tera term

type" fx 8 webui.bin 0x7f200000 0x7f200000 -a

send file xmodem in tera term

type" boot "enter"

afer that login your ipcamera webpage

webui are http://(ip)index.htm. without this ipcamera says error 404 not found

