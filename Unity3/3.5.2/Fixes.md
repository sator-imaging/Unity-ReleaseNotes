# Unity 3.5.2
https://unity3d.com/unity/whats-new/unity-3.5.2

## Fixes

<ul>
<li>Android: Possible fix for random crashes in OpenGL ES driver on Galaxy Nexus ICS.</li>
<li>Android: Touch problems related to ICS upgrades on some devices have been fixed.</li>
<li>Android: Caching.CleanCache() was always returning false (without cleaning the cache).</li>
<li>Android: Fixed Webcam texture initialization problem on ICS device.</li>
<li>Editor: Catch more corner cases when detecting Visual Studio installations.</li>
<li>Editor: Fixed out-of-memory crash when showing AudioClip's inspector while in play mode.</li>
<li>Editor: PvrTexTool updated to version 2.10.87.498.</li>
<li>Editor: Fixed crash when using SendMessage, a non-null argument is passed to a parameterless receiver.</li>
<li>Editor: Fixed used textures stats to display in statistics view</li>
<li>Fixed memory leak when the profiler is attached.</li>
<li>Fixed WebPlayer crash when downloading an AssetBundle.</li>
<li>Fixed a bug in mouse delta handling for non HID enabled mice.</li>
<li>Fixed an out of memory crash on audio preview.</li>
<li>Fixed race condition while hashing assets for the cache server.</li>
<li>Fixed crash in Resources.Load if the resource being loaded referenced a non existing asset.</li>
<li>Fixed out of memory crash when building a player with a lot of assets cross references between scenes.</li>
<li>Fixed bug where SkinnedMeshRenderers marked as Occluders would result in bad occlusion. SkinnedMeshes can only be marked as Occludees now and the bounding volume of the skinned mesh is used during PVS Calculation.</li>
<li>Fixed crash when reloading scripts after launching Unity with a compile error.</li>
<li>Flash: Fixed integer division semantics.</li>
<li>Flash: Fixed memory leak in native methods returning structs.</li>
<li>Flash: Fixed crash on constructors passing fields as byref arguments.</li>
<li>Flash: Fixed RuntimeServices_ToBool_Object being invoked, but not implemented.</li>
<li>Flash: Fixed endianness error on byte[].</li>
<li>Flash: Fixed crashes on monobehaviour deserialization on asset bundles.</li>
<li>Flash: Fixed particle system not being scriptable again.</li>
<li>Flash: Fixed www.error being set to seemingly random strings, even if there was no eror.</li>
<li>Flash: Fixed crashing on fatal errors on errors thrown in coroutines.</li>
<li>Flash: Fixed fatal errors on www.texture access.</li>
<li>Flash: Fixed flash preloader bar on black background.</li>
<li>Flash: Fixed bug where array.CopyTo() fails if the destinationsize is larger than sourcesize.</li>
<li>Flash: Fixed fields of type List crashing on Instantiate().</li>
<li>Flash: Fixed serialization of List.</li>
<li>Flash: Fixed multiple issues with SwfPostprocessor resulting in issues with swf not getting verified or causing stack under - or overflows.</li>
<li>Flash: Many small actionscript conversion issues fixed.</li>
<li>Flash: GuiTexture is rendering correctly again.</li>
<li>Flash: Particles are rendering correctly again.</li>
<li>Flash: Texture2D setPixels with larger textures doesn't crash anymore.</li>
<li>Flash: UnityContent .setSize(width,height), working correctly.</li>
<li>Flash: useGuiLayout works.</li>
<li>Flash: No more crashes on gui.window.</li>
<li>Flash: No more crashes on physics/charactercontroller collisions.</li>
<li>Flash: Physics, fixed issues with objects shooting into space or being sticky.</li>
<li>Flash: Array of Structs aren't being (incorrectly) serialized anymore.</li>
<li>Flash: ParticleSystem now script accessible.</li>
<li>Flash: Serialization of non-public monobehaviour now works.</li>
<li>Flash: Issues with coroutines throwing FlashPlayer verify and stack size errors fixed.</li>
<li>Flash: EncodeToPNG now works.</li>
<li>Flash: Support for c# packing of array data in  types.</li>
<li>Flash: Correct handling of numeric casts of infix expressions (ex: (int)(f * g)).</li>
<li>Flash: Fix serialization of List</li>
<li>Flash: Fix SwfPostprocessor; cases where player was throwing fatal error indicating that files are not available / verifier error on constants.</li>
<li>Flash: Fix SwfPostprocessor; fix max stack size calculation</li>
<li>Flash: Fix WWW.GetAudioClip() usage in StartCoroutine crash.</li>
<li>Graphics: Fixed vertex colors being swapped in CombineMeshes</li>
<li>Graphics: Fixed projector errors with zero near plane</li>
<li>iOS: Fixed dynamic geometry performance regression in 3.5/3.5.1.</li>
<li>iOS: Fixed splash rotation, causing it to skew.</li>
<li>iOS: setting Application.targetFrameRate &lt;= 0, will force 60 fps (as on other platforms).</li>
<li>iOS: Fixed GL.InvalidateState causing INVALID_FRAMEBUFFER_OPERATION_EXT.</li>
<li>iOS: Fixed while line in splash screen on iPhones.</li>
<li>iOS: Fixed splash rotation, causing it to skew.</li>
<li>Legacy particles: ParticleRenderer and TrailRenderer will not leak memory if Time.timeScale is 0.</li>
<li>Mobile: Fixed SkinnedMeshRenderer crashes.</li>
<li>Navmesh: NavMeshAgent velocity will not become invalid when Time.timeScale is 0.</li>
<li>Navmesh: NavMeshAgent fixed occasional invalid position/velocity when destination and position are set to the same vector.</li>
<li>OS X: Fixed erratic mouse behavior with Microsoft mouse</li>
<li>Windows Player: Fixed occasional hang in multithreaded renderer when going in and out of fullscreen mode.</li>
</ul>
