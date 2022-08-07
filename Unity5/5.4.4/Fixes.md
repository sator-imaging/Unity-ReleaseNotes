# Unity 5.4.4
https://unity3d.com/unity/whats-new/unity-5.4.4

## Fixes

<ul>
<li>AI: Fix for an error when calling Warp and enabling a disabled NavMeshAgent. Errors in console: "!InCrowdSystem" and "!handle.IsValid()". (833396)</li>
<li>Android: Fixed a pause-resume incorrect behaviour in certain circumstances. (825170)</li>
<li>Android: Fixed crash on some devices when multiple sprite objects are in scene. (844606)</li>
<li>Android: Input.backButtonLeavesApp=true now exits gracefully. (845646)</li>
<li>Android: The platform setting for Android plugins now defaults to "Android" instead of "Any Platform". (824462)</li>
<li>Asset Pipeline: Fixed an issue where deleting asset labels manually from .meta files would not be picked up by the editor. (793711)</li>
<li>Asset Pipeline: Fixed an issue where asset and timestamp maps could get out of sync. (668043, 837519)</li>
<li>Asset Pipeline: Fixed regression where cache LZ4 compression was not being performed for uncompressed AssetBundles. (845859)</li>
<li>Audio: Fixed the issue which prevented streaming audio loading on 32-bit Apple devices which were upgraded to iOS 10. (832578)</li>
<li>Build Pipeline: Fixed a rare crash in the BuildReport system when building standalone player data. (856822)</li>
<li>Build Pipeline: Report build-time-generated streaming resources, such as texture atlases, at the correct size in the build report. (800613)</li>
<li>Build Pipeline: VR Splash Screen texture will no longer be included when building a project for a non-VR platform. (853619)</li>
<li>Collab: Auto Refresh is no longer force enabled even after Collab is turned off. (821909)</li>
<li>Core: Fixed hangs in the job system when running on certain platforms with a low number of cores e.g. older Windows Phones, UWP dual core machines. (791434)</li>
<li>Core: Fixed the logType passed to LogCallback in the event of an unhandled exception. (814160)</li>
<li>Core: Fixed an issue where a prefab instance could be incorrectly marked inactive when first loading a scene. (801761)</li>
<li>Core: Fixed a rare issue where prefab references from scene objects would be show as missing when using text serialization. (850947)</li>
<li>Editor: Fixed case of WebViews appearing blank in Editor main window on MacOS 10.12.1 (Sierra). (842708)</li>
<li>Editor: Fixed editor focus when multiple light probes have been selected. (824962)</li>
<li>Editor: Tweaked the output of the generated Visual Studio solution file to better match Visual Studio standard format to fix problems opening Unity generated projects with Rider GUI. (833866)</li>
<li>Graphics: Added additional error checking for compute buffers to catch invalid size and stride earlier to give a better error message. (834258)</li>
<li>Graphics: Added Material.SetBuffer with nameID overload. (853627)</li>
<li>Graphics: DX12 optimisation to reduce number of calls to CopyDescriptors.</li>
<li>Graphics: Fixed a crash during shutdown when using the DX9 graphics API. (846989)</li>
<li>Graphics: Fixed a crash when baking lightmaps in scenes with multiple terrains. (728648)</li>
<li>Graphics: Fixed a crash when deleting a Shader that was used by some Materials in the scene. (851359)</li>
<li>Graphics: Fixed a crash when switching scenes whilst reflection probes are updating. (832595)</li>
<li>Graphics: Fixed a crash when using dynamic batching. (839035)</li>
<li>Graphics: Fixed a crash when using Material.SetColor and similar functions with some built-in Unity variable names. (849344)</li>
<li>Graphics: Fixed a problem with objects not rendering after resolution changes or entering/exiting fullscreen when using DX9 graphics API. (840897)</li>
<li>Graphics: Fixed a rare situation which could lead to a deadlock when running with graphics jobs enabled.</li>
<li>Graphics: Fixed an issue when GrabPass was used with forward rendering and graphics jobs are enabled. (836947)</li>
<li>Graphics: Fixed Camera.SetReplacementShader renders objects affected by projectors even when the tag does not match. (840141)</li>
<li>Graphics: Fixed case of Lighting preview windows not rendering correctly on Macs with Retina displays. (836815)</li>
<li>Graphics: Fixed crashes when using Compute Buffers from scripts which get garbage collected. Added a user warning to show if a Compute Buffer has not been released manually by the user. (830217)</li>
<li>Graphics: Fixed memory leak when instantiating materials (e.g. via renderer.material). (851689)</li>
<li>Graphics: Fixed multiple lights not rendering when in deferred mode and using Graphics Jobs setting. (821028)</li>
<li>Graphics: Fixed CommandBuffer.DrawMesh crash. (827803)</li>
<li>Graphics: Fixed selection of objects in Scene View if the scene contains reflective water. (769758)</li>
<li>Graphics: Improved transparency support on meshes with multiple materials. (817524)</li>
<li>Graphics: Skip rendering of default reflection in Deferred Shading when the reflection not set. (843813)</li>
<li>IL2CPP: Android; fixed an issue whereby compiler/linker error output were not captured. (851098)</li>
<li>IL2CPP: Emit proper C++ for unsafe methods that cast a void pointer to a type pointer and access a field from that type.</li>
<li>IL2CPP: Fixed a crash that can occur in the player when a virtual method was called on a value type and that value type implements an interface which had an overload of that virtual method. (849701)</li>
<li>IL2CPP: Fixed a runtime crash when trying to call interface methods on integral pointers in unsafe contexts. Issues seemed to only show up when code was built outside of Unity with the Microsoft .NET compiler. (851793)</li>
<li>IL2CPP: Implemented the array SetValue method for arrays of nullable types. (849072)</li>
<li>IL2CPP: Prevent a stack overflow in the player runtime when metadata for an infinitely nested recursive generic type used (like the FullName of that type). (856410)</li>
<li>IL2CPP: Prevented a compiler error in generated C++ code when calling Interlocked.CompareExchange from some managed code. (847838)</li>
<li>IL2CPP: Prevented a stack overflow exception in the player at run time when an infinitely nested generic method is used. (845174)</li>
<li>IL2CPP: Support managed stack traces on Android now. (846956)</li>
<li>iOS: Fixed an issue of freezes related to ARM atomics. (840773, 849280)</li>
<li>iOS: Fixed an issue where the keyboard could lose focus when rotating the device (814493)</li>
<li>iOS: Fixed audio ducking when background applications sound were muted after running Unity application. (828762)</li>
<li>iOS: Fixed Module Registration and Code Stripping for builds using the Mono scripting backend. (763240)</li>
<li>iOS: Fixed several crashes with regards to WWW and WebRequest. (852363, 814365, 823587)</li>
<li>iOS: Fixed touch input latency issue for iOS 10. (817056)</li>
<li>Lighting: Fixed a problem with reflection probes updating during runtime even when "Refresh Mode" was set to "Via Scripting". (820587)</li>
<li>Lighting: Fixed crash when building lighting on specific projects and scenes. (834235)</li>
<li>Lighting: Fixed lighting variation from light probes caused by the rendering order of objects and the "Light Probes" property on the objects. (840641)</li>
<li>Linux: Fixed a shutdown crash. (847976)</li>
<li>Metal: Improved handling of transparent rendering after post-opaque image effects when using MSAA.</li>
<li>Networking: Calling NetworkTransport.GetCurrentRTT causes editor crash when WebSockets are enabled. (829943)</li>
<li>Networking: CRC Mismatch on Wii U. (831101)</li>
<li>Networking: Fixed enabling of WebSockets maxing out a CPU core. (830108)</li>
<li>Networking: WebSockets client doesn't support multiple connections. (839116)</li>
<li>OpenGL: Fixed UI image mask when running in upscaled fullscreen mode. (849681)</li>
<li>Particles: Fixed occasional crash when using external forces module. (849084)</li>
<li>Physics: Ensure that 2D effector targets are limited to dynamic bodies only and do not allow the consideration of kinematic body types (performance improvement). (842783)</li>
<li>Profiler: Fixed issue where taking detailed memory snapshot did not work in some cases. (836589)</li>
<li>Scripting: Fixed MonoDevelop build errors when building UnityScript and Boo projects. (850350)</li>
<li>Services: Fixed a potential crash on player exit if Game Performance Service is enabled. (840591)</li>
<li>Shaders: Automatically upgrade any shaders using unity_SpecCube1, to fix unity_SpecCube1 related shader compile errors after a project upgrade. (825418)</li>
<li>Shaders: Fixed a shader compiler crash for shaders which had extra "}" tokens in them. (844355)</li>
<li>Shaders: Fixed crash when compiling very complex surface shaders. Optimised the memory usage during surface shader compilation. (825408)</li>
<li>Substance: Fixed case of emission shader parameter not being properly set on import when emission global illumination is set to realtime. (840181)</li>
<li>Substance: Fixed case of SubstanceArchive inspector unselecting ProceduralMaterials after being renamed. (840177)</li>
<li>Substance: Fixed crash when loading a substance with corrupted data. (842999)</li>
<li>Substance: Fixed issue where ProceduralTexture inspector preview would sometimes show invalid size and format. (829162)</li>
<li>UI: Fixed an issue whereby disabling parent canvas allowed child canvas to render. (842364)</li>
<li>UI: Fixed cases where UI elements didn't render immediately and sometimes not at all after reparenting elements. (821319, 837935)</li>
<li>UI: Fixed crash when deleting objects. (818122)</li>
<li>UI: Fixed jittery movement when scrolling ScrollRect. (819300)</li>
<li>UI: Fixed Sprite Packer not packing sprites with ETC1 when compressing sprites for Android (845448)</li>
<li>UI: Fixed threading problem when computing bounds which could lead to an infinite loop in the UI system. (846096)</li>
<li>UnityWebRequest: Fixed case of incorrect Content-Type request header for multipart form data in POST requests. (826626)</li>
<li>UnityWebRequest: Fixed case of POST requests not working with empty data. (851921)</li>
<li>UnityWebRequest: Fixed issue where escaped characters in URL would get unescaped. (850018)</li>
<li>Version Control: Fixed null reference exception after resolving an asset (e.g. prefab) whilst the asset is selected and displaying in the inspector. (657131)</li>
<li>VR: Fixed a memory leak when using a canvas and VRFocus is lost. (824508)</li>
<li>VR: Fixed crash when checking for Stereo VR Device during build. (845179)</li>
<li>WebGL: Fixed crash when user writes a file using custom ArrayBuffer. (847853)</li>
<li>Windows Store: Fixed an issue in building with C# projects enabled when dependency existed between them. (847985)</li>
<li>Windows Store: Fixed duplicate assembly warning when building Universal 8.1. (822480)</li>
<li>Windows Store: Fixed problem where incorrect GUID was being used in generated .csproj files. (835538</li>
</ul>

#### Revision: 5a3967d8c55d
