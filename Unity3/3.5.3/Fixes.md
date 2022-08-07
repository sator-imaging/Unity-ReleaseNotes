# Unity 3.5.3
https://unity3d.com/unity/whats-new/unity-3.5.3

## Fixes


#### Unity for Native Client has been updated to a new version of the NaCl SDK, which fixes some problems. Shipping NaCl games need to be rebuilt with Unity 3.5.3, as they will no longer work in future versions of Google Chrome otherwise!
<ul>
<li>Android: JDK 7 installations are now automatically detected on windows.</li>
<li>Android: Reading player preferences using the wrong value type now return the default value.</li>
<li>Android: Fixed a rare race-condition when quitting the application.</li>
<li>Android: Added support for gdbserver being packaged inside the application.</li>
<li>Android: Use of spaces in keystore alias/password is now allowed.</li>
<li>Android: Added better failure message when the wrong key password is provided.</li>
<li>Android: Force SHA1 digest algorithm when signing the application, to make sure it's accepted by Google Play Store.</li>
<li>Android: Force RSA key algorithm when creating keys, as suggested by Google.</li>
<li>Android: Workaround for the bug with Kindle's compositor where it incorrectly uses the alpha values from the Display Buffer.</li>
<li>Android: Added warning for shaders which compilation might cause crash on sgs2 updated to ics.</li>
<li>Android: Fixed returning from pause on Eclair devices -Android: fixed perf regression with batching/dynamic geometry on PowerVR GPUs.</li>
<li>Cache Server: Fixed problem where native assets (prefabs, materials, etc) would not refresh in the Editor when updated on disk and cache server is active.</li>
<li>Editor: Rotation doesn't create leftover animation curves anymore</li>
<li>Editor: Fixed "Deprecated EditorExtensionImpl" assets show up in projects converted from Unity 3.4</li>
<li>Editor: Fixed crash when selecting multiple ScriptableAssets of different types.</li>
<li>Editor: Fixed up serialized property error that causes a null ref when an array is the last element being drawn.</li>
<li>Editor: Fixed up asset labels so that they get saved to meta data and displayed in the inspector properly.</li>
<li>Editor: Correctly clear drag and drop buffer so that old data does not stay around causing issues.</li>
<li>Editor: Fixed wrong gizmo rendering on Windows with extremely high quad counts (e.g. drawing 10000 shaded cube gizmos).</li>
<li>Editor: Fixed crash on Windows when you have assets with names like "Tree A" and "TreeA" in the same folder ("revenge of MS-DOS short names!").</li>
<li>Graphics: Fixed static batching when there are source meshes without UV channels.</li>
<li>Graphics: Fixed CombineMeshes() outputting wrong vertex count. This fixes a bug with combined meshes not drawing on some graphics cards.</li>
<li>Graphics: Properly validate array size when setting Mesh.vertices from script.</li>
<li>Input: Correctly detect controller after it has been reconnected on Windows.</li>
<li>Input: Ignore obsolete DirectInput registry settings.</li>
<li>iOS: Fixed automatic .a plugin inclusion into Xcode project.</li>
<li>iOS: Fixed all the issues with splash orientation.</li>
<li>iOS: fixed issue with native UI on top of unity view with non-animated rotation.</li>
<li>iOS: Fixed linking with xcode4.5 dev preview</li>
<li>Mobile: Added additional logging when initializing the profiler (over Wi-Fi or USB), to aid debugging when device is not seen by the editor.</li>
<li>Mobile: Fixed fixed function shader generation in case of more then one TexGen CubeReflect samplers.</li>
<li>NavMesh: Optimize navmesh bake memory-usage. Instead of crashing, returns error when out of memory.</li>
<li>NavMesh: Setting agent destination does not break stopping distance behavior.</li>
<li>NavMesh: Agent respects explicitly set rotation of transform when updateRotation is set.</li>
<li>Networking: Fixed problem with connecting to a password protected server using a GUID.</li>
<li>Shaders: Fixed surface shader decal:blend mode when normal mapping or specular was used.</li>
<li>Shaders: Various fixes to mobile shader translator (HLSL -&gt; GLSL compiler).</li>
<li>Shaders: Fixed incorrect fog on some shader model 3.0 shaders on Windows.</li>
</ul>
