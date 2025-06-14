![](https://socialify.git.ci/PreviousAlone/Nnngram/image?description=1&forks=1&issues=1&name=1&owner=1&pulls=1&stargazers=1&theme=Dark)

# Nagram-reborn based on Nullgram

## What is Nullgram
[![Telegram](https://img.shields.io/static/v1?label=Telegram&message=@NullgramClient&color=0088cc)](https://t.me/NullgramClient)  [![Build CI](https://github.com/PreviousAlone/Nnngram/actions/workflows/ci.yml/badge.svg)](https://github.com/PreviousAlone/Nnngram/actions/workflows/ci.yml)

[中文](README_CN.md)  [日本語](README_JA.md)

Nullgram is an **free and open source** third-party Telegram client, based on the official source code for [Telegram App for Android](https://play.google.com/store/apps/details?id=org.telegram.messenger).

## Why Nullgram
Null used in computer programming for an uninitialized, undefined, empty, or meaningless value.
In the name of Nullgram, the purpose is to express that there is no such bad things. Nullgram won't push FCM-Notification "nmsl"[^2] or somethings like that to your phone, won't send ads[^4] to channels, won't compete maliciously[^5] or publish malicious rumors about competitors

## How to Contribute

### I want to add new feature

Great!

Make sure you fully understand [the Development Document](./docs/CONTRIBUTING.md).
If you haven't read it.**THEN GO READ IT.**

Then just create a new pull request and I should be review in a couple of days.

### I've encountered a bug!

First, make sure you have the latest version installed (check the channel, Play store versions usually have a delay).

Then, if the issue appears in the official Telegram client too, please submit it to the officials, (be careful not to show Nullgram in the description and screenshots, the official developers doesn't like us!).

Then, please detail your issue (ENGLISH ONLY), create an issue or submit it to our group with #bug.

Make sure using the issue template and writing the detailed version number I DO NOT KNOW WTF IS _I HAVE BEEN USING THE LATEST VERSION_

If you experience a crash, you can use logcat to catch the log (TAG: `Nnngram` ).

### Compilation Guide

You will require Android NDK rev. 21 and Android SDK 14

1. Download the Telegram source code from https://github.com/PreviousAlone/Nnngram
2. Download the ccache from [here](https://ccache.dev/) and make sure it is in your `PATH`.
3. Replace release.keystore in TMessagesProj/config with your own one.
4. Fill out RELEASE_KEY_PASSWORD, RELEASE_KEY_ALIAS, RELEASE_STORE_PASSWORD in gradle.properties to access your release.keystore
5.  Go to https://console.firebase.google.com/, create one android app with application ID `top.qwq2333.nullgram`, turn on firebase messaging and download google-services.json, 
    which should be copied to the same folder as TMessagesProj.
6. Open your terminal and run `./gradlew assembleRelease` to build the APK

## Sponsor

Thanks to Jetbrains for allocating free open-source licences for IDEs.

[<img src="docs/jetbrains-variant-3.png" width="200"/>](https://jb.gg/OpenSource)


[^1]: https://telegra.ph/%E6%9C%89%E5%85%B3-Nekogram-Lite-%E7%9A%84%E6%95%85%E4%BA%8B-04-09

[^2]: https://sm.ms/image/FAKi3mx6XwqlvRj

[^3]: https://t.me/NekogramX/418

[^4]: https://t.me/zuragram/392

[^5]: https://t.me/sayingArchive/15428
