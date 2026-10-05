# Kindle Bluetooth Controls

Kindles from 2016 and newer come with Bluetooth chips, which can connect to various wireless accessories. You might not realise this, because the setting is unavailable unless you register your Kindle to Amazon in an Audible-supported region. This plugin, based off scripts from gambatte-k2, gives you access to the official Kindle Bluetooth control menus without first having to ask Amazon's permission.

## Usage
1. Download the repo.
2. Connect your Kindle. It must be [jailbroken] and have [Universal Hotfix v2.3.7] and/or [KUAL] installed. It must be a recent model.
3. Copy over the contents of `documents` to `/mnt/us/documents/` and the contents of `extensions` to `/mnt/us/extensions/`
4. Safely eject you Kindle. You will have both scriptlet and KUAL shortcuts to enable/disable Bluetooth. 
5. It will work mainly with headphones/speakers, probably less so with anything else.

## Compatibility
Kindle Oasis (2016) and newer. Bluetooth does not exist on the original Kindle, Kindle Keyboard, Kindle 4, Kindle Touch and similar older Kindles. Scriptlets require the [Universal Hotfix v2.3.7].

## FAQs

### I want to connect a Bluetooth keyboard/game controller/page turner to my Kindle?
[Kindle Bluetooth only officially supports audio devices]. Instead, please use [kindle-hid-passthrough] with [kindle-button-mapper-rs], which uses an alternative Bluetooth stack to support devices other than just headphones and speakers.

### I want to use my Kindle as a word processor now that I have a Bluetooth keyboard connected?
Either use [KOReader]'s plaintext editor (Top menu >> Wrench/Screwdriver icon >> Text editor), [AbiWord for Kindle], [TextAdept for Kindle], or [N31welt's Text Editor for Kindle]

### I want to listen to audiobooks/music from my Kindle via Bluetooth headphones/speakers?
Please use [KinAMP]; it's a music player for the Kindle that really whips the llama's ass! 

### KOReader Bluetooth controls?
[KinAMP] adds Bluetooth controls to KOReader under Top menu >> Wrench/Screwdriver icon >> KinAMP Player (Page 2) >> KinAMP's hamburger menu >> Bluetooth and Bluetooth devices. You can enable/disable Bluetooth and connect to audio devices previously added in the official Kindle Bluetooth settings here (that's what this plugin is for). Please don't expect KinAMP to keep playing your audio as you switch from Kindle usermode to KOReader and back; expect to have to reconnect to your audio devices and restart your music/audiobook.

Otherwise, please use [kindle-hid-passthrough] with [kindle-button-mapper-rs] for more Bluetooth device options.

## What are the limitations?
This plugin does not...
- enable Amazon's official audio player (intended for Audible books). 
- enable Amazon's official Bluetooth switch in the top menu. As a workaround, this script provides ON and OFF switches.
- improve the Kindle's poor vanilla Bluetooth compatibility

The Bluetooth control menu may also fail to pop up if you play with it too much, switching it on and off. Rebooting may fix this.

### How does this interact with KOReader?

## See also
- [The original Readme](Original-Readme.md)
- [kindlebt, a Bluetooth API for Kindle PW5 and up](https://github.com/Sighery/kindlebt)
- [Using external keyboard with KOReader's Text Editor @ MoileRead Forums](https://www.mobileread.com/forums/showthread.php?t=359844)

## Credits
- [GreenCat777](https://github.com/GreenCat-777) @ Kindle Modding Community Discord
- [@CrazyElectron's gambatte-k2](https://github.com/crazy-electron/gambatte-k2) 

[jailbroken]: https://kindlemodding.org/
[Universal Hotfix v2.3.7]: https://kindlemodding.org/jailbreaking/Legacy/post-jailbreak/setting-up-a-hotfix/
[KUAL]: https://www.mobileread.com/forums/showthread.php?t=225030
[Kindle Bluetooth only officially supports audio devices]: https://www.amazon.com/gp/help/customer/display.html?nodeId=TIHMXAou9Wm1q17sg5
[kindle-hid-passthrough]: https://github.com/zampierilucas/kindle-hid-passthrough
[kindle-button-mapper-rs]: https://github.com/zampierilucas/kindle-button-mapper-rs
[KinAMP]: https://github.com/kbarni/KinAMP/
[KOReader]: https://github.com/koreader/koreader
[AbiWord for Kindle]: https://www.mobileread.com/forums/showthread.php?t=374237
[TextAdept for Kindle]: https://github.com/kbarni/textadept-kindle
[N31welt's Text Editor for Kindle]: https://www.mobileread.com/forums/showthread.php?t=341123
