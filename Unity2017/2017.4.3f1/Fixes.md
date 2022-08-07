# Unity 2017.4.3f1
https://unity3d.com/unity/whatsnew/unity-2017.4.3

## Fixes

<ul>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/965024/">965024</a>) - Android: Fixed possible crash with Performance Reporting enabled.</li>
<li>(1027494(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1018967">1018967</a>)) - Android: Only include selected abi's from .aar plugins.</li>
<li>(None) - Android: Updated JDK download link to lead to supported version.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/964886/">964886</a>) - Animation: Fixed an issue where modifying a Playable Graph playing AnimationClips in Editor would not play newly added clips.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1014724/">1014724</a>) - Asset Import: Fixed push pull dilation not being applied when importing lightmaps.</li>
<li>(None) - Build: Fixed build being strict strict.</li>
<li>(None) - Core: Fixed issue where the Unity splash screen's resources would not be unloaded.</li>
<li>(983772) - Core: Fixed very rare assert which can happen on old CPUs "Assertion failed: Null JobInfo in Steal".</li>
<li>(1018645) - Editor: Fixed performance issues for inspector window looking up custom editors.</li>
<li>(1014027) (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/952569">952569</a>)) - Editor: Fixed local assets being overwritten during collab update.</li>
<li>(1024888) (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1021293">1021293</a>)) - Editor: Fixed multi-edit of text field (specifically delayed numerical editors).</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/997954/">997954</a>) - GI: Fixed issue where an error code would be reported when switching scene visualization mode to Indirect or Emissive due to a lack of data.</li>
<li>(991393) - GI: Fixed a memory leak when exiting play mode with realtime GI enabled.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1000350/">1000350</a>) - GI: Fixed rare crash when seam stitching is enabled on object packed to the boundary of a lightmap.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/908068/">908068</a>) - GI: Fixed issue where the Progressive Lightmapper wasn't correctly dealing with some quad faces in models.</li>
<li>(1026358) - Graphics: Fixed a crash that could occur when modifying the GraphicsSettings asset - fixes importing the Adam Character Pack from the Asset Store.</li>
<li>(1018878 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/934897">934897</a>)) - Graphics: Fixed rare deadlock in CreateGpuProgram when graphics jobs are enabled.</li>
<li>(1003174) - Graphics: Fixed deadlock in graphics command buffer when updating constant buffers.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/972060/">972060</a>) - Graphics: Fixed crash on Mesh.ClearBlendShapes.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/944153/">944153</a>) - iOS: Fixed race condition with nil-ing "system RT" texture in DestroySystemRenderingSurfaceMTL.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1003824/">1003824</a>) - Linux: Updated SDL to 2.0.7, which fixes several input related issues for Linux users.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/977503/">977503</a>) - OSX: Fixed build not launching on Mac if its name includes '&amp;' or '&lt;' character while generating.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/995346/">995346</a>) - OSX: Fixed not being able to toggle between two Unity window.</li>
<li>(1016750) - Profiler: Fixed profiler deadlock when naming a class the same as an existing sample.</li>
<li>(1005409) - Profiler: Fixed issue with imbalanced Profiler.BeginSample/EndSample markers in user scripts.</li>
<li>(None) - Timeline: Fixed values not being removed on last Scale axis when removing keys with "Remove All Keys".</li>
<li>(None) - Timeline: Fixed removing keyframe not resetting the transform red color.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/934908/">934908</a>) - UI: Fixed Canvas raycast start position for screen and world space camera modes.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1021484/">1021484</a>) - UI: Removed requirement of using ForceUpdateRectTransform after setting RectTransforms position.</li>
<li>(None) - UI: Fixed issue where Canvas with CanvasScaler at same resolution as the screen does appear in the right position when enabling.</li>
<li>(None) - UI: Fixed issue with disabled canvas renderer changing parent canvas that is then deleted.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/990728/">990728</a>) - XR: Fixed inconsistency between Unity's input tracking and WSA input information in Windows Mixed Reality.</li>
</ul>

#### Revision: 21ae32b5a9cb
