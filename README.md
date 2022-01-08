# Android-11-AVD-not-working
the emulator process for AVD was killed/terminated.
If you get this kind of error when trying to run AVD for android 11 Api 30
but you don't get this error on android 10 AVD Api 29 or Lesser
Don't panic, you are in the right place. Here I will show you how to fix this

If you get this kind of error it's either of two things -:

    1.) intel Hardware Accelerated Execution Manager (HAXM) not installed
    2.) amdvlk32.dll or vulkan-1.dll not found
    
**How to fix this**

# 1.) intel Hardware Accelerated Execution Manager (HAXM) not installed

    a.) Download intel Hardward Accelerated Execution Manager (Haxm) directly from the official repository and install
    https://github.com/intel/haxm/releases
    b.) Install using android studio SDK Manager
      
