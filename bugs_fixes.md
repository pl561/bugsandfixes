# bugs and associated fixes
## Multiple Boot Systems Time Conflicts
https://help.ubuntu.com/community/UbuntuTime#Multiple_Boot_Systems_Time_Conflicts
http://askubuntu.com/questions/800914/clock-shows-wrong-time-after-switching-from-ubuntu-to-windows-10
fix: $ timedatectl set-local-rtc 1
