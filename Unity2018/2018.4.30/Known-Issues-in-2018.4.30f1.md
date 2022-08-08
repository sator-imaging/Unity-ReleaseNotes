# Unity 2018.4.30

https://unity3d.com/unity/whats-new/2018.4.30

## Known Issues in 2018.4.30f1



*   Audio: Crash on AudioSource::Stop when exiting Play mode ([1079263](https://issuetracker.unity3d.com/issues/crash-on-audiosource-stop-when-exiting-play-mode))
    
*   Linux: Focus cannot be properly gained on play mode, making keyboard input switch screens ([1109908](https://issuetracker.unity3d.com/issues/linux-focus-cannot-be-properly-gained-on-play-mode-making-keyboard-input-switch-screens))
    
*   Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.
    
*   macOS: If the Android Tools are not installed through the Hub, macOS 10.15 (Catalina) default security settings will prevent the Android NDK binaries being executed. These settings have to be changed or a signed Android NDK (r16b) will be needed to build Android. More information here: https://developer.android.com/ndk/downloads/older\_releases.