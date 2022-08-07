# Unity 2018.2.3f1
https://unity3d.com/unity/whatsnew/unity-2018.2.3

## Fixes

<ul>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1040282/">1040282</a>) -  2D  -  Fixed issue where the SpriteAtlas Inspector did not correctly update after calling <code>SpriteAtlasExtensions.SetPlatformSetting</code>.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1037553/">1037553</a>) -  2D  -  Fixed issue where changes to the "Max Texture Size" and "Compression" settings in the Sprite Atlas weren't saved properly.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1040280/">1040280</a>) -  2D  -  Fixed issue where SpriteAtlas packed Sprites did not render after <code>SetPlatformSettings</code> and <code>PackAtlases</code>.             </li>
<li>(1046157) -  2D  -  Fixed issue where Sprite Renderer was rendering from the wrong Sprite Atlas with a duplicate name because of a late binding issue.             </li>
<li>(1048645, 1041651) -  Android  -  Fixed issue where instant app installs failed with the internal build system, because there was no APK Signature Scheme v2.             </li>
<li>(1053353, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1041385/">1041385</a>) -  Android  -  Unity no longer destroys Gradle Daemons after every build; it now destroys them on Editor exit.             </li>
<li>(1053346, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1016755/">1016755</a>) -  Android  -  Fixed an issue where Android Gradle builds failed when a custom template used double asterixes.             </li>
<li>(1062024, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/941276/">941276</a>) -  Android  -  Fixed an issue where multithreaded rendering became enabled when upgrading from 2017.1.             </li>
<li>(1060076, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/956425/">956425</a>) -  Android  -  Added a friendly user message when using JDK other than 8.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1004980/">1004980</a>) -  Asset Bundles  -  Fixed an issue where it was impossible to build Variants using the <code>BuildPipeline</code> API that takes an <code>AssetBundleBuild</code> array.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1004980/">1004980</a>) -  Build Pipeline  -  Fixed issue where variant bundles built via a build map show an error and have pink texture.                            </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1058139/">1058139</a>) -  Editor  -  Added a 1px interior stroke to the color slider thumb, to improve visibility against the light background.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1051179/">1051179</a>) -  Editor  -  Fixed bug where opening the native color picker on macOS would immediately change a color field's value to the most recent color selected.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1047812/">1047812</a>) -  Editor  -  Fixed issue where Unity did not calculate GUI text width correctly when GUIStyle used Word Wrap.             </li>
<li>(1063416, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1040256/">1040256</a>) -  Editor  -  Fixed misplaced tooltip when moving UIElements position.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1012892/">1012892</a>) -  Editor  -  Appled fix to generate C# project and solution for all script editors when using Assets &gt; Open C# Project menu.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1037523/">1037523</a>) -  Editor  -  Fixed issue with .sln project names not being unique.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1047812/">1047812</a>) -  Editor  -  Fixed issue where GUI text width was not calculated correctly when GUIStyle used Word Wrap.             </li>
<li>(1032167) -  Graphics  -  Fixed race condition when using Reflection probes extensively.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1057610/">1057610</a>) -  Graphics  -  Fixed bug where a color with a max RGB component of 1 was decomposed as if it were an HDR color with exposure.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1047517/">1047517</a>) -  Graphics  -  Fixed <code>RenderTexture</code> Assets using the default color format even when selecting a different format.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1053308/">1053308</a>) -  IL2CPP  -  Fixed managed debugger exception handling issue which threw an exception if the type for a catch handler was not specified.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1056170/">1056170</a>) -  IL2CPP  -  Applied fix to correctly treat the timeout value passed to Socket.Poll as microseconds, instead of milliseconds.             </li>
<li>(1058474) -  IL2CPP  -  Fixed [RuntimeInitializeOnLoadMethod] not working during certain player builds when managed code stripping occurs.             </li>
<li>(1058475) -  IL2CPP  -  Fixed [Preserve] not working during certain player builds when managed code stripping occurs.             </li>
<li>(1044003) -  Kernel  -  Fixed crash on shutdown when calling <code>JobHandle.Complete()</code> or Scheduling jobs during <code>OnDisable</code> during engine shutdown.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1056554/">1056554</a>) -  Kernel  -  Added missing information to Scripted Importers serialization. This fixes script change detection so that Unity can reimport Assets correctly.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1056554/">1056554</a>) -  Kernel  -  Fixed Unity crashing when trying to preview an Asset with scripted importers.             </li>
<li>(1060093, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1056406/">1056406</a>) -  Kernel  -  Fixed crash and modified behaviour when passing null to <code>Transform.Find</code>.             </li>
<li>(1062524, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1049679/">1049679</a>) -   Linux  -  Fixed keyboard input buffering at low framerates on Linux.             </li>
<li>(None) -  Mono  -  Removed the 32-bit slice from Mono, so that macOS App Store submissions are not rejected.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1056126/">1056126</a>) -  OSX  -  Fixed regression of Gamepads and Joysticks not working in Mac OSX Standalone player.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/769969/">769969</a>) -  OSX  -  Fixed issuewhere the Player configuration window would not open when you clicked its tray icon in OSX Dock panel.             </li>
<li>(None) -  Package Manager  -  Fixed an issue where upm.log (and UnityLog.txt on Mac) would get spammed when running offline search requests.             </li>
<li>(None) -  Package Manager  -  Fixed an issue where existing npm configuration files would interfere with the Package Manager.             - (</li>
<li>(None) -  Package Manager  -  Fixed an issue where HTTP requests from Unity to the local upm server would abort after 2 minutes.             </li>
<li>(1061427) -  Package Manager  -  Fixed issue where packages downloaded for one registry became available on all registries.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1024363/">1062050</a>) -  Particles  -  Added a warning message that appears when you assign a non-read/write Mesh to a Renderer that won't be shown.             </li>
<li>(1062051, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1051205/">1051205</a>) -  Particles  -  Fixed crash and added a warning message that appears when you assign a non-read/write Mesh to the Shape module.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1043662/">1043662</a>) -  Physics  -  Fixed crash when deactivating/re-activating a transform in <code>RunTimeInitializeOnLoadMethod</code>, if there is a Rigidbody attached.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1030966/">1030966</a>) -  Physics  -  Fixed a bug when <code>WheelCollider.GetGroundHit</code> causes crash at <code>Scripting::ScriptingWrapperFor</code> if <code>WheelCollider</code> is null.             </li>
<li>(1061733, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1025263/">1025263</a>) -  Physics  -  Fixed a performance regression when using continuous collision detection on kinematic Rigidbody components,             </li>
<li>(1041208) -  Physics  -  Fixed an issue where <code>RaycastCommand</code> would yield a wrong result if input ray direction was not normialized.             </li>
<li>(1060013, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1050751/">1050751</a>) -  Physics  -  Fixed an issue where a Collider's underlying PhysX Transfrom did not update correctly when reparenting.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1064077/">1064077</a>) -  Scriptable Build Pipeline  -  Fixed an issue where Unity was stripping precompiled assembly serialized data in the Scriptable Build Pipeline.             </li>
<li>(1032183) -  Scripting  -  Fixed issue where packages would sometimes not compile when starting the Editor with "Assembly has reference to non-existent assembly" .asmdef errors.             </li>
<li>(None) -  Services  -  Fixed an issue which inadvertently enabled Analytics when creating a new project.              </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1044712/">1044712</a>) -  Shaders  -  Fixed issue where Custom Surface Shader did not handle Shadow correctly when used from <code>DrawMeshInstancedIndirect</code>.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1062117/">1062117</a>) -  Timeline  -  Fixed Animation Track refresh when Avatar Masks are updated on override tracks.             </li>
<li>(1046113) -  VR  -  Updated copy of warning and log message when using Canvas screen space overlay render mode with VR enabled.             </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1059497/">1059945</a>) -  XR  -  Fixed issue where XR plug-ins delivered via the Package Manager (notably ARCore and ARKit) produced warnings in the console window regarding multiple GUIDs.             </li>
<li>(None) -  XR  -  Shifted Gear VR Touchpad Axes to 16 and 17 in for consistency with other platforms.             </li>
<li>(None) -  XR  -  Updated Resonance audio plugins to version 1.2.1. Fixed a meta file issue in OSX standalone builds.          </li>
</ul>

#### Revision:   1431a7d2ced7
