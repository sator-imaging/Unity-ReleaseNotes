# Unity 2017.4.9f1
https://unity3d.com/unity/whatsnew/unity-2017.4.9

## Fixes

<ul>
<li>(1060074, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/956425">956425</a>) -  Android - Show a friendly user message when using JDK other than 8</li>
<li>(1049226) -  Asset Import - Fixed default texture format incorrectly changed to low quality.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1008836/">1008836</a>) -  Graphics - Fixed 32 bit index meshes not working with Mesh Compression properly.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/986332/">986332</a>) -  Graphics (Metal) - Fixed a crash or freeze instead of error message using old asset bundle.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1033216/">1033216</a>) -  Graphics - Rendering command buffers: Fixed using temporary render targets as UAV targets.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1035793/">1035793</a>) -  IL2CPP - Fixed an exception when child of Text Mesh Pro object is detached.</li>
<li>(1062524) -  Linux Player - Fixed keyboard input buffering at low framerates on Linux.</li>
<li>(1062061) -  Particles - Fixed a crash and add warning when assigning a non-read/write mesh to the shape module.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/962027/">962027</a>) -  Physics - Cloth, reset coefficients if mesh has changed type. Keep coefficients for similar mesh types.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/971056">971056</a>) -  Physics - Fixed an issue where activating interpolation on Rigidbody may cause jittery.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/969743">969743</a>) -  Physics - Fixed an issue where transforms are not correctly synced when using Rigibody.AddRelativeForce.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/976095">976095</a>) -  Physics - Fixed a cash when deativating a Gameobject with WheelColliderComponents.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/978753">978753</a>) -  Physics - Fixed an issuer where kinematic body's collision transform are not updated if instantiated as a child.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/985046">985046</a>) -  Physics - Fixed an issue where WheelCollider's damping rate has no effects in some cases.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/980186">980186</a>) -  Physics - Fixed a crash when two kinematic bodies using non-convex mesh collide.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1002396">1002396</a>) -  Physics - Fixed an issue where CharacterController.ClosestPoint may return incorrect value.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/984525">984525</a>) -  Physics - Fixed an issue where transforms are not correctly synced when using Rigibody.AddForceAtPos.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/987906">987906</a>) -  Physics - Fixed an issue where ClothComponent may be permanently disabled when deativate/reactivate GameObjet in play mode.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/973464">973464</a>) -  Physics - Fixed an error that pops up when changing the SkinnedMeshRenderer's mesh with ClothComponent on the same GameObject.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/996194">996194</a>) -  Physics - Fixed an issue where animated rigidbodyies don't affect other rigidbodies connected with joints.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1004443">1004443</a>) -  Physics - Fixed an issue where transforms are not correctly synced when using Rigibody.AddExplosionForce.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/969368">969368</a>) -  Physics - Fixed a memory leak when resizing collider.</li>
<li>( N/A) -  Profiler - Fixed an issue with the Profiler not blocking the network connection when sending frames that don't fit in the connection's buffer.</li>
<li>(1046268,<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1036657">1036657</a>) -  Scene Management - Fixed editor crashes on removing or adding RectTransform component to GameObject with attached Halo or Lens Flare component.</li>
<li>(1057078,<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1036699">1036699</a>) -  Scripting - Fixed a crash when dragging a script with a UI or RectTransform component requirement to a GameObject.</li>
<li>(1030942, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1002426">1002426</a>) -  Video - Fixed Audio from UnityEngine.Video.VideoPlayer is distorted when Audio Output Mode is Direct.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/986665/">986665</a>) -  Windows - Fix for an issue that prevented the mouse cursor from properly changing it's icon when resizing a standalone player window.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/994408/">994408</a>) -  Windows - Fix for an issue that allowed two instances of a standalone player to launch, even with Force Single Instance was enabled.</li>
<li>(1030307) -  Xbox One - Unity projects now build for Xbox One with .net 4.6 compatible scripts and the Roslyn compiler.</li>
</ul>

#### Revision: 6d84dfc57ccf
