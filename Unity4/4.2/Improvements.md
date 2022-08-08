# Unity 4.2

https://unity3d.com/unity/whats-new/unity-4.2

## Improvements



*   Android: Stylus support.
*   Android: Support for xxhdpi resolution icons.
*   Android: AndroidJNIHelper and AndroidJava classes will now throw exceptions on failed invocations.
*   Android: Enhanced performance of AndroidJava and reduced the load on the dalvik GC.
*   Android: If possible, use native sensors (accelerometer, compass, etc) instead of routing it through Java.
*   Android: Improved error messages when build fails; added Retry option when device deployment fails; automatically create adb tunnel for profiler.
*   Android: OBB is now exported in the root folder when exporting an android project.
*   Android: Remove Eclipse project support in favor of Android project support.
*   Asset Bundles: Compressed AssetBundles built with 4.2 or later will have reduced runtime memory usage when decompressing.
*   Audio: Added a more informative error message when the audio device is changed during work in the editor or at runtime (i.e. when plugging in a screen that has built-in audio device such as HDMI screens).
*   Building: Show a warning when assembly's internal and file names don't match. This can cause issues on platforms that do AOT.
*   Editor: Added EditorGUIUtility.ShowObjectPicker to let editor extensions use it on demand.
*   Editor: Added a Select Prefab item in the Hierarchy View context menu.
*   Editor: Added EditorWindow.maximized bool. Use this to query if a window is maximized, set it to maximize/unmaximize a window. Is always false if the window is not docked.
*   Editor: Gradient API now has alphaKeys and colorKeys properties.
*   Editor: New #SCRIPTNAME\_LOWER# token for use in script templates.
*   Editor: Popups, buttons, color pickers, etc. in the inspector can now be opened by pressing Space.
*   Editor: Show warning in inspector when you have non-power-of-two texture that cannot be compressed.
*   Editor: Switching between DX9 and DX11 in player settings does not require editor restart now.
*   Editor: Trying to open a project that is already open in another Unity instance will now simply display an error and then bring up the project selector (except in batch mode where it keeps triggering a fatal error and exits).
*   Graphics: Optimized sorting of renderable objects for smaller CPU load.
*   Graphics: Exposed Light.alreadyLightmapped to scripts.
*   Graphics: reduced memory footprint of non-readable meshes.
*   Graphics: Added WebCamTexture.videoVerticallyMirrored. Use Case: on iOS, when you use non-readable webcam texture, GL texture will be created on top of camera's target pixel buffer, which is vertically "flipped".
*   iOS: Ability to disable "Replace" button when overwriting existing build.
*   iOS: Added Objective-C VideoPlayer, to playback video to view or to a texture.
*   iOS: Enforced keyboard to be shown on main thread (to play nicely with iOS6).
*   iOS: Improved support for AppController subclassing and unity view integration with native UI.
*   iOS: In case of unhandled exceptions iOS player now will generate crash report instead of exiting silently.
*   iOS: Made Unity iOS apps PIE compatible.
*   iOS: Added iPhone.vendorIdentifier and iPhone.advertisingIdentifier with iPhone.advertisingTrackingEnabled APIs for better manual control of what device ID to use.
*   iOS: Xcode project cleaned up a bit.
*   iOS: Native VideoPlayback can be now paused/resumed. You can seek and check if it is playing.
*   iOS: Added UNITY\_VERSION macro support for native code in trampoline. We also added a UNITY\_4\_2\_0 macro to make it future-proof (we will add macros like that for future releases too). We now support these ways of checking the version:
    *   you can use it like MSC\_VER macro, i.e. if you want some code to be enabled only when using unity 4.4.1 or newer, do #if UNITY\_VERSION >= 441.
    *   you can do it in a way that resembles iOS SDK versioning, e.g. for version 4.4.1 and newer #ifdef UNITY\_4\_4\_1.
    *   you can combine them, e.g. #if defined(UNITY\_4\_4\_1) && UNITY\_VERSION < UNITY\_4\_4\_1
*   Linux: Improved inter-application copy/paste.
*   Linux: Add fullscreen scaling fallback for devices that don't support GL\_EXT\_framebuffer\_blit.
*   Mecanim: Allow scrolling when adding transition.
*   Mecanim: Return warning message in console to user when we detect an invalid avatar while importing.
*   Mobile: Optimized a bunch of rendering places to be more tiled-GPU friendly (as is common on mobile). This includes shadows, deferred lighting and most of image effects.
*   Mobile: Added RenderTexture.DiscardContents with separate flags for color/depth discard.
*   Mobile: Greatly improved performance of fixed function shaders on OpenGL ES 2.0. There's no reason to use ES 1.1 anymore.
*   Mobile: Switched to one FBO object per RenderTexture; performance improvement with render texture switches.
*   NavMesh: General crowd performance improvements.
*   Profiler: Now roughly estimates how much application binary and loaded libraries take.
*   Profiler: Open webstreams (for Asset Bundles etc.) report their used sizes.
*   Profiler: Removed log spamming when manually connecting to IP.
*   Scripting: Avoid pausing some threads during Mono garbage collection on Windows, OS X, and iOS. Helps prevent audio stutters during GC.
*   Scripting: Added HideFlags.None enum value.
*   Scripting: While compiling C# scripts, you can now use classes from System.Xml.Linq namespace.
*   Shaders: Ability to output custom Z buffer value from shaders. Previously, a bug in Cg compiler prevented this on D3D9, we've worked around that. Note that some platforms (OpenGL ES 2.0, Flash) don't have ability to write custom values into Z buffer from pixel shaders.
*   Shaders: Add ability to override how lightmaps are applied in surface shaders.
*   Shadows: Better sorting of shadow casters for GPU efficiency.
*   Shadows: Improved shadowmap filtering on OpenGL. It will use native GPU bilinear shadow filter when available, just like D3D9 and D3D11 does. No more "shadows are worse on Mac than on Windows"! Note: native shadowmap filtering disabled for Spot lights on Linux due to driver issues.
*   Shuriken: Added script binding for ParticleSystem simulation space.
*   Shuriken: Exposed particle axis of rotation to scripting API.
*   Standalone: Added "fullscreen at native resolution" player setting.
*   Standalone: Added player setting for single instance mode.
*   Substance: Cloned ProceduralMaterials now inherit the original substance's animation rate.
*   Substance: It is now possible to reliably assign ProceduralTextures from a SBSAR to the shader associated to a ProceduralMaterial from another SBSAR.
*   Substance: ProceduralMaterial.ClearCache now takes effect immediately instead of being taken into account at next RebuildTextures call.
*   Substance: ProceduralTextures created from a cloned ProceduralMaterial now have the same name and "RAW/Compressed" format as the original textures.
*   Substance: Reimporting substances that have been modified in Play mode is now multithreaded.
*   Substance: Editor scripts can now modify a ProceduralMaterial's size/format/behaviour using SubstanceImporter.Get/SetPlatformTextureSettings.
*   Web Player: the "Release Channels" context menu now lists actual versions used for different channels.