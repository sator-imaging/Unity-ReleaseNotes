# Unity 4.6.5

https://unity3d.com/unity/whats-new/unity-4.6.5

## Fixes



*   Android: Apply Holo or Material theme explicitly instead of DeviceDefault.
*   Android: Apply user theme if set.
*   Android: Fixed Auto target graphics mode on devices which think they support ES 3.0 without proper hardware.
*   Android: Fixed crash in Mono caused by invocation of wrong method.
*   Audio: Fixed the "Disable Audio" option; the flag is now correctly used by the standalone player to disable the audio system.
*   Editor: Fixed Camera.SetTargetBuffers with AA-ed renderbuffers.
*   Graphics: Fixed OpenGL vertex attribute state tracking issue with multithreading.
*   IMGUI: Fixed calculation of TextGenerator vertices position when lineSpacing is 0.
*   iOS: Added Xcode 6.2 compatibility.
*   iOS: Fixed memory corruption and crash initiated by calling WebCamTexture.Stop().
*   iOS: Fixed WebCamTexture.didUpdateThisFrame.
*   iOS/Android: Fixed a crash with MSAA depth render textures.
*   iOS/IL2CPP: Added a null terminator to string arrays when they were marshaled.
*   iOS/IL2CPP: Additional code size improvements from generic sharing:
    *   Allow partial sharing (e.g. Dictionary is shared with Dictionary).
    *   Allow sharing when the type parameter constraint is an interface.
    *   Share enums and their base types as generic parameters.
*   iOS/IL2CPP: Allow il2cpp.exe to work correctly if there is a space in the installation path.
*   iOS/IL2CPP: Allow thread-local static fields to work correctly in generic classes. Specifically, this corrects the Parse SDK crash in 4.6.4p1.
*   iOS/IL2CPP: AudioMixerSnapshot.TranslateTo no longer throws null reference exception on IL2CPP.
*   iOS/IL2CPP: Cast non-pointer references types to System.Object for comparison in conditional statements.
*   iOS/IL2CPP: Corrected an InvalidCastException that can occur when setting an array value.
*   iOS/IL2CPP: Corrected the behavior of CultureInfo.CreateSpecificCulture.
*   iOS/IL2CPP: Now do not write extern declarations inside p/invoke wrappers for methods that return a class or delegate.
*   iOS/IL2CPP: Fixed an infinite recursion when constructing generic type.
*   iOS/IL2CPP: Fixed Interlocked.Exchange and Interlocked.CompareExchange for interfaces.
*   iOS/IL2CPP: Fixed an issue with managed exceptions not being thrown by a method called by Method.Invoke in some cases.
*   iOS/IL2CPP: Fixed multidimensional array interfaces.
*   iOS/IL2CPP: Fixed overflow arithmetic instruction handling.
*   iOS/IL2CPP: Fixed a crash with StrangeIOC.
*   iOS/IL2CPP: Fixed a number of problems related to WebRequest and asynchronous I/O:
    *   Fixed race condition in Monitor code that lead to 5 second stalls in Monitor.Exit().
    *   Fixed socket I/O requests getting stuck in ThreadPool on POSIX/iOS.
    *   Fixed ThreadPool not re-using idle worker threads (lead to potentially very high memory consumption and bad performance).
    *   Fixed ThreadPool upper thread count limits being very low; now roughly the same as on Mono.
    *   Fixed ThreadPool.SetMinThreads() and SetMaxThreads() having no effect.
