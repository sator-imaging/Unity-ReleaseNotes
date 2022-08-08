# Unity 4.1

https://unity3d.com/unity/whats-new/unity-4.1

## Fixes



*   Android/iOS: Updated PrefetchSocketPolicy() to return true instead of throwing an exception.
*   Android: Added local ref cleanup code to AndroidJNI to support more user based local refs per frame.
*   Android: Added manifest flags to avoid multiple instances of the same application.
*   Android: Added the ability to pass null arguments through the JNI bridge.
*   Android: Added workaround for "Could not reserve enough space for object heap" error.
*   Android: Added workaround for Tegra shader compiler bug when texture samplers are not reported.
*   Android: Fixed "Unity Remote" accelerometer input.
*   Android: Fixed a crash when returning to main Activity after downloading an OBB, when using development player.
*   Android: Fixed an issue where async updates of the TouchScreenKeyboard.text property would void any input from the keyboard.
*   Android: Fixed an issue where huge switch case statements could crash/yield the wrong result.
*   Android: Fixed an issue where the application would consume a significant amount of cpu even though the application was paused.
*   Android: Fixed an issue where the wrong activity might get launched by the editor.
*   Android: Fixed an issue where webcam textures would take over the entire screen on JB devices.
*   Android: Fixed an issue with missing features/permissions in the AndroidManifest.
*   Android: Fixed cpu detection, some devices reported more cores than was actually present.
*   Android: Fixed error message when current build is aborted by the user.
*   Android: Fixed issue on Adreno with skinning on gles11.
*   Android: Fixed loading data on devices where /data/app is symlink'd.
*   Android: Fixed problem with status bar being hidden even though 'Status Bar Hidden' was unchecked.
*   Android: Fixed Touch.fingerId discrepancy before and after an application has been paused/resumed.
*   Android: Fullscreen video now respects lights-out mode.
*   Android: Made sure correct screen resolution is set before Awake is called on scripts.
*   Android: Touches outside TouchScreenKeyboard no longer result in a cancelation event.
*   Android: TouchScreenKeyboard.text is now set to initial value on cancel.
*   Audio: Fixed deadlock in IT playback code.
*   Audio: Replacing the AudioClip on an AudioSource no longer affects playback speed if the clips have different sampling rates.
*   Audio: Sounds started by PlayOneShot are no longer stopped by Play.
*   Documentation: Fixed documentation of MonoBehavior stating Awake() is not called for disabled behaviours.
*   DX11: Fixed render-to-cubemap (including point light shadows) on DX10.0 level GPUs.
*   Editor: Project Browser.
*   Fixed so valid drag and drops in second column removes the drag label (OSX issue only).
*   Center preview when framing. This also makes it a better experience when changing preview size, since the selected item does not jump vertically.
*   Editor: Asset name are no longer allowed to be empty.
*   Editor: Ensure selection is framed in Object Picker when showing.
*   Editor: Fix a regression when GUI could be rendered in the wrong spot in deferred mode.
*   Editor: Fix file names for web players, if they project name contains a period ('.') character.
*   Editor: Fix that Object Picker showed script assets for MonoBehavior references.
*   Editor: Fixed all known issues with the results of "Generate Lightmap UVs" being different on Windows vs. Mac.
*   Editor: Fixed crash when loading fonts from asset bundles in editor.
*   Editor: Fixed scene view "Rendering Paths" visualization mode (got broken in 4.0).
*   Editor: Fixed text mode serialization of ProjectSettings
*   Editor: Fixed using asset folders with only 16-bit Unicode characters in their file names on Mac OS X.
*   Editor: Hitting Enter on an empty "open project" window will no longer crash the editor.
*   Editor: Immediate mode GUI windows closed during the Layout event will no longer crash the editor on Windows.
*   Editor: Import package window will now open to the last directory instead of the projects root.
*   Editor: Scripts will now receive an Update after they get recompiled and re-enabled.
*   Editor: Scripts will now receive Update events as the Game window is being resized.
*   Editor: The build player window will now default back to the active build target.
*   Fix crash when using an invalid Mesh on a SkinnedMeshRenderer
*   Fix mesh compression of skinned mesh bone weights.
*   Fixed "Out of memory" error when importing empty movie file.
*   Fixed bug in the Cache Server where it runs out of memory when uploading a lot of files to it and the disk speed is very slow.
*   Fixed crash during asset creation for scenes that do UnloadUnusedAssets() from within editor scripts.
*   Fixed crash when calling Mesh.GetTriangleStrip() on an empty submesh.
*   Fixed division-by-zero in keyframe reduction for empty clips.
*   Fixed division-by-zero in Quaternion.RotateTowards() when angle between quaternions is zero.
*   Fixed outputs from previous asset import not being cleared upon failed import.
*   Fixed TextureImporter Inspector to save settings correctly when disabling the platform overrides.
*   Graphics: Fix issue when calling Camera.Render () from an image effect. Validation now takes place to ensure that the camera you are calling Render on is not the currently rendering camera.
*   Graphics: Fixed error messages with a skewed camera matrix (also coming to 4.0.1 soon).
*   Graphics: Fixed multiple point light shadows not quite working in forward rendering.
*   Graphics: Fixed rare crash with richly formatted text rendering.
*   Graphics: Fixed shadow casting of Line & Trail Renderers.
*   Graphics: Respect Hard Shadows Only quality setting in Deferred rendering.
*   iOS: Fix WWW class to handle all 2xx HTTP status codes as successful.
*   iOS: Fixed an issue with native plugin inclusion when file name contains '~' symbol.
*   iOS: Fixed Camera.SetTargetBuffers issue on dx (it was considered to be rendering on screen always).
*   iOS: Fixed log output to device console when Xcode is not attached and device is running iOS 6.0 or later.
*   iOS: Fixed rare crash when acceleration events were delivered simultaneously from concurrent threads.
*   iOS: Fixed view stretching after device unlocking.
*   iOS: Main display rendering resolution can be changed correctly through both new and old API (fix for known issue).
*   License: Fixed issue with license expired errors on trials which were not yet expired.
*   Mac OS X Standalone: Fixed fullscreen mode bugs on OS X 10.6
*   Mecanim: Fix root motion when you have a CharacterController disabled, now the Animator should correctly apply the root motion to your GO when the CharacterController is disabled.
*   Mecanim: Fixed @ conventions for Humanoid animations.
*   Mecanim: Fixed character orientation not being correct on some assets.
*   Mecanim: Fixed crash when BlendTree child node as a 0 speed.
*   Mecanim: Fixed crash when deleting certain Sub StateMachine.
*   Mecanim: Fixed crash when editing a playing animation in DCC while game is playing.
*   Mecanim: Fixed deletion of multiple Transitions.
*   Mecanim: Fixed DeltaPosition/Rotation with generic animation.
*   Mecanim: Fixed Generic animation loosing root motion on additionnal masked layer.
*   Mecanim: Fixed mouth of character opening during Mirror.
*   Mecanim: Fixed revert button not working in Avatar setup tool.
*   Mecanim: Fixed spinning wrist on some retargeted animation.
*   Mecanim: Fixed State timing being wrong when editing Animation Start/Stop time.
*   Mecanim: Fixed undo of Parameter deletion.
*   Mecanim: Fixed warning when using ApplyRootMotion with Kinematic RigidBodies.
*   Mecanim: Generic Avatars do not show Configure button.
*   NavMesh: Fixed issue where agents isPathStale flag was not set correctly when changing walkableMask or navmesh layer cost.
*   NavMesh: Fixed issue where OffMeshLinks would sometimes wrongly generate two-way instead of one-way links.
*   NavMesh: Fixed issue where setting an invalid path on agent would return true.
*   Physics: Fix CharacterController.bounds.
*   Shaders: Fixed various issues in HLSL->GLSL shader translator; most notably nested loops now work properly.
*   Shuriken: Fixed a memory leak (also coming to 4.0.1 soon).
*   Shuriken: Fixed angular velocity setting range being clamped to 0..1.
*   Shuriken: Fixed crash on a particle system without a particle renderer.
*   Shuriken: Fixed wrong Shape in presence of parenting with scale (also coming to 4.0.1 soon).
*   Substance: Baking substances textures on X360 is fixed.
*   Substance: Fixed "Export Bitmaps".
*   Substance: isLoadTimeGenerated can be set again.
*   Substance: When baking compressed textures for iOS, only square PVRTC textures are baked.
*   Substance: when updating projects from older versions, substances should now have all their parameters displayed in the inspector.
*   Terrain: Fixed too dark unlit side in tree creator billboard shaders.
*   Time.deltaTime is now correctly set to 0 when starting up with Time.timeScale=0.
*   Web Player: Fix using WWW class in use cases where yield is never called on the WWW instance.
*   Web Player: Web player channels can now be used to downgrade a channel if a newer version then intended had been downloaded
*   Webplayer: Maximum bound socket count is now 50, addresses security issue.
*   Windows: Fix crash when hitting "Quit" in standalone player configuration dialog.
*   Windows: Fixed rare crash of standalone players when exiting back to desktop.
*   Xbox360: Fixed crash when calling Application.Quit in scenes containing XMA encoded AudioClips.