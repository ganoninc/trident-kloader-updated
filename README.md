# Trident + Kloader Updated 

Trident+kloader is a utility that makes use of the Trident exploit chain.  
* Original Trident exploit: https://github.com/benjamin-42/Trident  

The original version by torachiyo didn't work for some firmwares/ devices, so here it is updated.  
* Original Verion can be found here: Trident + Kloader for iPhone 4S http://bbs.feng.com/forum.php?mod=viewthread&tid=11005851&extra=page%3D1  


It allows people with 32-Bit devices on iOS 9.1-9.3.4 to downgrade their device, without the use of a fully fledged jailbreak!

Usage description and Information can be found futher down!  

## Supported Firmwares/Devices:

* iPhone 4S [iPhone4,1 (N94AP)]:
  * iOS 9.1 (Boulder 13B143)
  * iOS 9.2.1 (Dillon 13D15)
  * iOS 9.3 (Eagle 13E233)
  * iOS 9.3 (Eagle 13E237)  
  * iOS 9.3.1 (Eagle 13E238)
  * iOS 9.3.2 (Frisco 13F69)
  * iOS 9.3.3 (Genoa 13G34)
  * iOS 9.3.4 (Genoa 13G35)

* iPhone 5 GSM [iPhone5,1 (N41AP)]:
  * iOS 9.3.2 (Frisco 13F69) (use version ipa 1.2.1)
  * iOS 9.3.3 (Genoa 13G34) (use version ipa 1.2.4)

* iPhone 5 Global [iPhone5,2 (N42AP)]:
  * iOS 9.2 (Castlerock 13C57)
  * iOS 9.2.1 (Dillon 13D15)
  * iOS 9.3.2 (Frisco 13F69)
  * iOS 9.3.4 (Genoa 13G35)

* iPhone 5c GSM [iPhone5,3 (N48AP)]:
  * iOS 9.2.1 (Dillon 13D15)
  * iOS 9.3.2 (Frisco 13F69)
  * iOS 9.3.3 (Genoa 13G34)

* iPhone 5c Global [iPhone5,4 (N49AP)]:
  * None (yet)

* iPad 2 WiFi [iPad2,1 (K93AP)]:
  * iOS 9.1 (Boulder 13B143)
  * iOS 9.2 (Castlerock 13C57)
  * iOS 9.2.1 (Dillon 13D15)
  * iOS 9.3 (Eagle 13E233)
  * iOS 9.3 (Eagle 13E237)
  * iOS 9.3.1 (Eagle 13E238)
  * iOS 9.3.2 (Frisco 13F69)
  * iOS 9.3.3 (Genoa 13G34)
  * iOS 9.3.4 (Genoa 13G35)

* iPad 2 GSM [iPad2,2 (K94AP)]:
  * iOS 9.1 (Boulder 13B143)
  * iOS 9.2 (Castlerock 13C57)
  * iOS 9.2.1 (Dillon 13D15)
  * iOS 9.3 (Eagle 13E233)
  * iOS 9.3 (Eagle 13E237)
  * iOS 9.3.1 (Eagle 13E238)
  * iOS 9.3.2 (Frisco 13F69)
  * iOS 9.3.3 (Genoa 13G34)
  * iOS 9.3.4 (Genoa 13G35)

* iPad 2 CDMA [iPad2,3 (K95AP)]:
  * iOS 9.1 (Boulder 13B143)
  * iOS 9.2 (Castlerock 13C57)
  * iOS 9.2.1 (Dillon 13D15)
  * iOS 9.3 (Eagle 13E233)
  * iOS 9.3 (Eagle 13E237)
  * iOS 9.3.1 (Eagle 13E238)
  * iOS 9.3.2 (Frisco 13F69)
  * iOS 9.3.3 (Genoa 13G34)
  * iOS 9.3.4 (Genoa 13G35)

* iPad 3 Wifi [iPad3,1 (J1AP)]:
  * iOS 9.3.4 (Genoa 13G35)

* iPad 3 CDMA [iPad3,2 (J2AP)]:
  * iOS 9.3.2 (Eagle 13E238)

* iPad 3 GSM [iPad3,3 (J2AAP)]:
  * iOS 9.3.3 (Genoa 13G34)

* iPod touch 5 [iPod5,1 (N78AP)]:
  * iOS 9.1 (Boulder 13B143)
  * iOS 9.3.2 (Frisco 13F69)

* iPad 2 Wifi (Mid 2012) 16gb-Only-Model [iPad2,4 (K93AAP)]  
  * iOS 9.1 (Boulder 13B143)
  * iOS 9.2 (Castlerock 13C57)
  * iOS 9.2.1 (Dillon 13D15)
  * iOS 9.3 (Eagle 13E233)
  * iOS 9.3 (Eagle 13E237)
  * iOS 9.3.1 (Eagle 13E238)
  * iOS 9.3.2 (Frisco 13F69)
  * iOS 9.3.3 (Genoa 13G34)
  * iOS 9.3.4 (Genoa 13G35)
 
 
### The following devices can be downgraded to 6.1.3 with Trident+Kloader:
(Because the OTA update for iOS 6.1.3 is still signed for devices sold with iOS 5.0)

* iPhone 4S [iPhone4,1 (N94AP)]
* iPad 2 WiFi [iPad2,1 (K93AP)]
* iPad 2 GSM [iPad2,2 (K94AP)]
* iPad 2 CDMA [iPad2,3 (K95AP)]

I successfully downgraded my iPad2,1 from 9.3.3 to 6.1.3 using those updated sources, the libimobiledevice MinGW Build (https://mega.nz/#!tt9zTB6D!S_uzQWfogZIuKzLACrFY56Rb_CTC0Oj0X1re6myU3T0) and odysseusOTA (http://dayt0n.github.io/odysseus/odysseus-0.999.zip) on Windows 10.


#### A compiled ipa made by DjSn0wfall is in the build directory, use Cydia Impactor to install it. 

Wait a few seconds after pressing the start button.

##### Mini guide for iPad 2,1 (Wifi only)

On my iPad2 (Wifi only), I saw a vertical green line on the right of the screen.

After I put my iPad 2 (Wifi only) in sleep mode with libimobiledevice
```Bash
idevicediagnostics sleep
```

and when the screen was black I used odysseusOTA with the correct 6.1.3 IPSW for my iPad2 (Wifi only)

```Bash
idevicerestore -e iPad2,1_6.1.3_10B329_Restore.ipsw
```
##### Important note about the mini guide

** iPhone 4S and iPad 2 (Wifi + 3G) users should follow another guide because this one doesn't downgrade the baseband, so if you don't downgrade the baseband too, your phone or the cellular connection of your iPad 2 will not work. Check this tutorial on reddit: https://www.reddit.com/r/jailbreak/comments/5l9pqy/tutorial_how_to_downgrade_to_ios_613_on_the/
