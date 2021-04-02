<img width="128" height="128" src="https://i.imgur.com/MFgAUdY.png" alt="icon_square">

# Xposed-Disable-FLAG_SECURE

Xposed Module to Disable `FLAG_SECURE`, enabling screenshots and recording in apps that normally wouldn't allow it.

This module is to specifically support Android 8-11.

## Requirements:

- Android 8.0+ (Oreo/SDK 26)

## Usage for LSPosed:

- Enable the module
- Select `System Framework`
- Select the target app in which you want to enable screenshots
- Reboot

## Note:

- This app does not prevent apps from detecting that you've taken a screenshot or recorded it like Snap or Instagram.
  This only enables it in apps that prohibit screenshots and recording. So don't screenshot your girlfriend's nudes.
  (You probably don't have one since you're reading this anyway)


- Apps Tested on:
    - Amazon Prime Video (Screenshots and Screen Recording of Media)
    - Telegram (Secret Chat & Disappearing Media)
    - Reddit (Anonymous Browsing Mode)
    - Google Chrome (Incognito Mode)
    - Brave Browser (Incognito Mode)


- This app is a fork of the existing apps but with better compatibility:
    - https://github.com/veeti/DisableFlagSecure/
    - https://github.com/LSPosed/DisableFlagSecure/
