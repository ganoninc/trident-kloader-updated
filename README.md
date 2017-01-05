# Trident + Kloader updated 

The original version by torachiyo didn't work for the iPad2,1 (Wifi only) iOS 9.3.3 and 9.3.1, so here it is updated.

I successfully downgraded my iPad2,1 from 9.3.3 to 6.1.3 using those updated sources, the libimobiledevice MinGW Build (https://mega.nz/#!tt9zTB6D!S_uzQWfogZIuKzLACrFY56Rb_CTC0Oj0X1re6myU3T0) and odysseusOTA (http://dayt0n.github.io/odysseus/odysseus-0.999.zip) on Windows 10.

* Original Trident exploit: https://github.com/benjamin-42/Trident
* Original Trident + Kloader for iPhone 4S: http://bbs.feng.com/forum.php?mod=viewthread&tid=11005851&extra=page%3D1


It should work on the following devices:

* iPhone4,1 (N94AP), iOS 9.3 (Eagle 13E233)
* iPhone4,1 (N94AP), iOS 9.3 (Eagle 13E237)
* iPhone4,1 (N94AP), iOS 9.3.1 (Eagle 13E238)
* iPhone4,1 (N94AP), iOS 9.3.2 (Frisco 13F69)
* iPhone4,1 (N94AP), iOS 9.3.3 (Genoa 13G34)
* iPhone4,1 (N94AP), iOS 9.3.4 (Genoa 13G35)
* iPhone5,1 (N41AP), iOS 9.3.2 (Frisco 13F69)
* iPhone5,2 (N42AP), iOS 9.2.1 (Dillon 13D15)
* iPhone5,2 (N42AP), iOS 9.3.2 (Frisco 13F69)
* iPhone5,3 (N48AP), iOS 9.3.2 (Frisco 13F69)
* iPhone5,3 (N48AP), iOS 9.3.3 (Genoa 13G34)
* iPad2,1 (K93AP), iOS 9.3.1 (Eagle 13E238)
* iPad2,1 (K93AP), iOS 9.3.2 (Frisco 13F69)
* iPad2,1 (K93AP), iOS 9.3.3 (Genoa 13G34)
* iPad2,2 (K94AP), iOS 9.3.2 (Frisco 13F69)
* iPad2,3 (K95AP), iOS 9.3.2 (Frisco 13F69)
* iPad2,3 (K95AP), iOS 9.3.3 (Genoa 13G34)
* iPad2,4 (K93AAP), iOS 9.3.2 (Frisco 13F69)
* iPad3,1 (J1AP), iOS 9.3.4 (Genoa 13G35)
* iPad3,2 (J2AP), iOS 9.3.2 (Eagle 13E238)
* iPad3,3 (J2AAP), iOS 9.3.3 (Genoa 13G34)
* iPod5,1 (N78AP), iOS 9.3.2 (Frisco 13F69)

But only those devices can be downgraded to iOS 6.1.3 because the OTA update for iOS 6.1.3 is still signed for devices sold with iOS 5.0:

* iPhone4,1 (N94AP), iOS 9.3 (Eagle 13E233)
* iPhone4,1 (N94AP), iOS 9.3 (Eagle 13E237)
* iPhone4,1 (N94AP), iOS 9.3.1 (Eagle 13E238)
* iPhone4,1 (N94AP), iOS 9.3.2 (Frisco 13F69)
* iPhone4,1 (N94AP), iOS 9.3.3 (Genoa 13G34)
* iPhone4,1 (N94AP), iOS 9.3.4 (Genoa 13G35)
* iPad2,1 (K93AP), iOS 9.3.1 (Eagle 13E238)
* iPad2,1 (K93AP), iOS 9.3.2 (Frisco 13F69)
* iPad2,1 (K93AP), iOS 9.3.3 (Genoa 13G34)
* iPad2,2 (K94AP), iOS 9.3.2 (Frisco 13F69)
* iPad2,3 (K95AP), iOS 9.3.2 (Frisco 13F69)
* iPad2,3 (K95AP), iOS 9.3.3 (Genoa 13G34)

## A compiled ipa is in the build directory, use Cydia Impactor to install it. 

Wait a few seconds after pressing the start button.

### Mini guide for iPad 2,1 (Wifi only)

On my iPad2 (Wifi only), I saw a vertical green line on the right of the screen.

After I put my iPad 2 (Wifi only) in sleep mode with libimobiledevice
```Bash
idevicediagnostics sleep
```

and when the screen was black I used odysseusOTA with the correct 6.1.3 IPSW for my iPad2 (Wifi only)

```Bash
idevicerestore -e iPad2,1_6.1.3_10B329_Restore.ipsw
```
### Important note about the mini guide

** iPhone 4S and iPad 2 (Wifi + 3G) users should follow another guide because this one doesn't downgrade the baseband, so if you don't downgrade the baseband too, your phone or the cellular connection of your iPad 2 will not work. Check this tutorial on reddit: https://www.reddit.com/r/jailbreak/comments/5l9pqy/tutorial_how_to_downgrade_to_ios_613_on_the/
