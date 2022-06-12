# shell_script_to_clone_HDD_with_clonezilla

works with linux debian bulls eye. 5 partitions

shell script, copy and paste into text editor, save as a .sh file, make it executable

script to clone internal hard disk drive 5 partitions to external hard disk drive. copy the script to a USB stick

first: Download and use Clonezilla to clone your internal hard disk drive.
Once finished, don't exit, but go to command line and login as root.
command: sudo -i password: no password requested 
create a folder into /media (i create a folder with my debian account name)
create inside /media/your_debian_account_login/ another folder: the name of your USB stick (i use "sauv_donnees")
mount the USB stick into this folder
command: mount /dev/sdXY /media/your_debian_account_login/name_of_your_USB_stick
go to this folder,
execute bash script

this script is for a debian bullseye linux distribution. It should work with another but not tested
Here my configuration:
5 partitions
/dev/sda1 - EFI System - FAT (version 32 bit)
/dev/sda2 - linux file system ext4 - label: root
/dev/sda3 - linux file system ext4 - label: home
/dev/sda4 - linux file system ext4 - label: others
/dev/sda5 - swap linux

Before executing the script: Open it with text editor Read, read, read (only french comments)

there is no warranty and won't be responsible for anything

you may use it as you want

Regards
