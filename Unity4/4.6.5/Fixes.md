# Unity 4.6.5
https://unity3d.com/unity/whats-new/unity-4.6.5

## Fixes

<ul>
<li>Android: Apply Holo or Material theme explicitly instead of DeviceDefault.</li>
<li>Android: Apply user theme if set.</li>
<li>Android: Fixed Auto target graphics mode on devices which think they support ES 3.0 without proper hardware.</li>
<li>Android: Fixed crash in Mono caused by invocation of wrong method.</li>
<li>Audio:&nbsp;Fixed the "Disable Audio" option; the flag is now correctly used by the standalone player to disable the audio system.</li>
<li>Editor: Fixed Camera.SetTargetBuffers with AA-ed renderbuffers.</li>
<li>Graphics: Fixed OpenGL vertex attribute state tracking issue with multithreading.</li>
<li>IMGUI: Fixed calculation of TextGenerator vertices position when lineSpacing is 0.</li>
<li>iOS: Added Xcode 6.2 compatibility.</li>
<li>iOS: Fixed memory corruption and crash initiated by calling WebCamTexture.Stop().</li>
<li>iOS: Fixed WebCamTexture.didUpdateThisFrame.</li>
<li>iOS/Android: Fixed a crash with MSAA depth render textures.</li>
<li>iOS/IL2CPP: Added a null terminator to string arrays when they were marshaled.</li>
<li>iOS/IL2CPP: Additional code size improvements from generic sharing: 
<ul>
<li>Allow partial sharing (e.g. Dictionary is shared with Dictionary).</li>
<li>Allow sharing when the type parameter constraint is an interface.</li>
<li>Share enums and their base types as generic parameters.</li>
</ul></li>
<li>iOS/IL2CPP: Allow il2cpp.exe to work correctly if there is a space in the installation path.</li>
<li>iOS/IL2CPP: Allow thread-local static fields to work correctly in generic classes. Specifically, this corrects the Parse SDK crash in 4.6.4p1.</li>
<li>iOS/IL2CPP: AudioMixerSnapshot.TranslateTo no longer throws null reference exception on IL2CPP.</li>
<li>iOS/IL2CPP: Cast non-pointer references types to System.Object for comparison in conditional statements.</li>
<li>iOS/IL2CPP: Corrected an InvalidCastException that can occur when setting an array value.</li>
<li>iOS/IL2CPP: Corrected the behavior of CultureInfo.CreateSpecificCulture.</li>
<li>iOS/IL2CPP: Now do not write extern declarations inside p/invoke wrappers for methods that return a class or delegate.</li>
<li>iOS/IL2CPP: Fixed an infinite recursion when constructing generic type.</li>
<li>iOS/IL2CPP: Fixed Interlocked.Exchange and Interlocked.CompareExchange for interfaces.</li>
<li>iOS/IL2CPP: Fixed an issue with managed exceptions not being thrown by a method called by Method.Invoke in some cases.</li>
<li>iOS/IL2CPP: Fixed multidimensional array interfaces.</li>
<li>iOS/IL2CPP:&nbsp;Fixed overflow arithmetic instruction handling.</li>
<li>iOS/IL2CPP: Fixed a crash with StrangeIOC.</li>
<li>iOS/IL2CPP: Fixed a number of problems related to WebRequest and asynchronous I/O: 
<ul>
<li>Fixed race condition in Monitor code that lead to 5 second stalls in Monitor.Exit().</li>
<li>Fixed socket I/O requests getting stuck in ThreadPool on POSIX/iOS.</li>
<li>Fixed ThreadPool not re-using idle worker threads (lead to potentially very high memory consumption and bad performance).</li>
<li>Fixed ThreadPool upper thread count limits being very low; now roughly the same as on Mono.</li>
<li>Fixed ThreadPool.SetMinThreads() and SetMaxThreads() having no effect.</li>
</ul></li>
<li>iOS/IL2CPP: Fixed an issue with open delegates that returned void.</li>
<li>iOS/IL2CPP: Fixed code generation for unsafe fixed arrays.</li>
<li>iOS/IL2CPP: Fixed crash in some cases when accessing an enum inside a generic class.</li>
<li>iOS/IL2CPP: Fixed crash related to arrays of Enums on 64-bit.</li>
<li>iOS/IL2CPP: Fixed crash related to arrays of Enums on 64-bit.</li>
<li>iOS/IL2CPP: Fixed crashes in socket code due to sockets being destroyed too early and prevent Thread.IsAlive from returning true after thread has terminated.</li>
<li>iOS/IL2CPP: Fixed File::Replace when destinationBackupFileName is null.</li>
<li>iOS/IL2CPP: Fixed IL2CPP failure to convert an assembly which contained Ldtoken instruction on field that was declared in a generic type. This issue affected CSVHelper.dll plugin.</li>
<li>iOS/IL2CPP: Fixed issues with exception thrown from DateTime constructor, DateTime ToUniversalTime, DateTime ToLocalTime, DateTime IsDaylightSavingTime.</li>
<li>iOS/IL2CPP: Fixed occasional code generation issues when multiple local enum variables are used in conditional expressions.</li>
<li>iOS/IL2CPP: Fixed support for enums nested in generic types.</li>
<li>iOS/IL2CPP: Fixed support for type/method names using non ASCII characters.</li>
<li>iOS/IL2CPP: Fixed TerrainData.GetAlphaMaps crashing on IL2CPP.</li>
<li>iOS/IL2CPP: Forward declare empty types (created to end infinite recursion) that are used as method arguments.</li>
<li>iOS/IL2CPP: Generate C++ code which will compile when a nested generic passes the maximum depth for recursive nested generics.</li>
<li>iOS/IL2CPP: Handle 4D arrays.</li>
<li>iOS/IL2CPP: Handle custom attributes with generic types and arrays of generic types.</li>
<li>iOS/IL2CPP: Handle delegate invoke with nested delegates where the method which is invoked on the outer delegate is a static method.</li>
<li>iOS/IL2CPP:&nbsp;Implemented Assembly.CodeBase by returning the value of AssemblyName.Name.</li>
<li>iOS/IL2CPP: Make Activator.CreateInstance work for arrays.</li>
<li>iOS/IL2CPP: Match the behavior of the Mono scripting backend by not stripping the Animation code from the engine when code stripping is enabled.</li>
<li>iOS/IL2CPP: Match the Mono behavior which allows inflated generic delegate types like System.Action to be marshaled as normal delegates.</li>
<li>iOS/IL2CPP: Now allow Encoding.GetEncoding to correctly.</li>
<li>iOS/IL2CPP: Now support Type.MakeGenericType for runtime creation of generic types where the generic arguments are reference types.</li>
<li>iOS/IL2CPP: Prevent a stack overflow in il2cpp.exe when it converts have an infinitely recursive generic type with an array generic argument.</li>
<li>iOS/IL2CPP: Return the correct number of write and error sockets from the Socket::Select method.</li>
<li>iOS/IL2CPP: Type.GetType throws an ArgumentException now when the provided type name was wrong.</li>
<li>iOS/IL2CPP: Use the proper type for the result of the IL sub opcode.</li>
<li>iOS/IL2CPP: Use the Size field of the StructLayout attribute to pad marshaled types if necessary. This allows Marshal.SizeOf to return the correct value for these types.</li>
<li>iOS/ILCPP: Do not emit metadata for generic types at compile time. This significantly decreases the size of the final binary in most cases.</li>
<li>iOS/Metal: Fixed crash in WarmupAllShaders when called in update with AA-ed backbuffer.</li>
<li>iOS/Metal: Fixed MSAA+post effects interop (MSAA RT was forcibly resolved after opaque geometry, even when no after-opaque image filters were present).</li>
<li>iOS/Metal: Fixed WebCamTexture.videoVerticallyMirrored.</li>
<li>Mecanim: Fixed different behaviours of negative scale of animations in 4.5 and 4.6.</li>
<li>Mecanim: Fixed FBX import not supporting both blend shapes and boned animation in the same file by upgrading FBX SDK to 2015.</li>
<li>Networking: Added a connection timeout to prevent hangs when the network speed is extremely slow.</li>
<li>Networking: Skip proxy check when using the "file://" protocol on Windows.</li>
<li>OSX Editor: Avoid App Nap mode in editor's batch mode, so build performance doesn't degrade.</li>
<li>Physics 2D: Fixed missing contacts when performing either 2D Box/Circle-cast methods.</li>
<li>Physics 2D: 2D physics will now give deterministic results on the same device when entering play-mode in the editor.</li>
<li>Physics 2D: Ensure that when recreating the Box2D world that we reinstate the gravity setting and not use the default.</li>
<li>Rendering: Fixed crash when reading font's metadata for a font without style info.</li>
<li>Rendering: Now the back buffer is cleared after the resolution is changed from a script in&nbsp;Windows standalone.</li>
<li>Scripting: Allow a component which derives from a type in UnityEngine.UI and is built in a custom assembly to be used in the project.</li>
<li>Serialization: Reapplied part of non-deterministic material serialization fix, but without increasing memory usage during building.</li>
<li>Shaders: Fixed loop generation (GLSL/Metal).</li>
<li>Shaders: Fixed vector_insert_TODO appearing in some shaders (GLSL/Metal).</li>
<li>UI: Caret on InputField now blinks at proper frequency.</li>
<li>UI: Clamp setting canvas group alpha between 0-1 on API call.</li>
<li>UI: Destroying a RectTransform that is queued to for a layout rebuild would freeze unity.</li>
<li>UI: Fixed a bug where multiple Layout Group components on the same GameObject were not prevented even though it was not supported.</li>
<li>UI: Fixed an issue where the pointer click world position/normal might not be properly associated with the event if multiple modules or hits were present.</li>
<li>UI: Fixed bug which caused caret to no longer appear in InputField after game object was deactivated and reactivated.</li>
<li>UI: Fixed division by zero bug in GridLayoutGroup.</li>
<li>UI: Fixed events being blocked by disabled UI elements.</li>
<li>UI: Fixed instantiating a prefab containing a Selectables will not throw console errors.</li>
<li>UI: Fixed Mac-only crash during Canvas sorting.</li>
<li>UI: Fixed nested masking not getting the correct stencil value and failing.</li>
<li>UI: Only do cut, copy, paste, and select all if holding down just Ctrl (Cmd on Mac), not if additional modifier keys are also held down. This prevents these actions from happening when intending to type characters that use Ctrl (Cmd on Mac) as part of the key combination.</li>
<li>UI: Prevent out of range exception that happened in InputField under certain circumstances due to an unwanted recursive call.</li>
<li>UI: UI items now work with Scene View searching.</li>
<li>WebPlayer: Fix crash when when elementType was queried from uninitialized elementClass.</li>
<li>Windows Phone 8: Uppercase first letter in InputField.</li>
<li>Windows Store Apps: Build&amp;Run disabled when using Unity CSharp projects.</li>
<li>Windows Store Apps: Fixed problems with build from editor when C# projects are enabled.</li>
<li>Windows Store Apps: Fixed deadlock when resizing window.</li>
<li>Windows Store Apps: Mouse presence now is detected by mouse activity, which is much more reliable.</li>
<li>Windows Store Apps:Touch position will be correctly transformed when SwapChainPanel doesn't occupy full screen.</li>
<li>Windows Store Apps/Windows Phone 8: When unloading unused assets or switching to another scene, prefabs will be correctly reloaded and won't loose references. Previous behavior was - sometimes textures, mono behaviors, etc in prefabs would be lost, this would result for e.g., in textures not showing up in objects instantiated from prefabs.</li>
<li>Windows Store Apps/Windows Phone: Fixed NullReferenceException in SerializationWeaver.</li>
<li>WWW: Fixed&nbsp;incorrect HTTP status 100 when POST data was relatively large.</li>
</ul>
