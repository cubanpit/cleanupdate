# cleanupdate

**WARNING:** I do not actively use this script anymore (because I moved to NixOS), so it can be considered unmantained. Feel free to open issues or pull requests though, I am happy if it can still be useful to anyone.

Simple script to update and clean an Arch-based system.

The script can switch between Italian and English languages.


### Features

 - update packages from repositories;
 - update packages from AUR (with `yay`, `trizen` or `pamac`);
 - search and uninstall orphaned packages;
 - clean pacman cache;
 - clean temporary or unuseful files;
 - clean old journald logs;
 - suggest solution to most common pacman errors;

If the [environment variable](https://wiki.archlinux.org/index.php/Environment_variables) `CU_PKEXEC` is set to `true` the authentication is done with `pkexec` instead of `sudo`.

Further details are available within the manual page, in Italian or English.


### Installation

This script has been created for an Arch-based system, you need to have `pacman` as package manager to use it properly.
Other needed dependencies are:

 - `bash`: obviously;
 - `polkit` or `sudo`: in order to obtain administrative privileges;
 - `pacman-contrib`: provides `paccache`, for cleaning package manager cache;
 - `ncurses`: used to obtain terminal size or color codes (`/bin/tput`);
 - `yay`: optional, to enable AUR update feature, first in priority;
 - `trizen`: optional, to enable AUR update feature, second in priority;
 - `pamac`: optional, to enable AUR update feature, third in priority;

Some features should work on any modern Linux system, you can copy those part and create your own script (remember to check the license).

This script is available on AUR as `cleanupdate-git`, so you can install it manually or with your favourite `pacman` helper.
Installing from AUR adds a `.desktop` file in your system, this way the script should be available as `cleanupdate` in your application menu, obviously you can also launch it from the command line.

Otherwise, you can simply download the `cleanupdate` file from this repository and make it executable
```
chmod +x cleanupdate
```
Then you can manually launch it with
```
./cleanupdate
```


### Thanks

 - Mariano Messora, corrections to English translation.
 - PC ZERO from Manjaro Italia Forum, idea and base design for the icon.
