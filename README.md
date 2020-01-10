**UPDATE: [Star my X230-Hackintosh](https://github.com/mighildotcom/X230-Hackintosh) repo for latest updates. I no longer maintain this one. X230 guides are applicable for X230t also.**

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/mighil) [![捐赠](https://img.shields.io/badge/%E6%8D%90%E8%B5%A0-%E6%94%AF%E4%BB%98%E5%AE%9D-blue)](https://res.cloudinary.com/mighil/image/upload/v1578647638/donate-to-mighil.png) [![捐赠](https://img.shields.io/badge/%E6%8D%90%E8%B5%A0-%E5%BE%AE%E4%BF%A1-green)](https://res.cloudinary.com/mighil/image/upload/v1578647638/donate-to-mighil.png)

**Note: You're nothing but an a-hole if you sell EFI folder (config) that's readily available for free.**

# X230T Hackintosh

![X230T Hackintosh Guide](https://mighil.com/wp-content/uploads/2019/07/thinkpad-x230t-hackintosh.jpg)

Here's a guide to running macOS Mojave 10.14.3 (18G95) on a Thinkpad X230T without any hassle. The base EFI files are from Jack Zhang. I've modded it a bit. And yeah, you can update the device to 10.14.6 after updating Clover. I'll update the EFI files for 10.14.6 in a few days. Maybe I'm lucky, along with the other features, **Facetime and iMessage are working flawlessly** out of the box. In-built WiFi doesn't work.

## Tweak X230T's BIOS Settings (Do This First)

**Go to BIOS settings → Restart → Load Setup Defaults**

![](https://mighil.com/wp-content/uploads/2019/07/x230t-bios-default-settings.jpg)

**Go to BIOS Settings → Startup, select UEFI only disable CSM support.**

![](https://mighil.com/wp-content/uploads/2019/07/x230t-bios-csm-no.jpg)

## Fast (Half-Arsed) Install Method (Not Recommended)

Try this method if you own an extra SSD/HDD and a MacBook that supports the latest version of macOS Mojave. Here are the steps to follow:

1. Replace the old SSD/HDD in the MacBook with the new one. Yes, this requires manually removing the old HDD/SSD.
2. Boot up the MacBook and press Command Btn + R.
3. Fresh install the MacOS that came with your device. Then update it to the latest version of Mojave.
4. Install [Clover configurator](https://mackie100projects.altervista.org/download-clover-configurator/), mount the partition and replace the native EFI files with the respective EFI files in this repo.
5. Take that SSD and install it on a X230T. 

## My X230 Tablet Specs

* i7-3520m (Similar to a 13″ mid-2012 MacBook Pro)
* 16GB RAM
* Samsung PM810 Series 256 GB SSD (for MacOS Mojave)
* KingSpec 128GB mSATA SSD (For Windows)

![X230 Tablet Hackintosh With Stylus Support](https://res.cloudinary.com/mighil/image/upload/v1563945739/x230t-digitizer-pen-hackintosh_hhqgdr.gif)

## What Doesn’t Work?

* Inbuilt WiFi, you can hack BIOS and install a Mac-compatible WiFi card. I highly recommend a external device like Comfast CF-811AC
* Fingerprint reader

## Before You Install Mojave 10.14.3

Kindly note that WiFi won’t work after installing Mojave. Ethernet LAN will work.

So, be prepared if you just own one machine for the whole process. I highly recommend you to get hold of another device for preparing USB, and downloading MacOS DMG, EFI folder, Clover configurator files.

## Hackintosh Guide for ThinkPad X230 Tablet

1. Install [Transmac](https://www.acutesystems.com/scrtm.htm) on a Windows machine. It has a 15-day trial period and works flawlessly flashing DMG files to USB.

2. Download the [MacOS 10.14.3 with clover dmg file](https://pan.baidu.com/s/1Kv9XldS0GQVzsVu8fk9yPQ). Use **epv2** as the password to open the link. It’s a link to MacOS 10.14.3 bundled with Clover bootloader. **[Mirror Download Link](https://mirrors.dtops.cc/iso/MacOS/daliansky_macos/macOS%20Mojave%2010.14.3%2818D42%29%20Installer%20with%20Clover%204859.dmg)**.

3. Download the EFI folder from this repo.

4. Download [Clover Configurator for macOS](https://mackie100projects.altervista.org/download-clover-configurator/) (latest version).

5. Connect a 16GB USB flash drive.

6. Open Transmac. In the left pane, right-click the USB Drive and select Format Disk for Mac

7. Again in the left pane, right-click the USB Drive and select Restore with Disk Image. Then select the DMG file I mentioned in (2). Flashing process will take a few minutes depending on the size of .dmg and speed/port of the USB drive.

8. Install [DiskGenius](https://www.diskgenius.com/).

9. Locate the USB drive in DiskGenius. Delete the EFI folder and replace it with the new EFI folder. [Refer to this video](https://youtu.be/u15vmZ9obJY?t=75).

10. Plug the USB drive into the X230T and boot from USB.

11. Format the disk drive to APFS, install macOS Mojave, and restart the system.

12. Connect Hackintosh system to the Internet via LAN cable or a Mac-compatible external WiFi adapter.

13. Download Clover Configurator and refer to 6:32 of [this video](https://youtu.be/u15vmZ9obJY?t=391).

14. You may use [Karabiner-Elements](https://pqrs.org/osx/karabiner/) if the keyboard mappings (command and option) are acting up.

### Support
![Donate](https://res.cloudinary.com/mighil/image/upload/v1578647638/donate-to-mighil.png)
