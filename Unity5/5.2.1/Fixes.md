# Unity 5.2.1
https://unity3d.com/unity/whats-new/unity-5.2.1

## Fixes

<ul>
<li>(711225) -  2D : Fixed memory leak when using Sprite object field in custom inspector.</li>
<li>(572545) -  2D: Clamp sprite pivot values (-100k to 100k) now instead of accepting any value (including infinity).</li>
<li>(722701) -  Analytics: Fixed data dispatcher to send data after airplane mode is turned OFF on iOS.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/adreno-opengles2-shader-calibration-scene-does-not-work-with-opengles2-on-adreno-devices">716159</a>) -  Android - Fixed fallback to Gamma color space rendering for projects that are configured to use linear rendering.</li>
<li>(710244) -  Android - Fixed status bar not shown and touch offset on Kitkat+ when using native activity.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/android-unexpected-permissions-added-into-unity-androidmanifest">705138</a>) -  Android: Fixed INTERNET permission on Android even if there are no network calls in the scripts.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/android-auto-rotation-switches-accelorometer-input">678003</a>) -  Android: Fixed sensor compensation issue affecting devices when rotated180 degrees.</li>
<li>(none) -  Android: Removed some egl errors from the log when probing for GLES API level.</li>
<li>(717028) -  Android:&nbsp;Fixed performance regression when using native rendering plugins.</li>
<li>(708088) -  Animation: Fixed an issue whereby animation window was still recording when scene was saved.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/system-dot-reflection-dot-targetinvocationexception-importing-plugin">718709</a>) -  API Updater: Fixed crash in AssemblyUpdater when a type had methods with names starting with get_/set_ .</li>
<li>(679703) -  Asset Loading: Now allow extension dlls to be imported outside of project folder.</li>
<li>(719416) -  AssetBundle: Fixed the issue that sometimes several AssetBundles would have same internal name.</li>
<li>(722104) -  Bug Reporter: Fixed email field not being saved on Windows 10.</li>
<li>(none) -  D3D12: Fixed a crash when using compute buffers.</li>
<li>(none) -  D3D: Fixed broken positioning of render when upscaling to native desktop resolution.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/full-screen-input-dot-mouseposition-output-does-not-match-the-displayed-view-on-the-screen">715666</a>) -  D3D: Mouse coordinates no longer go out of bounds when upscaling to desktop resolution.</li>
<li>(713782) -  Deployment Management: Fixed OSX non development players crash on startup.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/deployment-management-editor-log-doesnt-show-assets-in-resource-folders-when-building">712887</a>) -  Deployment Management: Include assets inside Resources folder in the build size report.</li>
<li>(687656), (<a href="http://issuetracker.unity3d.com/issues/broken-ui-when-changing-camera-viewport-rect-on-unity-5-on-android">693423</a>) -  Editor: Added a printed warning to the gameview if there is no fullscreen camera present.</li>
<li>(none) -  Editor: Fixed 'Access denied' error on Windows when trying to move readonly files.</li>
<li>(666743) -  Editor: Fixed an issue where calling EditorWindow.GetWindow() too early could cause the editor to crash.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/resource-busy-mac-opening-new-project-throws-resource-busy-dialog-on-mac">705555</a>) -  Editor: Fixed A bug when opening new project threw "Moving file failed" dialog on Mac.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/sceneview-cant-select-objects-in-scene-view-without-dragging-around-it">719367</a>) -  Editor: Fixed scene view picking when in linear mode.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/unity-crashes-when-calling-dontdestroyonload-this-if-alphabetical-sorting-is-enabled">725519</a>) -  Editor: Fixes crash when exiting play-mode with Alphabetical Sort enabled.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/model-crash-when-model-with-blendshapes-has-normals-set-to-none-in-import-settings">704016</a>) -  Editor: Made sure blendShapes normals were not imported if None was set in Import Setting.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/per-platform-default-quality-settings-gets-lost-when-we-exit-unity-editor-while-being-in-play-mode">701240</a>) -  Editor: Save correct quality settings when quitting Unity editor during the play mode.</li>
<li>(721563) -  Editor: Slowdown in Project window with Unity 5.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/error-message-when-baking-real-time-gi-int-indices-kdynamiclightmap-plus-realtimeoffset-dot-dot-dot">722655</a>) -  GI: Calculate atlas index offset correctly when snapshotting a scene.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/realtime-gi-file-not-found-errors-displayed-when-upgrading-project-to-unity-5-dot-2">714050</a>), (701937) -  GI: Fixed the case where GI file not found errors were displayed when upgrading project to Unity 5.2.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/reflectionprobes-crash-when-reflection-probe-is-moved-in-global-illumination-scene-view">718263</a>) -  GI: Fixed a crash when moving reflections probes in GI visualisation views.</li>
<li>(none) - GI: Fixed loading a LightmapSnapshot.asset with realtime GI data. The issue was introduced in 5.2.0p1.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/light-commandbuffer-global-shader-properties-regression-in-5-dot-2">720748</a>) -  Graphics: Fixed global shader property changes done from Light CommandBuffers not affecting later rendering (5.2 regression).</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/regression-video-player-not-working-with-new-rendering-api-on-osx">719494</a>) -  Graphics: Fixed regression on GetNativeTextureID</li>
<li>(689461) -  IL2CPP: Added support for access default parameter values via reflection.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/il2cpp-t-doesnt-implement-ilist">717904</a>) -  IL2CPP: Allow a cast of T[] to IList (where BaseT is a base class of T) to work correctly.</li>
<li>(702684) -  IL2CPP: Allow il2cpp.exe to work if a '#' character is in the installation path.</li>
<li>(714759) -  IL2CPP: Allow WebRequest to work with IPv6 addresses.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/building-il2cpp-which-includes-the-jsonfx-library-throws-not-implemented-on-non-abstract-class">705898</a>) -  IL2CPP: Corrected a code generation error with the JsonFX library with the error message: "not implemented on non-abstract class".</li>
<li>(719084) -  IL2CPP: Corrected an error in the negation of a float converted from an unsigned integer.</li>
<li>(723439) -  IL2CPP: Corrected C++ code generation when a struct inherits from a generic interface.</li>
<li>(717058) -  Il2CPP: Corrected the behavior of Marshal.OffsetOf for structures with explicit packing.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/il2cpp-mathf-dot-roundtoint-method-doesnt-work-correctly">700792</a>) -  IL2CPP: Implemented the correct rounding behavior (banker's rounding) for the Math.Round method.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/unity-ios-player-will-crash-if-use-messagpack-serializer">661630</a>), (<a href="http://issuetracker.unity3d.com/issues/il2cpp-unsupported-internal-call-for-il2cpp-monocustomattrs">690171</a>) -  IL2CPP: Implemented the CustomAttributeData.GetCustomAttributes methods for attributes with a default constructor.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/il2cpp-keyvaluepair-throws-nullreferenceexception-and-crashes">722375</a>) -  IL2CPP: Prevent a NullReferenceException exception from being thrown in the KeyValuePair ToString method when the value is a reference type.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/il2cpp-error-in-xcode">722433</a>) -  IL2CPP: Prevent a used block from being marked as dead during conversion if it is immediately after a try block with an explicit leave opcode.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/il2cpp-missingmethodexception-is-thrown-if-tz4net-is-used">715013</a>) -  IL2CPP: Prevent the exception "MissingMethodException: No constructor found for System.Resources.RuntimeResourceSet::.ctor(System.IO.UnmanagedMemoryStream)" from occurring when the TZ4NET assembly is used.</li>
<li>(674706) -  IL2CPP:&nbsp;Allow GetCurrentProcess to work.</li>
<li>(none) -  IL2CPP:&nbsp;Allow il2cpp.exe to run when its installation path includes a '#' character followed by a space character.</li>
<li>(690171) -  IL2CPP:&nbsp;Corrected a KeyNotFoundException during code generation in the VTableBuilder.GetVirtualMethodTargetMethod method of il2cpp.exe.</li>
<li>(712470) -  IL2CPP:&nbsp;Corrected Marshal.OffsetOf when using enums fields with FieldOffsetAttribute</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/il2cpp-bug-enumerator-had-no-aot-code-generated">712713</a>) -  IL2CPP:&nbsp;Ensure methods needed for enum arrays are converted.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/ulink-crash-the-ios-player-when-using-il2cpp">715965</a>) -  IL2CPP:&nbsp;Fixed assert on socket error.</li>
<li>(712929) -  IL2CPP:&nbsp;Fixed comparison to Epsilon.</li>
<li>(712553) -  IL2CPP:&nbsp;Fixed error when using 64-bit Interlocked operations on 32-bit devices.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/ios-gchandle-dot-alloc-throws-error-on-il2cpp-build">716138</a>) -  IL2CPP:&nbsp;Fixed pinning of structures with ExplicitLayout.</li>
<li>(721435) -  IL2CPP:&nbsp;Fixed reading pointers with multiple levels of indirection.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/il2cpp-fails-to-convert-unsafe-void-star-to-a-struct-pointer-type">718696</a>) -  IL2CPP:&nbsp;Fixed unsafe pointer to struct assignment.</li>
<li>(721329) -  IL2CPP:&nbsp;Fixed various performance issues by doing less type initialization at startup.</li>
<li>(676797) -  IL2CPP:&nbsp;Implemented the IsTransparentProxy icall, which always returned false.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/uncaught-exception-in-il2cpp-icalls-mscorlib-system-array-clearinternal">710797</a>), (705882) -  IL2CPP:&nbsp;Prevent a type T from being stripping if it is used an GenericClass field in a MonoBehavior or ScriptableObject that is already being preserved.</li>
<li>(716991) -  IL2CPP:&nbsp;Speed up retrieving classes by name.</li>
<li>(none) -  iOS/IL2CPP: Completed the IPv6 implementation.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/ios-append-not-working-after-the-launch-screen-changes">723961</a>) -  iOS: Fixed append regression when certain splash screens are changed after initial build.</li>
<li>(704992) -  iOS: Fixed path stripping when trailing characters are present</li>
<li>(707385) -  iOS: Fixed touch screen keyboard when switching between single/multi line.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/www-ios-creating-a-www-request-without-saving-a-reference-to-it-triggers-a-crash">708549</a>) -  iOS: Fixed WWW crash when not keeping reference to instance.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/ios-player-crashes-when-using-dictation-on-ios-7">677907</a>) -  iOS: Fixed interop of OpenGL ES and Siri overlay</li>
<li>(none) -  iOS: Fixed iOS 9 side by side multitasking. It will work only if target resolution is native and it's not being overridden via script.</li>
<li>(none) -  iOS: Fixed multitasking snapshot creation.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/ios-touch-screen-keyboard-doesnt-get-closed-after-resuming-app">709943</a>), (716625), (<a href="http://issuetracker.unity3d.com/issues/ios-keyboard-is-invisible-after-returning-from-browser-on-ios7">713488</a>) -  iOS: Fixed numerous issues on iOS7 related to restoring app from background.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/ios-some-unicode-characters-not-displayed">718387</a>), (720698) -  iOS: Fixed system dynamic font support on iOS 9 where only the first font could be read from certain font collections and font substitutes, as identified by the OS, were not handled.</li>
<li>(none) -  iOS: Fixed WWW not reporting error in some cases (like no networking available).</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/unwrapper-gives-different-results-between-platforms">706367</a>) -  Lightmapping: Fixed lightmap UV generation to be identical across platforms.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/animator-events-are-not-invoked-if-animator-is-disabled-and-updated-externally">718896</a>) -  Mecanim: Allow SMB function call even when Animator is disabled but updated manually by user.</li>
<li>(717680) -  Mecanim: Fixed a crash when reimporting animations used in an overridecontroller.</li>
<li>(722058) -  Mecanim: Fixed a crash when setting an Override Controller with no controller to override.</li>
<li>(none) -  Mecanim: Fixed memory leak with Animator.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/mecanim-null-reference-when-transitioning-from-sub-state-machine-to-exit-node">719292</a>) -  Mecanim: Fixed null reference when creating transition to an empty state machine.</li>
<li>(713552) -  Mecanim: Fixed Transition inspector not showing the proper transition.</li>
<li>(none) -  Mecanim: Fixes crash when having an OnStateMachineEnter on first eval.</li>
<li>(719156) -  Networking: Fixed scene objects with NetworkTransform not synching.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/networkidentity-dot-onrebuildobservers-allows-not-ready-connections">718027</a>) -  Networking: Prevent adding network connections that are not ready as observers.</li>
<li>(none) -  OpenGL ES: Fixed missing 1x1 mip levels in textures.</li>
<li>(708698) -  OpenGL: Fixed OSX standalone crash</li>
<li>(719654) -  OpenGL: Fixed shader compilation error when using GLSL precision qualifier.</li>
<li>(708072) -  OpenGL: Fixed Unity shader compiler crash when compiling for OpenGL target.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/particles-are-blinking-when-there-are-two-identical-particle-systems">624081</a>) -  Particles: Fixed issue causing batched particles drawn after an object with negative scale to flip and become invisible.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/particle-system-changing-position-makes-particles-emit-along-line">714872</a>) -  Particles: Fixed issue where moving emitters in the editor would cause them to emit their particles along a trajectory from their start position.</li>
<li>(none) -  Physics2D: Ensure that 'Infinity' cannot be specified for 2D collider offset.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/changing-rigidbody2d-teleports-it-to-00-when-entering-play-mode">707400</a>) -  Physics2D: Stop Rigidbody2D X/Y Constraints from occasionally moving the body to the world origin.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/trigecollider2d-ontriggerenter2d-gets-called-even-though-the-collider-never-actually-reaches-the-trigger-collider">713073</a>) -  Physics2D: Stop trigger-contacts being reported early when using continuous collision detection.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/all-of-the-2d-joint-motor-speeds-are-grossly-off-after-upgrade-to-new-unity-version">721704</a>) -  Physics: Fixed SliderJoint2D motor-speed backwards compatibility prior to 5.1.1p3.</li>
<li>(718787) -  Plugins: Editor would report incorrectly that native plugin is colliding with itself.</li>
<li>(716978) -  Profiler: Fixed Rendering detailed stats. Stats for Draw Calls and Total Batches were previously swapped.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/profiler-missing-statistics-of-manually-rendered-camera">699695</a>) -  Profiler: Show profiler statistics of manually rendered camera.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/unity5-audioimporter-dot-containssamplesettingsoverride-error-samsung-tv">704481</a>) -  Samsung TV: Fixed "Unknown Platform" error when passing "Samsung TV" to AudioImporter.ContainsSampleSettingsOverride.</li>
<li>(717774) -  Samsung TV: Fixed issue where Development builds would inappropriately report security errors.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/texture-doesnt-render-properly-in-2013-stv">718017</a>) -  Samsung TV: Fixed issue where some textures would not display properly on 2013 TVs.</li>
<li>(none) -  Scripting: GL.IssuePluginEvent(eventID) is now obsolete.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/grabpass-drawn-texture-is-shifted-to-the-right">724452</a>) -  Shaders: Fixed GrabPass missing game view viewport offset in the editor.</li>
<li>(716161) -  Shaders: HLSL shader compilation fIxed floating point division by zero by initialising x components of surfIN members to 1.0.</li>
<li>(none) -  SpritePacker: Prevent Sprite Packing called randomly due to bug in hash Generation.</li>
<li>(719252) -  Tizen: Fixed crashes on launch of Tizen projects.</li>
<li>(none) -  Tizen: Fixed Tizen Store certification errors.</li>
<li>(none) -  Tizen: Implemented an API to retrieve the window handle.</li>
<li>(none) -  Tizen: Improvements to error messages.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/mesh-script-with-overriden-onpopulatemesh-and-updatematerial-causes-crash">719777</a>) -  UI: Fixed crash related to using multiple materials / submeshes on UI elements.</li>
<li>(<a href="http://issuetracker.unity3d.com/issues/layout-under-a-scrollrect-does-no-perform-its-layout-logic">721345</a>), (<a href="http://issuetracker.unity3d.com/issues/ui-scroll-rect-is-interfering-with-grid-layout-group">722086</a>) -  UI: Fixed ScrollRect causing immediate child view with LayoutGroup to not get layout callbacks.</li>
<li>(684885) -  UI: Fixed issue where Selectables (image, toggle, etc) would hold a reference to a sprite when a new scene was loaded. This would lead to the sprite staying in memory even if the reference was not in the new scene.</li>
<li>(204016) -  UI: RawImage component now uses the same vertex generation code as normal image components fixing a slight vertex offset error.</li>
<li>(716209) -  Universal Windows Apps: Fixed crash in WebcamTexture.</li>
<li>(717274) -  Universal Windows Apps: Fixed plugin processing.</li>
<li>(712699) -  Universal Windows Apps: Splash screen is correctly resized with app window.</li>
<li>(715960) -  Version Control: Do not use cached status for checking editability in VCS.</li>
<li>(none) -  VisualStudio - Fixed a bug where VisualStudio could fail to open if it was busy while Unity was trying to open it.</li>
<li>(711316) -  VR: Fixed point light rendering issue with deferred renderer.</li>
<li>(722915), (723184) -  VR: Fixed regression with linear lighting and anti aliasing on windows.</li>
<li>(none) - VR: Fixed GearVR plugin issue. GearVR builds now render properly.</li>
<li>(722122) -  VR: GearVR: Fixed gles20 rendering crash.</li>
<li>(none) -  VR: Overall stability improved.</li>
<li>(716227) -  Windows Phone 10: Fixed an issue whereby the touchscreen keyboard was not working.</li>
<li>(none) -  Windows Phone: Fixed RuntimeInitializeOnLoad to support WP8.1.</li>
<li>(712688) -  Windows Store Apps: App window is correctly activated with independent input source enabled.</li>
<li>(710903) - Windows Phone 8: Fixed an issue with build and run for projects with spaces in their names.</li>
<li>(720701) -  Windows Store Apps: Fixed invalid IL code in UnityEngine.Networking.dll.</li>
<li>(none) -  Windows Store Apps: UnityEngine.pdb file is installed along UnityEngine.dll.</li>
<li>(712019) -  WSA/UWP: Hide D3D11 warning D3D11_MESSAGE_ID_SETPRIVATEDATA_CHANGINGPARAMS.</li>
</ul>
