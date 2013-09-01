update-mirrorlist
================

A pacman mirrorlist updater

Usage: update-mirrorlist [options]
	
Update options:
-m <num>   Set max number of mirrors

Other options:
-h  Show this help
-v  Show version and exit
-r  Restore original mirrorlist
-c  Check mirrorlist for errors

update-mirrorlist updates the pacman mirrorlist by retrieving 
a fresh list from http://www.archlinux.org/mirrorlist/
		       
See /etc/pacman.d/update-mirrorlist.conf for configuration
