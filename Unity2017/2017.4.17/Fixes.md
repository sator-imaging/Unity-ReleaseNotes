# Unity 2017.4.17
https://unity3d.com/unity/whatsnew/unity-2017.4.17

## Fixes

<ul>
<li><p>AI: Fixed NavMesh baking issue that appears when an Obstacle is at a certain proximity to another mesh (<a href="https://issuetracker.unity3d.com/issues/nav-mesh-pathfinding-bakes-incorrectly-when-gameobjects-are-placed-very-specifically">1044247</a>, 1098887)</p></li>
<li><p>Android: Fixed a crash for Android 9 (Pie) where ServiceConnection.onNullBinding() does not exist. (1091766)</p></li>
<li><p>Android: Fixed case of white flash when starting a Unity android app. (<a href="https://issuetracker.unity3d.com/issues/android-white-screen-before-splash-screen">929955</a>, 1087299)</p></li>
<li><p>Audio: Fixed FMOD shutdown to avoid a deadlock (<a href="https://issuetracker.unity3d.com/issues/android-google-play-video-recording-freezes-the-application-when-unlocking-the-device">1046752</a>, 1086869)</p></li>
<li><p>Build Pipeline: Fixed an issue where Scene Asset Bundles could not influence managed and native code stripping. (<a href="https://issuetracker.unity3d.com/issues/assetbundlemanifestpath-does-not-work-when-building-scenes-asset-bundles">1052180</a>)</p></li>
<li><p>Editor: Fixed Null reference Exceptions occurring while typing in the project window search bar (<a href="https://issuetracker.unity3d.com/issues/editor-typing-in-project-window-search-bar-during-play-mode-causes-nullreference-exceptions">1077389</a>, 1092366)</p></li>
<li><p>Editor: Unity Editor will no longer automatically unlock assembly reload (<a href="https://issuetracker.unity3d.com/issues/certain-editor-gui-interactions-automatically-reset-lockreloadassemblies">960397</a>)</p></li>
<li><p>IL2CPP: Fixed calls to native functions from delegates using stdcall calling convention, even if explicitly marked as cdecl. Caused problems on windows x86 (and UWP x86), leading to rare crashes in code using SSLStream (<a href="https://issuetracker.unity3d.com/issues/uwp-network-dll-triggers-an-exception-in-uwp-il2cpp-build">1044485</a>)</p></li>
<li><p>IL2CPP: Fixed IL2CPP build failing if Visual Studio 2019 is installed on the machine.</p></li>
<li><p>Licenses: Fixed an issue where licence activation didn't work when using the -nographics command line flag (<a href="https://issuetracker.unity3d.com/issues/using-nographics-causes-a-command-line-license-activation-to-fail">1043511</a>, 1088048)</p></li>
<li><p>Physics: Fixed RaycastHit.textureCoord performance issue, was internally copying whole mesh index buffer for no good reason (<a href="https://issuetracker.unity3d.com/issues/raycasthit-dot-texturecoord-is-very-slow">1065218</a>)</p></li>
</ul>
