# A. Allwinner_C10_Tablet_Resources
A collection of details and resources for the C10 Allwinner running Android 14

# B. Specs and Caveats
1) CPU - 
    4 x big 
    4 x small
2) RAM - 
    3GB - Physical
    5GB - Virtual
3) OpenGL ES - 
    3.2
4) Storage - 
    64GB - Max
    ~24GB - used/reserved by system
5) No real sensors except accelerometer
6) VNDK Level - 33
    Android Version - 14
7) Virtual A/B
8) No publicly released Kernel Sources
9) Security Patch Level (System) - March 2024 - Does not pass strong integrity due to the google policy of having received a security patch within the last year
10) VBMeta is disabled upon unlocking the bootloader
    Do not alter any other partition except init_boot to ensure bootability upon locking the bootloader
11) Display resolution - 1280 x 800
12) No 3.5mm headphone jack
13) Display Size - 10 inches
14) Main camera - 8MP (with a single-tone LED flash)
15) Front camera - 5MP
16) 10-point Multi-touch
17) GSI image type - system-arm64-ab.img

# C. Bootloader Unlock Procedure
1) Spam build number in Settings>About
2) Enable OEM Unlocking in System>Developer options
3) Reboot to bootloader - adb reboot bootloader/vol down+power
4) fastboot oem unlock
5) Restart by fastboot reboot
6) Unlocked BL Successfully
