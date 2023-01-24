---
layout: default
---
[< back](./)

## 6800U VRAM Warning!

## The Problem

When installing AMD Adrenalin, **do not click the “Factory reset” checkbox** - it will reset your VRAM allocation. Clicking this box, or adjusting the “Memory Optimizer” feature in AMD Adrenalin, will cause VRAM to reset to as low as 512MB, which will cut gaming performance by 50% or more.

In AMD Adrenalin settings, Performance > Tuning, there is an option called **Memory Optimizer (don’t use this feature - it will break your VRAM).** I**f you touch that drop down in any way and apply either productivity or gaming, it will break the dedicated VRAM assigned to the GPU and your gaming performance will be cut significantly.**

<img width="700" alt="image" src="https://user-images.githubusercontent.com/6972693/214380224-b727c177-4fb1-4cca-9e70-34aa201bbb19.png">


## The Fix

There are two fixes to this issue - a BIOS reflash which isn’t currently possible (Ayaneo has not released any BIOS updates for us to do this) and the second method is to completely drain your Ayaneo 2’s battery to reset BIOS settings (there isn’t a CMOS battery in these units). To drain the battery: 

- Play a long video, benchmark, game, or other power heavy task until your device turns off (usually around 4%).
- Turn your device back on, and continue draining until it dies a second time.
- You should not be able to turn your device back on. If you can, continue draining the battery until you’re not longer able to turn the device back on and have it boot.
- Once battery is drained, plug in a charger and your VRAM should be reset back to factory amounts (3GB VRAM on 16GB RAM Ayaneo 2 models, 6GB VRAM on 32GB RAM Ayaneo 2 models)

***
[< back](./)
