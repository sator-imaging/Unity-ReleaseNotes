# Unity 4.7.0

https://unity3d.com/unity/whats-new/unity-4.7.0

## Fixes



*   Android: Buildpipe - Do not run dex if exporting the project (746248).
*   Android: Fixed NullReferenceException on x86 devices running Android 5.0 or newer.
*   Android: Fixed OBB deployment on Android 6.0 and some older devices (734408).
*   Android: Marshmallow - Fixed issues when querying for custom permissions (750227).
*   BlackBerry: Fixed crash that would happen with some projects on the Passport after consecutive runs (670282).
*   Editor: Prefab is being updated correctly in the Project View when Apply or GameObject/Apply Changes to Prefab is selected and Cache Server is enabled (702141, 662597).
*   GLES3: Fixed a crash on MSAA resolve to render texture (719502).
*   Graphics: Fixed crash when attempting to use dynamic batching with a mesh that has no vertices or indices (710447).
*   iOS: Added build & run support for Xcode 7.1 (739935).
*   iOS: Fixed a crash relating to GLES context management on iOS7 (677907).
*   iOS: Fixed a crash when attempting to batch empty meshes.
*   iOS: Fixed CRC check when using WWW.LoadFromCacheOrDownload(url, fileVersion, crc) (737503).
*   iOS: Fixed legacy launch screens on iOS 9.1.
*   iOS: Fixed simulator support on Xcode 7.1 (740343).
*   iOS: Fixed the keyboard input preview from not showing up in certain situations (724035).
*   iOS/IL2CPP: Avoid stack overflow crash due to large allocation with alloca (739685).
*   iOS/IL2CPP: Changed the conv.i8 opcode implementation to handle sign extension correctly so that a conversion from a large negative int to a uint to a long in C# works as expected (716811).
*   iOS/IL2CPP: Corrected the behavior of Array.SetValue and Array.GetValue for integer values used with an enum array (732205).
*   iOS/IL2CPP: Correctly initialize the metadata for default parameter values that are obtained via reflection (745793, 737565).
*   iOS/IL2CPP: Enabled profiling of GC allocations (735880).
*   iOS/IL2CPP: Fixed race condition during cleanup of thread pool threads (738232).
*   iOS/IL2CPP: Generate proper C++ code for a type with two fields that have the same type and name (735413).
*   iOS/IL2CPP: IL2CPP: Prevent a possible deadlock when using System.Threading.ReaderWriterLock (732317).
*   iOS/IL2CPP: Improved the error message when the byte code stripper is unable to locate an assembly (734534).
*   iOS/IL2CPP: Now allow the \[Preserve\] attribute to correctly prevent stripping of a method in a nested type (738356).
*   iOS/IL2CPP: Prevent a crash in the player in MetadataCache::GetTypeInfoFromTypeDefinitionIndex when a constrained call is made to a generic virtual method defined on a value type (737853).
*   iOS/IL2CPP: Prevent a KeyNotFoundException exception from occurring during code conversion when a generic method is used with at least one generic argument that exceeds the maximum generic recursion depth (730233).
*   iOS/IL2CPP: Prevent a memory leak that caused some GCHandles, including those used to reference MonoBehaviour instances, from being correctly reclaimed by the garbage collector (736167).
*   iOS/IL2CPP: Prevent a NullReferenceException exception from occurring during the processing of the Preserve attribute which can obscure the actual cause of a problem (717997).
*   iOS/IL2CPP: Prevent an intermittent hang with asynchronous sockets (718885).
*   iOS/IL2CPP: Prevent generated C++ code from including a header file that was not generated when the type which could have been generated in that header is used only in an attribute applied to an assembly (737996).
*   iOS/IL2CPP: Provide proper managed stack traces when the C++ compiler inlines method calls (739956).
*   iOS/IL2CPP: Set default stack size to 1MB to match Mono behavior (733799).
*   MacOSX Standalone: Fixed Fullscreen Window mode freeze on El Capitan (10.11) (737716).
*   Metal: Fixed shader translation of matrix+scalar, matrix-scalar, matrix/scalar operations (693714).
*   UI: Fixed issue that caused FontUpdateTracker to add an additional RebuildForFont handler whenever a Text component was enabled using a font with no other active Text components using that font (687059).
*   Windows 10: Fixed incorrect display of Korean characters on Windows 10 (if Korean language pack is not installed) and Windows Phone 10; Unity will now fallback to "Malgun Gothic" font (746437).
*   Windows: SystemInfo.operatingSystem returns correct value on Windows 10 machines now.
*   WWW: Fixed handling of filenames with non-latin characters (572394).

#### Revision: 9c73fd3cda99