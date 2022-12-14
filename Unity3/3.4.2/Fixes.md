# Unity 3.4.2

https://unity3d.com/unity/whats-new/unity-3.4.2

## Fixes

- [Editor](#editor)
- [Android](#android)
- [iOS](#ios)
- [Monodevelop](#monodevelop)
- [Webplayer](#webplayer)


### Editor

*   Fixed crash when editing audio source.
*   Fixed issues with garbage collection in Asset Store editor bindings which could cause the Asset Store to report JavaScript errors about undefined variables (most frequently "this.fromContext.results", "a.title" or "b.title").

### Android

*   Fixed crash with Unity Android non-pro ('basic') license.
*   Fixed corrupted splash image on Icecream-Sandwich.
*   Allow audio playback only when application is focused (prevents audio on the unlock screen).
*   Made sure the on-device-profiler only uses active network interfaces.
*   Fixed an issue where mscorlib.dll could not be found.

### iOS

*   Fixed random crashes when building with Xcode 4.2 (iOS SDK 5.0).
*   Fixed crash with auto-rotation on iOS 5.
*   Disabled workaround for ipad2 driver bug with msaa+colormask+blend when running on iOS 5 (was fixed by Apple).
*   Made Cache Path for AssetBundles be compatible with new Apple Guidelines: /Library/Caches instead of /Documents.

### Monodevelop

*   Fixed compilation issues of Javascript.

### Webplayer

*   Workaround for NVidia driver issue in Mac OS X 10.7.2, which makes web players display garbage on certain NVidia GPUs.