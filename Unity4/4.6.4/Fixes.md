# Unity 4.6.4

https://unity3d.com/unity/whats-new/unity-4.6.4

## Fixes



*   AI: Fixed potential hang when NavMesh connecting wrong side of thin polygons to neighbor tile.
*   Android: Fixed auto rotation, Input.acceleration and gyroscope when using Java activity.
*   Android: Fixed back button crash on some Samsung devices.
*   Android: Fixed checkjni exception when passing array in JNI at ART.
*   Android: Workaround for animation glitch with onscreen keyboard.
*   Asset Management: Show the path to the YAML meta file when there is an error reading it.
*   Editor: Android; fixed JDK detection when Java was in PATH.
*   Editor: Fixed scene view Show Mips visualization.
*   Editor: Fixed crash when undoing a prefab hierarchy change.
*   iOS: Added a fix for Unity runs out of memory while building large project (had to revert part of fix for 655473).
*   iOS: Fixed https failures in some cases.
*   iOS: Fixed iPad Mini 3rd gen detection.
*   iOS: Fixed on-screen keyboard not playing nicely with forced screen orientation.
*   iOS: Fixed splash screen issues in non-Pro mode.
*   iOS: Improved Xcode project parser robustness for invalid input.
*   iOS/IL2CPP: Added support for setting thread names on OS X.
*   iOS/IL2CPP: Added support for WebRequest to HTTPS addresses when using the Api Compatibility Level setting of .NET 2.0 Subset.
*   iOS/IL2CPP: Allow the LogInAsync method in the Parse SDK to work correctly.
*   iOS/IL2CPP: Always initialize type information before accessing static fields.
*   iOS/IL2CPP: Assembly.Load() now accepts assembly name in full name format.
*   iOS/IL2CPP: Corrected a number of problems related to WebRequest and ThreadPool interaction.
*   iOS/IL2CPP: Corrected a problem with Delegate.CreateDelegate.
*   iOS/IL2CPP: Corrected the C++ compiler error in generated code: "error: cast from pointer to smaller type 'il2cpp\_array\_size\_t' (aka 'int') loses information"
*   iOS/IL2CPP: Correctly write include definitions for an generic class with a const field.
*   iOS/IL2CPP: Emit the proper metadata for parameters static inflated generics methods.
*   iOS/IL2CPP: Explicitly declare generic types and array types that are created at run-time via Type.MakeGenericType and Type.MakeArrayType in the il2cpp\_extra\_types.txt file, so that IL2CPP will AOT compile them.
*   iOS/IL2CPP: Fixed a case where having throw statement at the end of a method would cause IL2CPP to crash.
*   iOS/IL2CPP: Fixed a problem with shift operators, resulting in problems with MD5 calculation, crypto, amongst other things.
*   iOS/IL2CPP: Fixed a queuing bug that might lead to WebRequests arriving at the same time and being used incorrectly.
*   iOS/IL2CPP: Fixed an issue that caused IL2CPP crash when passing null as value to array parameter in custom attribute constructor.
*   iOS/IL2CPP: Fixed array marshaling when passing an incorrect argument.
*   iOS/IL2CPP: Fixed Array.CopyTo() fast path, which was doing the wrong thing when the source array was a value type and destination array was not.
*   iOS/IL2CPP: Fixed C++ compile error in some cases when using fields with the same name in a class hierarchy.
*   iOS/IL2CPP: Fixed C++ linker error in some cases when using generic method constraints.
*   iOS/IL2CPP: Fixed C++ linker error in some cases when using generic parameters.
*   iOS/IL2CPP: Fixed code generation for delegates having parameters tagged with the Out attribute.
*   iOS/IL2CPP: Fixed conversion error in obscure edge case of method overrides through metadata and signature.
*   iOS/IL2CPP: Fixed crash when calling MethodInfo.ReturnTypeCustomAttributes.GetCustomAttributes on a constructor.
*   iOS/IL2CPP: Fixed crash when System.Console was included in link.xml.
*   iOS/IL2CPP: Fixed deadlock or timeouts when C# code does BeginInvoke+EndInvoke on a worker thread and the pool had only one thread.
*   iOS/IL2CPP: Fixed exceptions thrown while using System.Configuration.ApplicationSettingsBase.
*   iOS/IL2CPP: Fixed IL2CPP crash in some cases when using virtual generic methods.
*   iOS/IL2CPP: Fixed issue with String.Intern which was not always returning the correct string.
*   iOS/IL2CPP: Fixed List.FindAll().
*   iOS/IL2CPP: Fixed MethodInfo.GetBaseDefinition().
*   iOS/IL2CPP: Fixed networking RPC call registration not working on IL2CPP backend.
*   iOS/IL2CPP: Fixed null reference exception when calling TripleDES.Create.
*   iOS/IL2CPP: Fixed order of properties returned by Type.GetProperties().
*   iOS/IL2CPP: Fixed rare crash when calling Type.GetMethods.
*   iOS/IL2CPP: Fixed single core CPU system resulting in ThreadPool with no threads.
*   iOS/IL2CPP: Fixed WebRequests getting stuck in socket polling stage when the stage should be skipped.
*   iOS/IL2CPP: Fixed ParameterInfo.Attributes always returned ParameterAttributes.None for parameters.
*   iOS/IL2CPP: Fixed assert "pthread\_equal (pthread\_self (), m\_Handle) && 'Must be called on current thread!'".
*   iOS/IL2CPP: Fixed deadlock on shutdown if socket polling thread was still waiting for network traffic.
*   iOS/IL2CPP: Fixed deadlock when socket exits polling stage when I/O pool was at max capacity and worker threads were in wait state.
*   iOS/IL2CPP: Fixed race condition in static constructor calling.
*   iOS/IL2CPP: Fixed thread interruption logic incorrectly thinking that another thread was still waiting.
*   iOS/IL2CPP: Handle code generation for an struct which has an array of enums as a field.
*   iOS/IL2CPP: Handle IL code which uses one local variable as an array index more than once, with different values.
*   iOS/IL2CPP: Handle NULL const string values.
*   iOS/IL2CPP: Handle out and ref marshaling of a delegate with a struct that has no instance fields.
*   iOS/IL2CPP: Implement marshaling of the SafeHandle type.
*   iOS/IL2CPP: Implemented Assembly.GetName().
*   iOS/IL2CPP: Implemented Assembly.GlobalAssemblyCache so that is always returned false.
*   iOS/IL2CPP: Implemented marshaling of the System.Runtime.InteropServices.HandleRef type.
*   iOS/IL2CPP: Implemented marshaling support for explicit struct layouts.
*   iOS/IL2CPP: Implemented MethodBase.GetMethodFromHandle with two arguments for a non-generic type.
*   iOS/IL2CPP: Implemented missing Marshal.PtrToStructure overload which takes object reference.
*   iOS/IL2CPP: Implemented the use of SizeParamIndex for marshaling.
*   iOS/IL2CPP: Improved support for MakeGenericMethod.
*   iOS/IL2CPP: Now allow the ExternalCall method to be compiled using the IL2CPP scripting backend.
*   iOS/Metal: Fixed RenderTexture mipmap generation in cases of ReadPixels immediately after drawing.
*   Linux: Fixed an issue causing crash with native plugins using STL types.
*   Linux: Hide system cursor when using software cursor.
*   Oculus: Resolved Build Settings issue where Standalone players were not receiving the correct Build Settings when Oculus Plugin was present in project.
*   OpenGL ES 3: Fixed half-float render texture formats being set to "not supported" incorrectly.
*   Physics 2D: Fixed a behaviour issue in Box2D itself where non-dynamic/dynamic contacts always use continuous collision detection.
*   Physics 2D: Fixed inaccurate 2D OverlapArea, OverlapAreaAll & OverlapAreaNonAlloc query methods.
*   Physics 2D: Fixed incorrect calculation of fraction & distance using Physics2D BoxCast/CircleCast methods (and variants).
*   Physics 2D: OnJointBreak() will no longer have garbage passed in as the breaking force. Note that under Unity 4.6, it is not possible to report the actual force the joint was subject to when it broke; OnJointBreak will be passed the joint's configured maximum force. This behaviour is fixed in Unity 5 to report the actual force that broke the joint.
*   Scripting: Fixed C# compiler generating incorrect IL in some cases for iterator finally blocks.
*   Scripting: Fixed context menus on derived objects.
*   Scripting: Fixed infinite loop on error in GetAllNetworkInterfaces.
*   Stripping: Fixed the issue which was making stripping completely disabled for Mono scripting backend.
*   Serialization: Changed serialization of Materials and Ogg Vorbis audio streams to eliminate non-deterministic behaviour when building players and asset bundles.
*   Shadows: Fixed precision issues with large non-receiver objects in deferred rendering.
*   SpritePacker: Set SpriteAtlas textures as non-readable to lower memory consumption (sprite packer only considers non-readable sprites for packing anyway).
*   Substance: Fixed 'atom not found' error messages at link time when building for iOS in release or distribution mode with extra symbol stripping options.
*   UI: Fixed overriding/inheriting of pixel perfect status in child canvases.
*   Video: Fixed Theora movie playback skipping frames at beginning and general sync improvement.
*   Webplayer: Fixed Windows webplayer crash when requested window area was 0.
*   Webplayer: Pre-initialized OSX screen manager so that orthographic camera transforms could be initialized.
*   WebPlayer: Properly initialize multisampled OpenGL framebuffers.
*   Windows Phone 8: Modified MainPage.xaml.cs to account for devices that don't have hardware buttons.
*   Windows Phone/Windows Store Apps: Capabilities are now read correctly from manifest file.
*   Windows Phone/Windows Store Apps: SendMessage can now be called with Int64 value.
*   Windows Store Apps: Fixed VS solution generation with paths containing unicode characters.
*   Windows Store Apps: Increased timeout when checking assembly compatibility.
*   Windows Store Apps: Use exception log type for exceptions now.
*   Windows Store Apps/Windows 8.1: When creating D3D backbuffer, Unity will take width/height from SwapChainPanel component instead of CoreWindow, SwapChainPanel's offset from CoreWindow will also be taken into account.
*   Windows Store Apps/Windows Phone 8: Fixed a memory leak, which was occurring in various places. For e.g., in physics collision callbacks such as OnCollisionEnter(Collision collision).
*   Windows Store Apps/Windows Phone: Better error message when AssemblyConverter fails to resolve type.