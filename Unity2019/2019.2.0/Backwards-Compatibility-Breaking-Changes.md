# Unity 2019.2.0

https://unity3d.com/unity/whats-new/2019.2.0

## Backwards Compatibility Breaking Changes



*   2D: Updated the 2D Project Template manifest.json to include 'com.unity.2d.sprite' and 'com.unity.2d.tilemap' as core packages.
    
*   Android: Android Gradle plugin version updated up to 3.4.
    
*   Android: Deprecated x86 support.
    
*   Android: Increased the minimum Vulkan API version for Adreno drivers to 1.0.38.
    
*   Animation: Changed the evaluation order to evaluate constraints before the LateUpdate script. ([1123107](https://issuetracker.unity3d.com/issues/sampling-the-position-of-the-gameobject-with-update-function-does-not-yield-the-correct-position))
    
*   Asset Import: Added a warning when multiple sub-Assets are imported with the same name or type. This often happens when importing Models with multiple Meshes or Materials that have the same name in the .fbx file. Their resulting file ID (and thus references to them) may break or change if Unity re-imports them and finds a new sub-Asset with the same name before finding the existing one.
    
*   Asset Import: Starting with the Unity 2019.3 release, you need an external plugin to import Cinema4D files directly in Unity. The External Tools forum provides updates: https://on.unity.com/c4d.
    
*   Editor: Changed default shortcut for **Stage**/**Go Back** from **O** to **H** to avoid shortcut conflicts in Project templates.
    
*   Editor: Removed most of the legacy Module Manager. Only extension modules located inside the Unity install are loaded now. Also completely removed the **Modules...** menu item and window.
    
*   Editor: UGui Objects use ObjectFactory and default Presets when created from the GameObject menu in the Editor.
    
*   Facebook: Added deprecation warning for Facebook Gameroom platform.
    
*   Graphics: Added Rendering Layer Mask to Lights as a filtering option during shadow passes in Scriptable Render Pipelines. This is similar to Renderers Rendering Layer Masks.
    
*   Graphics: Added support for graphics API switching when restarting Unity.
    
*   Graphics: Asynchronous Shader compilation: Blit now never uses cyan dummy Shader.
    
*   Graphics: Asynchronous Shader compilation: DrawProcedural now skips rendering during compilation instead of trying to use the dummy Shader.
    
*   Graphics: Moved the Async Shader Compilation option from Preferences to Project Settings.
    
*   Prefabs: Prefabs created by dragging into the hierarchy are now parents to the correct parent, instead of being a root object. The correct parent will thus be set in `Awake` calls.
    
*   Scripting: Made the recommended Visual Studio installer upgrade version 2019
    
*   Scripting: Made the `GarbageCollector.GCMode` property only throw an exception on unsupported platforms when trying to change it's value, not when reading it.
    
*   Timeline: Clip properties can no longer be animated by recording. Clip properties are animated with the Curves view.
    
*   Timeline: Updated Timeline package version to 1.1.0.
    
*   XR: Moved Vuforia support to a package.
    
*   XR: Oculus (Standalone) and OpenVR (Standalone) package names have been changed to use (Desktop) instead of (Standalone).