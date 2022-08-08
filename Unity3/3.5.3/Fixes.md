# Unity 3.5.3

https://unity3d.com/unity/whats-new/unity-3.5.3

## Fixes



#### Unity for Native Client has been updated to a new version of the NaCl SDK, which fixes some problems. Shipping NaCl games need to be rebuilt with Unity 3.5.3, as they will no longer work in future versions of Google Chrome otherwise!

*   Android: JDK 7 installations are now automatically detected on windows.
*   Android: Reading player preferences using the wrong value type now return the default value.
*   Android: Fixed a rare race-condition when quitting the application.
*   Android: Added support for gdbserver being packaged inside the application.
*   Android: Use of spaces in keystore alias/password is now allowed.
*   Android: Added better failure message when the wrong key password is provided.
*   Android: Force SHA1 digest algorithm when signing the application, to make sure it's accepted by Google Play Store.
*   Android: Force RSA key algorithm when creating keys, as suggested by Google.
*   Android: Workaround for the bug with Kindle's compositor where it incorrectly uses the alpha values from the Display Buffer.
*   Android: Added warning for shaders which compilation might cause crash on sgs2 updated to ics.
*   Android: Fixed returning from pause on Eclair devices -Android: fixed perf regression with batching/dynamic geometry on PowerVR GPUs.
*   Cache Server: Fixed problem where native assets (prefabs, materials, etc) would not refresh in the Editor when updated on disk and cache server is active.
*   Editor: Rotation doesn't create leftover animation curves anymore
*   Editor: Fixed "Deprecated EditorExtensionImpl" assets show up in projects converted from Unity 3.4
*   Editor: Fixed crash when selecting multiple ScriptableAssets of different types.
*   Editor: Fixed up serialized property error that causes a null ref when an array is the last element being drawn.
*   Editor: Fixed up asset labels so that they get saved to meta data and displayed in the inspector properly.
*   Editor: Correctly clear drag and drop buffer so that old data does not stay around causing issues.
*   Editor: Fixed wrong gizmo rendering on Windows with extremely high quad counts (e.g. drawing 10000 shaded cube gizmos).
*   Editor: Fixed crash on Windows when you have assets with names like "Tree A" and "TreeA" in the same folder ("revenge of MS-DOS short names!").
*   Graphics: Fixed static batching when there are source meshes without UV channels.
*   Graphics: Fixed CombineMeshes() outputting wrong vertex count. This fixes a bug with combined meshes not drawing on some graphics cards.
*   Graphics: Properly validate array size when setting Mesh.vertices from script.
*   Input: Correctly detect controller after it has been reconnected on Windows.
*   Input: Ignore obsolete DirectInput registry settings.
*   iOS: Fixed automatic .a plugin inclusion into Xcode project.
*   iOS: Fixed all the issues with splash orientation.
*   iOS: fixed issue with native UI on top of unity view with non-animated rotation.
*   iOS: Fixed linking with xcode4.5 dev preview
*   Mobile: Added additional logging when initializing the profiler (over Wi-Fi or USB), to aid debugging when device is not seen by the editor.
*   Mobile: Fixed fixed function shader generation in case of more then one TexGen CubeReflect samplers.
*   NavMesh: Optimize navmesh bake memory-usage. Instead of crashing, returns error when out of memory.
*   NavMesh: Setting agent destination does not break stopping distance behavior.
*   NavMesh: Agent respects explicitly set rotation of transform when updateRotation is set.
*   Networking: Fixed problem with connecting to a password protected server using a GUID.
*   Shaders: Fixed surface shader decal:blend mode when normal mapping or specular was used.
*   Shaders: Various fixes to mobile shader translator (HLSL -> GLSL compiler).
*   Shaders: Fixed incorrect fog on some shader model 3.0 shaders on Windows.