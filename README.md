# cleanupdate

Simple script to update and clean an Arch-based system.

The script can switch between Italian and English languages.


### Features

 - update packages from repositories;
 - update packages from AUR (with `pacaur` or `yaourt`);
 - search and uninstall orphaned packages;
 - clean pacman cache;
 - optimize (defragment) pacman database;
 - clean temporary or unuseful files;
 - clean old journald logs;
 - suggest solution to most common pacman errors;

Further details are available within the script documentation page, in Italian or English.


### Installation

This script has been created for an Arch-based system, you need to have `pacman` as package manager to use it properly.
Some features should work on any modern Linux system, you can copy those part and create your own script (remember to check the license).

This script is available on AUR as `cleanupdate-git`, so you can install it manually or with your favourite `pacman` helper  
```yaourt -S cleanupdate-git```  
or  
```pacaur -S cleanupdate-git```  
Installing from AUR adds a `.desktop` file in your system, this way the script should be available as `cleanupdate` in your application menu.
You can also launch it from the command line  
```cleanupdate```

Otherwise, you can simply download the `cleanupdate` file from this repository and make it executable  
```chmod +x cleanupdate```  
Then you can manually launch it with  
```./cleanupdate```

### Thanks

 - Mariano Messora, corrections to English translation.
 - PC ZERO from Manjaro Italia Forum, idea and base design for the icon.
