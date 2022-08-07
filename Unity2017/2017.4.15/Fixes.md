# Unity 2017.4.15
https://unity3d.com/unity/whatsnew/unity-2017.4.15

## Fixes

<ul>
<li><p>2D: Fixed tiled animated Sprites glitch when iterating over frames. (<a href="https://issuetracker.unity3d.com/issues/tiled-animated-sprites-glitch-out-when">1076834</a>, 1093240)</p></li>
<li><p>Android: Fixed crash in "AudioManager::ShutdownReinitializeAndReload" with Bluetooth headset pairing. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-android-crash-on-audiomanager-shutdownreinitializeandreload-with-bluetooth-headset-pairing">1086597</a>)</p></li>
<li><p>Android: Fixed unpredictable ordering with FixedUpdate. (<a href="https://issuetracker.unity3d.com/issues/android-fixedupdate-scheduling-is-unpredicatable">1071756</a>)</p></li>
<li><p>IL2CPP: Fixed COM Objects representing Windows.Foundation.IAsyncAction and Windows.Foundation.IAsyncOperation getting destroyed after converting them to System.Threading.Tasks.Task via "AsTask" extension method. (<a href="https://issuetracker.unity3d.com/issues/uwp-il2cpp-runtime-failure-on-call-to-windows-dot-storage-dot-streams-dot-getresults">1086209</a>)</p></li>
<li><p>IL2CPP: Support Marshal.SizeOf for types with a generic base class when the base class does not use the generic type in any field. (<a href="https://issuetracker.unity3d.com/issues/marshal-dot-sizeof-causes-argumentexception-errors-in-il2cpp-builds">1083239</a>)</p></li>
<li><p>iOS: Fixed a crash in iOS 7 due to the use of [UIScreen coordinateSpace]. (<a href="https://issuetracker.unity3d.com/issues/2017-dot-4-ios-nsinvalidargumentexception-in-uiscreen-coordinatespace-crashes-app-with-signal-sigabrt-on-ios-7-devices">1050777</a>, 1093249)</p></li>
<li><p>iOS: Fixed an issue where the namespace UnityEditor.iOS.Xcode was not found when running the Editor in batch mode. (<a href="https://issuetracker.unity3d.com/issues/unityeditor-dot-ios-dot-xcode-is-not-found-when-running-editor-in-batch-mode">1018716</a>, 1082694)</p></li>
<li><p>iOS: Fixed screen.safeArea not reported correctly when orientation is changed. (<a href="https://issuetracker.unity3d.com/issues/ios-iphonex-screen-dot-safearea-is-ignored-in-portrait-mode-until-screen-orientation-is-changed">1028312</a>, 1044173)</p></li>
<li><p>Physics: Fixed a crash when setting a too small size to Terrain size. (<a href="https://issuetracker.unity3d.com/issues/crash-in-physx-shdfnd-sort-physx-pxscontactpatch-dot-dot-dot-when-gameobject-collides-with-a-terrain-created-by-script">1048878</a>, 1079802)</p></li>
<li><p>Physics: Fixed an issue where colliders without physics material don't return correct default material in Physics Settings. (<a href="https://issuetracker.unity3d.com/issues/accessing-unassigned-colliders-material-returns-and-sets-different-material-than-the-physics-manager-default-material">1058082</a>, 1080052)</p></li>
<li><p>Physics: Fixed an issue where mass properties are not correctly updated when changing collider scale. (<a href="https://issuetracker.unity3d.com/issues/rigidbody-dot-centerofmass-is-miscalculated">1024453</a>, 1079803)</p></li>
<li><p>Physics: Fixed an issue where transform to CharacterController in OnControllerColliderHit is ignored. (<a href="https://issuetracker.unity3d.com/issues/character-controllers-change-of-position-in-oncharactercontrollerhit-is-ignored">1005564</a>, 1080047)</p></li>
<li><p>Scripting: Fixed crash with message box "GetThreadContext failed". (1082246)</p></li>
<li><p>Scripting Upgrade: Fixed hang when running tests in Editor. (971923)</p></li>
<li><p>Shaders: Fixed not able to load shaders from AssetBundles that were created in 2017.2. (1096788)</p></li>
</ul>

#### Revision: 5d485b4897a7
