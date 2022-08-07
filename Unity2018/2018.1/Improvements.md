# Unity 2018.1
https://unity3d.com/unity/whats-new/unity-2018.1.0

## Improvements

<ul>
<li><p>Android: Added ability to use the activity attribute when setting max aspect ratio since API 26.</p></li>
<li><p>Android: Added API 26 and 27 to scripting and the Editor.</p></li>
<li><p>Android: Added support for Linear Rendering without additional fullscreen blit on Android O.</p></li>
<li><p>Android: Added <code>GUIUtility.systemCopyBuffer</code> support.</p></li>
<li><p>Android: Added <code>InputTouch.radius</code> and <code>InputTouch.radiusVariance</code> properties (currently works on a limited set of devices).</p></li>
<li><p>Android: Improved shader compilation time.</p></li>
<li><p>Android: Improved <code>Ping</code> class performance on devices supporting ICMP sockets. More information added to <code>Ping</code> scripting documentation. (<a href="https://issuetracker.unity3d.com/issues/ping-causes-lag-on-android-devices">972519</a>, 1005103)</p></li>
<li><p>Android: Unity is now slightly smarter about guessing the location of the Android SDK if you didn't fill it out in the Preferences.</p></li>
<li><p>Android: Unity now imprints the product name into Unity's default Android banner, making it easier to distinguish between apps on Android devices where the banner is used for showing the app.</p></li>
<li><p>Android: Updated Gradle template to not strip symbols from *.so files, because they already are stripped where needed.</p></li>
<li><p>Android: [Gradle] Added more variables to <code>build.gradle</code>.</p></li>
<li><p>Animation: Transition exit time condition now works with negative state speed parameter. (<a href="https://issuetracker.unity3d.com/issues/animation-with-negative-speed-multiplier-parameter-ignores-animator-state-transitions">941112</a>)</p></li>
<li><p>Animation: Using Reset in the Inspector while Recording an animation creates a key for each supported modified property at the current frame. (<a href="https://issuetracker.unity3d.com/issues/animationwindow-transform-reset-is-not-recorded">766821</a>)</p></li>
<li><p>Animation: <code>AnimationUtility.SetAnimationEvents</code> now sorts <code>AnimationEvent</code>s by time. (<a href="https://issuetracker.unity3d.com/issues/animationutility-dot-setanimationevents-does-not-trigger-events-correctly-if-event-array-is-not-sorted-by-time">913430</a>)</p></li>
<li><p>Asset Import: In optimized mode, if a root bone is specified in the unoptimized SkinnedMeshRenderer and its Transform is exposed, it now stays as it is. Otherwise, Unity sets it to root. (<a href="https://issuetracker.unity3d.com/issues/skinned-mesh-renderer-bounds-offsets-when-applying-optimize-go-if-bounds-were-predefined-by-user">972082</a>, 988438)</p></li>
<li><p>Audio: Added minDistance/maxDistance information to the native Audio plug-in interface, so spatializers can implement near-field effects.</p></li>
<li><p>Audio: Fixed Audio Profiler stall of about 0.7 ms in the main loop, which was happening even for empty Scenes.</p></li>
<li><p>Build Pipeline: The build process progress bar now shows progress updates on shaders that have more than 100 variants to prevent editor from appearing unresponsive during long builds.</p></li>
<li><p>Documentation: The Scripting Reference now shows which assembly an API is implemented in.</p></li>
<li><p>Editor: Added lightmap overlap visualization for debugging.</p></li>
<li><p>Editor: Added Rename option to the the Project view's right-click menu. (773117)</p></li>
<li><p>Editor: Added the ability to duplicate any read-only sub-asset in the Project View to get a writable copy. Select any sub-asset and go to Edit &gt; Duplicate.</p></li>
<li><p>Editor: Added time ruler, dynamic grid lines, and the ability to select and zoom to specific intervals in the Profiler timeline.</p></li>
<li><p>Editor: Added <code>Application.wantsToQuit</code> and <code>Application.quitting</code> events to <code>EditorApplication</code>, enabling the user to control the Editor quit process. (802175)</p></li>
<li><p>Editor: Added <code>UnityEngine.TestTools.Utils</code> to the Playmode test framework. This namespace contains utility classes to compare 'Vector2', 'Vector3', 'Vector4', <code>Quaternion</code>, Color and <code>float</code> types using <code>NUnit</code> constraints.</p></li>
<li><p>Editor: Clarified message shown in Build Settings window when the current license does not support the platform. (957929)</p></li>
<li><p>Editor: HDR color fields in the Inspector now use gradient overlay to indicate underexposed colors where the max color component is less than 1/255.</p></li>
<li><p>Editor: HDR color fields now always appear with HDR badge in the Inspector, irrespective of their current value.</p></li>
<li><p>Editor: It is no longer possible to start multiple EditMode or PlayMode test runs at the same time from the Test Runner UI. (<a href="https://issuetracker.unity3d.com/issues/testrunner-playmode-test-leaves-behind-inittestscene-dot-dot-dot-scene-assets-after-test-runs">945000</a>)</p></li>
<li><p>Editor: Optimizations to Editor startup time.</p></li>
<li><p>Editor: Profiler now displays 3 frames of context, and supports jobs spanning more than one frame.</p></li>
<li><p>Editor: Profiler Window: Improved performance of Hierarchy View.</p></li>
<li><p>Editor: Redesigned the color picker window with exposure-based HDR controls. <img src="/sites/default/files/2018_1_feature_color-picker.png" alt="description"></p></li>
<li><p>Editor: Reduced some heap allocations incurred every frame when drawing a serialized property with a PropertyDrawer.</p></li>
<li><p>Editor: Removed a workaround for WebViews that had been added for macOS Sierra 10.12.1.   This prevents a warning message in the Editor.log file every time a WebView is added to the main window.</p></li>
<li><p>Editor: The Editor console window now displays a timestamp from when the entry was logged.</p></li>
<li><p>Editor: The Mute Audio option in the Editor / Game View now persists after Editor reload. (<a href="https://issuetracker.unity3d.com/issues/mute-audio-not-saved">785243</a>)</p></li>
<li><p>Editor: Unity now adds references and defines from <code>mcs.rsp</code> to generated .csproj for MonoDevelop, VS Code and Rider.</p></li>
<li><p>Editor: Unsupported shaders are now grouped in the shader selection dropdown in the Material inspector.</p></li>
<li><p>Editor: You can now select the text in the Profiler Window's "Details" sections. (787073)</p></li>
<li><p>Editor: <code>ExecuteMenuItem</code> can now quit the macOS EditorApplication.</p></li>
<li><p>GI: Creation of <code>LightingDataAsset</code> is now a job.</p></li>
<li><p>GI: Upgrades Enlighten SDK to version: 3.09.P1.62184</p> 
<ul>
<li>Fix for SetThreadAffinityMask crashes, backported from a newer version of Embree (CS-1196)</li>
<li>Fix in IffWriter, so that &gt; 4GB file sizes fail instead of corrupting the file. (CS-1193)</li>
<li>Fix for <code>CalcPrecomputedVisibilityWorkspaceSize()</code> returning an error (CS-1204)</li>
<li>Unity no longer emits warnings for deprecated attributes that the schema definition has assigned default values to.</li>
</ul></li>
<li><p>Graphics: - Directly render and sample into depth-cube map without additional color RT.</p> 
<ul>
<li>Enabled hardware PCF for shadow point light.</li>
<li>Added support for Vulkan.</li>
</ul></li>
<li><p>Graphics: Add option to Texture Importer to select red color channel for Single Channel Textures</p> 
<ul>
<li>Added support for R8 uncompressed format</li>
<li>Added support for EAC_R compressed textures</li>
<li>Red channel Single Channel Textures use R8, EAC_R, BC4 formats</li>
</ul></li>
<li><p>Graphics: Added new attribute <code>ToggleUI</code>, which you can use to display a checkbox in the Shader's Inspector without generating a keyword (unlike <code>Toggle</code> and <code>ToggleOff</code>). (<a href="https://issuetracker.unity3d.com/issues/maximum-number-256-of-shader-keywords-exceeded-in-srp">986865</a>)</p></li>
<li><p>Graphics: Added support for ETC textures with <code>Texture2D.PackTextures</code>, similar to DXT.</p></li>
<li><p>Graphics: Added <code>MeshRenderer.subMeshStartIndex</code> property.</p></li>
<li><p>Graphics: Change to allow you to attach async compute command buffers to Cameras and Lights.</p></li>
<li><p>Graphics: Enabled instancing flexible array size for Vulkan.</p></li>
<li><p>Graphics: Improved shader import handling when using <code>#pragma target</code>.  If you are not using <code>#pragma geometry</code>, <code>#pragma hull</code> or <code>#pragma domain</code> statements to specify entrypoint functions, Unity drops these shader features (geometry or tessellation) from the internal shader capabilities requirement, allowing greater compatibility across non-DX11 graphics targets. In practise, this now allows using <code>#pragma target 5.0</code> with Metal, as long as geometry shaders are not used.</p></li>
<li><p>Graphics: Improved <code>Mesh.CombineMeshes</code> to include only vertices of selected submeshes instead of the entire Mesh. (<a href="https://issuetracker.unity3d.com/issues/mesh-dot-combinemeshes-combines-verts-of-all-meshes-instead-of-just-the-submeshes">895464</a>)</p></li>
<li><p>Graphics: In forward rendering, Unity no longer fetches 2x2 white shadowmask textures when lighting a dynamic GameObject with a Mixed light using baked occlusion. (952761)</p></li>
<li><p>Graphics: You can now directly render and sample into depth-cube maps without additional color RT.   Hardware PCF for shadow Point light is now enabled.
  Added support for PS4, XB1, desktop GL Core, GLES3, WebGL 2.0, Metal.</p></li>
