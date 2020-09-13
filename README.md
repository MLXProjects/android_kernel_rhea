# android_kernel_rhea -> cm-11.0
This is the CM11 kernel (version 3.0.101) for the Samsung Galaxy Pocket Plus (a.k.a. coriplus) GT-S5301 device.  
# History
This kernel was originally released for the Pocket Neo (corsica, S5310) but was adapted by me in order to make touch and other things work on coriplus.  
# Current status
Touchscreen works, bluetooth is (sort-of) working and there's an effort to make the Wi-Fi work here (half-works). RIL seems to work.  
Power management seems to be mostly working as the power on/off/suspend works, but at suspend the phone may sometimes shutdown.  
I suspect this is a touch driver issue, as before modding it the suspend worked nicely. Also, as the kernel had DT2W (double tap to wake) support at the other touch driver, that may conflict with current touch (which hasn't dt2w support).  
Bluetooth driver stops responding after startup and restarts itself after searching for devices and/or trying to pair.  
Wi-Fi driver seems to work correctly.
# coriplus hardware
Processor: Broadcom BCM21654 (not the G variant!)  
RAM: 512MB (450~480MB available from the system)  
Display: ILI9341 C (240x320 2.8", 140DPI aprox.)  
Wi-Fi & BT chip: Broadcom BCM4334  
Storage: 3.7GB  
Main partitions: system 896MB, userdata 1.2GB, cache ~500MB, boot & recovery both 8MB  
