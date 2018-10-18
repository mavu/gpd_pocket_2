# gpd_pocket_2
Some config files for a better Debian experience on the GPD Pocket 2

### some notes on DPI
The .Xresources file lists a "wrong" value for DPI for the P2 screen.
The actual value would be something in the area of 300, but for me 
162 seems to give a good compromise between readability and screen 
space.

### xserver video driver
The Pocket 2 can use 2 different drivers for X:
The "old" 'intel' driver or the newer 'modesetting' driver.

The 'intel' driver seens to produce less tearing, but does not seem to allow rotation in the xorg.conf.d/ files.
Use either 10-modesetting.conf OR the 10-intel.conf file.

If you use the 10-intel.conf, you will have to rotate the screen manually or some other way.

### screen rotation at boot
If you want the screen to be rotated correctly at boot time (for the consoles not X) add "fbcon=rotate:1" in your /etc/default/grub like in the example.


### these are just some personal files. for a more complete guide look at https://github.com/ishtob/gpd-pocket-2-arch-guide
