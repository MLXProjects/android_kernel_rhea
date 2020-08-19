# android_kernel_rhea -> zaninplus
This branch uses the Zanin kernel as base for coriplus (instead of using corsica's one) as they're more compatible.  
Yes, the name is a fusion of zanin and coriplus :P  

# Why use another device? 
As known -by me-, the original corsica kernel boots just fine on coriplus, but there are some problems with power management and such things. Also Wi-Fi/BT chip is different (BCM4330 on corsica vs BCM4334 on coriplus). Using another device which has almost the same hardware increases greatly the kernel stability and thus becomes more usable.  
Also, trying to get the corsica kernel to work correctly is hard because I don't have the skills to know most things about how the kernel works. 

# How to compile this? 
I recommend using the arm-linux-androideabi 4.6 toolchain (from AOSP or another source is fine), but IIRC 4.9 arm-eabi works fine. Other toolchains weren't tested. 
After setting ARCH=arm and CROSS_COMPILE=/path/to/your/toolchain/bin/arm-blah- you need to make using *cyanogenmod_zanin_defconfig*.
