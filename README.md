# Xcode9-lstdc-.6.0.9
Move Xcode 9 to Xcode10 to fix the lib stdc++


# Chinese version: Zhihu Link<herf= https://zhuanlan.zhihu.com/p/166520287> 

# English version:

Error：
ld: library not found for -l stdc++.6.0.9
Reason：
Xcode10 removed lib stdc++.6.0.9, Xcode 9 still has it.
Method 1：

Method 2：
add stdc++ from Xcode9 to Xcode10
1. location (Real)
cp Real/lstdc*  /Applications/Xcode.app/Contents/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS.sdk/usr/lib


2. location（Simultaion）
cp Simultaion/lstdc*  /Applications/Xcode.app/Contents/Developer/Platforms/iPhoneSimulator.platform/Developer/SDKs/iPhoneSimulator.sdk/usr/lib
