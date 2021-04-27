- [Frequently asked questions](#frequently-asked-questions)
  - [How to use the new always available instant restart?](#how-to-use-the-new-always-available-instant-restart)
  - [How can I use directX 12](#how-can-i-use-directx-12)
  - [Should I use 11 or 12](#should-i-use-11-or-12)
- [Technical issues](#technical-issues)
  - [Why are my graphics/keybinds resseting?](#why-are-my-graphicskeybinds-resseting)
  - [Nothing disables Vsync](#nothing-disables-vsync)
  - [How to handle the input lag/broken vsync](#how-to-handle-the-input-lagbroken-vsync)
  - [Why is RayTracing disabling itself?](#why-is-raytracing-disabling-itself)
- [General improvements](#general-improvements)
  - [Nvidia Reflex](#nvidia-reflex)
    - [What is Nvidia Reflex?](#what-is-nvidia-reflex)
    - [What Nvidia reflex is NOT?](#what-nvidia-reflex-is-not)
    - [How to enable Nvidia Reflex for Ghostrunner](#how-to-enable-nvidia-reflex-for-ghostrunner)
  - [AMD improvements](#amd-improvements)
- [Resources](#resources)
- [Useful links](#useful-links)

# Frequently asked questions

## How to use the new always available instant restart?
In settings, ensure instant restart is set to 'on'. If you wish to rebind the key, it's the same entry as for quick restart on death, there is no new entry for this functionality.

## How can I use directX 12
To choose which directX to use, launch the game via steam, not a desktop shortcut. Alternatively add "-dx12" (without the quotes) to steam launch options.

## Should I use 11 or 12
DX11 for stability. DX12 if you want ray tracing and have an RTX card or dx11 is causing you issues


# Technical issues
## Why are my graphics/keybinds resseting?
Go to %LOCALAPPDATA%\Ghostrunner\Saved\Config\WindowsNoEditor
Set the things you want, then right click each file > properties > set as read-only.

## Nothing disables Vsync
This seems to be a rare issue where the in-game setting does not work. No workarounds are known, try to completley wipe the game and config, then reinstall.

## How to handle the input lag/broken vsync
Vsync in games tends to be subpar, Nvidia(and AMD for the most part) does it better.
Also, disable Windows 10 game mode, as well as this: <https://www.windowscentral.com/how-disable-and-remove-game-bar-windows-10-creators-update>

## Why is RayTracing disabling itself?
Seems to be a common bug, reasons and solutions are not yet known.


# General improvements

## Nvidia Reflex

### What is Nvidia Reflex?
In layman's terms Nvidia Reflex decreases the time taken for a frame to be rendered and sent to your display, which helps decrease latency. The benefit of it is varied, there are tons of variables that go into how well it will work, but worst case scenario as far as we know is that it won't do anything, so there is no disadvantages to keeping it enabled (apart from perhaps power consumption but that's negligible). 

### What Nvidia reflex is NOT?
Nvidia Reflex will NOT directly increase your FPS. While it can technically happen, it would be an indirect result of reducing the GPU load which would reduce thermal throttling and give you higher FPS, but because Reflex acts also as a frame limiter, it will prevent the framerate from raising too high which would bring the temperatures back up.

Nvidia Reflex is not a universal tool that works for all applications. It's up to the game developer to implement this in code, google to find an availability list (Obviously for Ghostrunner it's available).

### How to enable Nvidia Reflex for Ghostrunner
1. Update your graphics drivers to latest version (**You should always keep your GPU drivers up-to-date!!!**)
2. Enable "Ultra Low Latency" mode:
- Open Nvidia Control Panel (Right click on your desktop and the option is there)
- Click the "Manage 3D settings" tab on the left
- Scroll down until you see "Low Latency Mode" and set it to Ultra
- Hit apply
3. Start Ghostrunner and go to Settings > Video
4. Scroll all the way down and in the dropdown pick "Enabled + Boost" (In temperature constrained scenarios it might be beneficial to not enable Boost, test for yourself)

## AMD improvements
Equivalent settings are in per-app options in Radeon Adrenalin software. Enable Radeon Anti-lag or Enchanced Sync. Disable waiting for vertical refresh rate.

# Resources
- [Begginner's guide](https://docs.google.com/spreadsheets/d/1jWBOuxSY-zlBgzhkYnsVYtNJFscbObve67g9Xy_biV0/edit)
- [Inbounds speedtech doc](https://docs.google.com/spreadsheets/d/1RVfpfNUJEUBfPfs1Ch-7rmXD_IFO37Iyw50tFEgnEbY/edit?usp=sharing)
- [Out of Bounds speedtech doc](https://docs.google.com/spreadsheets/d/1r6YV0NYDE0wTVllcY1qSab4n7Z-VYIdu4Z3DuqsDE48)

# Useful links
- Micrologist's [trainer](https://github.com/Micrologist/GhostrunnerTrainer/releases)
- Dmgvol's [save unlocker](https://github.com/Dmgvol/GRUnlocker)

---
  <p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/Kellegram/Ghostrunner_faq">Ghostrunning FAQ</a> by <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://github.com/Kellegram">Kellegram</a> is licensed under <a href="http://creativecommons.org/licenses/by-nc/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY-NC 4.0<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/nc.svg?ref=chooser-v1"></a></p>  









