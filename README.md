# Graphics-Switcher

# General Information
- Bash file for switching between NVIDIA and Intel's video cards
- Besides switching between graphics cards, it also fixes the video/screen tearing when using <b> Intel cards </b>.
- This script does not fix screen tearing on NVIDIA Graphics Cards, that's why we need to switch between them.
- ** IMPORTANT ** This script might not work properly with NVIDIA QUADRO video cards. For more information see: https://github.com/bauca/graphics-switcher/issues/3

# Open PRs
- (05/07/2021) - https://github.com/bauca/graphics-switcher/pull/4 - PR claims to use `prime-select query` command for the detection of the active GPU thus dropping off the requirement of `mesa-utils` (Still needs to be tested before merged).

# Release notes
- (03/08/2017) - Updated requirements list as suggested by issue #2 (https://github.com/bauca/graphics-switcher/issues/2).
- (16/07/2017) - Updates to this script are planned to be released by <strike> late  August </strike>.

# List of Requirements 
- Ubuntu 16.04 LTS
- Nvidia binary driver - version 375.66 from nvidia-375 (proprietary, tested) (*)
- glxinfo

- <b>Tested on:</b> Ubuntu 16.04 LTS - GeForce GT 735m + Intel Mesa - SonyVAIO FIT 15

(*) It might work with older or newer versions of the driver.

# How to use (for dummies) / Installation
  Assuming that you have an internet connection and you have fresh installed your ubuntu 16.04 LTS, follow the instructions below:
	
- Open terminal and type: sudo apt-get update
- Install the latest (375.66) Nvidia binary driver by following these steps:

	
	1 - Open the Ubuntu's 'System Settings' from ubuntu's left bar.
	
	2 - Click on the 'Software & Updates' icon.
	
	3 - Select the tab 'Additional Drivers'.
	
	4 - Check 'Using NVIDIA binary driver - version 375.66 from nvidia-375 (proprietary, tested).
	
	5 - Click on 'Apply Changes', wait until the installation is complete.
	
	6 - Reboot
	
				
- Install 'glxinfo' by opening terminal and typing: sudo apt-get install mesa-utils
- Download or Clone the graphics-switch script.
- Open a terminal within the folder where graphics-switch bash file is located and type: chmod a+x Graphics-Switcher
- Run the script by typing: ./Graphics-Switcher.


