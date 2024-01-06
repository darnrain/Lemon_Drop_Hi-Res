![banner](https://github.com/darnrain/Lemon_Drop_Hi-Res/assets/60840489/84991fb0-06d5-4424-ba9d-06e3031abc99)
<p align="center">
Welcome to the future of music...<br>
The Lgv20 was first with the Android Nougat operating system.<br>
Now it's the first running in True Native Mode.<br>
With all 4 DACs enabled.<br>
A total of 98,304 channels in true stereo.<br>
</p>
<p align="center">
Warning<br>
Please always lower your volume levels before playing audio.<br>
Please listen at a safe volume level.<br>
</p>
<p align="center">
Lemon Drop Hi-Res development status: Active.<br>
latest release: v152.1<br>
Lemon Drop Hi-Res audio source code GitHub​<br>
</p>

<details>
<summary>Readme.</summary>
<br>
What's the the most important thing I need to do, before I root the Lgv20?

Before you flash the KDZ to downgrade your firmware for rooting, make a DUMP with LGUP all files, you don't need to dump system or cache. Put it in a very safe place, like google drive. It will have your EFS and your EFS has the IMEI number of that particular phone. If your EFS ever becomes corrupted then you can re-flash your EFS from your backup to get cell signal working again.

Can I just edit step3.bat and install the latest twrp in there?<br>
No. You need the old version of twrp to format data, then you can update twrp to the latest version. You only need to remove the encryption on the data partition once, when rooting your phone. The old version of twrp is the only version I know of, that can remove the encryption on the data partition.

My camera does not work after installing Lemon Drop Hi-Res?
If you were on LIneageOS or crDroid and then flashed Stock Oreo, then your camera may not work afterwords. The only fix that I know of is to root your phone again. Flash the KDZ to downgrade your firmware and root again.

What is the EFS?
"EFS stands for Encrypting File System, which is really important part of networking and communication for Android Smartphones, It also contains your device IMEI data."

Can all Lgv20 phones be rooted?
Most but not all.
How to check to see if you can root, lgv20 Anti-Rollback Version ARB<br>
https://xdaforums.com/t/how-to-check-to-see-if-you-can-root-lgv20-anti-rollback-version-arb.4372451/

Can my LS997 install the Lemon Drop Rom?
As far as I know there is no Oreo Stock rom for the LS997, so Auto_Debloat will not work on that model of phone. But you may be able to install Lineage OS depending on your firmware. Check your ARB.

Sprint LG V20 Model (LS997): Comprehensive Overview of Guides and Resources (and why most LS997 phones are unrootable)
https://www.reddit.com/r/lgv20/comments/h98lbe/sprint_lg_v20_model_ls997_comprehensive_overview/
</details>

<details open>
<summary>What works?</summary>
<br>
-Google Play Store
-Google Assistant
-Audio (input all three mics, & output)
-Display (with image retention fix & tweaked KCAL settings for optimal color)
-Bluetooth
-FM works on (H910) mod for VS995 & US996 link
-IR Remote
-LGMusic Player (for H910)
-Second screen
-usb
-Media playback
-fast charging
-Hardware buttons
-Camera (Camera improvement tweaks)
-GPS (USA gps fix by default & other countries optional) link
-Fingerprint
-DAC (Hi-Res Music Player Enabler v151.1 & (Enable system wide Quad DAC support. V8.2)
-Radio (VoLTE & Wifi Calling only tested on H910 with AT&T)
-Wifi (dual channel bonding on 2.4GHz + speed tweaks)
-Thermal Throttling (70c default max temp) link
-Video output via hdmi
-DRM Widevine L1

What does not work?

-Miracast (removed due to security concerns)

Known issues.

When using wired headphones the DAC needs to say on all the time, or you will have no audio and video will run slow. It's due to Hardware-Offloaded Audio Processing, in other words all the audio is routed through the ESS DAC. No software audio decoding on Lemon Drop Hi-Res, it's all hardware.
</details>

<details open>
<summary>Install Lemon Drop Hi-Res v151.1 H910-H915.</summary>
<br>
Warning ONLY flash on the H910-H915

What's included in v151.1?
Modded boot.img<br>
Triton removed<br>
LG RCT removed (root checker tool)<br>
twrp-3.7.0_9-0-h910<br>
Updated Oreo Modem Drivers<br>
Magisk v24.3<br>
ezV2020 Kernel v1.0<br>
New GPU drivers 313.0 V11<br>
Hi-Res Music Player Enabler v151.1<br>
DAC_Enabler+LGMusic_v1.3_Oreo<br>
Speed mod v5.31 includes image retention fix<br>
Thermal_Engine_Mod_v7.0_70c<br>
Enable system wide Quad DAC support. V8.2<br>
Added AdAway default blocklist to /system/etc/hosts (aka ad blocker)<br>
Added United States GPS Fix<br>
Added Camera improvement tweak<br>
Added Internet Speed Tweaks<br>
Added the Lemon Drop boot logo<br>
Added Zram of 2GB + LZ4 algorithm + Zram optimization tweaks<br>
Added Hide boot warning message<br>
Added dual channel bonding on 2.4GHz<br>
High Impedance on headphones under 50 ohm.<br>

Updating Lemon Drop Hi-Res.
Flash in twrp to update.

Installation instructions:
Before installing Lemon Drop Hi-Res, your phone needs to be rooted with the latest version of twrp. The H915 needs to install the H910 twrp.

Update twrp. twrp-3.7.0_9-0-h910.img

With the phone powered off, hold the down volume button and plug in usb to computer and phone.

type on your computer:

fastboot flash recovery twrp-3.7.0_9-0-h910.img
fastbboot reboot
take battery out
put back in
go into twrp by doing a factory reset. How to factory reset the Lgv20

1. First download the two required files.

If you are having issues downloading the rom you can try this download manager for Firefox.
Turbo Download Manager

H910_20g_Oreo_full_rooted.zip
Lemon_Drop_Hi-Res_v151.x_H910-H915_Lgv20_flashable.zip

2. Then copy both files to the micro sdcard on phone
3. Reboot into twrp
4. Click Wipe
5. Format Data Partition (this will erase your internal storage on the phone)
6. Click back and reboot into recovery again. aka twrp
7. Flash H910_20g_Oreo_full_rooted.zip
8. Flash Lemon_Drop_Hi-Res_v151.x_H910-H915_Lgv20_flashable.zip
9. Reboot into system, run setup

Notes:
You can use an app like package manager to debloat more apps on your phone.

Good idea to reinstall your EFS to get cell signal working. Under How to Root the H910 and install Lemon Drop Hi-Res? You only need to do this once.

You can DeGoogle at any time, if you want. Under I want to DeGoogle after installing Lemon Drop Hi-Res, how can I do that?
</details>
