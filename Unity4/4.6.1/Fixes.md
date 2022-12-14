# Unity 4.6.1

https://unity3d.com/unity/whats-new/unity-4.6.1

## Fixes



*   Android: Added splitting of level files in APK to fix slow loading problem.
*   Android: Avoid reading expensive metrics in DisplayInfo more than once per frame.
*   Android: Fixed crash on certain Adreno HW with OS version 4.4.2 or more recent 4.4.x.
*   Android: Fixed crash on XPeria Play.
*   Android: Fixed forwarding of input events to Java when Unity is paused but activity is still running.
*   Android: Fixed frame rate on Tegra devices when doing GPU profiling.
*   Android: Workaround for corrupted font textures on older Adreno drivers.
*   Android: Fixed a crash in glDrawElements() on some devices.
*   Android: Fixed an issue with ProGuard when obfuscating an exported project.
*   Android: Fixed build-tools version check.
*   Android: Fixed erratic touch input when not using NativeActivity.
*   Android: Fixed NEON detection on 64 bit Android.
*   Android: Fixed Unity UI ScrollView/Mask on PowerVR SGX.
*   Android: Joystick input optimization; fixed slowdown on some older devices.
*   Android: Support for xxxhdpi icons.
*   Android: Updated SDK and JDK requirements to match Android 5.0.
*   Android: Added additional fallback font "DroidSansFallback" (but also keeping "Droid Sans Fallback") to fix for e.g. Korean font on older Android devices. Asian fonts are still not working on many - Android 5 devices.
*   Asset Loading: Fixed performance regression when loading scene in the Editor.
*   Audio: Not streamed VBR audio files loaded with WWW.GetAudioClip now play and loop correctly.
*   Core: Fixed undoing Add/Remove RectTransform and will no long break the scene gizmos.
*   Core: Fixed bug in anchoredPosition3D property on RectTransform that caused coordinates to be swapped.
*   Debugger: Fixed crash when stepping into a breakpoint on 64-bit OSX standalone player.
*   DX9: Add black bars in fullscreen mode to maintain aspect ratio.
*   DX11: Fixed GPU video memory detection on some GPUs. Was wrongly disabling shadows & deferred on some Intel ones, for example.
*   Editor: Fixed asset bundle building stealing window focus when Editor is in the background.
*   Editor: Fixed version control plugin and shader compiler sometimes stopping prematurely.
*   Editor: Fixed crash on scene load when prefabs have unsaved child objects.
*   Editor: Add support for importing .DDS cubemaps.
*   Editor: Fixed selection change being undone if click also initiates a drag (Windows only).
*   Editor: Corrected a problem launching MonoDevelop and moving to the proper line of a script file on OSX.
*   Editor: Fixed the error thrown when closing asset label list with escape key.
*   Editor: Reduced memory usage of streamed audio clips.
*   Editor: Fixed AssetModificationProcessor.OnWillSaveAssets checking out files that were not Saved and OnWillDeleteAssets always marking assets for delete.
*   Editor: Fixed Canvas editor for nested Canvas showing UI as if it were a root Canvas if the GameObject was inactive.
*   Editor: Fixed Canvas editor which was not working well with multi-object editing.
*   Editor: Sprite asset inspector in single mode now shows correct values.
*   OpenGL ES :Changed default PlayerSettings Graphics Level to Auto for all platforms using OpenGL ES (was Force OpenGL ES 2).
*   OpenGL ES: Sphere map texture coordinate generation fixes.
*   Graphics: Fixed custom cursors when hovering over black bars in fullscreen mode.
*   Graphics: Fixed incorrect sprite tangent handling on ARM NEON capable devices.
*   Graphics: Fixed occasional crashes when switching the graphics device. Happens in editor when toggling between DX9 and DX11, or on Windows Phone when resuming the app.
*   GUI: Fixed vertical position of text cursor.
*   Inspector: Fixed bool properties with DecoratorDrawers not reserving space for them correctly.
*   Inspector: Disable the asset label editor UI if any of the selected assets are not open for edit.
*   iOS: Add player setting to target iOS 8.0 and 8.1.
*   iOS: Disable tree billboard mipmaps; mipmap generation was causing hiccups.
*   iOS: Do not use AVAudioSessionRouteChangeNotification on pre-iOS6 devices.
*   iOS: Fixed a memory leak in QueryADID().
*   iOS: Fixed visual issues when setting screen orientation via Screen.orientation.
*   iOS: Added support for iPad Mini 3 and iPad Air 2.
*   iOS: Fixed splash screen issues on iPhone 6+, and frame buffer resolution issues.
*   iOS: Fixed crash in Resources.UnloadUnusedAssets after GameCenter login.
*   iOS: Removed unnecessary error messages in GameCenter API.
*   iOS: Don't count the size of the executable twice in the detailed profiler memory snapshot.
*   iOS: Fixed player remaining paused after interstitial ads in certain cases.
*   iOS: Fixed click-through in on-screen keyboard.
*   iOS: Fixed crash when Game Controller gets attached on iOS 8.
*   iOS: Fixed debug log spam in Social API.
*   iOS: Fixed iAD Show method crash when calling it while Ad is not yet loaded.
*   iOS: Fixed WWW crash.
*   iOS: Xcode 6 fixes - OSX no longer have BGRA\_EXT; allow iOS8 sdk.
*   iOS: Added support for iPhone 6 icons.
*   iOS: Fixed a crash when a broken socket is written into.
*   iOS: Fixed DPI estimation for newer devices.
*   iOS: Fixed location support on iOS 8.
*   iOS: Fixed memory leak in WWW class.
*   iOS: Report size of assemblies after bytecode stripping to reduce ambiguity.
*   iOS: Work around an Xcode splash screen bug in iOS 8 landscape iPhone apps.
*   iOS: Added OnApplicationFocus() support.
*   iOS: Fixed a linker issue breaking simulator builds.
*   iOS: Fixed a crash in when closing Game Center leaderboard under specific conditions.
*   iOS: Use new font file location on iOS 8.2.
*   License: Activation on OS X 10.10 Yosemite failed on some older hardware.
*   Linux: Fixed incorrect behaviour on large XFS filesystems.
*   Linux: Don't report button/axis data when input field has focus.
*   Linux: Fixed numeric keypad input.
*   Mac OS X Standalone player: Use old location for Application.persistentDataPath if it exists.
*   Mac OS X: Fixed File limits not being set to Maximum amount and Defaulting to 256 open files.
*   Mac OS X: Bring back GPU profiler for NVIDIA GPUs on 10.9 and newer versions.
*   Mecanim: Fixed AnimatorController not being built properly when used in prefabs.
*   Mecanim: Fixed AnyState transitions disappearing in some specific cases.
*   Mecanim: Fixed transitions being duplicated when dragging StateMachines into StateMachines.
*   Mecanim: Show an error when transitions to state that doesn't exist are found.
*   Mono: Fixed issue with System.Console.InputEncoding and System.Console.OutputEncoding not changing the encoding when set.
*   OpenGL: Fixed fullscreen rendering on Windows.
*   Physics 2D: Added Physics2D.minPenetrationForPenalty property to control the penetration radius allowed before any separation impulse for is applied.
*   Physics 2D: Changing 2D collider state between trigger and non-trigger modes now maintains contact state (enter/stay/exit callbacks are correct).
*   Physics 2D: CircleCollider2D editing handles now show in the correct location when X/Y rotation is involved.
*   Physics 2D: Provide option to turn on/off the ability to detect a collider that overlaps the start of any 2D line/ray cast
*   Physics 2D: RaycastHit2D distance is now correctly calculated.
*   Physics 2D: ReferenceAngle for both HingeJoint2D and SliderJoint2D are now maintained when the components are disabled then re-enabled.
*   Physics 2D: Rigidody2D.MovePosition() no longer causes gravity to be ignored when in constant use.
*   Physics 2D: PhysicsMaterial2D bounciness now has an upper limit of 100000 rather than 1.
*   Physics 2D: Ensure that Physics2D.Raycast(all) does not produce an infinite end-point resulting in nothing being hit.
*   Physics 2D: Fixed bad Rigidbody2D interpolation when changing body position via a Transform component change.
*   Physics 2D: 2D physics colliders now correctly transform under full 3D rotation.
*   Scripting: Fixed stack overflow in class loader.
*   Scripting: Fixed Win32\_IN6\_ADDR.
*   Shaders: Fixed support for more than 16 textures on D3D11.
*   Shaders: Fixed view\*projection matrix (UNITY\_MATRIX\_VP) sometimes getting out of sync.
*   Shaders: Fixed wrong OpenGL ES 3.0 shader code generation in some cases of tangents and glsl\_no\_auto\_normalization being used simultaneously.
*   Standalone: Fixed random crash in 64-bit standalone players.
*   Standalone: Don't force-reload textures/shaders on resolution change, meaning AssetBundle.Unload(false) works as expected again.
*   Substance: Empty image inputs slots are now treated as transparent black.
*   Substance: Fixed "ThreadedObjectActivationQueue not empty" assert.
*   Substance: Some output computations would sometimes not take place when the content of image inputs had changed programmatically.
*   TouchInput: Switched timestamps from ms to us internally, to avoid 0-length delta times.
*   UI: Fixed an issue with some UI shaders not 1/2 texel offsetting correctly on DX9.
*   UI: Disabled layout components are now disregarded from layout calculations.
*   UI: Fixed memory leak in material when reloading assemblies in the editor.
*   UI: Fixed bug where Slider would snap handle to center around cursor when dragging handle instead of retaining the position of the cursor inside the handle.
*   UI: Fixed crash when stripping was enabled.
*   UI: Fixed error message when prefab was loaded that contained a input field.
*   UI: Fixed InputField bug that text did not visibly update when the text property was set from scripting.
*   UI: Fixed InputField OnValueChange not being called when setting InputField.text from script.
*   UI: Fixed issue in GridLayoutGroup that would cause elements to sometimes be offset wrong depending on what startCorner mode was used.
*   UI: fixed issue where input field would not be activated properly if navigation was None.
*   UI: Fixed logic for getting or creating Canvas when creating UI element, which sometimes failed to create a Canvas. -UI: Fixed Selectable logic to find adjacent Selectable in a given direction, which was applying the rotation twice in the logic, producing incorrect results for objects with rotation.
*   UI: InputField now calls UpdateLabel when textComponent get a SetLayoutDirty.
*   UI: Make sure we only notify children of mask state change after we have disabled the parent. This means that the children will be able to correctly examine the mask state.
*   UI: Make the canvas group a behaviour so it can be enabled / disabled. Updated code that uses this group to properly handle disabled groups, and not change the values when enabling or disabling.
*   UI: Only send end drag events when we end dragging, not on all pointer up events.
*   UI: Fixed issue where sort overridden canvas wouldn't get their depth set and therefore no events.
*   UI: Fixed issue where return on touch keyboard would not submit even if MultiLineSubmit was selected.
*   UnityEvents: Fixed an issue where modifying a unity event during invoke could lead to corruption of the UnityEvent, and events not being called properly.
*   UnityEvents: Fixed an issue with code stripping on iOS which was causing some UnityEvent calls to throw a null reference exception.
*   Version Control: Removed warning when saving scene and Perforce integration was enabled.
*   Version Control: Allow changing credentials and reconnect even when a connection is already being established.
*   Version Control: Get rid of double messages in the console windows from a range of VCS commands.
*   Version Control: Fixed plugin stop when reading a recent deleted file.
*   Version Control: Removed out-of-sync state when file is deleted on server.
*   Version Control: Revert recursively.
*   Video: Non Unity-encoded video no longer has a duration of -1.
*   WebPlayer: Mac x86\_64 web plugin loads proper x86\_64 Mono bundles.
*   WebPlayer: Fixed a security issue.
*   Windows Phone: Texture.ReadPixels works correctly in landscape modes.
*   Windows Phone/Store Apps: Fixed crash that sometimes happened on Application.LoadLevelAsync.
*   Windows Phone/Store Apps: Fixed an issue which caused UnityScript methods that return an IEnumerator but that do not yield throw exception on execution.
*   Windows Phone/Store Apps: Referencing generic methods in scripts no longer crashes the build.
*   Windows Phone/Store Apps: Fixed a memory leak and in rare cases a crash when doing a lot of async loading.
*   Windows Phone: Fixed touchscreen keyboard reappearing after pressing back button while GUI.TextArea has focus (WP8.1 apps only).
*   Windows Phone: Fixed an issue which caused Lumia 530 devices to freeze with black screen (WP8.1 apps only).
*   Windows Player: Fixed custom cursors not showing up correctly in fullscreen mode.
*   Windows Player: Fixed window being always on top after switching from DX9 fullscreen to desktop windowed mode.
*   Windows Store Apps: Using Winmd C++ plugins should work correctly now.
*   Windows Store Apps: It is now possible to launch Unity WSA player on-demand.