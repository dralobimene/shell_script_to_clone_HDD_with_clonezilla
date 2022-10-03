# shell_script_to_clone_HDD_with_clonezilla (5partitions)

works with linux debian bulls eye. 5 partitions

shell script, copy and paste into text editor, save as a .sh file, make it executable
<br>
script to clone internal hard disk drive 5 partitions to external hard disk drive. copy the script to a USB stick

first: Download and use Clonezilla to clone your internal hard disk drive.<br>
Once finished, don't exit, but go to command line and login as root.<br>
command: sudo -i password: no password requested <br>
create a folder into /media (i create a folder with my debian account name)<br>
create inside /media/your_debian_account_login/ another folder: the name of your USB stick (i use "sauv_donnees")<br>
mount the USB stick into this folder<br>
command: mount /dev/sdXY /media/your_debian_account_login/name_of_your_USB_stick<br>
go to this folder,<br>
execute bash script<br>
<br>
this script is for a debian bullseye linux distribution. It should work with another but not tested<br>
Here my configuration:<br>
5 partitions<br>
/dev/sda1 - EFI System - FAT (version 32 bit)<br>
/dev/sda2 - linux file system ext4 - label: root<br>
/dev/sda3 - linux file system ext4 - label: home<br>
/dev/sda4 - linux file system ext4 - label: others<br>
/dev/sda5 - swap linux<br>
<br>
Before executing the script: Open it with text editor Read, read, read (only french comments)<br>
<br>
there is no warranty and won't be responsible for anything<br>
<br>
you may use it as you want<br>
<br>
Regards<br>
Licence:<br>
Do what you want with it.
