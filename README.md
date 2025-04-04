# Disable-FLAG_SECURE

Xposed Module to Disable `FLAG_SECURE`, enabling screenshots, screen sharing and recording in apps that normally
wouldn't allow it.

![Download-Count](https://img.shields.io/github/downloads/Xposed-Modules-Repo/com.varuns2002.disable_flag_secure/total?color=blue)

## Usage for LSPosed:

- Enable the module
- Select `System Framework`
- Select the target app in which you want to enable screenshots
- Reboot

## Note:

- This app does not prevent apps from detecting that you've taken a screenshot or recorded it like Snap or Instagram.
  This only enables it in apps that prohibit screenshots and recording. So don't screenshot your girlfriend's nudes.
  (You probably don't have one since you're reading this anyway)

- This module may work on other apps too with or
  without [`liboemcrypto.so disabler`](https://github.com/Magisk-Modules-Repo/liboemcryptodisabler).
  ([Read Additional Instructions](#additional-information-on-drm-encrypted-content))

- Untested but may work on [LSPatch](https://github.com/LSPosed/LSPatch)

- You can contribute names of apps [here](https://github.com/VarunS2002/Xposed-Disable-FLAG_SECURE) that are working and
  are not listed here, so I can add it to the list.

- If you face any issue or have a suggestion then feel free to open an
  issue [here](https://github.com/VarunS2002/Xposed-Disable-FLAG_SECURE).

- This app is a fork of the existing apps but with better compatibility:
    - https://github.com/veeti/DisableFlagSecure/
    - https://github.com/LSPosed/DisableFlagSecure/
    - https://gitlab.com/azhao12345/disableflagsecure/

- Apps Tested on:
    - Amazon Prime Video
    - Netflix ([Read Additional Instructions](#additional-information-on-drm-encrypted-content))
    - Disney+ ([Read Additional Instructions](#additional-information-on-drm-encrypted-content))
    - Telegram (Secret Chat & Disappearing Media)
    - Reddit (Anonymous Browsing Mode)
    - Google Chrome (Incognito Mode)
    - Brave Browser (Incognito Mode)
    - WhatsApp (View Once Media & Profile Picture)
    - Firefox (Incognito Mode)
    - Toffee OTT
    - Booking.com

### Additional Information on DRM encrypted content

This is applicable only for some apps on some devices. If you aren't facing any issues, you can ignore these
instructions.

When playing DRM encrypted content, most devices will use hardware decryption capabilities. This hardware decryption
will push the video directly onto the screen, bypassing any screenshots/screenshare/recording functionality.

One possible solution is to disable this hardware decryption by installing the Magisk
module [`liboemcrypto.so disabler`](https://github.com/Magisk-Modules-Repo/liboemcryptodisabler). This will force the
device to not use hardware decryption and in combination with this module will enable screenshots, screen sharing and
recording.

Installing this module might have unintended consequences, such as lowered video quality and a reduced Widevine security
level.
[Read more](https://forum.xda-developers.com/t/magisk-module-liboemcrypto-disabler-for-drm-protected-content-netflix-my5-etc.3794393)
