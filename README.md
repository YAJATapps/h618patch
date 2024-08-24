## H618 patches  

diff -r from AOSP build tree to the OEM tree with changes to support OrangePi Zero 2W. 

H618-Android12-Src is the official source code from the manufacturer's website and I have been able to compile and run it.  

android-12.0.0_r11 is downloaded from https://android.googlesource.com/

This includes changes to go from:  
android-12.0.0_r11 -> H618-Android12-Src  

Identical folders like bionic/ are not included.  

Excluded dirs (since they only exist in H618):  
device/softwinner/  
longan/  
vendor/  

**Note:** These changes were not intended to be applied on any random aosp version with patch. Its purpose is to identify the main changes that were required to boot on this device.  
Example: The fs_mgr, vold etc.
