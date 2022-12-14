# Unity 4.6.7

https://unity3d.com/unity/whats-new/unity-4.6.7

## Fixes



*   (none) - Android: Fixed readback from backbuffer into RenderTexture with incompatible color formats.
*   (695889) - FBX: Upgraded to FBX SDK 2015.1.
*   (690295) - Graphics: Fix for asset bundle content changes between subsequent generations due to uninitialised vertex buffer data.
*   (689087) - iOS: Added a limit for iOS acceleration event queue.
*   (681384) - iOS: Added additional Japanese fallback font.
*   (699574) - iOS: Added iOS Thai font for 8.2.
*   (701425) - iOS: Added support for Xcode 6.3.2 and Xcode 7 beta.
*   (705241) - iOS: Don't add header files to IL2CPP Xcode project.
*   (705208) - iOS: Fixed font metadata caching.
*   (669728) - iOS: Fixed hang when exiting minimal controls mode while playing fullscreen movie.
*   (698720) - iOS: Fixed IL2CPP project append.
*   (687297) - iOS: Fixed Watchkit extensions build.
*   (695118), (701548) - iOS/IL2CPP: Added support for PreserveAttribute to prevent classes, methods, fields and properties from being stripped in IL2CPP.
*   (700507) - iOS/IL2CPP: Avoid deadlock during UnloadUnusedAssets.
*   (698060) - iOS/IL2CPP: Correct an error in generated code when a constrained generic parameter type was used in a nested lambda expression.
*   (698589) - iOS/IL2CPP: Correct RPC implementation for the UnityEngine.Networking namespace.
*   (691607), (667147) - iOS/IL2CPP: Corrected an exception during code conversion which had the error message "Invalid global variables count" when converting some UnityScript assemblies.
*   (704018) - iOS/IL2CPP: Ensure that GetCurrentMethod returns the proper value, even when the generated native method is inlined.
*   (695179) - iOS/IL2CPP: Fixed a crash which occurs when Ldvirtftn opcode is used on a non-virtual method.
*   (691404) - iOS/IL2CPP: Fixed a rare case when bytecode stripper would incorrectly strip wrong overloaded generic virtual method.
*   (694535) - iOS/IL2CPP: Fixed an issue which sometimes caused IL2CPP to not call static constructors when Unity created class instances from native code.
*   (696986) - iOS/IL2CPP: Fixed ConstructorInfo.Invoke() returning null for Nullable types.
*   (694436) - iOS/IL2CPP: Fixed generated code in if (...) block if the condition operand was an IntPtr.
*   (694436) - iOS/IL2CPP: Fixed generated marshaling code for marshaling IntPtr into any other primitive type.
*   (673249) - iOS/IL2CPP: Fixed managed stack traces.
*   (702879) - iOS/IL2CPP: Fixed marshaling arrays of structs marked with \[Out\] attribute.
*   (697563) - iOS/IL2CPP: Generate correct C++ code for a generic virtual method which returns an IEnumerator and has a generic constraint defined on the method it overrides.
*   (696187) - iOS/IL2CPP: Prevent a C++ compiler error in generated code about an undeclared identifier with the test "Unused local just for stack balance".
*   (691077) - iOS/IL2CPP: Prevent a crash in the NetworkManager initialization when the Stripping Level option is not set to Disabled.
*   (702696) - iOS/IL2CPP: Prevent a runtime exception with IL code in an enumerator's MoveNext method when the enumerator's return type is a constrained generic type.
*   (703294) - iOS/IL2CPP: Prevent an exception during code generation when the default value of a field is not the same type as the field.
*   (697757) - iOS/IL2CPP: Prevent the exception: "System.ArgumentException: enumType is not an Enum type." from occurring for a generic type used with an enum type argument.
*   (704069) - iOS/IL2CPP: Prevent the player build process from using older generated C++ source files from a previous build.
*   (694840) - iOS/IL2CPP: Propagate managed exceptions which occur in the GUIWindow OnGUI method properly.
*   (700533) - MonoDevelop: Fixed issue with Attach button in attach to process dialog not responding to clicks.
*   (691008) - UI: When compiling scripts for the player, appropriate UnityEngine.UI.dll will be referenced now.
*   (673152) - UI: Fixed value of InputField.text when another field is being edited.
*   (689600) - UI: Number of rendering batches created for UI scene are back down to 4.6.4 number.
*   (694769) - WebPlayer: Fixed bad scaling in UI (regression).