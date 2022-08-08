# Unity 5.3.2

https://unity3d.com/unity/whats-new/unity-5.3.2

## Improvements



*   Compute: Improved compute shader import times, particularly on Windows. Since 5.1 we were always compiling them for GL4.3+GLES3.1 too, while most people only need DX11. (706098)
*   Editor: Added link to learn more about Unity Cloud Build in the Build Player window.
*   Editor/Scenes: Add Scene.GetRootGameObjects() to return the root game objects of the scene.
*   Editor/Scenes: Add SceneManager.CreateScene() API to allow creating new empty scene at runtime.
*   GI: Light probes and ambient (everything with SH calculations) match ground truth more closely now. (754898)
*   IL2CPP: Optimize method prologues for code size and incremental builds.
*   iOS: Added bitcode support. (752178)
*   iOS/IL2CPP: Added support for Xcode 7.3 (don't use \_\_declspec attributes).
*   Samsung TV: Added support for 2016 TVs.
*   Tizen: Now supports tizenstore URL protocol to open up Tizen store pages.
*   tvOS: Enable Dynamic GI.
*   VR: Applications that lost focus no longer throttle the CPU.