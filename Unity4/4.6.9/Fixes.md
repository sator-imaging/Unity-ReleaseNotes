# Unity 4.6.9
https://unity3d.com/unity/whats-new/unity-4.6.9

## Fixes

<ul>
<li>(676381) -  AI: Fixed crash when navmesh polygon count exceeds internal maximum.</li>
<li>(661775) -  AI: Fixed occasional crash on selecting a NavMeshAgent in editor while Navigation window is open.</li>
<li>(none) -  Android: Fixed an issue where textures didn't load properly on Tegra devices.</li>
<li>(721346) -  Android: Fixed status bar not shown and touch offset when status bar was not hidden.</li>
<li>(703290) -  Asset Importing: Force script compilation to happen synchronously when the overall asset import process is happening synchronously too.</li>
<li>(704016) -  Editor: Made sure blendShapes normals were not imported if None was set in Import Setting.</li>
<li>(none) -  iOS: Added DeviceGeneration Enums for iPhone6S, iPhone6S Plus, iPad Pro 1st Generation, and iPad Mini 4th Generation.</li>
<li>(none) -  iOS: Disabled bitcode by default to work around build issues on Xcode 7.</li>
<li>(none) -  iOS: Enabled SSL for HWStats analytic reporting.</li>
<li>(none) -  iOS: Fixed crash while building iOS project on El Capitan.</li>
<li>(728134) -  iOS: Fixed Game Center authentication crash on iOS 9.0.</li>
<li>(718387), (720698) -  iOS: Fixed system dynamic font support on iOS 9 where only the first font could be read from certain font collections and font substitutes, as identified by the OS, were not handled.</li>
<li>(689461) -  iOS/IL2CPP: Added support for access default parameter values via reflection.</li>
<li>(731652) -  iOS/IL2CPP: Allow default parameter values for nullable types to be converted to C++ correctly.</li>
<li>(714759) -  iOS/IL2CPP: Allow WebRequest to work with IPv6 addresses.</li>
<li>(723439) -  iOS/IL2CPP: Correct C++ code generation when a struct inherits from a generic interface.</li>
<li>(730563) -  iOS/IL2CPP: Correct the generated C++ code when MonoPInvokeCallback is used to specify a type which has marshaling directives. The marshaling directives from that type will be used, and a compile error in the generated C++ code will no longer occur.</li>
<li>(705898) -  iOS/IL2CPP: Corrected a code generation error with the JsonFX library with the error message: "not implemented on non-abstract class".</li>
<li>(719084) -  iOS/IL2CPP: Corrected an error in the negation of a float converted from an unsigned integer.</li>
<li>(707376) -  iOS/IL2CPP: Ensure IL2CPP generates valid numeric identifiers under all system languages.</li>
<li>(719378) -  iOS/IL2CPP: Ensure PreserveAttribute on type preserves default constructor.</li>
<li>(732814) -  iOS/IL2CPP: Fixed a crash in the il2cpp::icalls::mscorlib::System::Reflection::MonoMethod::get_base_definition method.</li>
<li>(715965) -  iOS/IL2CPP: Fixed assert on socket error.</li>
<li>(703908) -  iOS/IL2CPP: Fixed Directory.GetFiles using search pattern with embedded '*'.</li>
<li>(712553) -  iOS/IL2CPP: Fixed error when using 64-bit Interlocked operations on 32-bit devices.</li>
<li>(716138) -  iOS/IL2CPP: Fixed pinning of structures with ExplicitLayout.</li>
<li>(721435) -  iOS/IL2CPP: Fixed reading pointers with multiple levels of indirection.</li>
<li>(718696) -  iOS/IL2CPP: Fixed unsafe pointer to struct assignment.</li>
<li>(718708) -  iOS/IL2CPP: Generate correct C++ code when an extension method as a constrained generic type which is another generic type defined in a different assembly.</li>
<li>(721329) -  iOS/IL2CPP: IL2CPP:&nbsp;Fixed various performance issues by doing less type initialization at startup.</li>
<li>(714759) -  iOS/IL2CPP: Implemented host name resolution with IPv6.</li>
<li>(700792) -  iOS/IL2CPP: Implemented the correct rounding behavior (banker's rounding) for the Math.Round method.</li>
<li>(717904) -  iOS/IL2CPP: Now allow a cast of T[] to IList (where BaseT is a base class of T) to work correctly.</li>
<li>(727395) -  iOS/IL2CPP: Prevent a crash in Application.LoadLevel now.</li>
<li>(722375) -  iOS/IL2CPP: Prevented a NullReferenceException exception from being thrown in the KeyValuePair ToString method when the value was a reference type.</li>
<li>(722433) -  iOS/IL2CPP: Prevented an used block from being marked as dead during conversion if it was immediately after a try block with an explicit leave opcode.</li>
<li>(715013) -  iOS/IL2CPP: Prevented the exception "MissingMethodException: No constructor found for System.Resources.RuntimeResourceSet::.ctor(System.IO.UnmanagedMemoryStream)" from occurring when the TZ4NET assembly was used.</li>
<li>(716991) -  iOS/IL2CPP: Speed up retrieving classes by name.</li>
<li>(none) -  Shaders: Fixed support for "framebuffer fetch" (mostly iOS) functionality on OpenGL ES 3.0 and Metal.</li>
<li>(none) -  UI: Fixed API breaking change where GetMousePointerEventData required a parameter.</li>
<li>(694380), (683346) -  Windows Phone 8.1: Fixed random hang, when application returned from suspend mode, for ex., when performing In App Purchase.</li>
<li>(717935) -  Windows Store Apps: Fixed audio on Windows 10.</li>
</ul>

#### Revision: 44099fd26189
