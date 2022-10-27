## Changelog

### v2.0.1 October 27, 2022
- Update Opencore Boot wallpapers again
- kext upgrade to new version
- For MacOS Monterey users, please go to config to enable `AirportItlwm-Monterey.kext` and disable `AirportItlwm.kext` to ensure WiFi
- This version supports MacOS Ventura

### v2.0 October 18, 2022
- Updated with new backgrounds to match MacOS 13
- Upgrade OpenCore to 0.8.6 development version

**Note:this version only supports MacOS 13 beta, users using MacOS 12 please use v1.9**

### v1.9 August 23, 2022
- Updated OpenCore background to mica background
- Customized AppleALC
- Update OpenCore boot version to 0.8.4 development version

### v1.8 July 22, 2022
- Guided update to the official version of OpenCore0.8.2
- Modify the touchpad to GPIO interrupt mode
- Fixed the silent problem of restarting from win to Mac `The sound card driver for win needs to be updated to a non-win version driver, that is, the official version of Realtek is used`
- This version only supports the 12 system (the 15.X and 11 versions will no longer be supported )
- If you need to upgrade 13 Beta, please manually upgrade OpenCore 0.8.3 Beta and wifi driver and then update 13 Beta

### v1.7 June 5, 2022
- Modified and streamlined some items
- used OpenCore development version 0.8.2
- To upgrade Mac OS 13 please go to close `avoidruntimederfg`
- Thanks to the big guy [Baio1977](https://github.com/Baio1977) for the optimization and improvement

### v1.6 June 3, 2022
- Optimized graphics card
- Changed OpenCore boot background
- Uploaded DSDT

### v1.5 April 29, 2022
- OpenCore boot version upgraded to `0.8.0`

### v1.4 March 13, 2022
#### This version has technical problems and is urgently removed from the shelf. Please wait for the repair to be completed and it will be put on the shelves again.
- Fixed sleep (if there is a problem with sleep go to Hackintool's power and click a screwdriver to fix it)
- Customized sound card
- Follow OpenCore official upgrade to OpenCore boot version `0.7.9`
- HDMI cannot be repaired temporarily
- Differentiated OC boot for three Mac versions

### v1.3 February 19, 2022
- Upgrade the OC boot version to `0.7.8` with the official
- Still having trouble sleeping
- Customized USB
- Differentiated OC boot for three Mac versions

### v1.2 February 7, 2022
- Built in card reader to make it appear as native Apple card reader
- Found a problem with sleep, waiting for the next version to fix
-Fixed that Mac information would be displayed on Windows causing Windows to show inactive
- Added AsusSMC to enable keyboard to have ASUS native functionality
- Differentiate between three versions of EFI

### v1.1 January 25, 2022
-Fixed that the nuclear display has a certain probability of turning on and running the progress bar after the black screen
- Repair the battery display capacity and the actual battery situation do not match
- Modify the theme of the startup item interface
- Remove some unnecessary drivers and SSDT based on `V1.0`

### v1.0 January 24, 2022
- Support to install the latest Mac OS Monterey 12.2
- OpenCore version is latest `0.7.7`
