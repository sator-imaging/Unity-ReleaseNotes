# Unity 2018.4.32

https://unity3d.com/unity/whats-new/2018.4.32

## Known Issues in 2018.4.32f1



*   macOS: If the Android Tools are not installed through the Hub, macOS 10.15 (Catalina) default security settings will prevent the Android NDK binaries being executed. These settings have to be changed or a signed Android NDK (r16b) will be needed to build Android. More information here: https://developer.android.com/ndk/downloads/older\_releases.
    
*   Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.
    
*   Windows: The Cursor is visible when Cursor.visible is set to false and new InputSystem package is used ([1273522](https://issuetracker.unity3d.com/issues/the-cursor-dot-visible-equals-false-does-not-work-when-inputsystem-package-is-installed))
    
*   Polybrush: \[PolyBrush\] Something went wrong saving brush settings Warning is thrown when Saving a Brush after opening the PolyBrush Window ([1315475](https://issuetracker.unity3d.com/issues/polybrush-something-went-wrong-saving-brush-settings-warning-is-thrown-when-saving-a-brush-after-opening-the-polybrush-window))
    
*   Shader System: Freeze or crash with various stack traces when opening a project while connected to a VPN service ([1025558](https://issuetracker.unity3d.com/issues/editor-freezes-slash-crashes-when-connected-to-nordvpn))
    
*   Audio: \[editor\]\[fmod\]\[macOS\] Editor is preventing Mac OS from entering sleep mode automatically ([995866](https://issuetracker.unity3d.com/issues/editor-is-preventing-mac-os-from-entering-sleep-mode-automatically))
    
*   Packman: Package Manager doesn't show available updates ([1304459](https://issuetracker.unity3d.com/issues/package-manager-doesnt-show-available-updates))
    
*   Linux: Focus cannot be properly gained on play mode, making keyboard input switch screens ([1109908](https://issuetracker.unity3d.com/issues/linux-focus-cannot-be-properly-gained-on-play-mode-making-keyboard-input-switch-screens))
    
*   Audio: Crash on AudioSource::Stop when exiting Play mode ([1079263](https://issuetracker.unity3d.com/issues/crash-on-audiosource-stop-when-exiting-play-mode))