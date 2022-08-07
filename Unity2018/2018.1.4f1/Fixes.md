# Unity 2018.1.4f1
https://unity3d.com/unity/whatsnew/unity-2018.1.4

## Fixes

<ul>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/980197/">980197</a>) - Editor: Test runner can now start tests on iOS/tvOS.</li>
<li>(1006601) - Licenses: Fixed issue that long time idle Editor failed to activate license for the first time.</li>
<li>(1010774(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1006311/">1006311</a>)) - Asset Import: Fixed ImportAsset crashes.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/980970/">980970</a>) - Asset Import: Fixed crash when re-importing certain model with "Generate Lightmap UVs" setting enabled.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1016639/">1016639</a>) - 2D: Fixed undo not removing GameObject created from dropping Sprite into Hierarchy Window.</li>
<li>(1021969(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1015836/">1015836</a>)) - 2D: Fixed Sprite Pivot setting appearing when Sprite Mode is set to Multiple but not appearing when it's set to Single.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1021484/">1021484</a>) - UI: Fixed issue with setting position followed by setting parent losing proper positioning.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1010047/">1010047</a>) - XR: Fixed dark VR view with Linear Color space and Single-Pass Rendering.</li>
<li>(1024560(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1014022/">1014022</a>)) - iOS: Disabled builtin cache in iOS UnityWebRequest backend for consistency with other platforms.</li>
<li>(1024558(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1011741/">1011741</a>)) - iOS: Fixed UnityWebRequest not becoming done when aborted.</li>
<li>(1026717) - Shaders: Fixed several custom shader include path corner cases making the system more robust against random script errors.</li>
<li>(None) - Graphics: Improve compute shader debug label support.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1014724/">1014724</a>) - Asset Import: Fixed lighting differences compared to older versions of Unity.</li>
<li>(1011566(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1011514/">1011514</a>)) - Asset Import: Upgraded to FBX SDK 2018.1.1, link to libfbxsdk dynamically on all builds.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/952966/">952966</a>) - Animation: Fixed evaluation of multi-outputs playables. Allows for fixing Timelines.</li>
<li>(1007989) - Scripting - Scripting Upgrade: Fixed issue loading circularly dependent assets while using scripting runtime version 4.x.</li>
<li>(1031063(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/967406/">967406</a>)) - Animation - Animation Recorder: Fixed recording an "Animator" controller generates 80 errors in the console.</li>
<li>(1030295) - Multiplayer: Fixed Host becomes broken\deleted after big packet has been sent.</li>
<li>(1029909) - Scripting: Fixed memory snapshot profiler.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1018162/">1018162</a>) - Scripting Upgrade: Fixed crash when calling Process.Start() to open a folder.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1010809/">1010809</a>) - Graphics: Fixed some backface culling corner cases (case 1010809).</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/965024/">965024</a>) - Services: Fixed possible crash with Performance Reporting enabled.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/984292/">984292</a>) - Android: Fixed black screen on Adreno GPU when using Postprocessing Stack and GLES2 graphics API.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/972927/">972927</a>) - Apple TV: Remove 2x App store icon slices that cause App Store validation to fail.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1024859/">1024859</a>) - iOS: Fixed manual signing with development certificates.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1011604/">1011604</a>) - iOS: Fixed crash when usbmuxd proxy is still running during app exit.</li>
<li>(None) - Graphics: Metal: Fixed tessellation shaders using instancing from failing to load.</li>
<li>(1026722) - Xbox One: Unity projects now build for Xbox One with .net 4.6 compatible scripts and the Roslyn compiler (case 1026722).</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1003917/">1003917</a>) - Audio: Fixed usage of deprecated WebAudio setters.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1003912/">1003912</a>) - Audio: Added Chrome Audio Auto-play policy workaround.</li>
<li>(None) - Graphics: Fixed errors when using Typeless D3D11 32 bit texture formats.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1029439/">1029439</a>) - 2D: Fixed tiles with invalid textures being rendered with the Tile Color only, instead of displaying the last used Sprite texture.</li>
<li>(1028457) - 2D: TilemapRenderer is now able to render when a SRP is set.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1024422/">1024422</a>) - 2D: Fixed tilemap painting being disabled if the tile map is parallel to the current Scene view camera, and within a margin of 5 degrees.</li>
</ul>

#### Revision: 1a308f4ebef1
