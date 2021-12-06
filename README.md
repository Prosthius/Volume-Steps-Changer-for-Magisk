# Volume steps changer for magisk
___
## What is this mod? 
It doubles the media volume steps from 15 to 30 and call volume steps from 7 to 14.
Inspired by mods such as the xposed volume steps+ mod and custom roms alike I thought I'd give magisk a spin after being out of the android development scene for a while.

___

## How does it work? 
it works by using magisk system.prop to add a build prop line
``` 
ro.config.media_vol_steps=30
ro.config.vc_call_vol_steps=14
```
___

# Requirements
+ magisk 19.0+
+ Android 9 or higher (Works on android 11!)
___
# Installation
Flash the zip in magisk module installer.

# FAQ
+ __will this work on X device?__ 
   Since this just makes build.prop edits that every android should accept because of the code to accept theese is in the [AudioService.java](https://android.googlesource.com/platform/frameworks/base/+/master/services/core/java/com/android/server/audio/AudioService.java#624)
