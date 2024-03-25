This repository contains scripts for fixing common MACOS issues

Current scripts
Retwork Reset 
-The network reset script erases the preference(plist) files responisble for determining network settings before restarting the device. While the device is restarting,
the absence of those files is detected and the system restores them from a system image effectivly resetting them back to their default configuration.

TimeFix(WIP)
-disables automatic time updates, wipes two files that commonly cause time issues, runs a command to resync the time, then restarts the device to replace the missing files

FindBadFolders
-checks the contents of possible bad folder locations before returning the largest 10 folders in each location. This allows for the quick identification of oversized "system" files (Created by applications) allowing them to be purged.
Note when purging oversized folders to be aware that the associated application might become disfuntional requireing a reinstall, so I would recommend backing up any work that requires that application specifically.
This is only necessary when the "system data" portion of the Harddrive is significantly oversized (i.e. <30GB)

