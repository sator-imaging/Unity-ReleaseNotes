# Unity 4.6.3
https://unity3d.com/unity/whats-new/unity-4.6.3

## iOS 64 bit / il2cpp fixes


#### A whole bunch of fixes were done for initial iOS 64 bit support (released in 4.6.2):
<ul>
<li>Break IL instruction is now a no-op instead of a crash.</li>
<li>Don't allow to select ARM64 architecture when using Mono scripting backend.</li>
<li>Don't include .NET metadata into the binary.</li>
<li>Ensure that the HideInInspector and ResourceRequest types are not stripped so they can be used if necessary.</li>
<li>Fixed an issue with Socket.Poll, where socket instances where not removed from the list if inactive.</li>
<li>Fixed Application.RequestUserAuthorization not working.</li>
<li>Fixed a problem with generic classes where the generic type argument lives in a different assembly from the type definition.</li>
<li>Fixed array of interfaces also being marked as interfaces.</li>
<li>Fixed Attribute.GetCustomAttribute crash.</li>
<li>Fixed C++ compile error for marshaled types.</li>
<li>Fixed C++ compile error for methods with two or more generic arguments of the same type.</li>
<li>Fixed C++ compile error when there's a struct array field in a marshalable struct that is marshaled as ByValArray.</li>
<li>Fixed C++ compile error when using Interlocked.CompareExchange/Exchange with null.</li>
<li>Fixed code generation for arrays of System.IntPtr, as well as IntPtr passed by reference.</li>
<li>Fixed code generation for generic methods with generic instance type constraints.</li>
<li>Fixed code generation for leave instructions jumping out of multiple exception handlers; fixes crash in Parse libraries.</li>
<li>Fixed code generation for unsafe structs with fixed fields.</li>
<li>Fixed crash in some cases when using ILeaderboard.</li>
<li>Fixed crash when calling GetCustomAttributes() and one of the methods happened to have a [DllImport] attribute.</li>
<li>Fixed CustomAttributes on constructors and method parameters.</li>
<li>Fixed deserialization of Dictionary.</li>
<li>Fixed Enum.IsDefined.</li>
<li>Fixed incorrect stripping in some cases when inheriting classes with interfaces.</li>
<li>Fixed issue with two dimensional arrays.</li>
<li>Fixed lock statement code generation when wrapping a try/catch statement.</li>
<li>Fixed memory corruption when using AssemblyName.</li>
<li>Fixed MethodInfo.ReturnParameter.</li>
<li>Fixed multiple Cryprography library issues.</li>
<li>Fixed RakNet being unavailable on IL2CPP, causing linker errors.</li>
<li>Fixed some race conditions in the low level threading primitives.</li>
<li>Fixed Type.GetNestedTypes() crash.</li>
<li>Fixed unsigned storage types for CustomAttributes.</li>
<li>Get the correct method to invoke via a delegate that points to an interface method.</li>
<li>Handle LdToken IL instruction correctly.</li>
<li>Handle non-ASCII characters in names.</li>
<li>Implemented dynamic library loading.</li>
<li>Implemented FieldInfo.GetRawConstantValue.</li>
<li>Implemented marshaling of fixed size strings as fields of structs and classes.</li>
<li>Implemented support for StructLayout and FieldOffset attributes in managed code, when not using for PInvoke.</li>
<li>iOS Internal profiler is now working on IL2CPP.</li>
<li>Make JsonFX library work with stripping.</li>
<li>Make reflection on constant fields work (with the exception of string, for which support is pending).</li>
<li>Never use microcorlib for iOS/IL2CPP.</li>
<li>Nullable now works correctly when being cast to/from object or T.</li>
<li>Prevented a duplicate symbol linker error for projects that use zlib in a static library by renaming the zlib symbols exported from the iOS/IL2CPP version of zlib.</li>
<li>Prevent the error "Cannot get stack type for Item" when "Item" is a type nested in a generic type.</li>
<li>Reduced the maximum depth to which IL2CPP tries to inflate generics. This fixed an issue which caused IL2CPP to never finish on certain C# patterns.</li>
<li>Runtime now attaches to native thread automatically if it's being called into from native code through reverse P/Invoke.</li>
<li>Support attributes that have arrays of System.Type arguments.</li>
</ul>
