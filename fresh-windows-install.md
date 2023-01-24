---
layout: default
---

[back](./)

## Fresh Windows Install

The Ayaneo 2 is almost a proper PC but comes with a bundled W11 that has caused issues for several of us here. Here’s a quick guide allowing you to setup your console with a fresh Windows version if you’re just formatting or changing your SSD.

**Note**: There is no Windows key to memorize or type in. It’s part of your Ayaneo’s motherboard. During Windows installation, Windows will automatically activate when it reaches the internet. If you’re not able to get online during the Windows installation, you can safely skip entering a key and it will later activate when your Ayaneo gets online. 

<br /> 

********************Needed :********************

- A wired keyboard
- A USB stick - 16gb or above
- A USB-C adapter to plug your USB to the Ayaneo (your Ayaneo 2 should have come with 2 of these)

<br /> 

**************Optional but useful :**************

- A wired mouse (makes the process a lot easier until you have your drivers up)
- Another computer (mandatory if your Ayaneo can not boot) - *this guide is for Windows, MacOS or Linux work too, I’ll let you check how to make a bootable USB yourself*.

<br /> 
<br /> 

## 1. Preparation


### Bootable USB :

Go [here](https://www.microsoft.com/software-download/windows11) and go through the **Create Windows 11 Installation Media** steps.

This will format your USB and make it so you can boot on it to fully reinstall windows.

<br /> 

### Drivers :

3 files to download: 

- Go to the Ayaneo [download page](https://ayaneo.com/support/download), and download the **AYANEO 2 Driver Package.**
- AMD 6800U drivers: [https://www.amd.com/en/support/apu/amd-ryzen-processors/amd-ryzen-7-mobile-processors-radeon-graphics/amd-ryzen-7-6800u](https://www.amd.com/en/support/apu/amd-ryzen-processors/amd-ryzen-7-mobile-processors-radeon-graphics/amd-ryzen-7-6800u)
- AMD Chipset drivers: [https://www.amd.com/en/support/chipsets/socket-fp5-mobile/amd-ryzen-and-athlon-mobile-chipset](https://www.amd.com/en/support/chipsets/socket-fp5-mobile/amd-ryzen-and-athlon-mobile-chipset)

Take all 3 downloads and put them into a folder on the root of the Bootable USB you created in the previous step (I usually put them in a folder called “Installation Files”. 

<br /> 

### Bonus :

Have the software you want to install at the ready too. 

You can check both [Toolbox & Tricks](https://cngjd.github.io/AyaNeo2-docs/toolbox-tricks.html) and [Getting rid of AyaSpace](https://cngjd.github.io/AyaNeo2-docs/getting-rid-of-ayaspace.html) to get some tools you might need for later.

No stress about it, once your console is up with Windows and the driver you’ll be able to download and setup whatever you want.

<br /> 

## 2. Formatting the Ayaneo

If needed, save what need to be, because everything on your Ayaneo is going to be deleted…

Plug the bootable USB and keyboard to it and turn off your device.

To boot on the usb stick, keep pressing LC & VOL+ when pushing the power button.

![Getting into BIOS](https://user-images.githubusercontent.com/50463438/214381043-59d995ad-891a-4568-94f5-110ff8967e16.png)

Select your USB on the window that presents itself.

Go through the [Windows setup process](https://www.google.com/search?client=firefox-b-d&q=how+to+install+windows+11+from+usb). **Note**: There is no Windows key to memorize or type in. It’s part of your Ayaneo’s motherboard. During Windows installation, Windows will automatically activate when it reaches the internet. If you’re not able to get online during the Windows installation, you can safely skip entering a key and it will later activate when your Ayaneo gets online. 

**Important note**: If you receive a BSOD (blue error screen) during Windows 11 install, please see the following guide: 

[DPC_Watchdog_Violation BSOD’s During Windows 11 Install](https://cngjd.github.io/AyaNeo2-docs/bsod-during-windows-install.html)

**Optional step**: The following formatting step is ***optional***, but it’s a great idea if you have a slow internet connection - saves you from having to re-download games and your personal data in the event you need to reinstall Windows in the future: 

- My recommendation would be to make a Windows partition of about 70-100GB in order to use some partitioning as I explain in [Example Setup](https://cngjd.github.io/AyaNeo2-docs/example-setup.html).

After you’re done installing Windows, you should be at the desktop before the next step. 

<br /> 

## 3. Install the drivers

Get the zip you downloaded prior from the Ayaneo website, extract it to a folder on your Ayaneo.

Open the start menu, search for **********Device Manager********** and open it.

Right click on your computer’s name and click Add Drivers

![Add Drivers to Device Manager](https://user-images.githubusercontent.com/50463438/214384746-4b000746-495d-4284-bd87-b971387746b6.png)


Select the uncompressed drivers folder, verify that the subfolder checkbox is checked and click next as much as needed.

After a reboot, open Device Manager and it should look like this (still 4 devices needing drivers): 

![After Ayaneo Driver Pack](https://user-images.githubusercontent.com/50463438/214385371-ddce0f13-8bf7-4f72-be27-fcd6dd73f29c.png)


Next step is to **install AMD Adrenalin** (you should have downloaded it in the initial steps of this guide):  [VERY IMPORTANT: read this to not permanently break your device](https://cngjd.github.io/AyaNeo2-docs/6800U_vram.html). 

Download link: [AMD Ryzen™ 7 6800U Drivers & Support](https://www.amd.com/en/support/apu/amd-ryzen-processors/amd-ryzen-7-mobile-processors-radeon-graphics/amd-ryzen-7-6800u)

And **disable the ability for Windows Update to install Manufacturer Apps, which can sometimes overwrite AMD drivers:** 

- Start Menu
- Search for **Device Installation** and open Device Installation Settings
- Select No and save.
![Device Installation Settings](https://user-images.githubusercontent.com/50463438/214386373-47693bd8-b59e-4751-a115-2698d1efb43e.png)

After Adrenalin completes and you reboot, Device Manager should only have 3 devices needing drivers, like this screenshot: 
![Device Manager After Adrenalin](https://user-images.githubusercontent.com/50463438/214386531-44478d5d-734c-4f8b-8652-07b2926ad90f.png)

Finally, run the AMD chipset driver you downloaded in earlier steps, leave all checkboxes for all drivers checked, and finish the installation. Then reboot. After you reboot, all devices in Device Manager should be working: 

![Device Manager After Chipset](https://user-images.githubusercontent.com/50463438/214416196-7176825a-76ec-47a3-9f3a-e72fd93d011a.png)


<br /> 

## 4. Update Windows

Open Windows Update and install all available updates. Make sure you click “Advanced Options” at the bottom, click the slider next to “Receive updates for other Microsoft products” to turn this feature on, then click “Optional updates” at the bottom. Select all checkboxes and install them. 

After the first round of Windows Updates are complete, restart your computer. After the restart run Windows Updates again to complete the update process. 

## 5. Finishing touch

Install [Ayaspace](https://ayaneo.com/product/AYASpace.html) or go the [Getting rid of AyaSpace](https://cngjd.github.io/AyaNeo2-docs/getting-rid-of-ayaspace.html) route


## 6.. Profit

Do whatever you want, install your games, launchers, and so on. Check [Toolbox & Tricks](https://cngjd.github.io/AyaNeo2-docs/toolbox-tricks.html), [Getting rid of AyaSpace](https://cngjd.github.io/AyaNeo2-docs/getting-rid-of-ayaspace.html) or [Example Setup](https://cngjd.github.io/AyaNeo2-docs/example-setup.html) for ideas.

[back](./)
