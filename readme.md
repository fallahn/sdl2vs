SDL2 Template Solution
----------------------

This solution demonstrates how to set up a basic SDL2 project for Android in Visual Studio 2019. The solution is explained in detail on [my blog](http://trederia.blogspot.com/2017/03/building-sdl2-for-android-with-visual.html).

## Modifications 2021-4-16

- Updated to use git submodules for SDL2 (since it has now migrated to git)

Once you have cloned this repository use `git submodule update --init` to obtain the source of SDL2, SDL_image and SDL_ttf

## Modifications 2020-01-15

- Microsoft Visual Studio 2019
- Fix crash on startup
- add hidapi lib
- fix x86 build
- Merge from from Mercurial > 2.0.11
- remove SDL_Application
- update AndroidManifest
- add free font and label hello world
- switch to c++17

## Modifications 2019-09-07

- Upgraded SDL2 sources to the latest from Mercurial (>2.0.10)
- Added SDL2-image
- Added SDL2-ttf
- Updated compiler and linker flags to be the same for both Debug and Release definitions

## Modifications 2019-01-11

The solution was upgraded to SDL 2.0.9 sources.

This version of SDL2 depends on Android SDK level 26, which at the time of writing does not ship with the latest Visual Studio.  As a result it is currently necessary to reconfigure Visual Studio to use separate installations of Android SDK and NDK.  The appropriate setting is found in Visual Studio under Tools > Options > Cross Platform > Android.

Because newer Android SDKs removed support for the Apache Ant build system, a Gradle project was substituted.  The Gradle project is a Visual Studio template and fully supported by Android/VC++.

— Evan Balster, [imitone](https://imitone.com) project
