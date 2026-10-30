# Tin Hat for Android

Tin Hat is a chat and voice app for groups of friends, on your own Tin Hat server or a friend's. This repository
holds the Android app's releases. More about Tin Hat: https://tinhat.dev

## Install
1. On your phone, open the [latest release](https://github.com/TinHatLabs/TinHatAndroid/releases/latest) and
   download `tinhat-<version>.apk`.
2. Open the download. Android asks once whether your browser (or files app) may install apps: allow it.
3. Open Tin Hat and enter your server's name or an invite link.

Tin Hat needs Android 10 or newer. It isn't on Google Play (yet).

## Updates
Tin Hat updates itself. It checks https://tinhat.dev/android/latest.json, which names the newest release here, and
believes it only with a valid signature by the Tin Hat release key. It downloads the APK from this repository's
release of that version and installs it only when the APK is signed with the same certificate as the Tin Hat already
on the phone. The first update asks once to allow Tin Hat to install apps.

Coming from 0.2.3 or earlier: install 0.2.4 or later by hand once; it updates itself from then on.

## Check a download
- The APK's signing certificate (SHA-256):
  `C9:EC:B6:BA:A1:6C:59:4C:E9:7B:97:A1:0B:CA:36:CE:B6:16:13:65:52:CE:FA:A0:8A:08:E8:8A:AA:F0:FE:20`
  (`apksigner verify --print-certs tinhat-<version>.apk`).
- Each release has `SHA256SUMS` and `latest.json`, signed with the Tin Hat release key (minisign):
  `RWQUG5ce+eVTK+HZgYoCViu7WY1nwnbLR8s54/zRQR0DLiACjVuh5Mkv`
  (`minisign -Vm SHA256SUMS -P RWQUG5ce+eVTK+HZgYoCViu7WY1nwnbLR8s54/zRQR0DLiACjVuh5Mkv`).

## Source
The Android app's source isn't published yet.
