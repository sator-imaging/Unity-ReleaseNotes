# Unity 5.2.4
https://unity3d.com/unity/whats-new/unity-5.2.4

## Fixes

<ul>
<li>2D: Optimisations in shader performance targeting non-ETC1 platforms. (728361)</li>
<li>AI: Fixed NavMeshAgent being unable to pass certain edges in navigation mesh. (717360)</li>
<li>Android: Android 6.0 - Ask for any dangerous permission on startup. (739831), (732504)</li>
<li>Android: Fixed NullReferenceException on x86 devices running Android 5.0 or newer.</li>
<li>Android: Fixed OBB deployment on Android 6.0 and some older devices. (734408)</li>
<li>Android: Fixed querying for custom permissions on Android Marshmallow. (750227)</li>
<li>Android: Fixed VRAM calculation on devices with 4GB or more RAM.</li>
<li>Android: Marshmallow - Added the possibility to disable the permission dialog by adding metadata to the activity.</li>
<li>Android: Reset key press on resume. (719645)</li>
<li>Android/IL2CPP: Fixed an issue whereby the shared library on IL2CPP-built apk did not load and caused DllNotFoundException. (736110)</li>
<li>Animation: Fixed crash when deleting AnimatorController asset.</li>
<li>API Updater: Fixed crashing when checking for obsolete API in assemblies referencing unity extensions. (734221)</li>
<li>AssetBundles: Loading an uncompressed AssetBundle with CreateFromMemory causes a crash, fixed. (698667)</li>
<li>Audio: Fixes issue when modifying exposed parameters in AudioMixer loaded from asset bundle. (734258)</li>
<li>Core: Fixed Asset Importer error when calling AssetDatabase.Refresh during import of assembly. (730559)</li>
<li>Editor: Fixed error message given when picking game objects with children set as visible. (729010)</li>
<li>Editor: Force reimport all models to ensure that generated lightmap UVs are consistent across platforms. (739787, 745698)</li>
<li>Graphics: Enabled rendering to cube map faces with multisample AA. (730570, 648624)</li>
<li>Graphics: Fixed incorrect stripping of vertex streams in certain situations when a mesh has a mixture on lightmapped and non-lightmapped shaders; e.g. the vertex colour stream was previously being incorrectly stripped. (683178, 725562)</li>
<li>Graphics: Fixed performance regressions due to shadow rendering jobs.</li>
<li>IL2CPP: Allow the [Preserve] attribute to correctly prevent stripping of a method in a nested type. (738356)</li>
<li>IL2CPP: Avoid compiler error due to duplicate FieldInfo definition.</li>
<li>IL2CPP: Avoid stack overflow crash due to large allocation with alloca. (739685)</li>
<li>IL2CPP: Correctly initialize the metadata for default parameter values that are obtained via reflection. (745793, 737565)</li>
<li>IL2CPP: Fixed ExecutionEngineException being thrown on System.Reflection.MonoProperty::GetterAdapterFrame. (737529)</li>
<li>IL2CPP: Fixed race condition during cleanup of threadpool threads. (738232)</li>
<li>IL2CPP: Prevent generated C++ code from including a header file that was not generated when the type which could have been generated in that header is used only in an attribute applied to an assembly. (737996)</li>
<li>IL2CPP: Properly handle additional, subtraction, and multiplication when the type of the left argument is smaller than the type of the right argument and the result will not fit in the type of the left argument and the result is stored across an IL block. (745691)</li>
<li>IL2CPP: Provide proper managed stack traces when the C++ compiler inlines method calls. (739956)</li>
<li>IL2CPP: Treat assemblies mentioned in the link.xml file as roots for code conversion, but not as roots for code stripping. This corrects a regression in build size on iOS. (749728)</li>
<li>iOS: Added workaround for iOS launch screen asset catalog bug. (736683, 739007)</li>
<li>iOS: Build Unity runtime with bitcode. For now bitcode is supported only in il2cpp non-development builds.</li>
<li>iOS: Don't show simulators when doing regular build. (742801)</li>
<li>iOS: Fixed an issue with newer Xcodes refusing to link simulator builds that previously worked fine. (748014)</li>
<li>iOS: Fixed release target being set to 4.0 when setting minimum iOS version to 9.0. (741993)</li>
<li>iOS/IL2CPP: Avoid duplicate data files in iOS packages. (746329)</li>
<li>iOS/IL2CPP: Set default stack size on iOS to 1MB to match Mono behavior. (733799)</li>
<li>License: Fixed license activation problems caused by updating Windows 10.</li>
<li>Mecanim: Added type check when firing events with Object parameters. (738428)</li>
<li>Mecanim: Fixed Animator.Play not working on 1st frame when enabling GameObject. (732739)</li>
<li>Mecanim: Fixed blending that was different when swapping OverrideController at runtime. (734681)</li>
<li>Mecanim: Fixed crash when enabling an Animator on an object that was disabled then re-enabled. (737437)</li>
<li>Mecanim: Fixed error when adding transition. (736520)</li>
<li>Mecanim: Fixed events being called when state is not playing. (727746)</li>
<li>Mecanim: Fixed speed being not applied correctly when manually updating Animator. (737582)</li>
<li>Mono: Preserve non-volatile XMM registers across calls on 64-bit Windows during JIT compilation. (691466)</li>
<li>OpenGL: Work around array buffer access crash.</li>
<li>Physics: Ensure that OnCollisionEnter2D is always called if a contact starts and ends during a single physics update. (742572)</li>
<li>Physics: Ensure that Physics2D OverlapAreaXXX checks are consistent with OverlapBoxXXX checks. (727734)</li>
<li>Physics: Fixed an issue where a static trigger collider would not report a contact when moved. (752059)</li>
<li>Physics: Fixed an issue where collision/trigger callbacks would not report if constantly modifying a Collider2D (that caused it to be regenerated). (752764)</li>
<li>Physics: Fixed NullReferenceException in the editor when dragging a Rigidbody2D in the scene whilst it is deleted. (740256)</li>
<li>Samsung TV: Center cursor before locking and then ignore mouse motion event while cursor is locked.</li>
<li>Scripting: OnTransformChildrenChanged message is now correctly sent to both old parent and new parent. (688317, 713431)</li>
<li>UI: Fixed a performance issue with fonts rebuilding. (735927)</li>
<li>UI: Fixed color conversion in BatchGenerator when using Linear color space. (730457)</li>
<li>UI: Fixed issue when instantiating and re-parenting canvases and prefabs. (736161, 742081)</li>
<li>UI: Fixed issue where nested canvas wouldn't update its children elements rendering position if moved.</li>
<li>UI: Fixed memory leak when destroying Canvas. (750109)</li>
<li>UI: Fixed the issue with deleting a world canvas during play when paused. (727793)</li>
<li>VR: Fixed a crash when trying to toggle showDeviceView to false before first Update. (749329)</li>
<li>VR: Fixed an issue where Oculus was starting while building the standalone player while Virtual Reality Supported is true. (748988)</li>
<li>VR: Fixed an issue where showDeviceView was not caching between runs in the Editor. Now forces to true on play. (750510)</li>
<li>VR: Fixed Issue loading the Oculus SDK on the first time running when starting a new project.</li>
<li>WebGL: Fixed heavy memory consumption when downloading asset bundles using WWW.LoadFromCacheOrDownload. (725862)</li>
<li>Windows Phone 8.0: Fixed regression with System.IO classes. (745932)</li>
<li>Windows Standalone: Fixed Unity Crash on Application.Quit with MultiTouch.</li>
<li>Windows Store Apps: Fixed .NET native invalid IL warnings. (729793)</li>
<li>Windows Store Apps: Fixed Assembly-CSharp* project debugging in Universal Windows 10 apps, breakpoints should work now. (745716)</li>
<li>Windows Store Apps: Fixed FileStream occasionally failing when writing large data. (745355)</li>
<li>Windows Store Apps: Fixed same files referenced by Assembly-CSharp and Assembly-CSharp-firstpass projects. (746296)</li>
<li>Windows Store Apps: Make explicit call UnityPause(1) to pause player until explicitly unpaused via UnityPause(0). (736611)</li>
<li>Windows Store: Fixed Unity producing invalid Visual Studio project files if Windows 10 SDK 10.0.10586.0 is installed (749600)</li>
</ul>

#### Revision: 98095704e6fe
