# qvm-autostart

Current Version 0.1 :) 

This script allow to setup auto start of any installeted program at Qubes AppVM template. 
On each AppVM boot program(s) will start with AppVM.

# How to install 

You can upload file `qvm-autostart` to template and after reboot you will be able 
to use autostart feature at any AppVM based on this template.

Or you can add it to only AppVM where you want to setup autostart.

Just upload/move/copy&paste `qvm-autostart` to
`/usr/bin/` 
then 
`cd /usr/bin/`
then
`sudo chmod +x qvm-autostart`

# How to use 
`usage: qvm-autostart [-h] [--remove] [--noterm] [--custom CUSTOM] application`

# Examples:

You want setup `gnome-terminal` to always autostart with AppVM
Simple:
`qvm-autostart gnome-terminal`
Remove:
`qvm-autostart --remove gnome-terminal`

You want to start firefox without terminal window (use `--noterm` if you do not want terminal appear)
`qvm-autostart --noterm firefox`
Remove:
``qvm-autostart --remove firefox`

If you want to start some script (ADVANCED):
`qvm-autostart --noterm --custom "/home/user/mysuperscript.sh" namesuperstart
Remove:
`qvm-autostart --remove namesuperstart







