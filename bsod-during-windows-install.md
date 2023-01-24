---
layout: default
---
[< back](./)

## DPC_Watchdog_Violation BSOD’s During Windows 11 Install

If Windows 11 BSOD’s (blue error screen) during installation, with a stop code of “DPC_Watchdog_Violation”, below is a list of recommendations. Our recommendation is to do all of the below tricks in order to have highest chances of a smooth Windows 11 installation. 

<img width="670" alt="image" src="https://user-images.githubusercontent.com/6972693/214380472-b37cc59d-4494-4a4f-bb23-84bc148040a1.png">

First fix is to remove your Ayaneo 2 from the Ayaneo Dock. For USB devices (keyboard, mouse, flash drive) use a USB-C hub or USB-C to USB-A adapters (2 of these adapters should have come with your Ayaneo 2). 

Second fix is removing the flash drive after Windows 11 finishes installing, when your computer is about to reboot. You’ll see a countdown message where Windows is preparing to restart your computer. Pull the Windows 11 installation flash drive out at this time and then let Windows reboot. This may fix the DPC_Watchdog_Violation error (which occurs just after the reboot and before Windows starts initial setup). 

<img width="612" alt="image" src="https://user-images.githubusercontent.com/6972693/214380504-bbd33ee4-6d1d-4a1f-891d-5a7e9fa2ff48.png">

Third fix is to turn off Fast Boot in BIOS. To do this: 

- Hold the power button down to turn your Ayaneo 2 completely off
- Hold down the LC and Volume+ buttons, then push the power button (just like the above screenshot)
- You should see a menu showing your SSD, your flash drive, and an option to enter setup. Choose the setup option and hit enter.
- Your computer will boot into BIOS.
- Arrow key over to the Boot menu and turn off Fast Boot.
- Also change the boot order so that your flash drive is the primary boot device (you’ll need to go through the Windows install again)
- Hit F10 to “Save and Exit” BIOS. Hit yes to save on the pop up that appears.
- Your computer will now reboot and begin the Windows installation process again
- You do not NEED to turn “Fast Boot” back on. Many sources recommend leaving Fast Boot off on all computers [for a number of reasons](https://www.makeuseof.com/what-is-windows-fast-startup-why-disable-it/).
- If you continue to run into any issues with blue screens during Windows install, please join the [Ayaneo Discord](https://discord.gg/DwqpsGDv) so we can help you.

***
[< back](./)