*   iOS/IL2CPP: Fixed an issue with open delegates that returned void.
*   iOS/IL2CPP: Fixed code generation for unsafe fixed arrays.
*   iOS/IL2CPP: Fixed crash in some cases when accessing an enum inside a generic class.
*   iOS/IL2CPP: Fixed crash related to arrays of Enums on 64-bit.
*   iOS/IL2CPP: Fixed crash related to arrays of Enums on 64-bit.
*   iOS/IL2CPP: Fixed crashes in socket code due to sockets being destroyed too early and prevent Thread.IsAlive from returning true after thread has terminated.
*   iOS/IL2CPP: Fixed File::Replace when destinationBackupFileName is null.
*   iOS/IL2CPP: Fixed IL2CPP failure to convert an assembly which contained Ldtoken instruction on field that was declared in a generic type. This issue affected CSVHelper.dll plugin.
*   iOS/IL2CPP: Fixed issues with exception thrown from DateTime constructor, DateTime ToUniversalTime, DateTime ToLocalTime, DateTime IsDaylightSavingTime.
*   iOS/IL2CPP: Fixed occasional code generation issues when multiple local enum variables are used in conditional expressions.
*   iOS/IL2CPP: Fixed support for enums nested in generic types.
*   iOS/IL2CPP: Fixed support for type/method names using non ASCII characters.
*   iOS/IL2CPP: Fixed TerrainData.GetAlphaMaps crashing on IL2CPP.
*   iOS/IL2CPP: Forward declare empty types (created to end infinite recursion) that are used as method arguments.
*   iOS/IL2CPP: Generate C++ code which will compile when a nested generic passes the maximum depth for recursive nested generics.
*   iOS/IL2CPP: Handle 4D arrays.
*   iOS/IL2CPP: Handle custom attributes with generic types and arrays of generic types.
*   iOS/IL2CPP: Handle delegate invoke with nested delegates where the method which is invoked on the outer delegate is a static method.
*   iOS/IL2CPP: Implemented Assembly.CodeBase by returning the value of AssemblyName.Name.
*   iOS/IL2CPP: Make Activator.CreateInstance work for arrays.
*   iOS/IL2CPP: Match the behavior of the Mono scripting backend by not stripping the Animation code from the engine when code stripping is enabled.
*   iOS/IL2CPP: Match the Mono behavior which allows inflated generic delegate types like System.Action to be marshaled as normal delegates.
*   iOS/IL2CPP: Now allow Encoding.GetEncoding to correctly.
*   iOS/IL2CPP: Now support Type.MakeGenericType for runtime creation of generic types where the generic arguments are reference types.
*   iOS/IL2CPP: Prevent a stack overflow in il2cpp.exe when it converts have an infinitely recursive generic type with an array generic argument.
*   iOS/IL2CPP: Return the correct number of write and error sockets from the Socket::Select method.
*   iOS/IL2CPP: Type.GetType throws an ArgumentException now when the provided type name was wrong.
*   iOS/IL2CPP: Use the proper type for the result of the IL sub opcode.
*   iOS/IL2CPP: Use the Size field of the StructLayout attribute to pad marshaled types if necessary. This allows Marshal.SizeOf to return the correct value for these types.
*   iOS/ILCPP: Do not emit metadata for generic types at compile time. This significantly decreases the size of the final binary in most cases.
*   iOS/Metal: Fixed crash in WarmupAllShaders when called in update with AA-ed backbuffer.
*   iOS/Metal: Fixed MSAA+post effects interop (MSAA RT was forcibly resolved after opaque geometry, even when no after-opaque image filters were present).
*   iOS/Metal: Fixed WebCamTexture.videoVerticallyMirrored.
*   Mecanim: Fixed different behaviours of negative scale of animations in 4.5 and 4.6.
*   Mecanim: Fixed FBX import not supporting both blend shapes and boned animation in the same file by upgrading FBX SDK to 2015.
*   Networking: Added a connection timeout to prevent hangs when the network speed is extremely slow.
*   Networking: Skip proxy check when using the "file://" protocol on Windows.
*   OSX Editor: Avoid App Nap mode in editor's batch mode, so build performance doesn't degrade.
*   Physics 2D: Fixed missing contacts when performing either 2D Box/Circle-cast methods.
*   Physics 2D: 2D physics will now give deterministic results on the same device when entering play-mode in the editor.
*   Physics 2D: Ensure that when recreating the Box2D world that we reinstate the gravity setting and not use the default.
*   Rendering: Fixed crash when reading font's metadata for a font without style info.
*   Rendering: Now the back buffer is cleared after the resolution is changed from a script in Windows standalone.
*   Scripting: Allow a component which derives from a type in UnityEngine.UI and is built in a custom assembly to be used in the project.
*   Serialization: Reapplied part of non-deterministic material serialization fix, but without increasing memory usage during building.
*   Shaders: Fixed loop generation (GLSL/Metal).
*   Shaders: Fixed vector\_insert\_TODO appearing in some shaders (GLSL/Metal).
*   UI: Caret on InputField now blinks at proper frequency.
*   UI: Clamp setting canvas group alpha between 0-1 on API call.
*   UI: Destroying a RectTransform that is queued to for a layout rebuild would freeze unity.
*   UI: Fixed a bug where multiple Layout Group components on the same GameObject were not prevented even though it was not supported.
*   UI: Fixed an issue where the pointer click world position/normal might not be properly associated with the event if multiple modules or hits were present.
*   UI: Fixed bug which caused caret to no longer appear in InputField after game object was deactivated and reactivated.
*   UI: Fixed division by zero bug in GridLayoutGroup.
*   UI: Fixed events being blocked by disabled UI elements.
*   UI: Fixed instantiating a prefab containing a Selectables will not throw console errors.
*   UI: Fixed Mac-only crash during Canvas sorting.
*   UI: Fixed nested masking not getting the correct stencil value and failing.
*   UI: Only do cut, copy, paste, and select all if holding down just Ctrl (Cmd on Mac), not if additional modifier keys are also held down. This prevents these actions from happening when intending to type characters that use Ctrl (Cmd on Mac) as part of the key combination.
*   UI: Prevent out of range exception that happened in InputField under certain circumstances due to an unwanted recursive call.
*   UI: UI items now work with Scene View searching.
*   WebPlayer: Fix crash when when elementType was queried from uninitialized elementClass.
*   Windows Phone 8: Uppercase first letter in InputField.
*   Windows Store Apps: Build&Run disabled when using Unity CSharp projects.
*   Windows Store Apps: Fixed problems with build from editor when C# projects are enabled.
*   Windows Store Apps: Fixed deadlock when resizing window.
*   Windows Store Apps: Mouse presence now is detected by mouse activity, which is much more reliable.
*   Windows Store Apps:Touch position will be correctly transformed when SwapChainPanel doesn't occupy full screen.
*   Windows Store Apps/Windows Phone 8: When unloading unused assets or switching to another scene, prefabs will be correctly reloaded and won't loose references. Previous behavior was - sometimes textures, mono behaviors, etc in prefabs would be lost, this would result for e.g., in textures not showing up in objects instantiated from prefabs.
*   Windows Store Apps/Windows Phone: Fixed NullReferenceException in SerializationWeaver.
*   WWW: Fixed incorrect HTTP status 100 when POST data was relatively large.