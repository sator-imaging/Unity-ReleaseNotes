# Unity 2018.2

https://unity3d.com/unity/whats-new/unity-2018.2.0

## The following are changes and fixes to 2018.2.0 features and regressions...

- [Fixes](#fixes)


### Fixes

*   Editor: Fixed Visual Studio reloads all package .csprojs when adding or removing a .cs file in the project ([1051901](https://issuetracker.unity3d.com/issues/visual-studio-reloads-all-package-csprojs-when-adding-or-removing-a-cs-file-in-the-project), 1051902)
    
*   Graphics: Fix framebuffer cleared to black when using Vuforia or other native rendering plugins with OpenGL ES ([1046360](https://issuetracker.unity3d.com/issues/vuforia-canvas-is-rendered-black-with-ar-camera-when-running-vuforias-build-with-mali-gpu))
    
*   Package Manager: Fixed the _package not found_ errors when creating a new project while offline. (1056225)
    
*   Scripting: Added missing 2017\_4\_OR\_NEWER symbol to 2018.x ([1050962](https://issuetracker.unity3d.com/issues/unity-2017-4-or-newer-preprocessor-is-not-recognised-when-using-number-if-unity-2017-4-or-newer-in-a-script), 1056576)
    
*   Scripting: Make Gradient APIs accessible from threads again ([1050296](https://issuetracker.unity3d.com/issues/scripting-slash-particles-gradient-scripting-api-thread-checks-have-changed-after-bindings-upgrade))
    
*   Scripting Upgrade: Fix System.IO.IOException when reading from Process output (1047186)
    
*   UI: Fix case 1056226: Show realtime shadow options when using mixed and realtime lights. ([1056226](https://issuetracker.unity3d.com/issues/ui-baked-and-realtime-shadow-options-are-no-longer-displayed), 1056228)
    
*   XR: Fixed a JobTempAlloc memory leak when unloading an ARFoundation scene (1051049)
    

#### Revision: 787658998520