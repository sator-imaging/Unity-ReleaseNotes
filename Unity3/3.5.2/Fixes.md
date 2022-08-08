# Unity 3.5.2

https://unity3d.com/unity/whats-new/unity-3.5.2

## Fixes



*   Android: Possible fix for random crashes in OpenGL ES driver on Galaxy Nexus ICS.
*   Android: Touch problems related to ICS upgrades on some devices have been fixed.
*   Android: Caching.CleanCache() was always returning false (without cleaning the cache).
*   Android: Fixed Webcam texture initialization problem on ICS device.
*   Editor: Catch more corner cases when detecting Visual Studio installations.
*   Editor: Fixed out-of-memory crash when showing AudioClip's inspector while in play mode.
*   Editor: PvrTexTool updated to version 2.10.87.498.
*   Editor: Fixed crash when using SendMessage, a non-null argument is passed to a parameterless receiver.
*   Editor: Fixed used textures stats to display in statistics view
*   Fixed memory leak when the profiler is attached.
*   Fixed WebPlayer crash when downloading an AssetBundle.
*   Fixed a bug in mouse delta handling for non HID enabled mice.
*   Fixed an out of memory crash on audio preview.
*   Fixed race condition while hashing assets for the cache server.
*   Fixed crash in Resources.Load if the resource being loaded referenced a non existing asset.
*   Fixed out of memory crash when building a player with a lot of assets cross references between scenes.
*   Fixed bug where SkinnedMeshRenderers marked as Occluders would result in bad occlusion. SkinnedMeshes can only be marked as Occludees now and the bounding volume of the skinned mesh is used during PVS Calculation.
*   Fixed crash when reloading scripts after launching Unity with a compile error.
*   Flash: Fixed integer division semantics.
*   Flash: Fixed memory leak in native methods returning structs.
*   Flash: Fixed crash on constructors passing fields as byref arguments.
*   Flash: Fixed RuntimeServices\_ToBool\_Object being invoked, but not implemented.
*   Flash: Fixed endianness error on byte\[\].
*   Flash: Fixed crashes on monobehaviour deserialization on asset bundles.
*   Flash: Fixed particle system not being scriptable again.
*   Flash: Fixed www.error being set to seemingly random strings, even if there was no eror.
*   Flash: Fixed crashing on fatal errors on errors thrown in coroutines.
*   Flash: Fixed fatal errors on www.texture access.
*   Flash: Fixed flash preloader bar on black background.
*   Flash: Fixed bug where array.CopyTo() fails if the destinationsize is larger than sourcesize.
*   Flash: Fixed fields of type List crashing on Instantiate().
*   Flash: Fixed serialization of List.
*   Flash: Fixed multiple issues with SwfPostprocessor resulting in issues with swf not getting verified or causing stack under - or overflows.
*   Flash: Many small actionscript conversion issues fixed.
*   Flash: GuiTexture is rendering correctly again.
*   Flash: Particles are rendering correctly again.
*   Flash: Texture2D setPixels with larger textures doesn't crash anymore.
*   Flash: UnityContent .setSize(width,height), working correctly.
*   Flash: useGuiLayout works.
*   Flash: No more crashes on gui.window.
*   Flash: No more crashes on physics/charactercontroller collisions.
*   Flash: Physics, fixed issues with objects shooting into space or being sticky.
*   Flash: Array of Structs aren't being (incorrectly) serialized anymore.
*   Flash: ParticleSystem now script accessible.
*   Flash: Serialization of non-public monobehaviour now works.
*   Flash: Issues with coroutines throwing FlashPlayer verify and stack size errors fixed.
*   Flash: EncodeToPNG now works.
*   Flash: Support for c# packing of array data in types.
*   Flash: Correct handling of numeric casts of infix expressions (ex: (int)(f \* g)).
*   Flash: Fix serialization of List
*   Flash: Fix SwfPostprocessor; cases where player was throwing fatal error indicating that files are not available / verifier error on constants.
*   Flash: Fix SwfPostprocessor; fix max stack size calculation
*   Flash: Fix WWW.GetAudioClip() usage in StartCoroutine crash.
*   Graphics: Fixed vertex colors being swapped in CombineMeshes
*   Graphics: Fixed projector errors with zero near plane
*   iOS: Fixed dynamic geometry performance regression in 3.5/3.5.1.
*   iOS: Fixed splash rotation, causing it to skew.
*   iOS: setting Application.targetFrameRate <= 0, will force 60 fps (as on other platforms).
*   iOS: Fixed GL.InvalidateState causing INVALID\_FRAMEBUFFER\_OPERATION\_EXT.
*   iOS: Fixed while line in splash screen on iPhones.
*   iOS: Fixed splash rotation, causing it to skew.
*   Legacy particles: ParticleRenderer and TrailRenderer will not leak memory if Time.timeScale is 0.
*   Mobile: Fixed SkinnedMeshRenderer crashes.
*   Navmesh: NavMeshAgent velocity will not become invalid when Time.timeScale is 0.
*   Navmesh: NavMeshAgent fixed occasional invalid position/velocity when destination and position are set to the same vector.
*   OS X: Fixed erratic mouse behavior with Microsoft mouse
*   Windows Player: Fixed occasional hang in multithreaded renderer when going in and out of fullscreen mode.