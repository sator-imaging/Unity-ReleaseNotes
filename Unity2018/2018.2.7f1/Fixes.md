# Unity 2018.2.7f1
https://unity3d.com/unity/whatsnew/unity-2018.2.7

## Fixes

<ul>
<li>(None) Asset Database: Improved performance of AssetDatabase when doing dependency analysis by ensuring that the analysis is run lazily when processing the refresh queue, instead of every time the queue is modified.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1066381/">1066381</a>) -   Deployment Management : Fixed a crash when using sprites with no texture with the splash screen.</li>
<li>(None) -  Android : Player binary files contain .note.unity section with version and stripping information. This is useful for certain automation tools.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1061635/">1061635</a>) -  Editor : Fixed a bug where control for LayerMask SerializedProperty would change value for all selected objects without user interaction.</li>
<li>(None) -  Editor : Fixed a potential crash when calling Provider.GetLatest</li>
<li>(1048493) -  Editor : Fixed slow search in project view and scene/hierarchy views by starting the search only when the user pauses from typing instead of searching after every character typed.</li>
<li>(1069263, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1066381/">1066381</a>) -  Graphics : Fixed a crash when using sprites with no texture with the splash screen.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1061004/">1061004</a>) -  Graphics : Fix for crunch compressed texture support in texture mip map streaming.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1065223/">1065223</a>) -  IL2CPP : Fixed deadlock on exit when calling back to managed code on a thread that doesn't exit before player shutdown.</li>
<li>(1068426, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1061635/">1061635</a>) -  Inspector functionality : Fixed a bug where control for LayerMask SerializedProperty would change value for all selected objects without user interaction.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1069065/">1069065</a>) -  Timeline : Fixed Drag and Drop of Playable Assets from Project folder onto Timeline tracks.</li>
<li>(1041817) -  XR : Scenes will no longer be y flipped when running on the HoloLens.</li>
</ul>

#### Revision: 4ebd28dd9664
