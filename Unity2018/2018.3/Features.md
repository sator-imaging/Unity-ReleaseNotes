# Unity 2018.3

https://unity3d.com/unity/whats-new/unity-2018.3.0

## Features



*   Android: Added AppBundle generation support.
    
*   Android: Added notch support for Android.
    
*   Android: Added support for requesting permissions at runtime for apps using API level 23 and above.
    
*   Android: Added support for using Kotlin source files as plugins.
    
*   Android: Added the automatic installation and configuration of OpenJDK when installing Unity Android support. Configuration to use manually installed JDKs is no longer officially supported.
    
*   Animation: Added SkinnedMeshRenderer.forceMatrixRecalculationPerRender. Set this property to manually render a skinned mesh multiple times within a single update. For example, for rendering out the results of an animation to a texture.
    
*   Asset Import: Added support for importing R16 textures.
    
*   Editor: Added ability to view each channel in the Texture Inspector.
    
*   Editor: Added improvements to the window tabs:
    
    *   The selected window tab is now highlighted using a blue outline.
    *   The width of the tab is now adjusted according to the length of the tab title.
    *   You can now scroll through open tabs with arrows when the number of open tabs exceeds the width of the window.
*   Editor: Introduced new searchable window to display and edit Project Settings and Preferences.
    
*   Editor: Rider installation path detection in Editor Preferences.
    
*   Facebook: The Facebook platform now uses Package Manager for Facebook SDK management. Configure this in the Facebook Build Settings (not the Package Manager UI).
    
*   GI: Added disc-shaped area Light type for baked lighting. Only available in the Progressive Lightmapper.
    

*   GI: Added preview version of GPU Lightmapper in Windows Editor. Select this in the Lighting window. The lightmapper is based on OpenCL and RadeonRays and works on all modern GPUs with more than 2Gb of dedicated memory.
    
*   Graphics: Added memory-less frame buffer depth to iOS Metal.
    
*   Graphics: Added shadow bias options to Particles, Lines, and Trails.
    
*   Graphics: Added support for render targets and the R16 texture format.
    
*   Graphics: Added texture 3D CopyTexture support.
    
*   Graphics: Added VFX editor run-time API.
    
*   IL2CPP: Added support for managed code debugging with IL2CPP on Xbox One.
    
*   Mobile: Added Dynamic Resolution Scaling support for Vulkan on Android and Metal on iOS.
    
*   Multiplayer: Added support for providing a custom network transport implementation to be used by Unity Multiplayer's high-level API. See documentation on `UnityEngine.Networking.NetworkManager.activeTransport` for details.
    
*   Package Manager: Added support for packages in the Project browser.
    
*   Particles: Added option to disable roll on billboard particles, which is particularly useful for VR applications.