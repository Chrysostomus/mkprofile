# mkprofile
A set of bash scripts to help creating installable custom live iso based on running manjaro system.

Mkrepo is bash script to create repository from installed AUR packages. It detects packages not found in manjaro repos, downloads PKGBUILDs for them from AUR, builds the packages in clean chroot using manjaro-tools, makes local repo out of them, uploads the repo online and adds it to pacman.conf. 

Mkprofile is another bash scripts that creates iso profile to be built with manjaro-tools. The createt profile shares the same dotfiles and installed packages as the host system, except for the drivers, which are managed by mhwd. Mkprofile calls mkrepo as needed to copy also the installed aur packages.
