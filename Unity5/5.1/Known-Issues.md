# Unity 5.1

https://unity3d.com/unity/whats-new/unity-5.1

## Known Issues



*   Editor: Renaming file-locked assets may lead to lost data.
*   On Windows, using a proxy server will crash Unity when trying to access the Asset Store.
*   Mecanim: Setting AnimatorState.speed to 0 doesn’t pause the animation as expected.
*   Mecanim: Switching runtime AnimatorState.speed from positive to negative break animation continuity.
*   Mecanim: Copy-Pasting StateMachines will not copy the Transitions inside of them.
*   Unity VR
    *   Oculus 0.6 runtime is required
    *   Mac and Gear VR support coming in 5.1.0 patch 1
    *   At this time if you wish to continue using Legacy Oculus plugins in your project we recommend you keep the 'Virtual Reality Supported' checkbox unchecked. In a later release this checkbox will have no impact if a legacy plugin is present.
    *   VRSettings.renderScale is non-functional, fixed in 5.1.0 patch 1
    *   Apps that use linear lighting won't render. Recommended to use gamma for now.
    *   If your app won't launch in VR mode, use command line option "-vrmode oculus"
    *   UI: Screen Space - Overlay not supported. Recommended to use Screen Space - Camera or World Space. "Scale With Screen Size" is recommended so UI looks the same on Gear VR.
    *   Toggling VRSettings.loadedDevice at runtime crashes, fixed in 5.1.0 patch 1