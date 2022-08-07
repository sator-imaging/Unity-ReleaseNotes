# Unity 4.1
https://unity3d.com/unity/whats-new/unity-4.1

## Fixes

<ul>
<li>Android/iOS: Updated PrefetchSocketPolicy() to return true instead of throwing an exception.</li>
<li>Android: Added local ref cleanup code to AndroidJNI to support more user based local refs per frame.</li>
<li>Android: Added manifest flags to avoid multiple instances of the same application.</li>
<li>Android: Added the ability to pass null arguments through the JNI bridge.</li>
<li>Android: Added workaround for "Could not reserve enough space for object heap" error.</li>
<li>Android: Added workaround for Tegra shader compiler bug when texture samplers are not reported.</li>
<li>Android: Fixed "Unity Remote" accelerometer input.</li>
<li>Android: Fixed a crash when returning to main Activity after downloading an OBB, when using development player.</li>
<li>Android: Fixed an issue where async updates of the TouchScreenKeyboard.text property would void any input from the keyboard.</li>
<li>Android: Fixed an issue where huge switch case statements could crash/yield the wrong result.</li>
<li>Android: Fixed an issue where the application would consume a significant amount of cpu even though the application was paused.</li>
<li>Android: Fixed an issue where the wrong activity might get launched by the editor.</li>
<li>Android: Fixed an issue where webcam textures would take over the entire screen on JB devices.</li>
<li>Android: Fixed an issue with missing features/permissions in the AndroidManifest.</li>
<li>Android: Fixed cpu detection, some devices reported more cores than was actually present.</li>
<li>Android: Fixed error message when current build is aborted by the user.</li>
<li>Android: Fixed issue on Adreno with skinning on gles11.</li>
<li>Android: Fixed loading data on devices where /data/app is symlink'd.</li>
<li>Android: Fixed problem with status bar being hidden even though 'Status Bar Hidden' was unchecked.</li>
<li>Android: Fixed Touch.fingerId discrepancy before and after an application has been paused/resumed.</li>
<li>Android: Fullscreen video now respects lights-out mode.</li>
<li>Android: Made sure correct screen resolution is set before Awake is called on scripts.</li>
<li>Android: Touches outside TouchScreenKeyboard no longer result in a cancelation event.</li>
<li>Android: TouchScreenKeyboard.text is now set to initial value on cancel.</li>
<li>Audio: Fixed deadlock in IT playback code.</li>
<li>Audio: Replacing the AudioClip on an AudioSource no longer affects playback speed if the clips have different sampling rates.</li>
<li>Audio: Sounds started by PlayOneShot are no longer stopped by Play.</li>
<li>Documentation: Fixed documentation of MonoBehavior stating Awake() is not called for disabled behaviours.</li>
<li>DX11: Fixed render-to-cubemap (including point light shadows) on DX10.0 level GPUs.</li>
<li>Editor: Project Browser.</li>
<li>Fixed so valid drag and drops in second column removes the drag label (OSX issue only).</li>
<li>Center preview when framing. This also makes it a better experience when changing preview size, since the selected item does not jump vertically.</li>
<li>Editor: Asset name are no longer allowed to be empty.</li>
<li>Editor: Ensure selection is framed in Object Picker when showing.</li>
<li>Editor: Fix a regression when GUI could be rendered in the wrong spot in deferred mode.</li>
<li>Editor: Fix file names for web players, if they project name contains a period ('.') character.</li>
<li>Editor: Fix that Object Picker showed script assets for MonoBehavior references.</li>
<li>Editor: Fixed all known issues with the results of "Generate Lightmap UVs" being different on Windows vs. Mac.</li>
<li>Editor: Fixed crash when loading fonts from asset bundles in editor.</li>
<li>Editor: Fixed scene view "Rendering Paths" visualization mode (got broken in 4.0).</li>
<li>Editor: Fixed text mode serialization of ProjectSettings</li>
<li>Editor: Fixed using asset folders with only 16-bit Unicode characters in their file names on Mac OS X.</li>
<li>Editor: Hitting Enter on an empty "open project" window will no longer crash the editor.</li>
<li>Editor: Immediate mode GUI windows closed during the Layout event will no longer crash the editor on Windows.</li>
<li>Editor: Import package window will now open to the last directory instead of the projects root.</li>
<li>Editor: Scripts will now receive an Update after they get recompiled and re-enabled.</li>
<li>Editor: Scripts will now receive Update events as the Game window is being resized.</li>
<li>Editor: The build player window will now default back to the active build target.</li>
<li>Fix crash when using an invalid Mesh on a SkinnedMeshRenderer</li>
<li>Fix mesh compression of skinned mesh bone weights.</li>
<li>Fixed "Out of memory" error when importing empty movie file.</li>
<li>Fixed bug in the Cache Server where it runs out of memory when uploading a lot of files to it and the disk speed is very slow.</li>
<li>Fixed crash during asset creation for scenes that do UnloadUnusedAssets() from within editor scripts.</li>
<li>Fixed crash when calling Mesh.GetTriangleStrip() on an empty submesh.</li>
<li>Fixed division-by-zero in keyframe reduction for empty clips.</li>
<li>Fixed division-by-zero in Quaternion.RotateTowards() when angle between quaternions is zero.</li>
<li>Fixed outputs from previous asset import not being cleared upon failed import.</li>
<li>Fixed TextureImporter Inspector to save settings correctly when disabling the platform overrides.</li>
<li>Graphics: Fix issue when calling Camera.Render () from an image effect. Validation now takes place to ensure that the camera you are calling Render on is not the currently rendering camera.</li>
<li>Graphics: Fixed error messages with a skewed camera matrix (also coming to 4.0.1 soon).</li>
<li>Graphics: Fixed multiple point light shadows not quite working in forward rendering.</li>
<li>Graphics: Fixed rare crash with richly formatted text rendering.</li>
<li>Graphics: Fixed shadow casting of Line &amp; Trail Renderers.</li>
<li>Graphics: Respect Hard Shadows Only quality setting in Deferred rendering.</li>
<li>iOS: Fix WWW class to handle all 2xx HTTP status codes as successful.</li>
<li>iOS: Fixed an issue with native plugin inclusion when file name contains '~' symbol.</li>
<li>iOS: Fixed Camera.SetTargetBuffers issue on dx (it was considered to be rendering on screen always).</li>
<li>iOS: Fixed log output to device console when Xcode is not attached and device is running iOS 6.0 or later.</li>
<li>iOS: Fixed rare crash when acceleration events were delivered simultaneously from concurrent threads.</li>
<li>iOS: Fixed view stretching after device unlocking.</li>
<li>iOS: Main display rendering resolution can be changed correctly through both new and old API (fix for known issue).</li>
<li>License: Fixed issue with license expired errors on trials which were not yet expired.</li>
<li>Mac OS X Standalone: Fixed fullscreen mode bugs on OS X 10.6</li>
<li>Mecanim: Fix root motion when you have a CharacterController disabled, now the Animator should correctly apply the root motion to your GO when the CharacterController is disabled.</li>
<li>Mecanim: Fixed @ conventions for Humanoid animations.</li>
<li>Mecanim: Fixed character orientation not being correct on some assets.</li>
<li>Mecanim: Fixed crash when BlendTree child node as a 0 speed.</li>
<li>Mecanim: Fixed crash when deleting certain Sub StateMachine.</li>
<li>Mecanim: Fixed crash when editing a playing animation in DCC while game is playing.</li>
<li>Mecanim: Fixed deletion of multiple Transitions.</li>
<li>Mecanim: Fixed DeltaPosition/Rotation with generic animation.</li>
<li>Mecanim: Fixed Generic animation loosing root motion on additionnal masked layer.</li>
<li>Mecanim: Fixed mouth of character opening during Mirror.</li>
<li>Mecanim: Fixed revert button not working in Avatar setup tool.</li>
<li>Mecanim: Fixed spinning wrist on some retargeted animation.</li>
<li>Mecanim: Fixed State timing being wrong when editing Animation Start/Stop time.</li>
<li>Mecanim: Fixed undo of Parameter deletion.</li>
<li>Mecanim: Fixed warning when using ApplyRootMotion with Kinematic RigidBodies.</li>
<li>Mecanim: Generic Avatars do not show Configure button.</li>
<li>NavMesh: Fixed issue where agents isPathStale flag was not set correctly when changing walkableMask or navmesh layer cost.</li>
<li>NavMesh: Fixed issue where OffMeshLinks would sometimes wrongly generate two-way instead of one-way links.</li>
<li>NavMesh: Fixed issue where setting an invalid path on agent would return true.</li>
<li>Physics: Fix CharacterController.bounds.</li>
<li>Shaders: Fixed various issues in HLSL-&gt;GLSL shader translator; most notably nested loops now work properly.</li>
<li>Shuriken: Fixed a memory leak (also coming to 4.0.1 soon).</li>
<li>Shuriken: Fixed angular velocity setting range being clamped to 0..1.</li>
<li>Shuriken: Fixed crash on a particle system without a particle renderer.</li>
<li>Shuriken: Fixed wrong Shape in presence of parenting with scale (also coming to 4.0.1 soon).</li>
<li>Substance: Baking substances textures on X360 is fixed.</li>
<li>Substance: Fixed "Export Bitmaps".</li>
<li>Substance: isLoadTimeGenerated can be set again.</li>
<li>Substance: When baking compressed textures for iOS, only square PVRTC textures are baked.</li>
<li>Substance: when updating projects from older versions, substances should now have all their parameters displayed in the inspector.</li>
<li>Terrain: Fixed too dark unlit side in tree creator billboard shaders.</li>
<li>Time.deltaTime is now correctly set to 0 when starting up with Time.timeScale=0.</li>
<li>Web Player: Fix using WWW class in use cases where yield is never called on the WWW instance.</li>
<li>Web Player: Web player channels can now be used to downgrade a channel if a newer version then intended had been downloaded</li>
<li>Webplayer: Maximum bound socket count is now 50, addresses security issue.</li>
<li>Windows: Fix crash when hitting "Quit" in standalone player configuration dialog.</li>
<li>Windows: Fixed rare crash of standalone players when exiting back to desktop.</li>
<li>Xbox360: Fixed crash when calling Application.Quit in scenes containing XMA encoded AudioClips.</li>
</ul>
