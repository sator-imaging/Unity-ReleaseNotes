# Unity 2018.2.8f1
https://unity3d.com/unity/whatsnew/unity-2018.2.8

## Fixes

<ul>
<li>(1071483 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1062852/">1062852</a>)) - Android: Fixed crash when returning null string from Java plugin.</li>
<li>(1065609) - Asset Import: Fixed renaming or changing the namespace containing a scripted importer breaking the auto-reimport mechanism.</li>
<li>(1073894) - Editor: Fixed an issue where launching Unity via Hub invalidates existing login for direct launchers.</li>
<li>(1075850) - Graphics: Fixed main thread stall deleting temporary render targets after calling ConvertTexture() from script.</li>
<li>(1076208) - Graphics: Fixed crash in intensive rendering scenes when using legacy graphics jobs.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1061224/">1061224</a>) - Graphics: Fixed crash in MinMaxAABB::MinMaxAABB when Legacy Deferred Render Path is used.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1033188/">1033188</a>) - Graphics: Fixed RGBA16 having swapped red/blue channels.</li>
<li>(1075574 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1070347/">1070347</a>)) - Graphics: Fixed issue where Camera FOV cannot be set to a value lower than 1.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1041458/">1041458</a>) - OSX: Fixed an issue where MacOS player would not go into correct screen mode when Command+F is pressed.</li>
<li>(1074390 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1058082/">1058082</a>)) - Physics: Fixed issue where colliders without physics material don't return correct default material in Physics Settings.</li>
<li>(1074389 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1009394/">1009394</a>)) - Physics: Fixed wrong UV returned in Raycast result when raycasting to a mesh collider that has negative scale.</li>
<li>(1074384 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1005564/">1005564</a>)) - Physics: Fixed issue where transform to CharacterController in OnControllerColliderHit is ignored.</li>
<li>(1074376) - Physics: Fixed an issue where some Physics Settings are not reset upon request.</li>
<li>(1074374 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1024453/">1024453</a>)) - Physics: Fixed issue where mass properties are not correctly updated when changing collider scale.</li>
<li>(1074373 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1048878/">1048878</a>)) - Physics: Fixed a crash when user sets a very small size to Terrain data.</li>
<li>(1066072 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1059467/">1059467</a>)) - Physics: Fixed an issue where kinematic bodies may not follow transform change after setting its postion after setting their position or rotation via Transform component.</li>
<li>(1074312) - Scene Management: Fixed crash in LightmapSettingsManager.CheckSettingsConsistency when calling UnloadSceneAsync right after a LoadScene(SingleMode).</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1052766/">1052766</a>) - Scene/Game View: Fixed issue where specifying frustum view point would actually use it as base for the near plane.</li>
<li>(1073275) - Scripting Upgrade: Fixed hang when disconnecting while reading/writing on a SslStream.</li>
<li>(1060892) - Scripting Upgrade: Fixed crash when entering playmode on OSX.</li>
<li>(1062208) - Scripting Upgrade: Fixed Android Runtime test instability.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1059122/">1059122</a>) - Scripting Upgrade: Fixed an issue where UnsafeUtility.GetFieldOffset could return 0 when the type is not initialized.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1065895/">1065895</a>) - Scripting Upgrade: Fixed crash when DynamicMethod is constructed into non-dynamic image.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1069236/">1069236</a>) - Scripting Upgrade: Fixed  crash when using unmanaged constraint.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/966667/">966667</a>) - UI: Fixed Chinesse bolded Arial font style looks wide in Editor.</li>
<li>(983200) - UI: Fixed spacing between characters is lost and text is stretched with bold font selected when built on certain platforms.</li>
</ul>

#### Revision: ae1180820377
