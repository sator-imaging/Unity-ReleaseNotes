# Unity 5.4.6
https://unity3d.com/unity/whats-new/unity-5.4.6

## Fixed

<ul>
<li>Android: Acquire context on focus before notifying player.   (837483)</li>
<li>Android: Disabled Debug markers on PowerVR Series 5 devices. (780958)</li>
<li>Android: Dropped obscured touch events to prevent tapjacking.    (900194)</li>
<li>Android: Fixed a crash in WebStreamDecomp after a long sequence of reading asset bundles.    (743739, 887242) </li>
<li>Android: Fixed a dangerous permission popup issue.   (851523)</li>
<li>Android: Fixed a rare crash on application exit due to UnityWebStreams not getting cleaned up properly.  (867508)</li>
<li>Android: Fixed an unnecessary internet permission requirement in empty project.  (892203)</li>
<li>Android: Fixed manifest merging with new android sdk tools.  (898979)</li>
<li>Android: Fixed pause/resume issues when loading with static splash image.    (867891)</li>
<li>Android: Fixed android application building with the latest android sdk. (888859)</li>
<li>Android: Make SoftInput not take fullscreen on landscape orientation.    (908868)</li>
<li>Android: SoftInput - Fixed input field hidden under keyboard when translucent flag was set. </li>
<li>Animation: Changing Animator.Speed during an animation transition will now correctly affect the cross-fade speed.    (898505)</li>
<li>Animation: Fixed IK on Feet not working properly when interrupting transitions.  (892043)</li>
<li>Animation: Fixed root rotation when importing a humanoid animation that used the "Copy From Other Avatar" feature.   (870185)</li>
<li>Animation: Improved build and asset bundle data determinism for Human components.    </li>
<li>Asset Bundles: Fix crash when loading GuiStyleState from an asset bundle (909472)</li>
<li>Build Pipeline: Fixed an issue with scene asset bundles that could cause multiple builds with the same scene generate different results. (895452)</li>
<li>Core: Fixed job system ending up with high CPU usage in certain circumstances eg. using UnityWebRequest.Send() in Editor after exiting Play mode.    (879675)</li>
<li>Editor - Other: Editor internal resources can now be rebuilt in 5.4.</li>
<li>Editor: Fixed OSX editor load failure when loading on case-sensitive file systems.   (890636)</li>
<li>Fix for Analytics events content type switches from Application JSON to application/x-www-form-urlencoded.   (852301)</li>
<li>Fixed an issue where Android devices' rendering could freeze or incorrectly render when using secondary cameras. (859561)</li>
<li>GI: Fixed a crash when creating reflection probes from OnWillRenderObject.   (873206)</li>
<li>Global Illumination: Fixed an issue where baked area light affected objects behind meshes where light shouldn't be present.  (875096)</li>
<li>Graphics: D3D9 - Make sure that internal resolves don't result in a drawn pixel – i.e single white pixel when using deferred mode.   (728324)</li>
<li>Graphics: Fixed a crash in GetBuildUsageTagFromAssets that was triggered by pro0ject that had ShaderVariants.    (890915)</li>
<li>Graphics: Fixed a periodic crash in shadow culling job code (GenerateCombinedDynamicVisibleListJob). (882704)</li>
<li>Graphics: Fixed an issue with Assert "Texture aux property (unity_SpecCube0_HDR) should never be a built-in name!".  (864237)</li>
<li>Graphics: Fixed clear artifacts on metal, if only UI camera is used in scene.    (909610)</li>
<li>Graphics: Fixed forward-only objects being rendered into Depth/DepthNormals textures multiple times when they had multiple submeshes and deferred shading was used.  (863954)</li>
<li>Graphics: Fixed SceneView GUI elements being very bright when HDR and Linear mode are enabled.   (878724)</li>
<li>Graphics: On DirectX, avoid presenting a fresh-black frame whilst performing screen resizing.    (849424)</li>
<li>Graphics: Set the ambient probe for the deferred reflections pass to fix a difference between graphics jobs and non-graphics jobs rendering. (863625)</li>
<li>IL2CPP: Fixed a a rare crash in IL2CPP on some Visual Studio installation setups with message "Unhandled Exception: System.InvalidOperationException: Builder was unable to build using selected toolchain (MsvcDesktopToolChain) or architecture (Unity.IL2CPP.Building.x64Architecture)!"   </li>
<li>IL2CPP: Fixed a race condition on iOS during method initialization.  (870973)</li>
<li>IL2CPP: Fixed the issue of memory snapshot profiler not showing multidimensional arrays. (888796)</li>
<li>IL2CPP: Modified the implementation of the IL Switch opcode to workaround a possible C++ compiler bug in Xcode 8.3.  (898861)</li>
<li>iOS: Added support in order to enable auto-rotation while broadcasting using ReplayKit.  -(861046)</li>
<li>iOS: Fixed Application.installMode for apps downloaded from AppStore (913886)</li>
<li>iOS: Fixed inclusion of ReplayKit framework in plugins.  (882013)</li>
<li>iOS: Removed extra notification sent on application launch.  (875180)</li>
<li>macOS: Fiexed an editor crash after Build &amp; Run for Android device. (917985)</li>
<li>Metal: Fixed an issue with setting DontCare load flag when running multithreaded.    </li>
<li>Physics: Fixed a crash caused by changing the value of the configuredInWorldSpace flag on a Joint attached to an inactive GameObject.    (883312)</li>
<li>Purchasing: Fixed an issue with Unity IAP emitting DuplicateTransaction failure for all non-consumable purchases when initialized.   (889321)</li>
<li>Scripting: Fixed a coroutine crash in Coroutine::CompareCoroutineEnumerator. (888302)</li>
<li>Shaders: Fixed advanced blend operations by requiring the shaders to be decorated with UNITY_REQUIRE_ADVANCED_BLEND(mode) declaration.   (750307)</li>
<li>Shaders: Fixed an incorrect translation from HLSL assembly for AND and OR operands. Fixes a crash when compiling shaders for GLCore. (883080)</li>
<li>Shaders: Fixed an internal error on a GLSL shader compiling corner case. (881103)</li>
<li>Sprites: Fixed an issue where OverrideGeometry on instantiated sprites produced differing results in the Editor and Standalone.  (863256)</li>
<li>Tizen: Fix a sensor bug that Input.gyro.gravity and Input.gyro.userAcceleration does not return a correct value. (931740)</li>
<li>Tizen: Resolved a crash that occurred when an app tried to exit. </li>
<li>UGUI: Fixed a crash when reparenting inactive object.    (898809)</li>
<li>UGUI: Fixed a memory leak in UGUI.</li>
<li>UI: Fixed a curve preview crash not updating when points changed but bounds did not. (856734)</li>
<li>UI: Fixed a memory leak in UI::DepthSortLayer(). Fixed a crash when UI Element m_Scale value was set to a large number, in the Editor or via script  (907581)</li>
<li>UI: Fixed an issue with corrupted text when text font was changed.   (904688)</li>
<li>UI: Fixed an occasional masking issue when using deferred rendering path on Linux.   (873678)</li>
<li>UI: Fixed scrollrect performance being slow when it had a lot of content.    (856381)</li>
<li>UI: Removed an extra call to CanvasRenderer.OnTransformChanged when canvas was set to ScreenSpace.Camera render mode, and the camera was transformed (886258)</li>
<li>UnityWebRequest: Fixed Editor freeze when exiting play mode with active UnityWebRequest with custom download handler script. (880565)</li>
<li>UnityWebRequest: Fixed high CPU when WebRequest with custom download handler script was aborted. (876027)</li>
<li>UnityWebRequest: Fixed redirect in editor when not in play mode. (879749)</li>
<li>VCS: Fix for editor not checking out scene file before first write in freshly loaded project.    (850239)</li>
<li>VR: Fixed a subtle timing bug on Rift that could cause a minor view stuttering in certain situations.    (886841)</li>
<li>VR: Updated Oculus to version 1.13 and GearVR to version 1.13.1. Fixes plugin loading issue in paths with non-ASCII characters.  </li>
<li>Windows Store: Fixed a rare case where games can get stuck in a busy loop on dual core devices.  (895766)</li>
</ul>
