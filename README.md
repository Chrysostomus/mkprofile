# mkrepo
Simple bash script to create repository from installed AUR packages. 

It detects packages not found in manjaro repos, downloads PKGBUILDs for them from AUR, builds the packages in clean chroot using manjaro-tools, makes local repo out of them, uploads the repo online and adds it to pacman.conf. It can be used to help cloning your manjaro system to a live iso.
