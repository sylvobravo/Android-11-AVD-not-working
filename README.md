# Android-11-AVD-not-working
the emulator process for AVD was killed/terminated.
If you get this kind of error when trying to run AVD for android 11 Api 30
but you don't get this error on android 10 AVD Api 29 or Lesser
Don't panic, you are in the right place. Here I will show you how to fix this

If you get this kind of error it's either of two things -:

    1.) intel Hardware Accelerated Execution Manager (HAXM) not installed
    2.) amdvlk32.dll or vulkan-1.dll not found
    
**How to fix this**

## 1.) intel Hardware Accelerated Execution Manager (HAXM) not installed

    a.) Download intel Hardward Accelerated Execution Manager (Haxm) directly from the official repository and install
    https://github.com/intel/haxm/releases
    b.) Install using android studio SDK Manager
        -Open the SDK Manager.
        -Click the SDK Update Sites tab and then select Intel HAXM.
        -Click OK.
        -After the download finishes, run the installer. Typically, you can find the installer in the following location:
        sdk/extras/intel/Hardware_Accelerated_ExecutionManager/IntelHAXMversion.dmg
        -Follow the on-screen instructions to complete the installation.
## 2.) amdvlk32.dll or vulkan-1.dll not found
    1. Download amdvlk32.dll 
       (https://www.dll-files.com/download/4ea0801efec4bd896087cda211baa04c/amdvlk64.dll.html?c=c2N3SlpFOVlSWmZmcHlsWVMyaVM1Zz09)
    2. Download vulkan-1.dll 
       (https://www.dll-files.com/download/dd77ed1733723e46d8b4ad541c086c6d/vulkan-1.dll.html?c=a3NsRGpTbllIcXRHMGZxeFVGZklUUT09)
    3. Extract the amdvlk32.dll and vulkan-1.dll Zip Files
    4. copy the amdvl32.dll and vulkan-1.dll files into your system path "C:\Windows\System32", 
       if your system supports 64 bits "C:\Windows\SysWOW64"
    5. That's it
 *Note:* If the name of the vulkan-1.dll is not vulkan-1.dll rename it to vulkan-1.dll
