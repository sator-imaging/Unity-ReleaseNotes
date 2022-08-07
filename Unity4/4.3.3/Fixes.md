# Unity 4.3.3
https://unity3d.com/unity/whats-new/unity-4.3.3

## Fixes

<ul>
<li>2D: Correctly initialise Sprite textureRect if all pixels are transparent.</li>
<li>2D: Fixed broken sprite mesh generation in certain cases.</li>
<li>2D: Fixed SpriteRenderer inspector memory leak.</li>
<li>Allowing user to re-activate Unity when upgrading from Windows 8 to Windows 8.1</li>
<li>Android: added fallback to 24/32bit display buffer when 16bit display buffer is selected but not supported by the device.</li>
<li>Android: fixed a crash due to threads still being attached to dvm when exited.</li>
<li>Android: Fixed an issue where loading native libraries from custom threads would fail</li>
<li>Android: fixed an issue where the application would suddenly quit on some Snapdragon devices.</li>
<li>Android: fixed an issue where touches where sometimes offset by the height of the status bar.</li>
<li>Android: fixed Application.systemLanguage.</li>
<li>Android: fixed issues when the input was processed in cases it shouldn't</li>
<li>Android: fixed mali crash</li>
<li>Android: fixed orientation attribute for proxy and java activities.</li>
<li>Android: fixed splash screen fit/fill.</li>
<li>Android: fixed the bug when cache cleaning didn't work properly</li>
<li>Android: fixed the bug when creating an output directory with the name of target .apk lead to build failure</li>
<li>Android: force remove any selection before closing the onscreen keyboard.</li>
<li>Android: proxy activity will now activate the native activity.</li>
<li>Animation Window: Scene selection sync with animation window no longer jumps around when clip changes</li>
<li>Editor: Editor.log should no longer be locked by adb.exe on windows.</li>
<li>Editor: Fix 'Keys' pane in Preferences showing light background in dark skin</li>
<li>Editor: Fixed importing prefab with Cloth</li>
<li>Editor: Generating Previews for Main Asset on the Asset Store Tools is working again for non PRO licenses</li>
<li>Editor: Quitting the editor should no longer be blocked by adb.exe on windows.</li>
<li>Graphics: Fixed crash when calling LineRenderer.Render() outside of a camera render.</li>
<li>Graphics: Fixed crash when using a GrabPass shader with Graphics.DrawTexture().</li>
<li>Graphics: Fixed textures in MaterialPropertyBlock sampling the wrong mipmap on some platforms.</li>
<li>Input: Bumped the number of available joystick axis to twenty.</li>
<li>iOS: Fixed crash when cancelling WWW download</li>
<li>iOS: Fixed crash while dictating for IMGUI input field</li>
<li>iOS: Fixed iPad Air &amp; iPad Mini Retina detection</li>
<li>iOS: Fixed unknown device type detection</li>
<li>Mac OS X Standalone: Fix accidental inclusion of unneeded files, resulting in wasted disk space for each player build.</li>
<li>Mecanim:  Animator State progress bar were broken</li>
<li>Mecanim: Fix backward compatibility issue with animation imported in 4.2 and then imported in 4.3, we did change the default behaviour between those two version on how transform animation are imported</li>
<li>Mecanim: Fixed problem with Additive Layers. Only Lopped clip were working correctly</li>
<li>Mecanim: Fixed problem with Additive Layers. Weird interpolation when total blend weight was smaller then 100% </li>
<li>Mecanim: Fixed problem with editing Additional Curves when Preview window is closed </li>
<li>Mecanim: Fixed Crash when importing a project with sync layer in Unity Basic</li>
<li>Mecanim: Fixes BlendTree being reset when viewing their Graph in LiveLink.</li>
<li>Mecanim: Fixes humanoid layers that has empty states.</li>
<li>Mecanim: Various fix to API documentation: Play, Crossfade, SetTrigger and  AnimatorControllerOverride</li>
<li>Meshes: Fixed crash with blend shapes that are morphing vertices not used in the mesh's geometry.</li>
<li>mobile: Fixed fog patching, to make sure we play good with preprocessor</li>
<li>NavMesh: fixed an issue where a disabled OffMeshLink would not re-enable on "Activated" check-box in editor</li>
<li>NavMesh: fixed an issue where stopped NavMeshAgent would start moving on carved NavMesh</li>
<li>NavMesh: fixed regression for crash when changing updatePosition on a NavMeshAgent not attached to a NavMesh.</li>
<li>NavMesh: fixed regression where NavMeshAgents with slow speeds would sometimes get stuck when moving around corners</li>
<li>Physics: Rigidbody2D rotation updates sometimes causing invalid local local rotations when placed in a deep hierarchy.</li>
<li>Physics: Unity crashes when rotating a complex PolygonCollider2D component.</li>
<li>Shaders: Fixed building shaders from Editor with -nographics option in batch mode.</li>
<li>Shaders: Fixed GLSL shaders messing up Mac Editor windows for one frame once in a blue moon.</li>
<li>Shaders: Fixed material.SetFloat, SetColor etc. performance issue in Editor (it was getting slower as more unique shader property names appeared).</li>
<li>Shuriken: Fixed some particle systems incorrectly pre warming when being reactivated.</li>
<li>Substances: Fixed Substance cache files being included in iCloud backups; could cause apps to be rejected on the App Store.</li>
<li>UnityObject: Fixing Internet Explorer detection, when plugin missing.</li>
<li>Windows Editor: Fixed a rare crash on toggling Direct3D 11 mode.</li>
<li>Windows Phone: UnityScript support fixes</li>
<li>Windows Player: Fixed memory use regression for static batches and non-read/writable meshes in 4.3.</li>
<li>Windows Store Apps/WP8 : AnimcationClip.SetCurve will work correctly now.</li>
<li>Windows Store Apps/WP8: Fall back to Clamp texture wrap setting for non-power of two size textures</li>
<li>Windows Store Apps/WP8: fixed ReferenceReWriter crash when project is being built, an unavailable API is used somewhere in user scripts/plugins and a method with a same name but no parameters is available.</li>
<li>Windows Store Apps/WP8: When compiling C#, JS or Boo files, Unity will not reference assemblies from other platform folders, for ex., assemblies from Assets\Plugins\iOS will not be used. This should fix the issue where Unity creates assemblies with references to other platforms.</li>
<li>Windows Store Apps: Blind fix for a rare crash when profiler tries to connect and there's an error in the Network.</li>
<li>Windows Store Apps: Check for DX debug support, fixes crash on Windows 8.1 using 8.0 debug player</li>
<li>Windows Store Apps: Debug, Release configuration won't crash when trying to connect to profiler, when no network adapters are available or some other fatal network error.</li>
<li>Windows Store Apps: Fix fixed function shaders not working under level 9.1 emulation in editor</li>
<li>Windows Store Apps: Fix mouse delta when cursor is hidden (was incorrect on some devices)</li>
<li>Windows Store Apps: Fix serialisation bug when you have fields wrapped with UNITY_EDITOR define.</li>
<li>Windows Store Apps: Fix several crashes in live tiles API</li>
<li>Windows Store Apps: Fixed a rare hang, when resizing window and calling InvokeOnAppThread with sync.</li>
<li>Windows Store Apps: Mouse and touch positions should be reported correctly on devices like Surface Pro (Windows 8.0 &amp; Windows 8.1), with and without Independent Input Source enabled.</li>
<li>Windows Store Apps: When changing window size, rendering won't get corrupted.</li>
<li>WP8: Fixed player crash when ID_CAP_IDENTITY_DEVICE capability is disabled from application manifest.</li>
<li>WP8: Rotate skybox and non-pixel correct GUIText to screen orientation</li>
</ul>
