# Unity 4.3.3

https://unity3d.com/unity/whats-new/unity-4.3.3

## Fixes



*   2D: Correctly initialise Sprite textureRect if all pixels are transparent.
*   2D: Fixed broken sprite mesh generation in certain cases.
*   2D: Fixed SpriteRenderer inspector memory leak.
*   Allowing user to re-activate Unity when upgrading from Windows 8 to Windows 8.1
*   Android: added fallback to 24/32bit display buffer when 16bit display buffer is selected but not supported by the device.
*   Android: fixed a crash due to threads still being attached to dvm when exited.
*   Android: Fixed an issue where loading native libraries from custom threads would fail
*   Android: fixed an issue where the application would suddenly quit on some Snapdragon devices.
*   Android: fixed an issue where touches where sometimes offset by the height of the status bar.
*   Android: fixed Application.systemLanguage.
*   Android: fixed issues when the input was processed in cases it shouldn't
*   Android: fixed mali crash
*   Android: fixed orientation attribute for proxy and java activities.
*   Android: fixed splash screen fit/fill.
*   Android: fixed the bug when cache cleaning didn't work properly
*   Android: fixed the bug when creating an output directory with the name of target .apk lead to build failure
*   Android: force remove any selection before closing the onscreen keyboard.
*   Android: proxy activity will now activate the native activity.
*   Animation Window: Scene selection sync with animation window no longer jumps around when clip changes
*   Editor: Editor.log should no longer be locked by adb.exe on windows.
*   Editor: Fix 'Keys' pane in Preferences showing light background in dark skin
*   Editor: Fixed importing prefab with Cloth
*   Editor: Generating Previews for Main Asset on the Asset Store Tools is working again for non PRO licenses
*   Editor: Quitting the editor should no longer be blocked by adb.exe on windows.
*   Graphics: Fixed crash when calling LineRenderer.Render() outside of a camera render.
*   Graphics: Fixed crash when using a GrabPass shader with Graphics.DrawTexture().
*   Graphics: Fixed textures in MaterialPropertyBlock sampling the wrong mipmap on some platforms.
*   Input: Bumped the number of available joystick axis to twenty.
*   iOS: Fixed crash when cancelling WWW download
*   iOS: Fixed crash while dictating for IMGUI input field
*   iOS: Fixed iPad Air & iPad Mini Retina detection
*   iOS: Fixed unknown device type detection
*   Mac OS X Standalone: Fix accidental inclusion of unneeded files, resulting in wasted disk space for each player build.
*   Mecanim: Animator State progress bar were broken
*   Mecanim: Fix backward compatibility issue with animation imported in 4.2 and then imported in 4.3, we did change the default behaviour between those two version on how transform animation are imported
*   Mecanim: Fixed problem with Additive Layers. Only Lopped clip were working correctly
*   Mecanim: Fixed problem with Additive Layers. Weird interpolation when total blend weight was smaller then 100%
*   Mecanim: Fixed problem with editing Additional Curves when Preview window is closed
*   Mecanim: Fixed Crash when importing a project with sync layer in Unity Basic
*   Mecanim: Fixes BlendTree being reset when viewing their Graph in LiveLink.
*   Mecanim: Fixes humanoid layers that has empty states.
*   Mecanim: Various fix to API documentation: Play, Crossfade, SetTrigger and AnimatorControllerOverride
*   Meshes: Fixed crash with blend shapes that are morphing vertices not used in the mesh's geometry.
*   mobile: Fixed fog patching, to make sure we play good with preprocessor
*   NavMesh: fixed an issue where a disabled OffMeshLink would not re-enable on "Activated" check-box in editor
*   NavMesh: fixed an issue where stopped NavMeshAgent would start moving on carved NavMesh
*   NavMesh: fixed regression for crash when changing updatePosition on a NavMeshAgent not attached to a NavMesh.
*   NavMesh: fixed regression where NavMeshAgents with slow speeds would sometimes get stuck when moving around corners
*   Physics: Rigidbody2D rotation updates sometimes causing invalid local local rotations when placed in a deep hierarchy.
*   Physics: Unity crashes when rotating a complex PolygonCollider2D component.
*   Shaders: Fixed building shaders from Editor with -nographics option in batch mode.
*   Shaders: Fixed GLSL shaders messing up Mac Editor windows for one frame once in a blue moon.
*   Shaders: Fixed material.SetFloat, SetColor etc. performance issue in Editor (it was getting slower as more unique shader property names appeared).
*   Shuriken: Fixed some particle systems incorrectly pre warming when being reactivated.
*   Substances: Fixed Substance cache files being included in iCloud backups; could cause apps to be rejected on the App Store.
*   UnityObject: Fixing Internet Explorer detection, when plugin missing.
*   Windows Editor: Fixed a rare crash on toggling Direct3D 11 mode.
*   Windows Phone: UnityScript support fixes
*   Windows Player: Fixed memory use regression for static batches and non-read/writable meshes in 4.3.
*   Windows Store Apps/WP8 : AnimcationClip.SetCurve will work correctly now.
*   Windows Store Apps/WP8: Fall back to Clamp texture wrap setting for non-power of two size textures
*   Windows Store Apps/WP8: fixed ReferenceReWriter crash when project is being built, an unavailable API is used somewhere in user scripts/plugins and a method with a same name but no parameters is available.
*   Windows Store Apps/WP8: When compiling C#, JS or Boo files, Unity will not reference assemblies from other platform folders, for ex., assemblies from Assets\\Plugins\\iOS will not be used. This should fix the issue where Unity creates assemblies with references to other platforms.
*   Windows Store Apps: Blind fix for a rare crash when profiler tries to connect and there's an error in the Network.
*   Windows Store Apps: Check for DX debug support, fixes crash on Windows 8.1 using 8.0 debug player
*   Windows Store Apps: Debug, Release configuration won't crash when trying to connect to profiler, when no network adapters are available or some other fatal network error.
*   Windows Store Apps: Fix fixed function shaders not working under level 9.1 emulation in editor
*   Windows Store Apps: Fix mouse delta when cursor is hidden (was incorrect on some devices)
*   Windows Store Apps: Fix serialisation bug when you have fields wrapped with UNITY\_EDITOR define.
*   Windows Store Apps: Fix several crashes in live tiles API
*   Windows Store Apps: Fixed a rare hang, when resizing window and calling InvokeOnAppThread with sync.
*   Windows Store Apps: Mouse and touch positions should be reported correctly on devices like Surface Pro (Windows 8.0 & Windows 8.1), with and without Independent Input Source enabled.
*   Windows Store Apps: When changing window size, rendering won't get corrupted.
*   WP8: Fixed player crash when ID\_CAP\_IDENTITY\_DEVICE capability is disabled from application manifest.
*   WP8: Rotate skybox and non-pixel correct GUIText to screen orientation