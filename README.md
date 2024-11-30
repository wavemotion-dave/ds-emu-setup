# DSi (or DSi XL,LL) Emulator Setup
This guide is intended to help would-be users of my emulators get it running on their DSi handheld system. This guide is not for the older DS-Lite/Phat (original DS units without an SD card slot) or for the later models (2DS/3DS/XL/LL). My emulators will run on those devices - but it requires either a flash cart (R4 or similar) or some other exploit that I'm not going to get into here.

In order to get homebrew emulators working on your DSi handheld, you will need some way of launching the emulators. This is normally done with some kind of exploit (or custom firmware - not covered by this guide). This guide will utilize the 'Camera Exploit' as described below.

# DSi Setup

First be sure you have an actual DSi unit. You can tell if your handheld is a DSi mainly by the presence of a _full-sized_ SD card slot on the right-side of the unit... but there is also a specific DSi logo imprinted on the bottom (with or without the XL/LL text depending on the size of the DSi handheld):

![DSi Logo](https://github.com/wavemotion-dave/ds-emu-setup/blob/main/png/dsi-logo.png)

Assuming you have such a DSi unit, the easiest way to get my emulators running is using the 'Camera Exploit' via the SD card. 

First you will need a standard SD card - anything from about 1GB to 16GB should work fine. I tend to use smaller capacity SD cards from either Sandisk or Toshiba. These 4GB cards will hold every classic game many times over and generaly won't cause any compatibility problems with the DSi. Here is an example of a card that I've used:

![SD Card](https://github.com/wavemotion-dave/ds-emu-setup/blob/main/png/sdcard.png)

Then I recommend you use the Standard SD Card formatter (not Windows format) to erase the card and provide for standard 32K sectors which is exactly what the DSi is expecting. I use the standard SD card formatter provided by the official SD Card association here: https://www.sdcard.org/downloads/formatter/

Once properly formatted, you need to install the TWL++ menu software, the camera exploit and setup the directories for gaming use. I've provided a ready-to-unzip snapshot of a virgin system (no game ROMs) to help you. You can download that from this link:  [TWL-Template.zip](https://fastupload.io/2b648a84b28e2ebd) - unzip this to the root directory of your SD card such that the root of that card has BOOT.NDS, my emulators (.NDS files) and about a half-dozen sub-directories. 

* In the 'roms' directory you will find other subdirectories to put your games.
* Many of my emulators require BIOS files for the given system (e.g. for Intellivision will need, at least, exec.bin and grom.bin). These must be placed in the /roms/bios folder.

Do not ask me for BIOS files or roms - that part is an exercise left up to the user. They aren't hard to find...

# Using the DSi and Launching Emulators

* Make sure the SD card is in the DSi unit (properly formatted as described above).
* Turn on the DSi and navigate to the Camera Icon.
* Select the Camera Icon and then click in the upper-right to select the 'SD CARD'
* There should be one and only one 'picture' in the SD card 'Album' - this is the Camera Exploit.
* Press the 'Album' icon containing the one 'picture' - this will launch the Camera Exploit and get you into the menu system.

![Camera](https://github.com/wavemotion-dave/ds-emu-setup/blob/main/png/camera.png)

Once you are in the menu system, you can navigate to select the emulator of choice and launch it by pressing the 'A' button.

![TWL Menu](https://github.com/wavemotion-dave/ds-emu-setup/blob/main/png/menu.png)

Enjoy!

# Addendum - if it doesn't work
It's possible that you have a DSi that needs an different Camera Exploit.  There are two (I provided the more common of the two in my ZIP file above)

If that's the case, download this alternate pit.bin file:  https://dsi.cfw.guide/assets/files/memory_pit/256/pit.bin 

And on the SD card, place it into the /TWL-Template/private/ds/app/484E494A$ directory (replacing the version that is in there).

And try again!


