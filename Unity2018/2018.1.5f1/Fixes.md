# Unity 2018.1.5f1
https://unity3d.com/unity/whatsnew/unity-2018.1.5

## Fixes

<ul>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/976095/">976095</a>) - Physics: Fixed crash when deativating a Gameobject with WheelColliderComponents.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/985046/">985046</a>) - Physics: Fixed an issue where WheelCollider's damping rate has no effects in some cases.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/971056/">971056</a>) - Physics: Fixed an issue where activaging interpolation on Rigidbody may cause jittery.</li>
<li>(918283) - Physics: Fixed a performance issue when reparenting rigidbody.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/980186/">980186</a>) - Physics: Fixed a crash when two kinematic bodies using non-convex mesh collide.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1002396/">1002396</a>) - Physics: Fixed a issue where CharacterController.ClosestPoint may return incorrect value.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/984525/">984525</a>) - Physics: Fixed a issue where transforms are not correctly synced when using Rigibody.AddForceAtPos.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/969743/">969743</a>) - Physics: Fixed a issue where transforms are not correctly synced when using Rigibody.AddRelativeForce.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/987906/">987906</a>) - Physics: Fixed an issue where ClothComponent may be permanently disabled when deativate/reactivate GameObjet in play mode.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/978753/">978753</a>) - Physics: Fixed an issuer where kinematic body's collision transform are not updated if instantiated as a child.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/973464/">973464</a>) - Physics: Fixed an error that pops up when changing the SkinnedMeshRenderer's mesh with ClothComponent on the same GameObject.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/962027/">962027</a>) - Physics: Fixed an issue where cloth may lose constraints when assigning a new mesh to SkinnedMeshRenderer.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/996194/">996194</a>) - Physics: Fixed an issue where animated rigidbodyies don't affect other rigidbodies connected with joints.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1004443/">1004443</a>) - Physics: Fixed a issue where transforms are not correctly synced when using Rigibody.AddExplosionForce.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/990728/">990728</a>) - XR: Added velocity and angular velocity to WMR controllers.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1029856/">1029856</a>) - Editor: Fixed performance issues in the clip drop down menu of the animation window when editing large clips.</li>
<li>(None) - Editor: Added support for Package Manager Manifest inclusion into whole-project .unitypackages, for the Content team to produce tutorials and demos that use new features supplied as Package Manager Packages.</li>
<li>(None) - XR: Fixed eye texture allocation on Oculus mobile platforms.</li>
<li>(1021978(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/961655/">961655</a>)) - Android: Fixed using memalign on Android due to compatibility issues causing crashes on some devices.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1030459/">1030459</a>) - Scripting Upgrade: Fixed compilation errors in Visual Studio when targeting .NET Standard 2.0.</li>
<li>(1040288) - Licenses: Fixed inaccurate text in license survey.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/973842/">973842</a>) - OSX: Fixed mouse events affecting Editor UI performance.</li>
<li>(None) - Scripting Upgrade: Fixed an issue where editor scripts could fail to recompile on windows.</li>
<li>(None) - Editor: Optimised Version Control icon overlay drawing in the Project Window.</li>
<li>(1005227) - Scripting: Fixed crash when calling DestroyImmediate(gameObject) in OnApplicationQuit. Fixed ZenInject crash that would happen sometimes after exiting play mode.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/987068/">987068</a>) - Shuriken: Fixed Timeline Control Track not applying start delay to particles.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1024481/">1024481</a>) - Editor: Fixed regression where play mode tint and play button style were not applied before entering play mode when done via menu command.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1033273/">1033273</a>) - Editor: Disabled "Open" button in AssetImporter inspector when viewed from a Preset as there is no asset associated with it at this time.</li>
<li>(1025807) - Graphics: Fixed crash issue that can arise in SRP when you have shadowcasting enabled but no visible shadow casters.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1038721/">1038721</a>) - GI: Fixed non-latin characters not being allowed in the Unity editor install path.</li>
<li>(1043476(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1041582/">1041582</a>)) - Editor: Fixed License activation fails when running Unity with command line arguments.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1038630/">1038630</a>) - Asset Import: Added validation for invalid constraints in FBX files.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1038488/">1038488</a>) - OSX: Fixed an issue where the Mac Player could launch with a black screen.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1037638/">1037638</a>) - Android: Fixed the issue that GI assets for the first scene have been added to the obb with "Split Application Binary" enabled.</li>
<li>(1045866) - XR: Enabling Oculus depth sharing causes pink Game view when Android is targeted.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1025479/">1025479</a>) - Daydream: Fixed rendering corruption appearing when switching back to Daydream mode.</li>
</ul>

#### Revision: 732dbf75922d
