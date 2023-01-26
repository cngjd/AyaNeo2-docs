---
layout: default
---
[<back](./)
## Check your drivers

Several users have noticed driver problems with their Ayaneo 2 devices right out of the box. We highly recommend checking Device Manager to make sure all devices are functioning correctly. If you notice anything isn’t working quite right, games are locking up, sound isn’t working, or your computer randomly reboots, updating drivers is a great initial step. 

If you want to “play it safe”, just install the 6800U drivers and chipset drivers from the links below. If you want to make sure all of your drivers are up to date, all 3 sets of drivers can be installed. 

All drivers can be downloaded from the following 3 links: 

- Go to the Ayaneo [download page](https://ayaneo.com/support/download), and download the **AYANEO 2 Driver Package.**
- AMD 6800U drivers: [https://www.amd.com/en/support/apu/amd-ryzen-processors/amd-ryzen-7-mobile-processors-radeon-graphics/amd-ryzen-7-6800u](https://www.amd.com/en/support/apu/amd-ryzen-processors/amd-ryzen-7-mobile-processors-radeon-graphics/amd-ryzen-7-6800u)
- AMD Chipset drivers: [https://www.amd.com/en/support/chipsets/socket-fp5-mobile/amd-ryzen-and-athlon-mobile-chipset](https://www.amd.com/en/support/chipsets/socket-fp5-mobile/amd-ryzen-and-athlon-mobile-chipset)

**To install the drivers: **
- Get the zip you downloaded prior from the Ayaneo website, extract it to a folder on your Ayaneo.
- Open the start menu, search for **Device Manager** and open it.
- Right click on your computer’s name and click Add Drivers

<img width="425" alt="image" src="https://user-images.githubusercontent.com/6972693/214899575-6663d208-4b24-4868-86aa-ec5a0574e117.png">

Select the uncompressed drivers folder, verify that the subfolder checkbox is checked and click next as much as needed. After drivers finish installing, restart your computer. 

Next step is to install AMD Adrenalin. **[VERY IMPORTANT: read this to not permanently break your device](https://www.notion.so/Read-this-6800U-VRAM-Warning-6f768cb51e964ae0bba4a371189df82c)**. Run the installer and click next until it finishes installing. Afterwards, you’ll want to **disable the ability for Windows Update to install Manufacturer Apps, which can sometimes overwrite AMD drivers:** 

- start menu
- search for **Device Installation** and open Device Installation Settings
- Select No and save.

<img width="591" alt="image" src="https://user-images.githubusercontent.com/6972693/214899862-de70fe53-a642-4888-9c97-14ad3541a159.png">

Finally, run the AMD chipset driver, leave all checkboxes for all drivers checked, and finish the installation. Then reboot. After you reboot, all devices in Device Manager should be working: 

<img width="429" alt="image" src="https://user-images.githubusercontent.com/6972693/214899922-26304188-d8c2-4a02-ae7a-87444b004531.png"> 

Your issues should now be resolved.

***
[<back](./)
