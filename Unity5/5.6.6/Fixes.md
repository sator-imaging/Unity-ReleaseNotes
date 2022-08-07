# Unity 5.6.6
https://unity3d.com/unity/whats-new/unity-5.6.6

## Fixes

<ul>
<li>Animation: Fixed a crash when an animator reset was triggered during a StateMachineBehaviour awake. (907324)</li>
<li>Animation: Fixed a crash when Animator instantiated from Script enters a Sub-State Machine with StateMachineBehaviour. (930814)</li>
<li>AppleTV: Removed 2x App store icon slices that cause App Store validation to fail. (972927)</li>
<li>Audio: Fixed an issue where unloading an asset bundle containing AudioClips would cause all other AssetBundle audio clips to be unloaded. (1019920 (902838)</li>
<li>Build Pipeline: Improved build pipeline performance for large builds. (None)</li>
<li>Build Pipeline: Fixed scene passed to OnProcessScene when entering Play Mode is not being loaded. (943435)</li>
<li>Editor: Fixed Editor crashes in "RenderSelectionOutline" when using ImageEffectAllowedInSceneView and set camera's targetTexture to null. (966404)</li>
<li>Editor: Fixed an issue with picking objects on Windows/D3D11. (943051)</li>
<li>Editor: Fixed various UnityEditor.VersionControl.Provider APIs when used with newly created VersionControl.Assets. (905161)</li>
<li>Editor: Fixed Skinned Mesh not being removed on undo. (925835)</li>
<li>Editor: Fixed undoing the activation of a UI layout component not undoing the side effects to the children RectTransforms. (1010407)</li>
<li>Editor: Fixed errors seen in the console and log related to temp TLS allocations. (926835)(921915)</li>
<li>Editor: Added an optional Async mode for Perforce Integration (see Editor Settings) to account for high latency with a remote server. (922829)</li>
<li>Editor: Fixed RectTransform causing the scene to be constantly flagged as dirty. (1010397)(966172)</li>
<li>GI: Fixed Meta pass values when using terrain mesh with MaterialPropertyBlock and Realtime GI.u(930042) - GI: Fixed Unnecessary error message being displayed in console. (935149)</li>
<li>GI: Fixed incorrect light modes being shown when multiple lights are selected. (929875)</li>
<li>Graphics: Fixed cullmode not being reset after Deferred and Forward rendering loops. (None)</li>
<li>Graphics: Fixed issue where not all requested shader variants ending up in an asset bundle. (948053)</li>
<li>Graphics: Fixed OpenGL ES crash due to problem with cached VertexAttribArray. (989484)</li>
<li>Graphics: Fixed crash in SkinnedMeshRenderer::PrepareSkinCommon when SkinnedMeshRenderer has Animator and Cloth attached. (941369)</li>
<li>Graphics: Fixed crash when opening project with BC6H texture. (971965)</li>
<li>Graphics: Fixed asserts and potential memory leaks when Skinned Mesh Renderers with the "Update When Offscreen" property enabled are not visible. (961692, 964998)</li>
<li>Graphics: Fixed crash during a visibility callback when a GameObject which was not visible is set inactive followed by setting a visible GameObject inactive. (968591)</li>
<li>Graphics: Fixed changing the projectors render queue in script not having an effect. (841236)</li>
<li>Graphics: Fixed issue where DrawMeshInstanced calls will render with inverse normals if the previous draw call used negative scaling. (956919)</li>
<li>Graphics: Fixed case when some of the cameras don't render anything because depth buffer contains garbage. (907391)</li>
<li>Graphics: Fixed crash in player when using non RGBA32 format 3D textures. (927145)</li>
<li>Il2CPP: Prevented a crash on iOS which can occur when a device is awakened during a blocking socket call with a SIGPIPE signal. (957651)</li>
<li>iOS: Fixed videos started with Handheld.PlayFullScreenMovie not resuming after returning to the app in some circumstances. (954593)</li>
<li>iOS: Fixed an issue where the launch image for iPhone X might not display correctly. (972995)</li>
<li>iOS: Fixed crash when opening an app via URL whilst mirroring display via Airplay. (995429)(960439)</li>
<li>iOS: Fixed black frame flickering when changing screen orientation via script. (994961) (953524)</li>
<li>iOS: Metal: Fixed MSAA corner case causing warning messages and validation error Marton Ekler. (58811)</li>
<li>iOS: Fixed an issue where fullscreen movies could no longer be dismissed with a tap on iOS 11. (940608)</li>
<li>iOS: iPhone X, fixed problem with missing keyboard Done/Cancel buttons. (979007)</li>
<li>iOS: Fixed standard shader specular highlights on mobiles. (1001377 (953606)</li>
<li>iOS: Fixed issue where Display.SetResolution silently failed during first frame. (1006820)(995079)</li>
<li>iOS: [Metal] Fixed potential GPU crash. (952284)</li>
<li>Linux: Fixed OnMouseDown not working with touch screens. (947049)</li>
<li>Multi-Display: Fixed non-primary display input for mouse events on standalone. (None)</li>
<li>OSX: Fixed changing Input Manager entries causing the player to become unresponsive. (900969)</li>
<li>Particles: Fixed console error message if deleting a Particle System whilst the Particle System Window is open. (971977)</li>
<li>Performance Reporting: Report device model field for Managed Exceptions. (980818) (980806)</li>
<li>Physics: Fixed scale not being taken into account when computing a collider's pose. (1019921)</li>
<li>Physics: Fixed memory leak when resizing BoxColliders. (969368)</li>
<li>Physics: Fixed PhysX crash when calling Physics.OverlapBoxNonAlloc on Android devices. (878407)</li>
<li>Resources: Improved Load performance in some circumstances. (980640)</li>
<li>Scene: Fixed DoImportScene crashing when importing FBX files. (1005311 (905817)</li>
<li>Scripting: Fixed crash when calling UnityEngine.Object.Instantiate on non-main thread. (992056)</li>
<li>Scripting: Fixed crash when using GitHub for Unity. (930358)</li>
<li>Scripting: Fixed Awake containing the wrong transform values when instantiated. (953068)</li>
<li>Shaders: Fixed shader compiler crash when compiling specific D3D9 shaders. (968997)</li>
<li>Shaders: Fixed an issue with the Shader Compiler which would result in GLSL based platforms not being able to compiler certain shaders. (919351)</li>
<li>Substance: Fixed a memory leak when using cloned ProceduralMaterials. (1005779)</li>
<li>Test Runner: Fixed missing category filter. (1008883)</li>
<li>UI: Fixed issue where an assigned fallback font would not be used. (911613)</li>
<li>Universal Windows Platform: Fixed building player with IL2CPP player fails when there are plugins that are marked read-only in the project. (959795)</li>
<li>Universal Windows Platform: Fixed .NET native compiler crash when using List or List in a serializable class. (979741)</li>
<li>Universal Windows Platform: Fixed reference rewriter not fixing references for System.Net.Sockets.Socket when DLL where it's being referenced was compiled against .NET 3.5. (947209)</li>
<li>Video: Fixed video not playing in build when building for a different platform. (964787)(925387)</li>
<li>VR: Shaders meant to be used in VR platforms will no longer be included in builds where VR support is disabled. (961763)</li>
<li>VR: Fixed Cardboard VR failing to initialize on certain Android devices. (1011576 (991127)</li>
<li>WebGL: Added indexedDB caching mechanism for XMLHttpRequest in WebGL. (937594)</li>
<li>Windows: Fixe crash on startup in case screen width/height player preferences in registry got corrupted. (979198)</li>
<li>Windows: Fixed resolution dialog not showing monitor list and crashing on pressing 'Play' button on some weird monitor setups. (996015)</li>
<li>XR: Fixed Daydream applications hanging before quiting to Android home when calling Application.Quit. (966173)</li>
<li>XR: Fixed LoadDeviceByName causing crash on Cardboard/Daydream in 5.6.5p3. (1016356(1016356)-</li>
</ul>
