# Unity 4.2
https://unity3d.com/unity/whats-new/unity-4.2

## Improvements

<ul>
<li>Android: Stylus support.</li>
<li>Android: Support for xxhdpi resolution icons.</li>
<li>Android: AndroidJNIHelper and AndroidJava classes will now throw exceptions on failed invocations.</li>
<li>Android: Enhanced performance of AndroidJava and reduced the load on the dalvik GC.</li>
<li>Android: If possible, use native sensors (accelerometer, compass, etc) instead of routing it through Java.</li>
<li>Android: Improved error messages when build fails; added Retry option when device deployment fails; automatically create adb tunnel for profiler.</li>
<li>Android: OBB is now exported in the root folder when exporting an android project.</li>
<li>Android: Remove Eclipse project support in favor of Android project support.</li>
<li>Asset Bundles: Compressed AssetBundles built with 4.2 or later will have reduced runtime memory usage when decompressing.</li>
<li>Audio: Added a more informative error message when the audio device is changed during work in the editor or at runtime (i.e. when plugging in a screen that has built-in audio device such as HDMI screens).</li>
<li>Building: Show a warning when assembly's internal and file names don't match. This can cause issues on platforms that do AOT.</li>
<li>Editor: Added EditorGUIUtility.ShowObjectPicker to let editor extensions use it on demand.</li>
<li>Editor: Added a Select Prefab item in the Hierarchy View context menu.</li>
<li>Editor: Added EditorWindow.maximized bool. Use this to query if a window is maximized, set it to maximize/unmaximize a window. Is always false if the window is not docked.</li>
<li>Editor: Gradient API now has alphaKeys and colorKeys properties.</li>
<li>Editor: New #SCRIPTNAME_LOWER# token for use in script templates.</li>
<li>Editor: Popups, buttons, color pickers, etc. in the inspector can now be opened by pressing Space.</li>
<li>Editor: Show warning in inspector when you have non-power-of-two texture that cannot be compressed.</li>
<li>Editor: Switching between DX9 and DX11 in player settings does not require editor restart now.</li>
<li>Editor: Trying to open a project that is already open in another Unity instance will now simply display an error and then bring up the project selector (except in batch mode where it keeps triggering a fatal error and exits).</li>
<li>Graphics: Optimized sorting of renderable objects for smaller CPU load.</li>
<li>Graphics: Exposed Light.alreadyLightmapped to scripts.</li>
<li>Graphics: reduced memory footprint of non-readable meshes.</li>
<li>Graphics: Added WebCamTexture.videoVerticallyMirrored. Use Case: on iOS, when you use non-readable webcam texture, GL texture will be created on top of camera's target pixel buffer, which is vertically "flipped".</li>
<li>iOS: Ability to disable "Replace" button when overwriting existing build.</li>
<li>iOS: Added Objective-C VideoPlayer, to playback video to view or to a texture.</li>
<li>iOS: Enforced keyboard to be shown on main thread (to play nicely with iOS6).</li>
<li>iOS: Improved support for AppController subclassing and unity view integration with native UI.</li>
<li>iOS: In case of unhandled exceptions iOS player now will generate crash report instead of exiting silently.</li>
<li>iOS: Made Unity iOS apps PIE compatible.</li>
<li>iOS: Added iPhone.vendorIdentifier and iPhone.advertisingIdentifier with iPhone.advertisingTrackingEnabled APIs for better manual control of what device ID to use.</li>
<li>iOS: Xcode project cleaned up a bit.</li>
<li>iOS: Native VideoPlayback can be now paused/resumed. You can seek and check if it is playing.</li>
<li>iOS: Added UNITY_VERSION macro support for native code in trampoline. We also added a UNITY_4_2_0 macro to make it future-proof (we will add macros like that for future releases too). We now support these ways of checking the version: 
<ul>
<li>you can use it like MSC_VER macro, i.e. if you want some code to be enabled only when using unity 4.4.1 or newer, do #if UNITY_VERSION &gt;= 441.</li>
<li>you can do it in a way that resembles iOS SDK versioning, e.g. for version 4.4.1 and newer #ifdef UNITY_4_4_1.</li>
<li>you can combine them, e.g. #if defined(UNITY_4_4_1) &amp;&amp; UNITY_VERSION &lt; UNITY_4_4_1</li>
</ul></li>
<li>Linux: Improved inter-application copy/paste.</li>
<li>Linux: Add fullscreen scaling fallback for devices that don't support GL_EXT_framebuffer_blit.</li>
<li>Mecanim: Allow scrolling when adding transition.</li>
<li>Mecanim: Return warning message in console to user when we detect an invalid avatar while importing.</li>
<li>Mobile: Optimized a bunch of rendering places to be more tiled-GPU friendly (as is common on mobile). This includes shadows, deferred lighting and most of image effects.</li>
<li>Mobile: Added RenderTexture.DiscardContents with separate flags for color/depth discard.</li>
<li>Mobile: Greatly improved performance of fixed function shaders on OpenGL ES 2.0. There's no reason to use ES 1.1 anymore.</li>
<li>Mobile: Switched to one FBO object per RenderTexture; performance improvement with render texture switches.</li>
<li>NavMesh: General crowd performance improvements.</li>
<li>Profiler: Now roughly estimates how much application binary and loaded libraries take.</li>
<li>Profiler: Open webstreams (for Asset Bundles etc.) report their used sizes.</li>
<li>Profiler: Removed log spamming when manually connecting to IP.</li>
<li>Scripting: Avoid pausing some threads during Mono garbage collection on Windows, OS X, and iOS. Helps prevent audio stutters during GC.</li>
<li>Scripting: Added HideFlags.None enum value.</li>
<li>Scripting: While compiling C# scripts, you can now use classes from System.Xml.Linq namespace.</li>
<li>Shaders: Ability to output custom Z buffer value from shaders. Previously, a bug in Cg compiler prevented this on D3D9, we've worked around that. Note that some platforms (OpenGL ES 2.0, Flash) don't have ability to write custom values into Z buffer from pixel shaders.</li>
<li>Shaders: Add ability to override how lightmaps are applied in surface shaders.</li>
<li>Shadows: Better sorting of shadow casters for GPU efficiency.</li>
<li>Shadows: Improved shadowmap filtering on OpenGL. It will use native GPU bilinear shadow filter when available, just like D3D9 and D3D11 does. No more "shadows are worse on Mac than on Windows"! Note: native shadowmap filtering disabled for Spot lights on Linux due to driver issues.</li>
<li>Shuriken: Added script binding for ParticleSystem simulation space.</li>
<li>Shuriken: Exposed particle axis of rotation to scripting API.</li>
<li>Standalone: Added "fullscreen at native resolution" player setting.</li>
<li>Standalone: Added player setting for single instance mode.</li>
<li>Substance: Cloned ProceduralMaterials now inherit the original substance's animation rate.</li>
<li>Substance: It is now possible to reliably assign ProceduralTextures from a SBSAR to the shader associated to a ProceduralMaterial from another SBSAR.</li>
<li>Substance: ProceduralMaterial.ClearCache now takes effect immediately instead of being taken into account at next RebuildTextures call.</li>
<li>Substance: ProceduralTextures created from a cloned ProceduralMaterial now have the same name and "RAW/Compressed" format as the original textures.</li>
<li>Substance: Reimporting substances that have been modified in Play mode is now multithreaded.</li>
<li>Substance: Editor scripts can now modify a ProceduralMaterial's size/format/behaviour using SubstanceImporter.Get/SetPlatformTextureSettings.</li>
<li>Web Player: the "Release Channels" context menu now lists actual versions used for different channels.</li>
</ul>
