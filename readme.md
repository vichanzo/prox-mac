# Prox-Mac
My notes on creating a hackintosh on an original Mac Pro A1186

1) First boot - got only a flashing white power light.
   - Google tells me to reseat the memory
   - I clean the dust off the RAM and reseat the RAM modules, and RAM trays.
2) Now I get the chime, but no apple logo, only garbled lines on a white screen
   - Clean the GPU and GPU slot.  Reseat the GPU
3) Boot and I get the apple logo but then it still goes to the white screen with garbled lines
4) Able to press and hold ctl and boot into usb with Ventoy.
   - Unable to use Ventor to boot into anything useful, keeps getting stuck on a black screen
5) now try easy to boot.  Able to install Debian Netinstall (Jesse)
   - Jesse repos aren't working
6) Repeat Easy2Boot with Bookwork (Debian 12)
   - this works
7) apt update
8) wget from github my initialize.sh (git openssh-server sudo ansible)
9) bash ./initialize
10) follow steps in https://pve.proxmox.com/wiki/Install_Proxmox_VE_on_Debian_12_Bookworm
11) wget gpg file
12) nano hosts file
13) nano etc/network/interfaces to switch to static IP
14) reboot to go to new IP
15) echo "deb [arch=amd64] http://download.proxmox.com/debian/pve bookworm pve-no-subscription" > /etc/apt/sources.list.d/pve-install-repo.list
16) apt update && full-upgrade
