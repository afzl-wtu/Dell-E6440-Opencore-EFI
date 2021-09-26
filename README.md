# Dell E6440 Opencore EFI Folder

What is working:
  Everything works except some issues in bluetooth and in sound when connected a Headphone

Wireless card is Intel 6235 working very well.

# Instructions:
    1. Change SMBIOS Serial Number with [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
          MacBookAir6,2 or MacBookPro11,4.   [Deatails](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#platforminfo)
    2. noise in headphones can be fixed by downloading using alc-verb in [AppleAlc](https://github.com/acidanthera/AppleALC/releases).
       open a terminal at the folder where alc-verb is downloaded. and give the following command
        hda-verb 0x1a SET_PIN_WIDGET_CONTROL 0x24           [Reference](https://osxlatitude.com/forums/topic/11316-how-to-fix-static-noisedistortioncrackling-sound-and-combo-jack-on-laptops/)
