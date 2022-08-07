# Unity 5.4.3
https://unity3d.com/unity/whats-new/unity-5.4.3

## Fixes


#### Also includes relevant fixes from Unity 5.3.7.

### 
<ul>
<li>2D: Fixed an issue with UV rounding errors when using the OverrideGeometry method on sprites. (823935)</li>
<li>Analytics: Fixed an invalid userId issue on WebGL.</li>
<li>Android: Added "Mute Other Audio Sources" option to Android player settings in editor.</li>
<li>Android: By default lower volume of the background audio instead of muting it. (807983)</li>
<li>Android: Fixed a case of audio stutter when launching Android player from a notification on the lockscreen. (818174)</li>
<li>Android: Return internal temporary cache and persistent data paths when external paths are unavailable. (826201)</li>
<li>Animation: Fixed a bug where deactivating a GameObject with an attached Animator might cause a crash. (822232)</li>
<li>Animation: Fixed a crash when receiving null property modification in animation recording. (832837)</li>
<li>Animation: Fixed an issue where Legacy animations could not be previewed. (845815)</li>
<li>Animation: Fixed erroneous "Playable was not Disposed" message being displayed. (826047)</li>
<li>Animation: Re-enabling playback/recording in play mode. (835544)</li>
<li>Asset Bundles: Fixed the assetBundle property of AssetBundleCreateRequest so that it waits instead of returning null when the bundle is not yet ready (824009)</li>
<li>Asset Bundles: Fixed a deadlock when decompressing LZMA bundle when stream had incompressible data. (844785, 841067)</li>
<li>Asset Pipeline: Fixed a regression where AssetDatabase.SaveAssets won't save changes made to a prefab inside OnPostprocessAllAssets. (830110)</li>
<li>Audio: Fixed a panning issue with spatialized sounds.</li>
<li>Build player: Reverted the change, which saved relative paths for build target but introduced issues for targets that needed to browse for folders instead of files (WebGL, etc). (829898)</li>
<li>CacheServer: Fixed creation of directories and an issue while sending file and socket was closed. (774264, 820297)</li>
<li>Collab: Fixed crashes with collab toolbar. (819150, 808412)</li>
<li>Editor: Fixed an issue with addition of duplicate references of auxiliary platform-specific editor DLLs to editor C# project. (832097)</li>
<li>Editor: Fixed drag'n'drop of shader onto a material not setting the correct shader keywords. (819900)</li>
<li>Editor: Fixed errors when capturing screen or sending images to remote. (793204)</li>
<li>Editor: Fixed icon quality regression caused by unnecessary image scaling step. (807375)</li>
<li>Editor: TargetInvocationException error no longer appears when importing Windows Store Apps plugins. (815720)</li>
<li>Editor: Fixed Codesigning for Mac Editor to prevent firewall from asking multiple times for permission. (819351)</li>
<li>Graphics: Fixed a crash in CommandBuffer.DrawRenderer of a particle renderer when current camera is null. (808298)</li>
<li>Graphics: Fixed GPU instancing not working with procedurally generated meshes. (828380)</li>
<li>Graphics: Fixed a memory leak when using the GI visualizers in the scene view.</li>
<li>Graphics: Fixed incorrect batching of Renderers with different MaterialPropertyBlocks. (833783)</li>
<li>Graphics: Fixed a potential crash when calling GetShaderSettingsForPlatform on Windows. (833425)</li>
<li>Graphics: Prevent scene modifications from within OnPreRender callbacks, similar to other callbacks. (829694)</li>
<li>Graphics: Texture2D.ReadPixels no longer reads from the wrong location on iOS/Metal when reading a subsection of an image. (826244)</li>
<li>Graphics: Fix for dark lightmap when changing sun shadow strength in mixed lighting mode. (819092)</li>
<li>Graphics: Fixed editor crash when opening old project that had legacy OpenGL2 selected. (819813, 829178)</li>
<li>Graphics: Fixed an occasional TrailRenderer crash when using Clear script API. (829326, 818524)</li>
<li>IL2CPP: A call to GetCurrentMethod in a generic method should return the generic method definition, not the inflated generic instance method. (840596)</li>
<li>IL2CPP: Correctly marshal an out array of structures which uses the LPStruct marshaling directive. (842538)</li>
<li>IL2CPP: Fixed generated C++ code not compiling when calling Math.Abs on an unsigned integer. (837974)</li>
<li>IL2CPP: Return an empty array from GetGenericArguments when it is called on a MethodInfo object from a non-generic method. Previously the runtime incorrectly threw an assert in this case. (838259)</li>
<li>iOS: Build and Run now doesn't clean Xcode project for Append builds. (839037)</li>
<li>iOS: Fix a race condition when changing resolution on startup on Metal. (820885)</li>
<li>iOS: Fix bug in retrieving of certain values of IScore larger than 32 bits. (820938)</li>
<li>iOS: Improved performance by resizing the constant buffer pool adaptively on Metal. (820692)</li>
<li>iOS: Fixed an input reset in editor when iOS device without Unity Remote is selected. (832368)</li>
<li>iOS: Fixed issues with iOS Input.touchPressureSupported incorrectly reporting false. (834172)</li>
<li>iOS: Fixed a crash when using Build and Run for iOS projects. (836165)</li>
<li>iOS: Fixed editor hanging if app was already running in Xcode 7.x when using Build and Run. (843181)</li>
<li>iOS: GameCenterPlatform.ShowLeaderboardUI now shows the specific leaderboard when requested (note, the symptoms are still observable on iOS 8.4 and 9.x due to a bug in the OS itself). (808537)</li>
<li>iOS: ILeaderboard.LoadScores now does callback if SetUsersFilter is called. (801369)</li>
<li>Kernel: Fixed local scale of duplicate game object not matching original local scale of game object if parent has rotation set. (815816)</li>
<li>Multiplayer: Fixed a crash with StartAsClient. (827122, 804744)</li>
<li>Multiplayer: Fixed issues concerning disconnect and error handling. (790431, 785347, 771860, 836170, 827884)</li>
<li>Multiplayer: Fixed weaver error handling of not supported types. (761588, 820982, 773323)</li>
<li>Multiplayer: Fixed weaver generation of Serialize and Deserialize functions. (756572, 737241, 775248)</li>
<li>Particles: Don't allow prewarm on non-looping systems. (825180)</li>
<li>Particles: Fixed a crash when using uninitialised curves. (833513)</li>
<li>Particles: Fixed an issue when rendering during OnPreRender using RenderWithShader. (837680)</li>
<li>Particles: Prevent restarting particle system when parent transform moves in the editor. (819881)</li>
<li>Physics: Fixed interpolation of rigid bodies that was losing accuracy over time. That may have led to interpolated bodies moving in a jittery way after hours of gameplay. (843507)</li>
<li>Physics: Ensure that BoxCollider2D.Cast correctly detects a multi-edge EdgeCollider2D. (833737)</li>
<li>Physics: Ensure that BoxCollider2D/PolygonCollider2D with large vertex but small area is created correctly. (820300)</li>
<li>Scripting: Fixed a crash on Invoke(null, …). (766144)</li>
<li>Scripting: Fixed TransformDirection and InverseTransformDirection operations being affected by scale. (819962)</li>
<li>Scripting: Prevent GetHostEntry from throwing a SocketException on Windows when the machine is not connected to any network. (840534)</li>
<li>Shaders: Added shader macros to support LOD + sampler variations for cubemaps and texture arrays. (832292)</li>
<li>Shaders: Fixes to tessellation shader compilation on OpenGL and OpenGL ES. (828454)</li>
<li>Shaders: Fixed some cases of unsupported shader variants leading to a crash. (830078, 819705)</li>
<li>Shaders: Fixed some cases where surface shader writing to o.Occlusion would not sample the texture with correct UVs. (765145, 840314, 710625, 730779)</li>
<li>Tizen: Added loading indicator in Tizen.</li>
<li>tvOS: Added support for top shelf wide image. (833452)</li>
<li>UI: Fixed an issue where the Disabled Trigger animation was triggered on hovering over a Button when this was not Interactable. (826310)</li>
<li>UI: Fixed a crash in RectTransform because it would send messages on the loading thread. (824011)</li>
<li>UI: Fixed a crash when deleting GameObject with ScrollView component. (819770)</li>
<li>UI: Improved performance of SetParent in deeply nested UI panels. (814484)</li>
<li>VR: Fixed a crash when switching between VR mode and non-VR mode with image effects applied. (829379)</li>
<li>VR: Fixed issue with Oculus causing controller input to fail for bumpers.</li>
<li>VR: Fixed VRSettings.renderViewportScale when single-pass stereo rendering is enabled. (817835)</li>
<li>VR: VRDevice.isPresent now works correctly when HMD is occluded from base stations in OpenVR. (818159)</li>
<li>VR: Fixed a crash in certain conditions when checking if device is available in OpenVR. (819998)</li>
<li>WebRequest: DownloadHandlerAssetBundle will become done once download finishes. (834148)</li>
<li>WebRequest: Fixed a crash when downloaded asset bundle had zero size. (834583)</li>
<li>WebRequest: Fixed redirect to a relative URL. (833647)</li>
<li>Windows Store: Location services can be enabled or disabled while the app is still running. (829648)</li>
<li>Windows Store: Player preferences are no longer lost between game sessions. (835218)</li>
<li>Windows Store: Fixed a crash in multi scene system caused by internal managers being garbage collected. (821570)</li>
<li>Windows Store: Fixed incorrect instanceID for component when cloning object with component contained in a struct inside list. (838737)</li>
<li>Windows: Prevent some cases of invalid window sizes causing D3D surface creation to fail. (825082).</li>
<li>Windows: Fixed potential lock when in fullscreen exclusive mode and minimising/maximising screen. (837783)</li>
</ul>

#### Revision: 01f4c123905a
