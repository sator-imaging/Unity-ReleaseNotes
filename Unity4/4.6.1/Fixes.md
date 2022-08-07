# Unity 4.6.1
https://unity3d.com/unity/whats-new/unity-4.6.1

## Fixes

<ul>
<li>Android: Added splitting of level files in APK to fix slow loading problem.</li>
<li>Android: Avoid reading expensive metrics in DisplayInfo more than once per frame.</li>
<li>Android: Fixed crash on certain Adreno HW with OS version 4.4.2 or more recent 4.4.x.</li>
<li>Android: Fixed crash on XPeria Play.</li>
<li>Android: Fixed forwarding of input events to Java when Unity is paused but activity is still running.</li>
<li>Android: Fixed frame rate on Tegra devices when doing GPU profiling.</li>
<li>Android: Workaround for corrupted font textures on older Adreno drivers.</li>
<li>Android: Fixed a crash in glDrawElements() on some devices.</li>
<li>Android: Fixed an issue with ProGuard when obfuscating an exported project.</li>
<li>Android: Fixed build-tools version check.</li>
<li>Android: Fixed erratic touch input when not using NativeActivity.</li>
<li>Android: Fixed NEON detection on 64 bit Android.</li>
<li>Android: Fixed Unity UI ScrollView/Mask on PowerVR SGX.</li>
<li>Android: Joystick input optimization; fixed slowdown on some older devices.</li>
<li>Android: Support for xxxhdpi icons.</li>
<li>Android: Updated SDK and JDK requirements to match Android 5.0.</li>
<li>Android: Added additional fallback font "DroidSansFallback" (but also keeping "Droid Sans Fallback") to fix for e.g. Korean font on older Android devices. Asian fonts are still not working on many - Android 5 devices.</li>
<li>Asset Loading: Fixed performance regression when loading scene in the Editor.</li>
<li>Audio: Not streamed VBR audio files loaded with WWW.GetAudioClip now play and loop correctly.</li>
<li>Core: Fixed undoing Add/Remove RectTransform and will no long break the scene gizmos.</li>
<li>Core: Fixed bug in anchoredPosition3D property on RectTransform that caused coordinates to be swapped.</li>
<li>Debugger: Fixed crash when stepping into a breakpoint on 64-bit OSX standalone player.</li>
<li>DX9: Add black bars in fullscreen mode to maintain aspect ratio.</li>
<li>DX11: Fixed GPU video memory detection on some GPUs. Was wrongly disabling shadows &amp; deferred on some Intel ones, for example.</li>
<li>Editor: Fixed asset bundle building stealing window focus when Editor is in the background.</li>
<li>Editor: Fixed version control plugin and shader compiler sometimes stopping prematurely.</li>
<li>Editor: Fixed crash on scene load when prefabs have unsaved child objects.</li>
<li>Editor: Add support for importing .DDS cubemaps.</li>
<li>Editor: Fixed selection change being undone if click also initiates a drag (Windows only).</li>
<li>Editor: Corrected a problem launching MonoDevelop and moving to the proper line of a script file on OSX.</li>
<li>Editor: Fixed the error thrown when closing asset label list with escape key.</li>
<li>Editor: Reduced memory usage of streamed audio clips.</li>
<li>Editor: Fixed AssetModificationProcessor.OnWillSaveAssets checking out files that were not Saved and OnWillDeleteAssets always marking assets for delete.</li>
<li>Editor: Fixed Canvas editor for nested Canvas showing UI as if it were a root Canvas if the GameObject was inactive.</li>
<li>Editor: Fixed Canvas editor which was not working well with multi-object editing.</li>
<li>Editor: Sprite asset inspector in single mode now shows correct values.</li>
<li>OpenGL ES :Changed default PlayerSettings Graphics Level to Auto for all platforms using OpenGL ES (was Force OpenGL ES 2).</li>
<li>OpenGL ES: Sphere map texture coordinate generation fixes.</li>
<li>Graphics: Fixed custom cursors when hovering over black bars in fullscreen mode.</li>
<li>Graphics: Fixed incorrect sprite tangent handling on ARM NEON capable devices.</li>
<li>Graphics: Fixed occasional crashes when switching the graphics device. Happens in editor when toggling between DX9 and DX11, or on Windows Phone when resuming the app.</li>
<li>GUI: Fixed vertical position of text cursor.</li>
<li>Inspector: Fixed bool properties with DecoratorDrawers not reserving space for them correctly.</li>
<li>Inspector: Disable the asset label editor UI if any of the selected assets are not open for edit.</li>
<li>iOS: Add player setting to target iOS 8.0 and 8.1.</li>
<li>iOS: Disable tree billboard mipmaps; mipmap generation was causing hiccups.</li>
<li>iOS: Do not use AVAudioSessionRouteChangeNotification on pre-iOS6 devices.</li>
<li>iOS: Fixed a memory leak in QueryADID().</li>
<li>iOS: Fixed visual issues when setting screen orientation via Screen.orientation.</li>
<li>iOS: Added support for iPad Mini 3 and iPad Air 2.</li>
<li>iOS: Fixed splash screen issues on iPhone 6+, and frame buffer resolution issues.</li>
<li>iOS: Fixed crash in Resources.UnloadUnusedAssets after GameCenter login.</li>
<li>iOS: Removed unnecessary error messages in GameCenter API.</li>
<li>iOS: Don't count the size of the executable twice in the detailed profiler memory snapshot.</li>
<li>iOS: Fixed player remaining paused after interstitial ads in certain cases.</li>
<li>iOS: Fixed click-through in on-screen keyboard.</li>
<li>iOS: Fixed crash when Game Controller gets attached on iOS 8.</li>
<li>iOS: Fixed debug log spam in Social API.</li>
<li>iOS: Fixed iAD Show method crash when calling it while Ad is not yet loaded.</li>
<li>iOS: Fixed WWW crash.</li>
<li>iOS: Xcode 6 fixes - OSX no longer have BGRA_EXT; allow iOS8 sdk.</li>
<li>iOS: Added support for iPhone 6 icons.</li>
<li>iOS: Fixed a crash when a broken socket is written into.</li>
<li>iOS: Fixed DPI estimation for newer devices.</li>
<li>iOS: Fixed location support on iOS 8.</li>
<li>iOS: Fixed memory leak in WWW class.</li>
<li>iOS: Report size of assemblies after bytecode stripping to reduce ambiguity.</li>
<li>iOS: Work around an Xcode splash screen bug in iOS 8 landscape iPhone apps.</li>
<li>iOS: Added OnApplicationFocus() support.</li>
<li>iOS: Fixed a linker issue breaking simulator builds.</li>
<li>iOS: Fixed a crash in when closing Game Center leaderboard under specific conditions.</li>
<li>iOS: Use new font file location on iOS 8.2.</li>
<li>License: Activation on OS X 10.10 Yosemite failed on some older hardware.</li>
<li>Linux: Fixed incorrect behaviour on large XFS filesystems.</li>
<li>Linux: Don't report button/axis data when input field has focus.</li>
<li>Linux: Fixed numeric keypad input.</li>
<li>Mac OS X Standalone player: Use old location for Application.persistentDataPath if it exists.</li>
<li>Mac OS X: Fixed File limits not being set to Maximum amount and Defaulting to 256 open files.</li>
<li>Mac OS X: Bring back GPU profiler for NVIDIA GPUs on 10.9 and newer versions.</li>
<li>Mecanim: Fixed AnimatorController not being built properly when used in prefabs.</li>
<li>Mecanim: Fixed AnyState transitions disappearing in some specific cases.</li>
<li>Mecanim: Fixed transitions being duplicated when dragging StateMachines into StateMachines.</li>
<li>Mecanim: Show an error when transitions to state that doesn't exist are found.</li>
<li>Mono:  Fixed issue with System.Console.InputEncoding and System.Console.OutputEncoding not changing the encoding when set.</li>
<li>OpenGL: Fixed fullscreen rendering on Windows.</li>
<li>Physics 2D: Added Physics2D.minPenetrationForPenalty property to control the penetration radius allowed before any separation impulse for is applied.</li>
<li>Physics 2D: Changing 2D collider state between trigger and non-trigger modes now maintains contact state (enter/stay/exit callbacks are correct).</li>
<li>Physics 2D: CircleCollider2D editing handles now show in the correct location when X/Y rotation is involved.</li>
<li>Physics 2D: Provide option to turn on/off the ability to detect a collider that overlaps the start of any 2D line/ray cast</li>
<li>Physics 2D: RaycastHit2D distance is now correctly calculated.</li>
<li>Physics 2D: ReferenceAngle for both HingeJoint2D and SliderJoint2D are now maintained when the components are disabled then re-enabled.</li>
<li>Physics 2D: Rigidody2D.MovePosition() no longer causes gravity to be ignored when in constant use.</li>
<li>Physics 2D: PhysicsMaterial2D bounciness now has an upper limit of 100000 rather than 1.</li>
<li>Physics 2D: Ensure that Physics2D.Raycast(all) does not produce an infinite end-point resulting in nothing being hit.</li>
<li>Physics 2D: Fixed bad Rigidbody2D interpolation when changing body position via a Transform component change.</li>
<li>Physics 2D: 2D physics colliders now correctly transform under full 3D rotation.</li>
<li>Scripting: Fixed stack overflow in class loader.</li>
<li>Scripting: Fixed Win32_IN6_ADDR.</li>
<li>Shaders: Fixed support for more than 16 textures on D3D11.</li>
<li>Shaders: Fixed view*projection matrix (UNITY_MATRIX_VP) sometimes getting out of sync.</li>
<li>Shaders: Fixed wrong OpenGL ES 3.0 shader code generation in some cases of tangents and glsl_no_auto_normalization being used simultaneously.</li>
<li>Standalone: Fixed random crash in 64-bit standalone players.</li>
<li>Standalone: Don't force-reload textures/shaders on resolution change, meaning AssetBundle.Unload(false) works as expected again.</li>
<li>Substance: Empty image inputs slots are now treated as transparent black.</li>
<li>Substance: Fixed "ThreadedObjectActivationQueue not empty" assert.</li>
<li>Substance: Some output computations would sometimes not take place when the content of image inputs had changed programmatically.</li>
<li>TouchInput: Switched timestamps from ms to us internally, to avoid 0-length delta times.</li>
<li>UI: Fixed an issue with some UI shaders not 1/2 texel offsetting correctly on DX9.</li>
<li>UI: Disabled layout components are now disregarded from layout calculations.</li>
<li>UI: Fixed memory leak in material when reloading assemblies in the editor.</li>
<li>UI: Fixed bug where Slider would snap handle to center around cursor when dragging handle instead of retaining the position of the cursor inside the handle.</li>
<li>UI: Fixed crash when stripping was enabled.</li>
<li>UI: Fixed error message when prefab was loaded that contained a input field.</li>
<li>UI: Fixed InputField bug that text did not visibly update when the text property was set from scripting.</li>
<li>UI: Fixed InputField OnValueChange not being called when setting InputField.text from script.</li>
<li>UI: Fixed issue in GridLayoutGroup that would cause elements to sometimes be offset wrong depending on what startCorner mode was used.</li>
<li>UI: fixed issue where input field would not be activated properly if navigation was None.</li>
<li>UI: Fixed logic for getting or creating Canvas when creating UI element, which sometimes failed to create a Canvas. -UI: Fixed Selectable logic to find adjacent Selectable in a given direction, which was applying the rotation twice in the logic, producing incorrect results for objects with rotation.</li>
<li>UI: InputField now calls UpdateLabel when textComponent get a SetLayoutDirty.</li>
<li>UI: Make sure we only notify children of mask state change after we have disabled the parent. This means that the children will be able to correctly examine the mask state.</li>
<li>UI: Make the canvas group a behaviour so it can be enabled / disabled. Updated code that uses this group to properly handle disabled groups, and not change the values when enabling or disabling.</li>
<li>UI: Only send end drag events when we end dragging, not on all pointer up events.</li>
<li>UI:  Fixed issue where sort overridden canvas wouldn't get their depth set and therefore no events.</li>
<li>UI: Fixed issue where return on touch keyboard would not submit even if MultiLineSubmit was selected.</li>
<li>UnityEvents: Fixed an issue where modifying a unity event during invoke could lead to corruption of the UnityEvent, and events not being called properly.</li>
<li>UnityEvents: Fixed an issue with code stripping on iOS which was causing some UnityEvent calls to throw a null reference exception.</li>
<li>Version Control: Removed warning when saving scene and Perforce integration was enabled.</li>
<li>Version Control: Allow changing credentials and reconnect even when a connection is already being established.</li>
<li>Version Control: Get rid of double messages in the console windows from a range of VCS commands.</li>
<li>Version Control: Fixed plugin stop when reading a recent deleted file.</li>
<li>Version Control: Removed out-of-sync state when file is deleted on server.</li>
<li>Version Control: Revert recursively.</li>
<li>Video: Non Unity-encoded video no longer has a duration of -1.</li>
<li>WebPlayer: Mac x86_64 web plugin loads proper x86_64 Mono bundles.</li>
<li>WebPlayer: Fixed a security issue.</li>
<li>Windows Phone: Texture.ReadPixels works correctly in landscape modes.</li>
<li>Windows Phone/Store Apps: Fixed crash that sometimes happened on Application.LoadLevelAsync.</li>
<li>Windows Phone/Store Apps: Fixed an issue which caused UnityScript methods that return an IEnumerator but that do not yield throw exception on execution.</li>
<li>Windows Phone/Store Apps: Referencing generic methods in scripts no longer crashes the build.</li>
<li>Windows Phone/Store Apps: Fixed a memory leak and in rare cases a crash when doing a lot of async loading.</li>
<li>Windows Phone: Fixed touchscreen keyboard reappearing after pressing back button while GUI.TextArea has focus (WP8.1 apps only).</li>
<li>Windows Phone: Fixed an issue which caused Lumia 530 devices to freeze with black screen (WP8.1 apps only).</li>
<li>Windows Player: Fixed custom cursors not showing up correctly in fullscreen mode.</li>
<li>Windows Player: Fixed window being always on top after switching from DX9 fullscreen to desktop windowed mode.</li>
<li>Windows Store Apps: Using Winmd C++ plugins should work correctly now.</li>
<li>Windows Store Apps: It is now possible to launch Unity WSA player on-demand.</li>
</ul>
