# rockpi-quad
This repo is custom firmware for the Rockpi/Raspberry Pi Quad SATA Hat developed by Raxda.

Links to official docs are here:
Installation:
https://wiki.radxa.com/Dual_Quad_SATA_HAT

Troubleshooting Forum:
https://forum.radxa.com/t/quad-sata-hat-assembly-and-troubleshooting/3879/123

Please consult these if having issues.

This custom firmware repo exists because when Raxda released the Penta SATA Hat for the Raspberry Pi 5, they updated certain databases involved with the quad project, completely breaking things. Firmware does not function on any raspbian firware past bookworm 12, and even on bookworm 12 several naming conventions are still broken. This repo is the fixed version of that. Works on Bookworm 12 lite (lite because of openmediavault) should work on the full installation.


--------------------------------------Weird Raxda Naming Conventions!-------------------------------------
Rockpi-sata.service is the daemon service usually mentioned online. It is not named this. It's rockpi-quad.service. it can be found in /lib/systemd/system/rockpi-quad.service
Custom power script is /usr/local/bin/power_toggle.sh
/etc/rockpi-quad.conf 
/etc/rockpi-quad.env
/usr/bin/rockpi-quad is where all other scripts can be found 
