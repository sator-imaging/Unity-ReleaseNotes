# Unity 4.6.3

https://unity3d.com/unity/whats-new/unity-4.6.3

## iOS 64 bit / il2cpp fixes



#### A whole bunch of fixes were done for initial iOS 64 bit support (released in 4.6.2):

*   Break IL instruction is now a no-op instead of a crash.
*   Don't allow to select ARM64 architecture when using Mono scripting backend.
*   Don't include .NET metadata into the binary.
*   Ensure that the HideInInspector and ResourceRequest types are not stripped so they can be used if necessary.
*   Fixed an issue with Socket.Poll, where socket instances where not removed from the list if inactive.
*   Fixed Application.RequestUserAuthorization not working.
*   Fixed a problem with generic classes where the generic type argument lives in a different assembly from the type definition.
*   Fixed array of interfaces also being marked as interfaces.
*   Fixed Attribute.GetCustomAttribute crash.
*   Fixed C++ compile error for marshaled types.
*   Fixed C++ compile error for methods with two or more generic arguments of the same type.
*   Fixed C++ compile error when there's a struct array field in a marshalable struct that is marshaled as ByValArray.
*   Fixed C++ compile error when using Interlocked.CompareExchange/Exchange with null.
*   Fixed code generation for arrays of System.IntPtr, as well as IntPtr passed by reference.
*   Fixed code generation for generic methods with generic instance type constraints.
*   Fixed code generation for leave instructions jumping out of multiple exception handlers; fixes crash in Parse libraries.
*   Fixed code generation for unsafe structs with fixed fields.
*   Fixed crash in some cases when using ILeaderboard.
*   Fixed crash when calling GetCustomAttributes() and one of the methods happened to have a \[DllImport\] attribute.
*   Fixed CustomAttributes on constructors and method parameters.
*   Fixed deserialization of Dictionary.
*   Fixed Enum.IsDefined.
*   Fixed incorrect stripping in some cases when inheriting classes with interfaces.
*   Fixed issue with two dimensional arrays.
*   Fixed lock statement code generation when wrapping a try/catch statement.
*   Fixed memory corruption when using AssemblyName.
*   Fixed MethodInfo.ReturnParameter.
*   Fixed multiple Cryprography library issues.
*   Fixed RakNet being unavailable on IL2CPP, causing linker errors.
*   Fixed some race conditions in the low level threading primitives.
*   Fixed Type.GetNestedTypes() crash.
*   Fixed unsigned storage types for CustomAttributes.
*   Get the correct method to invoke via a delegate that points to an interface method.
*   Handle LdToken IL instruction correctly.
*   Handle non-ASCII characters in names.
*   Implemented dynamic library loading.
*   Implemented FieldInfo.GetRawConstantValue.
*   Implemented marshaling of fixed size strings as fields of structs and classes.
*   Implemented support for StructLayout and FieldOffset attributes in managed code, when not using for PInvoke.
*   iOS Internal profiler is now working on IL2CPP.
*   Make JsonFX library work with stripping.
*   Make reflection on constant fields work (with the exception of string, for which support is pending).
*   Never use microcorlib for iOS/IL2CPP.
*   Nullable now works correctly when being cast to/from object or T.
*   Prevented a duplicate symbol linker error for projects that use zlib in a static library by renaming the zlib symbols exported from the iOS/IL2CPP version of zlib.
*   Prevent the error "Cannot get stack type for Item" when "Item" is a type nested in a generic type.
*   Reduced the maximum depth to which IL2CPP tries to inflate generics. This fixed an issue which caused IL2CPP to never finish on certain C# patterns.
*   Runtime now attaches to native thread automatically if it's being called into from native code through reverse P/Invoke.
*   Support attributes that have arrays of System.Type arguments.