# @AlexFLAVI35/android-enable-multiple-users (fix)
This package enables Multiple users account feature on Android devices without root or custom loader.

Based on this [article](https://beebom.com/how-enable-multiple-user-accounts-any-android/), it adds
(or replace) in `/system/build.prop` file, the following properties:
* fw.max_users=3
* fw.show_multiuserui=1

## How to use it

First download the `enabler.zip` cloning the releases directly from [here](https://github.com/AlexFLAVIUS35/android-enable-multiple-users/releases).

Put your Android phone in recovery mode (following the instruction of your specific device), or
using adb:

```bash
adb restart recovery
```

On your device, select `ADB sideload` to enable the upload of a zip file, while from your computer
use the following command to upload the file:

```bash
adb sideload enabler.zip
```

You should see:

```bash
Done.
Ready to reboot.
```
