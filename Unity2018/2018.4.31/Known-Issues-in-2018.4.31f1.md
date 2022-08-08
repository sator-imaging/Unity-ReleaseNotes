# Unity 2018.4.31

https://unity3d.com/unity/whats-new/2018.4.31

## Known Issues in 2018.4.31f1



*   macOS: If the Android Tools are not installed through the Hub, macOS 10.15 (Catalina) default security settings will prevent the Android NDK binaries being executed. These settings have to be changed or a signed Android NDK (r16b) will be needed to build Android. More information here: https://developer.android.com/ndk/downloads/older\_releases.
    
*   Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.
    
*   Audio: \[editor\]\[fmod\]\[macOS\] Editor is preventing Mac OS from entering sleep mode automatically ([995866](https://issuetracker.unity3d.com/issues/editor-is-preventing-mac-os-from-entering-sleep-mode-automatically))
    
*   WebGL: \[2018.4 only\] Editor freezes when enabling Play mode after Building ([1300269](https://issuetracker.unity3d.com/issues/webgl-editor-freezes-when-enabling-play-mode-after-building))
    
*   Packman: Package Manager doesn't show available updates ([1304459](https://issuetracker.unity3d.com/issues/package-manager-doesnt-show-available-updates))
    
*   Shader System: Freeze or crash with various stack traces when opening a project while connected to a VPN service ([1025558](https://issuetracker.unity3d.com/issues/editor-freezes-slash-crashes-when-connected-to-nordvpn))
    
*   Audio: Crash on AudioSource::Stop when exiting Play mode ([1079263](https://issuetracker.unity3d.com/issues/crash-on-audiosource-stop-when-exiting-play-mode))
    
*   Linux: Focus cannot be properly gained on play mode, making keyboard input switch screens ([1109908](https://issuetracker.unity3d.com/issues/linux-focus-cannot-be-properly-gained-on-play-mode-making-keyboard-input-switch-screens))
    
*   Window Management: Pop-up windows like Color Picker close upon clicking them when they are hovered on immediately after opening ([1239613](https://issuetracker.unity3d.com/issues/pop-up-windows-like-color-picker-get-closed-when-clicked-immediately-after-opening-it))