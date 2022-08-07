# Unity 2018.1.3f1
https://unity3d.com/unity/whatsnew/unity-2018.1.3

## Fixes

<ul>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/989243/">989243</a>) - Scripting: Fixed issue with Assembly.assemblyReferences being null when returned from CompilationPipeline.GetAssemblies().</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/986828/">986828</a>) - Editor: Fixed issue with .asmdef inspector showing "null" for references if there are .asmdef error emitted to the console.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/994284/">994284</a>) - Editor: Fixed .asmdef duplicate references not being listed in error message.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/981283/">981283</a>) - Editor: Fixed issue with error being emitted when changing the case in .asmdef filename.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/997908/">997908</a>) - Editor: Fixed issue with .asmdef inspector showing "null" for references if there are .asmdef error emitted to the console.</li>
<li>(None) - Scripting: Fixed Mac Editor Runtime Tests hanging 50% of the time.</li>
<li>(1014670(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1002035/">1002035</a>)) - UI: Improved the performance of the culling by RectMask2D.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/955571/">955571</a>) - AI: Fixed AyncOperations started with the NavMeshBuilder sometimes crashomg when being used in quick succession.</li>
<li>(None) - Graphics: [Metal] Fixed linear shadow samplers not always being used for compute shaders.</li>
<li>(None) - Scripting Upgrade: The target framework version in generated .csproj files will now be 4.7.1, to match the reference assemblies used to compile code in Unity.</li>
<li>(1023048) - Timeline: Fixed inline curves selection being on the first clip instead of the new one when recording a new clip, .</li>
<li>(1023049(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1006210/">1006210</a>)) - Timeline: Fixed timeline allowing for keyframing of materials, but not working as expected. Shows incorrectly mapped references.</li>
<li>(1011247) - Timeline: Fixed snapping on start of a clip when trimming.</li>
<li>(1016834) - Timeline: Fixed edit modes not validating track drop properly.</li>
<li>(1010322) - Timeline: Fixed clip released in invalid target will be stuck if in ripple mode.</li>
<li>(1023043) - Timeline: Fixed playable tracks accepting any kind of clips.</li>
<li>(1023046(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1011490/">1011490</a>)) - Timeline: Fixed values not being removed on last Scale axis when removing keys with "Remove All Keys".</li>
<li>(1024183) - Timeline: Fixed removing keyframe not resetting the transform red color.</li>
<li>(1023044) - Timeline: [Override Track] mute icon do not appear on the override tracks.</li>
<li>(None) - UI: Fixing issue with disabled canvas renderer changing parent canvas that is then deleted.</li>
<li>(None) - UI: Fixing issue with disabled canvas renderer changing parent canvas that is then deleted.</li>
<li>(None) - iOS: Metal: Improved ETC texture format support.</li>
<li>(1030108) - Editor: Fixed YAMLMerge parser crash when fields have 3 or more dashes in them.</li>
<li>(1030108(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1028596/">1028596</a>)) - Editor: Fixed "Unexpected end of stream" error when merging files.</li>
<li>(1032292(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1030233/">1030233</a>)) - GI: Fixed "Texture rectangle is out of bounds" error when baking in Indirect debug view.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1024863/">1024863</a>) - Graphics: Fixed issue where objects could remain blurry when stopping moving, due to a bug when updating the motion vector buffer.</li>
<li>(None) - XR: Fixed several issues related to BEV cameras not tracking or rendering on Windows 10 with HoloLens.</li>
<li>(1033762(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1021293/">1021293</a>)) - Editor: Fixed multi-edit of delayed numeric field when discarding changes.</li>
<li>(1033762(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1021293/">1021293</a>)) - Editor: Fixed multi-edit of text field (specifically delayed numerical editors).</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1015627/">1015627</a>) - Android: Fixed android video player rounded frame rate.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/972235/">972235</a>) - Android: Fixed android video playback of rotated video files.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/989005/">989005</a>) - Android: [Adreno][Android 4.4.4] Material.SetVectorArray submits garbage after first index.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1011085/">1011085</a>) - Android: Fixed android video player not reporting error when hardware decoder fails.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1015627/">1015627</a>) - Android: Fixed android video player rounding frame rate.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/972235/">972235</a>) - Android: Fixed android video playback of rotated video files.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/989005/">989005</a>) - Android: Fixed shader unsigned int casting to signed int failure on android 4.*.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1011085/">1011085</a>) - Android: Fixed android video player not reporting error when hardware decoder fails.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1031017/">1031017</a>) - Asset Import: Fixed importing material from a package causing a crash.</li>
<li>(1032691(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1021238/">1021238</a>)) - Android: Fixed reading files with hieroglyphs in their names from StreamingAssets using UnityWebRequest.</li>
<li>(1035718(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1028371/">1028371</a>)) - Android: Reduce spam to logcat on UnityWebRequest error.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1009961/">1009961</a>) - Shaders: Fixed surface shader analysis regression that prevented Input and SurfaceOutput structs from having same-named member fields.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1005576/">1005576</a>) - Animation: Fixed reimporting prefab with optimal animation compression settings multiple times corrupting animation.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1005576/">1005576</a>) - Asset Import: Fixed random animation corruption when importing the animation multiple times.</li>
<li>(None) - iOS: Optimization to iPhoneTime:GetTimeSinceStartup().</li>
<li>(None) - iOS: Optimised GetTimeSinceStartup().</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1014725/">1014725</a>) - Shaders: Fixed surface shader issue where inputs only used via derivative instructions were not considered as "actually used".</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1020341/">1020341</a>) - IL2CPP: Fixed DllNotFoundException when accessing NetworkInformation on UWP.</li>
</ul>

#### Revision: a53ad04f7c7f
