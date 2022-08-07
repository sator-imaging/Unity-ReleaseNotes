# Unity 5.2.3
https://unity3d.com/unity/whats-new/unity-5.2.3

## Fixes

<ul>
<li>(731143) -  2D: Fixed alphasplit parameter not getting reset when switching sprite/material on the fly</li>
<li>(733725) -  2D: Fixed: SpritePacker Crash after packing multiple high res sprites.</li>
<li>(729698) -  Android: Buildpipe - Fixed IndexOutOfRangeException thrown on plugin package collisions.</li>
<li>(712011) -  Android: Fix crash in dynamic batching</li>
<li>(689286) -  Android: Fixed an issue where a problematic EGL configuration was picked up on some Samsung devices.</li>
<li>(726878) -  Android: Fixed MSAA on newer ARM Mali devices like Samsung Galaxy S6</li>
<li>(728806) -  Android: Fixed MSAA RenderTextures on Tegra4 and K1 when using OpenGL ES 2.0</li>
<li>(715602), (731076), (704017), (731078) -  Android: Fixed non-working textures on some Tegra 3 and Tegra 4 devices.</li>
<li>(733897) -  Android: Fixed slow audio clip loading.</li>
<li>(none) -  Android: Fixed slow level loading.</li>
<li>(715447) -  Animation: Fixed animation of material properties in the animation window.</li>
<li>(714661) -  AssetBundle: Fixed the issue that AssetBundle names sometimes gets into inconsistent state between cache server/.meta files.</li>
<li>(723030) -  AssetBundle: Fixed the issue that the sprite atlas had been stored twice in AssetBundles.</li>
<li>(724561) -  Assets Loading: Fixed reading of assets stored in a text mode with UTF8 signature.</li>
<li>(739944) -  Editor: Fix for GUI methods in Update crashing the editor.</li>
<li>(728260), (725794), (726660), (727065), (727287), (727802), (728012), (728240), (728350), (728369), (728446), (728518), (728795), (728822), (728836), (729405), (729406), (729643), (729775), (729790), (729828), (729857), (729925), (729992), (730045), (730059), (730069), (730328), (730403), (730993), (731464), (731500), (731586), (732069), (732101), (732425), (732546), (732842), (732853), (733280), (733416), (733440), (734148), (735199), (735227), (735296), (735804), (735991), (736048), (737077) -  Editor: Fixed a crash in the editor when saving the scene.</li>
<li>(704738) -  Editor: Fixed incorrect DestroyGpuProgram being called.</li>
<li>(731107) -  Editor: Fixed occasional crash when importing assets on editor.</li>
<li>(698169) -  Editor: Fixed occlusion culling pre-visualisation in editor.</li>
<li>(715380) -  Editor: Unsupported texture compression formats now correctly fallback to default compression format for the platform.</li>
<li>(642609) -  Fixed crash on copying script with component requirements onto a GO which is missing the requirements.</li>
<li>(710195) -  Fixed issue where UI would not get rendered for disabled cameras when manually calling .Render().</li>
<li>(740573) -  FrameDebugger: Fixed draw call count jumping when there were realtime probes in the scene.</li>
<li>(none) -  GI: Fixed Enlighten saturating the command buffer and stalling because of it. Gives the biggest benefit in scenes with high rendering framerate and many animated realtime lights with non-zero bounce.</li>
<li>(none) -  GI: Fixed the reflection probe inspector breaking when reusing a cubemap (RenderTexture) from a realtime reflection probe on a custom reflection probe.</li>
<li>(708559) -  Graphics: Add error message if 3D texture is bound for rendering.</li>
<li>(740977), (740988) -  Graphics: Fix for shadow-casting light occlusion issues - disappearing realtime lights</li>
<li>(726799) -  Graphics: Fixed camera parameter changing from OnPreRender to work again.</li>
<li>(736709) -  Graphics: Fixed memory leak when rendering shadows.</li>
<li>(730171) -  Graphics: Fixed Screen.currentResolution in some cases reporting wrong resolution when in fullscreen on Windows</li>
<li>(734255) -  Graphics: Fixed upscaled fullscreen rendering being upside down in some situations</li>
<li>(727743) -  Graphics: Fixed use of Blit not correctly binding RandomWrite targets.</li>
<li>(728103) -  Graphics: Stopped reflection merging into emissive from stomping over render target alpha with 1.0</li>
<li>(716811) -  IL2CPP: Change the conv.i8 opcode implementation to handle sign extension correctly so that a conversion from a large negative int to a uint to a long in C# works as expected.</li>
<li>(733772) -  IL2CPP: Convert assemblies that are mentioned in a link.xml file but are not referenced by any other assemblies at compile time.</li>
<li>(735413) -  IL2CPP: Generate proper C++ code for a type with two fields that have the same type and name.</li>
<li>(734534) -  IL2CPP: Improve the error message when the byte code stripper is unable to locate an assembly.</li>
<li>(737853) -  IL2CPP: Prevent a crash in the player in MetadataCache::GetTypeInfoFromTypeDefinitionIndex when a constrained call is made to a generic virtual method defined on a value type.</li>
<li>(736167) -  IL2CPP: Prevent a memory leak that caused some GCHandles, including those used to reference MonoBehaviour instances, from being correctly reclaimed by the garbage collector.</li>
<li>(717997) -  IL2CPP: Prevent a NullReferenceException exception from occurring during the processing of the Preserve attribute which can obscure the actual cause of a problem.</li>
<li>(718885) -  IL2CPP: Prevent an intermittent hang with asynchronous sockets.</li>
<li>(730233) -  IL2CPP: Prevent an KeyNotFoundException exception from occurring during code conversion when a generic method is used with at least one generic argument that exceeds the maximum generic recursion depth.</li>
<li>(none) -  IL2CPP: Remove warnings in generated C++ code related to const problems.</li>
<li>(none) -  IL2CPP: The low level memory profiler no longer reports constant literals as fields with offset 0.</li>
<li>(715666) -  Input: Fixed mouse position going out of bounds in Fullscreen Window mode.</li>
<li>(715666) -  Input: Fixed render being positioned and sized incorrectly in D3D9 and D3D11 with Fullscreen Window mode.</li>
<li>(739935) -  iOS: Added build &amp; run support for Xcode 7.1.</li>
<li>(none) -  iOS: Don't constrain iPhone 6+ to single landscape orientation on launch.</li>
<li>(723360) -  iOS: Export correct image for iPad launch screen now,</li>
<li>(none) -  iOS: Fixed incorrect landscape launch orientation on iPad.</li>
<li>(none) -  iOS: Fixed legacy launch screens on iOS 9.1.</li>
<li>(none) -  iOS: Fixed minor launch screen placement issue on devices with large resolution screens.</li>
<li>(732806) -  iOS: Fixed occasional 1-frame glitches in dynamic font rendering.</li>
<li>(none) -  iOS: Fixed second-stage splashscreen on some devices with iOS 6 and 7.</li>
<li>(740343) -  iOS: Fixed simulator support on Xcode 7.1.</li>
<li>(742579) -  iOS: Work around for iOS 9.1 bug that sometimes causes launchscreen corruption when only landscape orientations are enable.</li>
<li>(725713) -  Mecanim: Avoid clearing sampling data set when invalidating animator.</li>
<li>(735656) -  Mecanim: Delete SMB instances when user delete a state/statemachine with SMB.</li>
<li>(732986), (733883), (734458) -  Mecanim: Fixed AnimationControllerPlayable calls not being forwarded from Animator to its playables.</li>
<li>(727244) -  Mecanim: Fixed AnimationEvents not called when at the begining of a State.</li>
<li>(none) -  Mecanim: Fixed BlendTree performance regression.</li>
<li>(734033) -  Mecanim: Fixed Crash when using OverrideController with no source Controller.</li>
<li>(726466) -  Networking: Added support for HLAPI packet queuing on channels using the ReliableFragmented QoS.</li>
<li>(697097) -  Networking: Added warning message when a scene cannot be added to NetworkManager.</li>
<li>(736714) -  Networking: Better log warning for UNet HLAPI Script CRC check now.</li>
<li>(725109) -  Networking: Clear error message when user try to add the two host with the same port</li>
<li>(733731) -  Networking: Fix for scene slots in NetworkManager not being saved all the time.</li>
<li>(none) -  Networking: Fix for UNetWeaver exception when making Metro builds.</li>
<li>(721917) -  Networking: Fixed code generation exception when a SyncVar uses a type from external DLL. This now generates a regular build error.</li>
<li>(698322) -  Networking: Fixed code generation exception when using certain built-in unity types such as Vector3 in SyncListStruct.</li>
<li>(714700) -  Networking: Fixed crash when sending an unsupported type (a class instance) via a network Command.&nbsp; This now generates a build error.</li>
<li>(739432) -  Networking: Fixed invalid generated IL for SyncListStruct with embedded array.</li>
<li>(726244) -  Networking: Fixed issues with zero length size or MTU size packets using NetworkConnection Send functions. This could break packet buffering for HLAPI connections.</li>
<li>(725363) -  Networking: Fixed missing Connect callback for local client.</li>
<li>(727133) -  Networking: Fixed movement problem for objects on clients with local-client-authority when snap threshold was set to a small value.</li>
<li>(730199) -  Networking: Fixed NullReference exception when using NetworkAnimator.</li>
<li>(738517) -  Networking: Fixed slow compilation when many ClientRpc functions.</li>
<li>(733731) -  Networking: Fixed the scene slots in NetworkManager and NetworkLobbyManager not marking the scene dirty when they are changed.</li>
<li>(736703) -  Networking: Fixed wrong item index for SyncList ADD operation.</li>
<li>(720436) -  Networking: prevent user to set minupdatetimeout to 0 via networkmanager menu</li>
<li>(730299) -  Networking: Removed misleading error messages that are generated during SyncList initialization.</li>
<li>(none) -  OpenGL: Added detection for cases when the geometry shader expects input topology that does not match with the given geometry. Also fail compilation when using unsupported topology (such as adjacency).</li>
<li>(none) -  OpenGL: Compute shaders: Fixed append/consume buffer counters.</li>
<li>(none) -  OpenGL: Fixed shader generation when reading back per-patch outputs in a hull shader.</li>
<li>(none) -  OpenGL: Fixed shadow normal bias for meshes that are missing vertex normals.</li>
<li>(735644) -  OpenGL: Fixed texture memory usage reporting in profiler, was twice the actual size for most textures.</li>
<li>(none) -  OpenGL: Fixed: compute shader buffer resolves when using multithreaded renderer.</li>
<li>(none) -  OpenGL: Shader compiler: Fix for conflicting shader input/output names in tessellation shaders.</li>
<li>(733928) -  OpenGL: Shader compiler: Fixed a corner case in constant buffer vec4 access.</li>
<li>(708722) -  OpenGL: Shader compiler: Fixed atomic ops handling in shaders.</li>
<li>(none) -  OpenGL: Shader compiler: Fixed geometry shader stream index handling.</li>
<li>(none) -  OpenGL: Shader compiler: Fixed input redirection on geometry shaders.</li>
<li>(none) -  OpenGL: Shader compiler: Handle RWTexture properties more accurately.</li>
<li>(none) -  OpenGL: Shader compiler: In geometry shaders, only emit vertex stream for GL ver &gt;=4.20.</li>
<li>(none) -  OpenGL: Shader compiler: Only emit the stream declarations if they're actually used.</li>
<li>(none) -  OpenGL: Shader compiler: OS X doesn't like EmitStream(0) so use EmitStream() instead.</li>
<li>(738778) -  Particles: Fixed sorting by distance.</li>
<li>(730386) -  Particles: Fixing regression when setting transform in LateUpdate</li>
<li>(682939) -  Physics: Allow slope limit to be considered for non-static objects.</li>
<li>(731470) -  Physics: Ensure that RectTransform is loaded prior to any Rigidbody2D or Collider2D so that initial position is correct.</li>
<li>(731054) -  Physics: Ensure that when changing the Joint2D connected RigidBody2D, all related Gizmos are reset.</li>
<li>(730822) -  Physics: Ensure that when ignoring collision layer/layer collisions, that existing contacts are re-evaluated.</li>
<li>(731057) -  Physics: Ensure that when Joint2D.EnableCollision is changed, all relevant contacts are re-evaluated.</li>
<li>(714572), (720398), (720408) -  Physics: Fixed a case where HingeJoint limits was not applied properly.</li>
<li>(714572), (720398), (720408) -  Physics: Fixed an axis-locking inconsistency in the HingeJoint when both min and max limits were set above 177 degrees, but still different.</li>
<li>(689159) -  Physics: Fixed Sphere-cast error against scaled non-convex meshes.</li>
<li>(714572), (720398), (720408) -  Physics: HingeJoint.angle is now returned as +/- 180 degrees, as in Unity4.</li>
<li>(712007) -  Physics: HingeJoint2D no longer produces incorrect reference angles from Rigidbody2D angles.</li>
<li>(714572), (720398), (720408) -  Physics: HingeJoints now have orientation to be compatible with Unity 4.</li>
<li>(714572), (720398), (720408) -  Physics: JointMotor.targetVelocity can now be negative as well as positive.</li>
<li>(719418) -  Physics: Physics2D, Collider2D &amp; Rigidbody2D IsTouching and IsTouchingLayers now correctly represents Box2D contact state.</li>
<li>(727734) -  Physics: Physics2D.CircleCastXXX and Physics2D.BoxCastXXX now correctly detect very fractional overlaps.</li>
<li>(702967) -  Physics: Setting Rigidbody.detectCollisions to false also affects queries now (e.g. Physics.RaycastAll).</li>
<li>(714572), (720398), (720408) -  Physics: The HingeJoint ""Connected Body"" will view the Joint anchor as a right-hand coordinate system. This means the Connected Body will view positive angles as going counter-clockwise around the Joint anchor.</li>
<li>(714572), (720398), (720408) -  Physics: The Rigidbody that share the GameObject with the HingeJoint will view the Joint anchor as a left-hand coordinate system. This means the Rigidbody will view positive angles as going clockwise around the Joint anchor.</li>
<li>(none) -  Samsung TV: Make Cursor.lockState API work in Samsung TV.</li>
<li>(none) -  Substance: Fix bitmap export. Bitmap export can now save bitmaps with the alpha channel setup according to the Unity material.</li>
<li>(725397), (728853), (729290) -  UI: Fix Editor crash that would sometimes trigger after pressing play/stop</li>
<li>(733005) -  Umbra : Fixed missing realtime lights after baking occlusion data.</li>
<li>(719421) -  VR: Fix HMD content failure after disconnect and reconnect</li>
<li>(716410), (716422  VR: Fix incorrect info and toggles while HMD was disconnected</li>
<li>(720052), (732183) -  VR: Fix Loss of Window focus crashes upon return</li>
<li>(736323) -  VR: Fix regression crash when HMD was disconnected at application start</li>
<li>(716500) -  VR: Fix stereoMirrorMode right eye flicker</li>
<li>(732236) -  VR: Fix VRDevice.IsPresent always returning true</li>
<li>(740962) -  VR: Fixed Crash when exiting play mode.</li>
<li>(none) -  VR: Fixed ShowDeviceView preventing drawing to the game view with any camera when false.</li>
<li>(722766) -  WebGL: Fix doppler effect being used on audio sources with spatial blend set to 2D</li>
<li>(733864) -  Windows Phone: Font will be visible again.</li>
<li>(none) -  Windows Phone: Reduced runtime memory usage by ~4 MB.</li>
<li>(735383) -  Windows Store Apps: Correctly generate Visual Studio namespace if package name has dot followed by a number. For ex., Test.2 package name will produce Test._2 namespace</li>
<li>(733548) -  Windows Store Apps: Use initial supported orientations from Player Settings.</li>
<li>(733864) -  Windows Universal 10: Fixed invisible text on ARM devices issue.</li>
<li>(735387) -  Windows Universal 10: Fixed screenshot capture failure.</li>
<li>(none) -  Windows Universal 10: Updated default project template to hide status bar by default</li>
<li>(713391) -  WSA: Fixed: Can't build &amp; run to SDK 8.1 if only VS2015 is installed.</li>
<li>(735384) -   XboxOne/IL2CPP: Correct metadata loading on startup.</li>
</ul>

#### Revision: f3d16a1fa2dd
