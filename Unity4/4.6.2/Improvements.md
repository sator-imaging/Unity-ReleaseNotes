# Unity 4.6.2

https://unity3d.com/unity/whats-new/unity-4.6.2

## Improvements



*   Audio: Added WWW.GetAudioClipCompressed. Allows AudioClips obtained via WWW class to be loaded into memory compressed, similar to "Compressed in Memory" import option.
*   Graphics: Added MaterialPropertyBlock.Set\*() methods to overwrite existing values in a MaterialPropertyBlock instead of adding duplicates.
*   iOS: Add basic launch screen support.
*   iOS: Expose “set pause” as ObjC API.
*   Linux: Added more font fallbacks for Latin and CJK.
*   Oculus GearVR: Enabled low latency audio support.
*   Oculus Plugin: Future Oculus Plugin releases will no longer require Direct\_To\_Rift.exe
*   Oculus: Added VR friendly splash screen for Unity Free.
*   Scene View: DrawGizmo attribute now reports errors when used incorrectly, and has better documentation.
*   Standalone: Screen.dpi implemented for OSX and Windows standalone platforms.
*   UI: Change Text.m\_Text to protected and Text.text to virtual. In this way users can have control over the text contents when extending Text.
*   UI: Expose EventSystem.firstSelected to API.
*   WebPlayer UnityObject: It is now possible to identify the webplayer runtime version before loading content. This makes it possible to load different content based on the runtime version already installed.