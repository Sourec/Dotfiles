#Sourec Dotfiles

These files are my dotfiles for my own personal use. They are published here
so that others may use my files as they wish for their own purposes. Note that
they are my own personal files, and as such contain personalized controls,
settings, and system-specific configuration.

##Requirements
* i3
* i3blocks
* Conky

##Optional
These are referenced in i3/config, but are not necessary for functionality.
* i3lock
* PCManFM
* Synapse

##Installation & Configuration
To install, simply download, extract, and drag "Dotfiles" to ~/. Then make a 
symlink from ~/.i3 to ~/Dotfiles/i3 and restart i3. There are some things
you may need to change:

* modes/battlemode/conkyrc and modes/standby/conkyc use wlan1 and eth1 for
  network adapters, as my system for some reason incremented those by one
  a while ago. You will need to change these for conky to read network status
  properly.
* modes/battlemode/conkyrc references /home/sourec/SecondaryStorage. This is
  a setting specific to my system, a 155 GB Windows-shaped hole before my 
  Linux partitions that has been filled with a BTRFS partition. References
  to it can be deleted. 

##License Note
Not all files here are strictly my own, and as such the license found in LICENSE.md (GPLv3) doesn't apply to those. For reference, those files are:

* i3/i3scripts/ (has its own README.md file explaining license, GPLv3)
* media/, although that might change evnetually
* Images under modes/standby/
* scripts/vlcinfo
* soundboard/cymcrash.ogg
* vim/plugin/
* vim/syntax/

If you verifiably own any of these files and are within the terms of your license to do so, feel free to raise an issue asking me to remove the file whose presence you object to.