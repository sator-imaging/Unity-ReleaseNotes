# Unity 4.7.0

https://unity3d.com/unity/whats-new/unity-4.7.0

## Improvements



*   Android: Added support for Marshmallow OS runtime permissions. Added possibility to disable permission dialog by adding activity metadata.
*   iOS/IL2CPP: Now allow null checks, array bounds checks, and divide by zero checks to be selectively included or omitted from generated C++ code by using a C# attribute on type, method, or property definitions.
*   iOS/IL2CPP: Enabled incremental build support using the "Append" option. Keep the generated code stable across additional, removal, and changes for string literals and non-generic types.
*   iOS/IL2CPP: Added support for the MethodImplOptions.NoInlining option to prevent methods in the generated C++ code from being inlined.