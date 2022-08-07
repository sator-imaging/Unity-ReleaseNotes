# Unity 5.0.1
https://unity3d.com/unity/whats-new/unity-5.0.1

## Fixes

<ul>
<li>AI: Fixed an issue where using all navmesh area types in mask didn't work.</li>
<li>AI: Fixed an issue where warping disabled agents would leak simulated agent.</li>
<li>Android: Always enable VSync on Android non-development builds.</li>
<li>Android: Build pipeline; fixed AAR manifest merging.</li>
<li>Android: Fixed an issue with the multithreaded job system which caused battery drain and bad performance.</li>
<li>Android: Fixed Auto target graphics mode on devices which wrongly claim to support OpenGL ES 3.0.</li>
<li>Android: Fixed crashes / touch problems when applying ForwardNativeEventsToDalvik to a non-NativeActivity.</li>
<li>Android: Fixed immersive mode when returning to activity in Lollipop.</li>
<li>Android: Fixed non-hidden status bar and status bar related touch issues.</li>
<li>Android: Fixed sensor compensation issue affecting devices when rotated180 degrees.</li>
<li>Android: Input - Fixed axis stuck on Android TV after hiding keyboard.</li>
<li>Android: Reenabled SSE skinning on x86.</li>
<li>Android: Removed some bogus print-outs to the logcat regarding gles_mode and development_player.</li>
<li>API Updater: Automatic update from ParticleSystem.CollisionEvent to ParticleCollisionEvent.</li>
<li>API Updater: Fixed API updater skipping assemblies in some scenarios.</li>
<li>API Updater: Fixed the issue causing crash while checking assemblies for obsolete API usage.</li>
<li>Asset Loading: Fixed loading of GI data from an AssetBundle.</li>
<li>Asset Loading: Fixed the crash when setting the AssetBundle name in OnPreprocessAudio() callback.</li>
<li>Asset Loading: Fixed the issue that streamed scenes don't draw layered UI in canvases correctly.</li>
<li>Asset Loading: Fixed the issue whereby streamed scene asset bundles do not allow more than one scene.</li>
<li>Asset Loading: Fixed the prefab async loading issue by loading the scripts first.</li>
<li>Asset Loading: Fixed the script loading issue when the references are between scripts.</li>
<li>Asset Loading: Updated the document to indicate we wanted complete asset paths.</li>
<li>Audio: Fixed "Trying to play disposed sound!" error message.</li>
<li>Audio: Fixed the "Disable Audio" option, the flag is now correctly used by the standalone player to disable the audio system.</li>
<li>Audio: Given AudioImporter overrideSamplerate a default value that makes sense.</li>
<li>BlackBerry: Fixed platform lookup from string to be case insensitive.</li>
<li>Bug reporter: Fixed issue with submitting files when temp path includes non-ASCII characters.</li>
<li>Bug reporter: Fixed the issue causing crash when attaching files on OSX 10.8.5.</li>
<li>Bug reporter: Fixed title field validation (the title is now mandatory).</li>
<li>Bug reporter: Hidden files are now always included in bug reports.</li>
<li>Bug reporter: Make sure the bug reporter triggers from the license error popup.</li>
<li>Bug reporter: Updated links to the new Bug Reporter (when it's started from outside the Editor).</li>
<li>BugReporter: Send empty subdirectories of directory attachment. Improved filtering of unnecessary subdirectories under Unity project. Can launch when some parts of the engine might not be initialized yet.</li>
<li>Deployment Management: Prevent simultaneous launches of Unity loading wrong project.</li>
<li>Don't allow AddComponent() calls on object that is currently being destructed (leads to crashes).</li>
<li>Editor: "Missing Prefab" placeholders now respects the active state of their parents.</li>
<li>Editor: Android - Don't allow to install x86 apk on arm device.</li>
<li>Editor: Disable vsync for all views except GameView on OSX.</li>
<li>Editor: Fixed an issue where Editor fails to validate serialization layout when building to Windows Store Apps.</li>
<li>Editor: Fixed crash when compressing GI cache files with lz4.</li>
<li>Editor: Fixed crash when using UnityEditorInternal.InternalEditorUtility.LoadSerializedFileAndForget to load a scene with containing stripped prefab instance objects</li>
<li>Editor: Fixed null-ref from SceneView when having a Hierarchy search filter.</li>
<li>Editor: Fixed performing Undo on prefab instances where the prefab parent was missing.</li>
<li>Editor: Fixed reading very very big scenes with more than 32767 monobehaviours created in Unity prior to Uniy 5.</li>
<li>Editor: Fixed the issue producing fatal error when choosing unwritable drive as a GICache folder on OSX.</li>
<li>Editor: Fixed undo parenting of prefab.</li>
<li>Editor: Necessity of rebuilding .meta files detected incorrectly for projects that contain only directories in Assets/.</li>
<li>Editor: OnOpenAsset callbacks are now called for all asset types when doubled clicked in the project browser.</li>
<li>Editor: Plugin inspector-set ARMv6 Android plugins incompatible to avoid collisions.</li>
<li>Editor: Prefab connection is now broken when rearranging components, even if the components are added to the instance. This enables you to rearrange components on prefab instances without losing the order when saving the scene.</li>
<li>Editor: Stripped prefab instance objects are now marked as stripped in the scene file, so the loading code does not try to upgrade objects which would issue wrong warnings and in worst case crashes.</li>
<li>Editor: Fixed editor lockup if left in the background and profiler was open.</li>
<li>GI: Changing directional mode in lighting tab does not force reflection probe.</li>
<li>GI: Clear lightmapping state when wiping the disk cache in order to avoid errors when building lighting.</li>
<li>GI: Fixed "Mobile/Unlit (Supports Lightmap)" shader and other fixed function shaders using lightmaps.</li>
<li>GI: Fixed rare crash in realtime GI pipeline caused by textures held by worker threads being released too early.</li>
<li>GI: Made Gradient ambient mode properly affect realtime and baked GI.</li>
<li>GI: Made lightmaps be properly compressed on mobile platforms.</li>
<li>GI: Report errors from jobs correctly when run in an external process.</li>
<li>GI: Reset the texture filter mode after rendering object preview in lighting window.</li>
<li>Graphics: Fixed vertices being lit entirely black on DirectX 11 when normals are missing and the vertex position is (0,0,0).</li>
<li>iOS: Added Xcode 6.3 compatibility.</li>
<li>iOS: Disabled unnecessary copies of dll files to the Xcode project directory.</li>
<li>iOS: Exposed iOSOverrideIPodMusic in player settings.</li>
<li>iOS: Fixed a typo in UnityRegisterViewControllerListener().</li>
<li>iOS: Fixed an issue with the job system which caused battery drain and bad performance.</li>
<li>iOS: Fixed changing from autorotation to enforced screen orientation in case of this orientation being already current.</li>
<li>iOS: Report a fake Status: HTTP header for informational purposes.</li>
<li>iOS: Show an error on removal of targets in Xcode project.</li>
<li>iOS/IL2CPP: Handle 4D arrays.</li>
<li>iOS/IL2CPP: Handle delegate invoke with nested delegates where the method which is invoked on the outer delegate is a static method.</li>
<li>iOS/Metal: Fixed fixed function shaders with cubemaps.</li>
<li>iOS/Metal: Fixed vector_insert_TODO appearing in some shaders.</li>
<li>iOS/Metal: Partially fixed performance issue on A7 devices when using Standard shader.</li>
<li>Linux: Fixed crash when swapping UI sprites.</li>
<li>Oculus: Plugin initialize fixed when GfxDevice had not been Initialized yet.</li>
<li>OpenGL: Fixed crash with -force-opengl in Windows Editor when trying to enable DirectX 11 via player settings.</li>
<li>Physics 2D: Added 'forceScale' property to SurfaceEffector2D to allow scaling of the impulse force used.</li>
<li>Physics 2D: Center-of-mass and Inertia can now be set on a Rigidbody2D component even if it has no Collider2D components attached.</li>
<li>Physics 2D: Disabled PlatformEffector2D component now fully disables contact processing.</li>
<li>Physics 2D: Fixed console warning of 'm_Effector == effector' when removing an effector inside a prefab.</li>
<li>Physics 2D: Fixed PlatformEffector2D so that when stopping inside a collider it doesn't cause a collision for 'one-way'</li>
<li>Physics 2D: Stop 2D colliders falling through EdgeCollider2D components.</li>
<li>Physics 2D: Stop crash when NULL passed to Collider2D.IsTouching, Physics2D.IsTouching or Physics2D.IsTouchingLayers.</li>
<li>Physics: OnJointBreak callback now has correct breaking force magnitude supplied as a parameter.</li>
<li>Profiler: Fixed editor slowdown if GPU profiler was enabled when the profiler was stopped or closed</li>
<li>Rendering: Now the back buffer is cleared after the resolution is changed from a script in Windows standalone.</li>
<li>Samsung TV: Fixed MissingMethodException being thrown when a scene was played that used STV specific APIs.</li>
<li>Samsung TV: Fixed UEP signing for 2015 TVs.</li>
<li>Scripting: Crash on Newtonsoft.Json.DeserializeObject(string) when serialized type has generic arrays.</li>
<li>Scripting: Fixed Application.logMessageReceivedThreaded not being called in main thread.</li>
<li>Scripting: Fixed crash when trying to invoking delegate bound to open generic method.</li>
<li>Scripting: Fixed infinite loop in NetworkInterface.GetAllNetworkInterfaces()</li>
<li>Scripting: Fixed VS / MonoDevelopment project synchronization when "Editor" was the only platform selected in plugins settings.</li>
<li>Scripting: Throw DivideByZero exception instead of crashing.</li>
<li>Serialization: Fixed crash when reading file references from long property names.</li>
<li>Shaders: WPOS semantic works in shaders again (alias of VPOS, i.e. screen position).</li>
<li>Sprites: Fixed the issue whereby Unity was doubling the memory needed for the Texture Atlases.</li>
<li>Terrain: Base map generation in Linear rendering mode is now done in linear space.</li>
<li>Terrain: Fixed a crash when a terrain was using TerrainData with missing textures.</li>
<li>Terrain: Fixed an issue where modifying terrain heights would result in an inconsistency between the visual and the collision.</li>
<li>Terrain: Fixed visual inconsistency when rendering with base pass.</li>
<li>Terrain: Standard terrain shaders now correctly support spot light / point light shadows.</li>
<li>Version Control: Set correct changeset description when renaming a changeset.</li>
<li>Version Control: Use saved changeset description when submitting.</li>
<li>Video: Fixed the issue whereby ogg movie playback skipping frames at beginning and general sync improvement.</li>
<li>VR: Fixed GearVR startup crash.</li>
<li>WebGL: Fixed deleting characters in text fields.</li>
<li>WebGL: Fixed reverting to proper window size when getting out of fullscreen mode.</li>
<li>WebGL: Fixed shift-arrow-key in text fields.</li>
<li>WebGL: Fixed WWW.audioClip.</li>
<li>Windows Standalone: -parentHWND command line argument works again.</li>
<li>Windows Store Apps: Fix issue where Unity was trying to locate Microsoft.CSharp.dll when processing some of the plugins, for ex., Facebook.Client.dll.</li>
<li>Windows Store Apps: Fixed player when installed to path containing unicode characters.</li>
<li>Windows Store Apps: Fixed resource fight on hyperthreading-enabled CPUs which might cause unstable performance on Windows.</li>
<li>Windows Store Apps/Windows Phone 8: UnityPlayer pdb files will be present again for Debug/Master configs.</li>
<li>Windows Store Apps/Windows Phone 8: When unloading unused assets or switching to another scene, prefabs will be correctly reloaded and won't loose references. Previous behavior was sometimes textures, mono behaviors, etc in prefabs would be lost, this would result for e.g., in textures not showing up in objects instantiated from prefabs.</li>
<li>WWW: Fixed incorrect HTTP status 100 when POST data was relatively large.</li>
<li>Xbox One: Implemented workaround fix for rendering failure when the console is set to instant-on standby and suspend/resume flow occurs.</li>
<li>Xbox One: Lightmap files are now included in the package manifest.  They are included as a part of the launch chunk. </li>
<li>Xbox One: ReadPixels glitch and performance slowdown: fixed and workaround implemented.</li>
</ul>

### Fixes that shipped in Unity 4.6.4 too
<ul>
<li>Android: Fixed back button crash on Samsung devices.</li>
<li>Android: Fixed checkjni exception when passing array in JNI at ART.</li>
<li>Android: Workaround for animation glitch with onscreen keyboard.</li>
<li>IL2CPP / Raknet: Fixed networking RPC call registration not working on IL2CPP backend.</li>
<li>iOS: Fixed iPad Mini 3rd gen detection.</li>
<li>iOS: Improved Xcode project parser robustness for invalid input.</li>
<li>iOS/IL2CPP: Added support for setting thread names on OS X.</li>
<li>iOS/IL2CPP: Added support for WebRequest to HTTPS addresses when using the Api Compatibility Level setting of .NET 2.0 Subset.</li>
<li>iOS/IL2CPP: Allow the LogInAsync method in the ParseSDK to work correctly.</li>
<li>iOS/IL2CPP: Always initialize type information before accessing static fields.</li>
<li>iOS/IL2CPP: Assembly.Load() now accepts assembly name in full name format.</li>
<li>iOS/IL2CPP: Correct a number of problems related to WebRequest and ThreadPool interaction: 
<ul>
<li>Fixed a queuing bug that may lead to WebRequests arriving at the same time and being used incorrectly.</li>
<li>Fixed assert "pthread_equal (pthread_self (), m_Handle) &amp;&amp; 'Must be called on current thread!'".</li>
<li>Fixed deadlock on shutdown if socket polling thread was still waiting for network traffic.</li>
<li>Fixed deadlock when socket exits polling stage when I/O pool is at max capacity and worker threads are in wait state.</li>
<li>Fixed performance load balancing issue in CullAllPerObjectLights that caused only one job to be run rather than many (occurred when high number of lights and low number of objects)</li>
<li>Fixed race condition in static constructor calling.</li>
<li>Fixed thread interruption logic incorrectly thinking that another thread was still waiting.</li>
<li>Fixed WebRequests getting stuck in socket polling stage when the stage should be skipped.</li>
</ul></li>
<li>iOS/IL2CPP: Corrected a problem with Delegate.CreateDelegate.</li>
<li>iOS/IL2CPP: Corrected the C++ compiler error in generated code: "error: cast from pointer to smaller type 'il2cpp_array_size_t' (aka 'int') loses information"</li>
<li>iOS/IL2CPP: Correctly write include definitions for a generic class with a const field.</li>
<li>iOS/IL2CPP: Emit the proper metadata for parameters static inflated generics methods.</li>
<li>iOS/IL2CPP: Explicitly declare generic types and array types that are created at run-time via Type.MakeGenericType and Type.MakeArrayType in the il2cpp_extra_types.txt file, so that IL2CPP will AOT compile them.</li>
<li>iOS/IL2CPP: Fixed a case where having throw statement at the end of a method would cause IL2CPP to crash.</li>
<li>iOS/IL2CPP: Fixed the problem with shift operators, resulting in problems with MD5 calculation and crypto, amongst other things.</li>
<li>iOS/IL2CPP: Fixed array marshaling when passing an incorrect argument.</li>
<li>iOS/IL2CPP: Fixed Array.CopyTo() fast path, which was doing the wrong thing when the source array was a value type and destination array was not.</li>
<li>iOS/IL2CPP: Fixed C++ compile error in some cases when using fields with the same name in a class hierarchy.</li>
<li>iOS/IL2CPP: Fixed C++ linker error in some cases when using generic method constraints.</li>
<li>iOS/IL2CPP: Fixed C++ linker error in some cases when using generic parameters.</li>
<li>iOS/IL2CPP: Fixed code generation for delegates having parameters tagged with the Out attribute.</li>
<li>iOS/IL2CPP: Fixed conversion error in obscure edge case of method overrides through metadata and signature.</li>
<li>iOS/IL2CPP: Fixed crash when calling MethodInfo.ReturnTypeCustomAttributes.GetCustomAttributes on a constructor.</li>
<li>iOS/IL2CPP: Fixed crash when System.Console is included in link.xml.</li>
<li>iOS/IL2CPP: Fixed deadlock or timeouts when C# code does BeginInvoke+EndInvoke on a worker thread and the pool has only one thread.</li>
<li>iOS/IL2CPP: Fixed exceptions thrown by using System.Configuration.ApplicationSettingsBase.</li>
<li>iOS/IL2CPP: Fixed IL2CPP crash in some cases when using virtual generic methods.</li>
<li>iOS/IL2CPP: Fixed IL2CPP crash when passing null as value to array parameter in custom attribute constructor.</li>
<li>iOS/IL2CPP: Fixed issue with String.Intern not always returning the correct string.</li>
<li>iOS/IL2CPP: Fixed List.FindAll().</li>
<li>iOS/IL2CPP: Fixed MethodInfo.GetBaseDefinition().</li>
<li>iOS/IL2CPP: Fixed null reference exception when calling TripleDES.Create.</li>
<li>iOS/IL2CPP: Fixed order of properties returned by Type.GetProperties().</li>
<li>iOS/IL2CPP: Fixed rare crash when calling Type.GetMethods.</li>
<li>iOS/IL2CPP: Fixed single core CPU system resulting in ThreadPool with no threads.</li>
<li>iOS/IL2CPP: Handle code generation for an struct which has an array of enums as a field.</li>
<li>iOS/IL2CPP: Handle IL code which uses one local variable as an array index more than once, with different values.</li>
<li>iOS/IL2CPP: Handle NULL const string values.</li>
<li>iOS/IL2CPP: Handle out and ref marshaling of a delegate with a struct that has no instance fields.</li>
<li>iOS/IL2CPP: Implemented Assembly.GetName().</li>
<li>iOS/IL2CPP: Implemented Assembly.GlobalAssemblyCache so that it always returns false.</li>
<li>iOS/IL2CPP: Implemented marshaling of the SafeHandle type.</li>
<li>iOS/IL2CPP: Implemented marshaling support for explicit struct layouts.</li>
<li>iOS/IL2CPP: Implemented MethodBase.GetMethodFromHandle with two arguments for a non-generic type.</li>
<li>iOS/IL2CPP: Implemented missing Marshal.PtrToStructure overload which takes object reference.</li>
<li>iOS/IL2CPP: Implemented the use of SizeParamIndex for marshaling.</li>
<li>iOS/IL2CPP: Improved support for MakeGenericMethod.</li>
<li>iOS/IL2CPP: Implemented marshaling of the System.Runtime.InteropServices.HandleRef type.</li>
<li>iOS/IL2PP: Fixed ParameterInfo.Attributes always returned ParameterAttributes.None for parameters.</li>
<li>iOS/Metal: Fixed RenderTexture mip-map generation in cases of ReadPixels immediately after drawing.</li>
<li>Linux: Fixed the issue which was causing crash with native plugins using STL types.</li>
<li>Linux: Hide system cursor when using software cursor.</li>
<li>Scripting: Fixed C# compiler generating incorrect IL in some cases for iterator finally blocks.</li>
<li>Stripping: Fixed the issue which was making stripping completely disabled for Mono scripting backend.</li>
<li>UI: Fixed overriding/inheriting of pixel perfect status in child canvases.</li>
<li>Windows Store Apps: Fixed VS solution generation with paths containing unicode characters.</li>
<li>Windows Store Apps: Use exception log type for exceptions now.</li>
<li>Windows Store Apps/Windows Phone 8: Fixed a memory leak, which was occurring in various places. For e.g., in physics collision callbacks such as OnCollisionEnter(Collision collision).</li>
</ul>
