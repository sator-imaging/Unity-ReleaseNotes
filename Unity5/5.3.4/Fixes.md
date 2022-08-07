# Unity 5.3.4
https://unity3d.com/unity/whats-new/unity-5.3.4

## Fixes

<ul>
<li>2D: Changing Rigidbody2D.gravityScale while a Rigidbody2D.MovePosition is in progress now works. (762771) </li>
<li>2D: Ensure Joint2D auto-configuration still works if joint is added from script (765870) </li>
<li>2D: Ensure that a TargetJoint2D added via script allows collisions with static colliders. (763922) </li>
<li>2D: Stop Rigidbody2D with Interpolation being placed at world origin for a single update upon start. (764769) </li>
<li>Analytics: Fixed unreliable event sending (especially AppStart) on WebGL. (770316) </li>
<li>Android: Added support for Vivante OpenGL ES 3 driver. (738821, 758155) </li>
<li>Android: Fixed alignment crash on some Android ARM devices. (768974) </li>
<li>Android: Fixed an issue where Ping wouldn't work in release mode. (734124) </li>
<li>Android: Fixed black screen or crash during startup on old PVR devices (Samsung Galaxy S I9000). (762875) </li>
<li>Android: Fixed bug in Texture.GetPixels for ETC compressed textures. (759195) </li>
<li>Android: Fixed rendering artifacts when using native plugins and multithreaded renderer. (772171) </li>
<li>Android: Fixed rendering on Vivante GPUs on Android 4.3 and older. (712890, 771890) </li>
<li>Android: IL2CPP; fixed build errors on NDK paths with whitespaces. (763447) </li>
<li>Android: IL2CPP; fixed crash on second startup after installation. (766698) </li>
<li>Android/IL2CPP; prevent a crash in the garbage collector when it attempts to scan a section of memory used for the code that may have been unmapped by the OS. (755201) </li>
<li>Animation: Fixed a crash when animating lights using the legacy Animation component. (772260) </li>
<li>Animation: Prevent crashes when clips are null for animations extracted from asset bundles whose dependencies have not loaded. (756463) </li>
<li>API Updater: Fixed "Sequence contains more than one matching element" crash. (760684) </li>
<li>API Updater: Fixed crash upon assembly resolution failures. (743463) </li>
<li>Asset Bundles: Only reimport when setting asset bundle name if cache server is connected. (714661) </li>
<li>AssetBundles: BuildAssetBundles will switch back to the original active build target when finished. (759142) </li>
<li>Audio: Disabled sound manager watch dog. (774356) </li>
<li>Core: Fixed an issue asynchronously loading a prefab with a large amount of assets. (771882) </li>
<li>Core: Fixed some errors with recently deleted objects (in WWWDelayCall; ClearPersistentDirty call; editor CEF integration).</li>
<li>Editor: Don't call OnLevelWasLoaded on the first scene when entering play mode. (759231) </li>
<li>Editor: Fix for clustering allocation while navigating. (747856) </li>
<li>Editor: Fixed a crash when selecting some prefabs. (766469) </li>
<li>Editor: Fixed an issue that made GameObjects disappear from the Editor if they have an associated editor script that made use of DontDestroyOnLoad. (754127) </li>
<li>Editor: Fixed an issue when opening a scene from the Project Browser while in playmode it resulted in that scene being loaded even after going out of playmode. (767728) </li>
<li>Editor: Fixed misleading texture decompression warning in graphics emulation. (760112) </li>
<li>Editor: Fixed startup when Unity is in a path with non-ASCII characters. (765159) </li>
<li>Editor: Fixed the issue of GUI.Windows background not being tinted by GUI.colors anymore. (756004) </li>
<li>Editor: Fixed the issue of marking scene dirty when creating prefab by dragging from Hierarchy window to Project. (758409) </li>
<li>Editor: Fixed the issue of marking the scene dirty when pressing the apply button on a prefab instance. (757027) </li>
<li>Global Illumination: Fixed crash in some scene loading scenarios. (768849) </li>
<li>Global Illumination: Fixed crash when building lighting with a specific scene setup. (767222) </li>
<li>Global Illumination: Fixed light probes not being used anymore in Standalone when a scene without light probes was loaded with Additive mode. (767161) </li>
<li>Global Illumination: Fixed multi-scene baking. (751599) </li>
<li>Global Illumination: Fully repaint inspectors after baking reflection probes; some previews were not updating before. (663992) </li>
<li>Global Illumination: When compositing the directional lightmap removed the clamping on the w-component of the generated pixels.</li>
<li>Graphics: Added profiler markers on async texture loading waits. </li>
<li>Graphics: Fixed .ogv movie files with stream markers beyond 16kb not imported correctly. (772013) </li>
<li>Graphics: Fixed "Trying to reload asset from disk that is not stored on disk" error when non-persistent objects are attempted to be reloaded from disk. (752613) </li>
<li>Graphics: Fixed a synchronization problem that was causing texture data not to be properly updated when changing quality settings at runtime. (752613) </li>
<li>Graphics: Fixed an issue where GrabPass could get source texture wrongly offset in some cases. (75508, 726067) </li>
<li>Graphics: Fixed an issue where setting a material's shader to null would crash the editor. (771292) </li>
<li>Graphics: Fixed an issue where TrailRenderer would randomly vanish/flicker. (740580)</li>
<li>Graphics: Fixed crash in SetGpuProgramName which could happen when the program isn't supported by the target graphics hardware (found on Android) . (772958) </li>
<li>Graphics: Fixed GenerateSecondaryUVs crashes on some meshes.</li>
<li>Graphics: Fixed MovieTextures sometimes being black in Mac Standalone (64 or Universal builds). (765928) </li>
<li>Graphics: Prevent Projectors from accepting invalid clip planes from a script. (506089, 535548) </li>
<li>Graphics/DX11: Fixed compute shader resource hazards found in certain cases when binding the same resource SRV and UAV on pixel and compute shader stages. (542251) </li>
<li>IL2CPP: Avoid crash when constructing error message. (770081) </li>
<li>IL2CPP: Correctly sort unsigned integers via the Array.Sort method. (774085) </li>
<li>IL2CPP: Prevent generated C++ code from failing to compile with errors like "error: use of undeclared identifier 'L_5'" in some cases. (773713, 768010) </li>
<li>IL2CPP: Properly marshal formatted classes (762883, 746313) </li>
<li>IL2CPP: Properly parse binary text assets. (771835) </li>
<li>iOS Metal: Fixed performance regression when doing in-frame clear (GL.Clear or command buffer Clear). (775362) </li>
<li>iOS: Fixed redirect for WWW. (723960) </li>
<li>Linux: Fixed MSAA in non-upscaled windows, force window recreation when requirements change for player window attributes. </li>
<li>Linux/GLCore: Fixed one more instance of render. (775575) </li>
<li>Mecanim: Fixed an issue with Animation clip length for bundled clip. (753888) </li>
<li>Mecanim: Fixed AnimationClip.SampleAnimation memory leak. (760612) </li>
<li>Mecanim: Fixed Animator with statemachine behaviour runtime compile error not firing callback on the right SMB. (756129) </li>
<li>Mecanim: Fixed assert when using Animator.MatchTarget.</li>
<li>Mecanim: Fixed long start play mode for scene with lots of controller. (769964) </li>
<li>Mecanim: Fixed StateMachineBehaviours on layer not being called properly. (765141) </li>
<li>Mono: Added IPv6 support on Windows. (767741) </li>
<li>Networking: Fixed a crash due to wrong initialization of connection. </li>
<li>Networking: Fixed an issue where ack didn't reset with connection resetting which lead to reliable traffic stale. (775226) </li>
<li>Networking: Removed annoying "Attempt to send to not connected connection" message. (775222) </li>
<li>Networking: Removing "no free events for message" as annoying. (775225) </li>
<li>Networking: Send Error: val &gt; 0 on user disconnect, results in memory write violation and editor crash. (754510) </li>
<li>OpenGL Core: Fixed twitching and incorrect rendering with skinning and UI components on GLCore + Mac + NVIDIA. (773476, 775275, 767857, 766778) </li>
<li>OpenGL Core: Fixed fullscreen mode when not using native resolution and using MSAA on Mac AMD GPUs. (775428, 776470) </li>
<li>OpenGL Core: Fixed fullscreen MSAA support with linear color space rendering. (774558, 774216) </li>
<li>OpenGL Core: Fixed Graphics API switching to OpenGL. (762687) </li>
<li>OpenGL Core: Fixed occasional game view flipping with image effects in the editor. (760196)</li>
<li>OpenGL Core: Fixed dynamic geometry performance issues on Mac + NVIDIA.  </li>
<li>OpenGL Core: Fixed stretched game view with some image effects in Mac editor. (757536, 757866)</li>
<li>OpenGL Core: Workaround for Nvidia shader compiler bug on OS X, affecting SSAO shader. (756028)</li>
<li>OpenGL Core/ES: Fixed scalar uniform handling in the shader translator. (772167) </li>
<li>OpenGL Core/ES: Fixed wrong shader code generation when redirecting variables, was affecting FastBloom shader. (772434) </li>
<li>OpenGL Core/ES: Shader compiler, fixed invalid uniform access in certain corner cases. (767343) </li>
<li>OpenGL ES: Fixed non-shadowmap depth textures on some devices. (768916) </li>
<li>OpenGL: Fixed point size support using GLSL PROGRAM snippets. (763875) </li>
<li>Particles: Fixed a culling regression, when particle systems leave the screen and come back. (773673) </li>
<li>Particles: Fixed error message due to default bounding box. (767419) </li>
<li>Physics: Fixed a PhysX crash issue in PxsCCDContext::updateCCD experienced by some VR applications.  (776187) </li>
<li>Profiler: Fixed crash when adding data from thread which was started during a frame. (758264) </li>
<li>Profiler: Fixed hang when EndSample did not have a matching BeginSample. (770225) </li>
<li>Shaders: Added support to the compute shader compiler to handle bools inside structures. </li>
<li>Shaders: Fixed Standard shader in some rare cases outputing NaN as pixel shader result. (766806) </li>
<li>Shadows: Fixed shadows disappearing for some off-screen shadows casters. (761152) </li>
<li>Substance: All inputs are now applied to a ProceduralMaterial on the first RebuildTextures() call after the material's textures have been read from cache. Previously, only the modified inputs were applied. </li>
<li>Substance: Fixed Editor freeze upon instantiation of resource. (771650) </li>
<li>Substance: Fixed broken detection and assignment of shader keywords resulting in wrong appearance of ProceduralMaterials in scenes when the ProceduralMaterial was not opened in the Inspector (some shader keywords were enabled when they should not). </li>
<li>Substance: Fixed cache hashing and management issue which could cause the cache to be considered valid again after having been invalidated (often seen after calling Resources.UnloadUnusedAssets()). </li>
<li>Substance: Fixed loading of files with special characters in their paths or names. </li>
<li>Substance: Fixed rare crash caused by using the wrong size when uploading ProceduralTextures. </li>
<li>Substance: Fixed upgrading UNITY 4.x project data, legacy shaders should now be used for these old projects instead of being incorrectly replaced by the Standard shader. (765510) </li>
<li>Tizen: Fixed error about copying whitelists while building on Windows. (773614) </li>
<li>UI: Fixed exceptions upon assembly/type resolution failures. (770048) </li>
<li>UI: Fixed memory leak where dirty renderers on a disabled canvas would still get added to the dirty list causing crashes on clear. (773533) </li>
<li>UI: Fixed sorting issue where gird based depth sorting would fail to recognize overlapping unbatchable items. (770804) </li>
<li>UI: Stopped raycast from traversing up the hierarchy when a canvas with override sorting is encountered. </li>
<li>UI: Vertical alignment of text sometimes appearing higher than expected. (760753) </li>
<li>Unity Ads: Updated to 1.5.6 version (fixes crash on Android 4.1 and earlier).</li>
<li>VR: Restart the VR Device if the Oculus Service fails. </li>
<li>Wii U: Fixed a crash on secondary error confirmation. (767206) </li>
<li>Windows Store: Fixed exported VS project failing to build for non-x86 CPU when there is a managed assembly in the project that's been compiled for x86. (770931) </li>
<li>Windows Store/IL2CPP: Fixed game crashing when its name is exactly 20 characters long. (769835) </li>
<li>Windows Store/IL2CPP: Fixed intellisense in generated Il2CppOutputProject to be able to correctly resolve Windows 10 headers. (771765) </li>
<li>Windows Store/IL2CPP: Fixed failing to build on top of a previous build when target directory is read-only. (766764) </li>
<li>Windows Store/IL2CPP: Graphics plugins now work. (770941) </li>
<li>Windows Store/IL2CPP: Reduced the amount of linker warnings when building.</li>
<li>Windows: Fixed Application.persistentDataPath when Product Name contains invalid path character. (756152) </li>
<li>Windows: Fixed unnecessary symbols exported for Windows Standalone Player executable. This was making some Nvidia drivers wrongly pick up integrated GPU instead of discrete one on some systems. </li>
<li>XBoxOne/IL2CPP: Allow a call to Guid.NewGuid to work correctly. (769711) </li>
</ul>
