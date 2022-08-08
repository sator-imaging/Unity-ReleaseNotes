# Unity 2018.1

https://unity3d.com/unity/whats-new/unity-2018.1.0

## Improvements



*   Android: Added ability to use the activity attribute when setting max aspect ratio since API 26.
    
*   Android: Added API 26 and 27 to scripting and the Editor.
    
*   Android: Added support for Linear Rendering without additional fullscreen blit on Android O.
    
*   Android: Added `GUIUtility.systemCopyBuffer` support.
    
*   Android: Added `InputTouch.radius` and `InputTouch.radiusVariance` properties (currently works on a limited set of devices).
    
*   Android: Improved shader compilation time.
    
*   Android: Improved `Ping` class performance on devices supporting ICMP sockets. More information added to `Ping` scripting documentation. ([972519](https://issuetracker.unity3d.com/issues/ping-causes-lag-on-android-devices), 1005103)
    
*   Android: Unity is now slightly smarter about guessing the location of the Android SDK if you didn't fill it out in the Preferences.
    
*   Android: Unity now imprints the product name into Unity's default Android banner, making it easier to distinguish between apps on Android devices where the banner is used for showing the app.
    
*   Android: Updated Gradle template to not strip symbols from \*.so files, because they already are stripped where needed.
    
*   Android: \[Gradle\] Added more variables to `build.gradle`.
    
*   Animation: Transition exit time condition now works with negative state speed parameter. ([941112](https://issuetracker.unity3d.com/issues/animation-with-negative-speed-multiplier-parameter-ignores-animator-state-transitions))
    
*   Animation: Using Reset in the Inspector while Recording an animation creates a key for each supported modified property at the current frame. ([766821](https://issuetracker.unity3d.com/issues/animationwindow-transform-reset-is-not-recorded))
    
*   Animation: `AnimationUtility.SetAnimationEvents` now sorts `AnimationEvent`s by time. ([913430](https://issuetracker.unity3d.com/issues/animationutility-dot-setanimationevents-does-not-trigger-events-correctly-if-event-array-is-not-sorted-by-time))
    
*   Asset Import: In optimized mode, if a root bone is specified in the unoptimized SkinnedMeshRenderer and its Transform is exposed, it now stays as it is. Otherwise, Unity sets it to root. ([972082](https://issuetracker.unity3d.com/issues/skinned-mesh-renderer-bounds-offsets-when-applying-optimize-go-if-bounds-were-predefined-by-user), 988438)
    
*   Audio: Added minDistance/maxDistance information to the native Audio plug-in interface, so spatializers can implement near-field effects.
    
*   Audio: Fixed Audio Profiler stall of about 0.7 ms in the main loop, which was happening even for empty Scenes.
    
*   Build Pipeline: The build process progress bar now shows progress updates on shaders that have more than 100 variants to prevent editor from appearing unresponsive during long builds.
    
*   Documentation: The Scripting Reference now shows which assembly an API is implemented in.
    
*   Editor: Added lightmap overlap visualization for debugging.
    
*   Editor: Added Rename option to the the Project view's right-click menu. (773117)
    
*   Editor: Added the ability to duplicate any read-only sub-asset in the Project View to get a writable copy. Select any sub-asset and go to Edit > Duplicate.
    
*   Editor: Added time ruler, dynamic grid lines, and the ability to select and zoom to specific intervals in the Profiler timeline.
    
*   Editor: Added `Application.wantsToQuit` and `Application.quitting` events to `EditorApplication`, enabling the user to control the Editor quit process. (802175)
    
*   Editor: Added `UnityEngine.TestTools.Utils` to the Playmode test framework. This namespace contains utility classes to compare 'Vector2', 'Vector3', 'Vector4', `Quaternion`, Color and `float` types using `NUnit` constraints.
    
*   Editor: Clarified message shown in Build Settings window when the current license does not support the platform. (957929)
    
*   Editor: HDR color fields in the Inspector now use gradient overlay to indicate underexposed colors where the max color component is less than 1/255.
    
*   Editor: HDR color fields now always appear with HDR badge in the Inspector, irrespective of their current value.
    
*   Editor: It is no longer possible to start multiple EditMode or PlayMode test runs at the same time from the Test Runner UI. ([945000](https://issuetracker.unity3d.com/issues/testrunner-playmode-test-leaves-behind-inittestscene-dot-dot-dot-scene-assets-after-test-runs))
    
*   Editor: Optimizations to Editor startup time.
    
*   Editor: Profiler now displays 3 frames of context, and supports jobs spanning more than one frame.
    
*   Editor: Profiler Window: Improved performance of Hierarchy View.
    
*   Editor: Redesigned the color picker window with exposure-based HDR controls. ![description](/sites/default/files/2018_1_feature_color-picker.png)
    
*   Editor: Reduced some heap allocations incurred every frame when drawing a serialized property with a PropertyDrawer.
    
*   Editor: Removed a workaround for WebViews that had been added for macOS Sierra 10.12.1. This prevents a warning message in the Editor.log file every time a WebView is added to the main window.
    
*   Editor: The Editor console window now displays a timestamp from when the entry was logged.
    
*   Editor: The Mute Audio option in the Editor / Game View now persists after Editor reload. ([785243](https://issuetracker.unity3d.com/issues/mute-audio-not-saved))
    
*   Editor: Unity now adds references and defines from `mcs.rsp` to generated .csproj for MonoDevelop, VS Code and Rider.
    
*   Editor: Unsupported shaders are now grouped in the shader selection dropdown in the Material inspector.
    
*   Editor: You can now select the text in the Profiler Window's "Details" sections. (787073)
    
*   Editor: `ExecuteMenuItem` can now quit the macOS EditorApplication.
    
*   GI: Creation of `LightingDataAsset` is now a job.
    
*   GI: Upgrades Enlighten SDK to version: 3.09.P1.62184
    
    *   Fix for SetThreadAffinityMask crashes, backported from a newer version of Embree (CS-1196)
    *   Fix in IffWriter, so that > 4GB file sizes fail instead of corrupting the file. (CS-1193)
    *   Fix for `CalcPrecomputedVisibilityWorkspaceSize()` returning an error (CS-1204)
    *   Unity no longer emits warnings for deprecated attributes that the schema definition has assigned default values to.
*   Graphics: - Directly render and sample into depth-cube map without additional color RT.
    
    *   Enabled hardware PCF for shadow point light.
    *   Added support for Vulkan.
*   Graphics: Add option to Texture Importer to select red color channel for Single Channel Textures
    
    *   Added support for R8 uncompressed format
    *   Added support for EAC\_R compressed textures
    *   Red channel Single Channel Textures use R8, EAC\_R, BC4 formats
*   Graphics: Added new attribute `ToggleUI`, which you can use to display a checkbox in the Shader's Inspector without generating a keyword (unlike `Toggle` and `ToggleOff`). ([986865](https://issuetracker.unity3d.com/issues/maximum-number-256-of-shader-keywords-exceeded-in-srp))
    
*   Graphics: Added support for ETC textures with `Texture2D.PackTextures`, similar to DXT.
    
*   Graphics: Added `MeshRenderer.subMeshStartIndex` property.
    
*   Graphics: Change to allow you to attach async compute command buffers to Cameras and Lights.
    
*   Graphics: Enabled instancing flexible array size for Vulkan.
    
*   Graphics: Improved shader import handling when using `#pragma target`. If you are not using `#pragma geometry`, `#pragma hull` or `#pragma domain` statements to specify entrypoint functions, Unity drops these shader features (geometry or tessellation) from the internal shader capabilities requirement, allowing greater compatibility across non-DX11 graphics targets. In practise, this now allows using `#pragma target 5.0` with Metal, as long as geometry shaders are not used.
    
*   Graphics: Improved `Mesh.CombineMeshes` to include only vertices of selected submeshes instead of the entire Mesh. ([895464](https://issuetracker.unity3d.com/issues/mesh-dot-combinemeshes-combines-verts-of-all-meshes-instead-of-just-the-submeshes))
    
*   Graphics: In forward rendering, Unity no longer fetches 2x2 white shadowmask textures when lighting a dynamic GameObject with a Mixed light using baked occlusion. (952761)
    
*   Graphics: You can now directly render and sample into depth-cube maps without additional color RT. Hardware PCF for shadow Point light is now enabled. Added support for PS4, XB1, desktop GL Core, GLES3, WebGL 2.0, Metal.
    
*   IL2CPP: Added C++ compiler configuration setting to Player Settings. Note: this setting does not affect platforms which generate an IDE project rather than an executable, such as iOS and UWP.
    
*   iOS: Added a checkbox to the iOS plugin importer: when checked, the plug-in is added to the "Embedded Binaries" folder. ([984264](https://issuetracker.unity3d.com/issues/ios-dynamic-libraries-are-not-added-to-the-embedded-binaries-list))
    
*   iOS: Added a default camera usage description when using Vuforia or ARKit. ([956291](https://issuetracker.unity3d.com/issues/vuforia-ios-camera-usage-description-remains-null-after-importing-vuforias-package-and-enabling-vuforia-support))
    
*   iOS: Added change to allow you to manipulate the caret position in Input Field with touch when Hide Mobile Input is set.
    
*   iOS: Added ETC2 as texture format for iOS OpenGL ES3.
    
*   iOS: Added `GUIUtility.systemCopyBuffer` support.
    
*   iOS: Improved iCould capability support in Xcode API.
    
*   iOS: Improved shader compilation time.
    
*   iOS: Improved support of the plist specification in Xcode API.
    
*   iOS: iOS plugin importer extension updated to support new iOS 11 frameworks.
    
*   Kernel: Improved error messages for YAML file reading so that it also reports filenames, which aids in the resolution of merge conflicts for meta files.
    
*   Licenses: Improved error handling for command line activation. ([834325](https://issuetracker.unity3d.com/issues/improve-error-handling-for-command-line-activation))
    
*   Linux: Added ability to allow games to provide their own controller configuration files.
    
*   Linux: Improved support for unconfigured/non-gamepad joysticks.
    
*   Multiplayer: Two or more channels can now share the messages order, so that messages which send via differnet channels are delivered in order.
    
*   OSX: Added Visual Studio for Mac to macOS Installer.
    
*   OSX: Fixed Editor crash when using GLCore on High Sierra with Intel 6xxx series GPU. ([956196](https://issuetracker.unity3d.com/issues/unity-editor-crashes-when-creating-3d-objects-when-game-view-is-visible-and-default-skybox-is-enabled-on-13-inch-macbook-pro))
    
*   Package Manager: Allow surface shaders compilation when relative path include are used inside a package.
    
*   Particles: Overriden Prefab values are now indicated/highlighted in the Inspector.
    
*   Particles: Sub-Emitters can now be triggered when conditions are met in the Trigger Module (e.g. when particles enter a collision volume).
    
*   Particles: You can now trigger Sub-Emitters from script, using the new `TriggerSubEmitter` script API.
    
*   Profiling: Added Editor startup profiling markers.
    
*   Scripting: Added a scripting callback which is called just before a cube map texture completes importing (`AssetPostprocessor::OnPostprocessCubemap`).
    
*   Scripting: Added new `GetAllocatedMemoryForGraphicsDriver` API. (896812)
    
*   Scripting: Improved "The referenced script on this Behaviour is missing!" error message to tell you which script is missing, where possible.
    
*   Scripting: Improved performance characteristics of `FindObjectsOfType` for scenes with large GameObject count.
    
*   Services: Updated Unity Ads SDK to v2.1.1. Note that this is via the update of the ads package to v2.0.7 - see 'Packages' section for details.
    
*   Shaders: Added a more granular way of specifying shader compilation requirements, compared to `#pragma target`.
    
    *   `#pragma require` XYZ for specific features that the shader requires.
    *   `SHADER_REQUIRE_XYZ` and `SHADER_AVAILABLE_XYZ` preprocessor defines are passed to shaders, based on which features are requested or are available.
*   Shaders: Added Windows support for shader include absolute paths longer than 260 characters.
    
*   Shaders: Compute shaders are now included in the shader cache. For example, tweaking a shader and then reverting the change fetches the shader from the cache instead of recompilation.
    
*   Shaders: Compute shaders now support `#pragma exclude_renderers` and `#pragma only_renderers`.
    
*   Shaders: Global shader properties are now visible to compute shaders. A global property value is used if the property is not set locally for the compute shader.
    
*   Shaders: Improved shader compilation speed.
    
*   Shaders: Proper shader include dependency tracking implemented. Whenever a shader include file is modified all the dependent shaders - and nothing else - will get reimported. ([646064](https://issuetracker.unity3d.com/issues/shadercompiler-shaders-do-not-get-recompiled-on-changes-in-includes), [916386](https://issuetracker.unity3d.com/issues/changing-files-included-in-compute-shader-doesnt-compile-before-compute-shader-is-changed), [957024](https://issuetracker.unity3d.com/issues/changes-to-cginc-files-does-not-cause-shaders-in-different-directories-to-recompile))
    
*   Shaders: Surface Shaders with many multi\_compile/shader\_feature variants import several times faster now (internally, Unity now multi-threads that process).
    
*   Shaders: You can now use `SetPropertyBlock` per Material (in the case of the multi-material renderer), and an optional Material index.
    
*   Shaders: `ComputeShader.Dispatch` now validates if all the properties are valid.
    
*   Shaders: `UNITY_PASS_FORWARDBASE`, `UNITY_PASSFORWARDADD`, etc. are now also defined for custom vertex / fragment shaders according to the pass type.
    
*   Timeline: Added support for exposed references on custom TrackAssets. ([976409](https://issuetracker.unity3d.com/issues/timeline-exposedreference-class-cannot-have-references-to-scene-objects-when-used-in-playable-track-asset-class))
    
*   Timeline: Added support for left trim on recorded Animation Track clips.
    
*   Timeline: Improved clip visual rendering.
    
*   Timeline: Improved workflow when autokeying animation tracks that contain clips.
    
*   Timeline: Introduced new modes for editing clips in the Timeline Editor. ![description](/sites/default/files/2018.1_timeline_editmodes.png)
    
*   Timeline: TrackAssets now allow multiple TrackClip types through base class specification. (950934)
    
*   UI: Added the ability to toggle the rounding of advance width. This allows you to get more consistent spacing between characters in a Text Mesh.
    
*   Universal Windows Platform: Added an option to select which configuration (debug/release/master) should be used when doing Build & Run.
    
*   Universal Windows Platform: Improved support for building project into longer paths.
    
*   Video: Added basic video bitrate control in MediaEncoder API.
    
*   Video: Video Decoding via Job System on many platforms (reducing overall thread count and improving performance).
    
*   Web: Improved performance for large data download using custom download handler script.
    
*   Web: `UnityWebRequest` now accepts URI instances alongside string URL (URI being faster). ([944500](https://issuetracker.unity3d.com/issues/osx-webrequestutils-dot-makeinitialurl-causes-cpu-spikes))
    
*   WebGL: Added indexedDB caching support for all build files in WebGL and for compiled WebAssembly code.
    
*   WebGL: You can now override `webglContextAttributes.premultipliedAlpha`.
    
*   Windows: Added a completely new, out-of-process crash handler for both the Windows Editor and Windows Standalone Player, improving reliability of error.log and minidump generation.
    
*   Windows: Added support to enable/disable exclusive mode on Windows through new `SetResolution` API overload. Consolidated platform specific fullscreen modes into a single cross platform `FullScreenMode` API.
    
*   Windows: Multiple improvements in crash handling:
    
    *   Unity applications that enable the Performance Reporting Service now receive Windows crash telemetry.
    *   Crash interception is now much more reliable, catching more categories of error, sooner and later in the application life.
    *   The crash UX for the player has been updated to remove the wordy English-only error message and display something generic before handing off to WER (which tells the user what happened in their native language).
*   Windows: When installing VS2017, Unity Download Assistant will now also include C++ modules so that IL2CPP builds work out of the box. ([1003155](https://issuetracker.unity3d.com/issues/installing-vs2017-through-unity-doesnt-install-c-plus-plus-tools-making-il2cpp-not-work))
    
*   XR: Android builds that support ARCore can now be built using target API version 14 or higher.
    
*   XR: Improved background rendering performance in ARCore by eliminating an unnecessary OpenGL state reset.
    
*   XR: Metal: Implemented the remaining draw call functionality (such as `Graphics.DrawProcedural`) for Single-Pass Stereo rendering, which was missing previously.
    
*   XR: Updated Vuforia to version 7.1.27.