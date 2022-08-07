# Unity 5.0.4
https://unity3d.com/unity/whats-new/unity-5.0.4

## Fixes

<ul>
<li>(none) -  Android:  Fixed an issue whereby unaligned access caused a crash on Tegra K1.</li>
<li>(691217) -  GLES: Fixed crash on Vivante GPUs when using binary shaders.</li>
<li>(699694) -  GLES: Fixed crash when using multithreaded renderer and using shader that uses vertex colors when the mesh data doesn't contain vertex colors.</li>
<li>(none) -  Graphics: Configurable vertex compression to fix lightmap UVs shifting.</li>
<li>(700474) -  Graphics: Fixed issue when loading single channel JPEGs using Texture2D.LoadImage.</li>
<li>(691599) -  Inspector: Fixed NullReferenceException caused by deleting objects during Inspector redraw.</li>
<li>(685439) -  iOS: Fixed an issue whereby lightmapped objects with legacy shaders lit with realtime light in legacy deferred no longer render incorrectly.</li>
<li>(695118), (701548) -  iOS/IL2CPP: Add support for PreserveAttribute to prevent classes, methods, fields and properties from being stripped in IL2CPP.</li>
<li>(700507) -  iOS/IL2CPP:&nbsp;Avoid deadlock during UnloadUnusedAssets.</li>
<li>(691607), (667147) -  iOS/IL2CPP: Correct an exception during code conversion which has the error message "Invalid global variables count" when converting some UnityScript assemblies.</li>
<li>(698060) -  iOS/IL2CPP: Corrected an error in generated code when a constrained generic parameter type is used in a nested lambda expression.</li>
<li>(698589) -  iOS/IL2CPP: Corrected RPC implementation for the UnityEngine.Networking namespace.</li>
<li>(704018) -  iOS/IL2CPP: Ensure that GetCurrentMethod returns the proper value, even when the generated native method is inlined.</li>
<li>(695179) -  iOS/IL2CPP: Fixed a crash which occurred when Ldvirtftn opcode was used on a non-virtual method.</li>
<li>(691404) -  iOS/IL2CPP:&nbsp;Fixed a rare case when bytecode stripper would incorrectly strip wrong overloaded generic virtual method.</li>
<li>(694535) -  iOS/IL2CPP:&nbsp;Fixed an issue which sometimes caused IL2CPP to not call static constructors when Unity created class instances from native code.</li>
<li>(696986) -  iOS/IL2CPP: Fixed ConstructorInfo.Invoke() returning null for Nullable types.</li>
<li>(694436) -  iOS/IL2CPP: Fixed IL2CPP generated code in if (...) block if the condition operand was an IntPtr.</li>
<li>(694436) -  iOS/IL2CPP: Fixed IL2CPP generated marshaling code for marshaling IntPtr into any other primitive type.693316</li>
<li>(673249) -  iOS/IL2CPP: Fixed managed stack traces.</li>
<li>(702879) -  iOS/IL2CPP: Fixed marshaling arrays of structs marked with [Out] attribute.</li>
<li>(697563) -  iOS/IL2CPP: Generate correct C++ code for a generic virtual method which returns an IEnumerator and has a generic constraint defined on the method it overrides.</li>
<li>(696187) -  iOS/IL2CPP: Pr700531event a C++ compiler error in generated code about an undeclared identifier with the test "Unused local just for stack balance".</li>
<li>(702696) -  iOS/IL2CPP: Prevent a runtime exception with IL code in an enumerator's MoveNext method when the enumerator's return type is a constrained generic type.</li>
<li>(703294) -  iOS/IL2CPP: Prevent an exception during code generation when the default value of a field is not the same type as the field.</li>
<li>(704069) -  iOS/IL2CPP: Prevent the player build process from using older generated C++ source files from a previous build.</li>
<li>(691008) -  iOS/IL2CPP: When compiling scripts for the player, appropriate UnityEngine.UI.dll will be referenced.</li>
<li>(671681) -  Lighting: Fixed inaccurate screenspace scissoring of lights with large range.</li>
<li>(none) - Mono: Double traverse object count to avoid stack overflow when freeing huge amounts of objects. </li>
<li>(none) -  Windows Store Apps: Fixed a rare crash at boot when reading AppxManifest.xml.</li>
<li>(690152) -  Xbox One: Fixed a bug that could cause game chat to fail when more than two players are involved.</li>
<li>(none) - Xbox One: Mono: Double traverse object count to avoid stack overflow when freeing huge amounts of objects.</li>
</ul>