<li><p>IL2CPP: Added C++ compiler configuration setting to Player Settings. Note: this setting does not affect platforms which generate an IDE project rather than an executable, such as iOS and UWP.</p></li>
<li><p>iOS: Added a checkbox to the iOS plugin importer: when checked, the plug-in is added to the "Embedded Binaries" folder. (<a href="https://issuetracker.unity3d.com/issues/ios-dynamic-libraries-are-not-added-to-the-embedded-binaries-list">984264</a>)</p></li>
<li><p>iOS: Added a default camera usage description when using Vuforia or ARKit. (<a href="https://issuetracker.unity3d.com/issues/vuforia-ios-camera-usage-description-remains-null-after-importing-vuforias-package-and-enabling-vuforia-support">956291</a>)</p></li>
<li><p>iOS: Added change to allow you to manipulate the caret position in Input Field with touch when Hide Mobile Input is set.</p></li>
<li><p>iOS: Added ETC2 as texture format for iOS OpenGL ES3.</p></li>
<li><p>iOS: Added <code>GUIUtility.systemCopyBuffer</code> support.</p></li>
<li><p>iOS: Improved iCould capability support in Xcode API.</p></li>
<li><p>iOS: Improved shader compilation time.</p></li>
<li><p>iOS: Improved support of the plist specification in Xcode API.</p></li>
<li><p>iOS: iOS plugin importer extension updated to support new iOS 11 frameworks.</p></li>
<li><p>Kernel: Improved error messages for YAML file reading so that it also reports filenames, which aids in the resolution of merge conflicts for meta files.</p></li>
<li><p>Licenses: Improved error handling for command line activation. (<a href="https://issuetracker.unity3d.com/issues/improve-error-handling-for-command-line-activation">834325</a>)</p></li>
<li><p>Linux: Added ability to allow games to provide their own controller configuration files.</p></li>
<li><p>Linux: Improved support for unconfigured/non-gamepad joysticks.</p></li>
<li><p>Multiplayer: Two or more channels can now share the messages order, so that messages which send via differnet channels are delivered in order.</p></li>
<li><p>OSX: Added Visual Studio for Mac to macOS Installer.</p></li>
<li><p>OSX: Fixed Editor crash when using GLCore on High Sierra with Intel 6xxx series GPU. (<a href="https://issuetracker.unity3d.com/issues/unity-editor-crashes-when-creating-3d-objects-when-game-view-is-visible-and-default-skybox-is-enabled-on-13-inch-macbook-pro">956196</a>)</p></li>
<li><p>Package Manager: Allow surface shaders compilation when relative path include are used inside a package.</p></li>
<li><p>Particles: Overriden Prefab values are now indicated/highlighted in the Inspector.</p></li>
<li><p>Particles: Sub-Emitters can now be triggered when conditions are met in the Trigger Module (e.g. when particles enter a collision volume).</p></li>
<li><p>Particles: You can now trigger Sub-Emitters from script, using the new <code>TriggerSubEmitter</code> script API.</p></li>
<li><p>Profiling: Added Editor startup profiling markers.</p></li>
<li><p>Scripting: Added a scripting callback which is called just before a cube map texture completes importing (<code>AssetPostprocessor::OnPostprocessCubemap</code>).</p></li>
<li><p>Scripting: Added new <code>GetAllocatedMemoryForGraphicsDriver</code> API. (896812)</p></li>
<li><p>Scripting: Improved "The referenced script on this Behaviour is missing!" error message to tell you which script is missing, where possible.</p></li>
<li><p>Scripting: Improved performance characteristics of <code>FindObjectsOfType</code> for scenes with large GameObject count.</p></li>
<li><p>Services: Updated Unity Ads SDK to v2.1.1.  Note that this is via the update of the ads package to v2.0.7 - see 'Packages' section for details.</p></li>
<li><p>Shaders: Added a more granular way of specifying shader compilation requirements, compared to <code>#pragma target</code>.</p> 
<ul>
<li><code>#pragma require</code> XYZ for specific features that the shader requires.</li>
<li><code>SHADER_REQUIRE_XYZ</code> and <code>SHADER_AVAILABLE_XYZ</code> preprocessor defines are passed to shaders, based on which features are requested or are available.</li>
</ul></li>
<li><p>Shaders: Added Windows support for shader include absolute paths longer than 260 characters.</p></li>
<li><p>Shaders: Compute shaders are now included in the shader cache. For example, tweaking a shader and then reverting the change fetches the shader from the cache instead of recompilation.</p></li>
<li><p>Shaders: Compute shaders now support <code>#pragma exclude_renderers</code> and <code>#pragma only_renderers</code>.</p></li>
<li><p>Shaders: Global shader properties are now visible to compute shaders. A global property value is used if the property is not set locally for the compute shader.</p></li>
<li><p>Shaders: Improved shader compilation speed.</p></li>
<li><p>Shaders: Proper shader include dependency tracking implemented. Whenever a shader include file is modified all the dependent shaders - and nothing else - will get reimported. (<a href="https://issuetracker.unity3d.com/issues/shadercompiler-shaders-do-not-get-recompiled-on-changes-in-includes">646064</a>, <a href="https://issuetracker.unity3d.com/issues/changing-files-included-in-compute-shader-doesnt-compile-before-compute-shader-is-changed">916386</a>, <a href="https://issuetracker.unity3d.com/issues/changes-to-cginc-files-does-not-cause-shaders-in-different-directories-to-recompile">957024</a>)</p></li>
<li><p>Shaders: Surface Shaders with many multi_compile/shader_feature variants import several times faster now (internally, Unity now multi-threads that process).</p></li>
<li><p>Shaders: You can now use <code>SetPropertyBlock</code> per Material (in the case of the multi-material renderer), and an optional Material index.</p></li>
<li><p>Shaders: <code>ComputeShader.Dispatch</code> now validates if all the properties are valid.</p></li>
<li><p>Shaders: <code>UNITY_PASS_FORWARDBASE</code>, <code>UNITY_PASSFORWARDADD</code>, etc. are now also defined for custom vertex / fragment shaders according to the pass type.</p></li>
<li><p>Timeline: Added support for exposed references on custom TrackAssets. (<a href="https://issuetracker.unity3d.com/issues/timeline-exposedreference-class-cannot-have-references-to-scene-objects-when-used-in-playable-track-asset-class">976409</a>)</p></li>
<li><p>Timeline: Added support for left trim on recorded Animation Track clips.</p></li>
<li><p>Timeline: Improved clip visual rendering.</p></li>
<li><p>Timeline: Improved workflow when autokeying animation tracks that contain clips.</p></li>
<li><p>Timeline: Introduced new modes for editing clips in the Timeline Editor. <img src="/sites/default/files/2018.1_timeline_editmodes.png" alt="description"></p></li>
<li><p>Timeline: TrackAssets now allow multiple TrackClip types through base class specification. (950934)</p></li>
<li><p>UI: Added the ability to toggle the rounding of advance width. This allows you to get more consistent spacing between characters in a Text Mesh.</p></li>
<li><p>Universal Windows Platform: Added an option to select which configuration (debug/release/master) should be used when doing Build &amp; Run.</p></li>
<li><p>Universal Windows Platform: Improved support for building project into longer paths.</p></li>
<li><p>Video: Added basic video bitrate control in MediaEncoder API.</p></li>
<li><p>Video: Video Decoding via Job System on many platforms (reducing overall thread count and improving performance).</p></li>
<li><p>Web: Improved performance for large data download using custom download handler script.</p></li>
<li><p>Web: <code>UnityWebRequest</code> now accepts URI instances alongside string URL (URI being faster). (<a href="https://issuetracker.unity3d.com/issues/osx-webrequestutils-dot-makeinitialurl-causes-cpu-spikes">944500</a>)</p></li>
<li><p>WebGL: Added indexedDB caching support for all build files in WebGL and for compiled WebAssembly code.</p></li>
<li><p>WebGL: You can now override <code>webglContextAttributes.premultipliedAlpha</code>.</p></li>
<li><p>Windows: Added a completely new, out-of-process crash handler for both the Windows Editor and Windows Standalone Player, improving reliability of error.log and minidump generation.</p></li>
<li><p>Windows: Added support to enable/disable exclusive mode on Windows through new <code>SetResolution</code> API overload. Consolidated platform specific fullscreen modes into a single cross platform <code>FullScreenMode</code> API.</p></li>
<li><p>Windows: Multiple improvements in crash handling:</p> 
<ul>
<li>Unity applications that enable the Performance Reporting Service now receive Windows crash telemetry.</li>
<li>Crash interception is now much more reliable, catching more categories of error, sooner and later in the application life.</li>
<li>The crash UX for the player has been updated to remove the wordy English-only error message and display something generic before handing off to WER (which tells the user what happened in their native language).</li>
</ul></li>
<li><p>Windows: When installing VS2017, Unity Download Assistant will now also include C++ modules so that IL2CPP builds work out of the box. (<a href="https://issuetracker.unity3d.com/issues/installing-vs2017-through-unity-doesnt-install-c-plus-plus-tools-making-il2cpp-not-work">1003155</a>)</p></li>
<li><p>XR: Android builds that support ARCore can now be built using target API version 14 or higher.</p></li>
<li><p>XR: Improved background rendering performance in ARCore by eliminating an unnecessary OpenGL state reset.</p></li>
<li><p>XR: Metal: Implemented the remaining draw call functionality (such as <code>Graphics.DrawProcedural</code>) for Single-Pass Stereo rendering, which was missing previously.</p></li>
<li><p>XR: Updated Vuforia to version 7.1.27.</p></li>
</ul>
