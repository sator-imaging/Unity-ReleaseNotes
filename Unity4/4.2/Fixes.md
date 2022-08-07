# Unity 4.2
https://unity3d.com/unity/whats-new/unity-4.2

## Fixes

<ul>
<li>Android: Support for Android SDK rev22.</li>
<li>Android: Added a workaround for ANR when using Apple magic mouse; fixed ANR caused by deadlock when using touch enabled controllers.</li>
<li>Android: Added exception checks to avoid crashes in AndroidJNI.</li>
<li>Android: Added JDK version detection.</li>
<li>Android: Application no longer quits if joystick button 'A' is pressed before the first level has loaded.</li>
<li>Android: Disabled shader cache on pre-Honeycomb devices due to buggy drivers; also disabled it on all Immersion GPUs due to driver bugs.</li>
<li>Android: Editor; when switching between building a project and an actual apk, project is no longer replaced by the apk.</li>
<li>Android: Fixed a problem with streaming assets in exported android project.</li>
<li>Android: Fixed an issue where it was impossible to delete a project on windows due to adb keeping a lock in the project directory.</li>
<li>Android: Fixed crash on GL context recreate.</li>
<li>Android: Fixed crash when trying to read a non-existent string field through JNI.</li>
<li>Android: Fixed IndexOutOfRangeException on faulty package name.</li>
<li>Android: Fixed occasional crash on Nexus4 in shader compilation.</li>
<li>Android: Fixed problem with crashing video player on 1st gen Kindle Fire.</li>
<li>Android: Fixed propagation of key input events to OnGUI().</li>
<li>Android: Fixed touch and stylus input on devices having a single surface emitting both at the same time.</li>
<li>Android: Re-initialization of UnityPlayer is now possible.</li>
<li>Android: Removed black screen rendered while loading first level using Unity free.</li>
<li>Android: Reworked LocationService and Compass, to only compensate the magnetic declination when location is updated.</li>
<li>Animation: Added error when assigning too few bind poses so mesh skin indexes would index out of bounds.</li>
<li>Animation: Fix null reference exception in Clip tab of Model Importer.</li>
<li>Audio: Fixed memory leak when attempting realtime streamed playback of tracker files (XM/MOD/IT/S3M). Realtime streamed playback is not supported for these files, but streams may still be used for loading the files fully before playing them.</li>
<li>Audio: Fixed some down-mixing issues when compressing multi-channel material for Android/iOS.</li>
<li>Audio: Fixed upside-down rendering of channels in previews.</li>
<li>Audio: Use of OnAudioFilterRead should no longer causes random crashes.</li>
<li>Audio: Fixed a memory leak when importing a large number of audio files at once.</li>
<li>Building: When list of included assets is printed to editor console, built-in resources have proper names now, instead of empty strings.</li>
<li>Caching: AssetBundles with a CRC not matching the request will be removed from the asset bundle cache.</li>
<li>CacheServer: Improved robustness of LRU size calculation when replacing files in the cache server.</li>
<li>Core: Fixed a crash where AsyncOperation.allowSceneActivation = false would cause an infinite loop when exiting playmode.</li>
<li>Core: Fixed crash when exiting playmode and allowSceneActivation being disabled.</li>
<li>Core: Fixed deadlock that could occur when asset bundles failed to load.</li>
<li>Core: Assets referenced by GUISkin are now corectly retained.</li>
<li>DX11: Fixed dynamic Meshes being inefficient on DirectX 11, mostly observable on WSA/WP8.</li>
<li>DX11: Fix crash when setting ComputeBuffer stride to zero.</li>
<li>DX11: Fixed Asset Store window not working on some machines when in DirectX 11 mode.</li>
<li>DX11: Fixed crash with stacked cameras, HDR and some image effect combinations.</li>
<li>DX11: Fixed some normal maps being decoded wrong (if the normal length has exceeded 1.0).</li>
<li>DX11: Make Raw compute buffer types actually work.</li>
<li>DX11: RenderTextures properly respect depthBits now; fixes really confusing behavior when a depth buffer was always created for a RenderTexture even if no depth buffer was requested.</li>
<li>DX11: Fixed some fixed function shaders (AlphaTest or projected textures), and some Fog combinations not working properly on Intel GPUs.</li>
</ul>

###  
<ul>
<li>Editor: Improved importing of semitransparent PSD texture files. They are premultiplied with white color; this will be accounted for in Unity now.</li>
<li>Editor: Active toolbar button rendered with correct style without a delay.</li>
<li>Editor: Animation preview rendering problems fixed.</li>
<li>Editor: AnimationWindow: Notify user if animating invalid game object hierarchy: When animating a object hiearchy user needs to ensure that names of object siblings are unique.</li>
<li>Editor: Calling Focus() on an invisible EditorWindow no longer crashes.</li>
<li>Editor: Camera frustum gizmo in Scene View now renders correctly when using normalized viewport rect.</li>
<li>Editor: Dark skin loads correctly after upgrading/activating a Pro license.</li>
<li>Editor: Displayed number of Asset Store previews in Project browser is consistent when zooming/resizing view.</li>
<li>Editor: Do not force RGBA format for normal maps when building for OpenGL ES targets.</li>
<li>Editor: Fix [HideInInspector] not working for shader properties.</li>
<li>Editor: Fix Aux Windows causing assert when closed on OS X.</li>
<li>Editor: Fix bad texture previews / mesh previews in linear lighting mode.</li>
<li>Editor: Fix broken occlusion culling overlay window.</li>
<li>Editor: Fix build target not updating correctly when switching between standalone platforms.</li>
<li>Editor: Fix color picker zoomed preview being upside down on OS X.</li>
<li>Editor: Fix copying of text in SelectableLabel in windows.</li>
<li>Editor: Fix crash if terrain alpha map textures get out of sync with the alpha map resolution setting.</li>
<li>Editor: Fix crash when loading assemblies with invalid references.</li>
<li>Editor: Fix crash while attempting to deserialize abstractly typed fields.</li>
<li>Editor: Fix flicker of progress bar when reserializing all assets to switch between text and binary serialization.</li>
<li>Editor: Fix inaccuracy caused by window margins in HandleUtility.WorldToGUIPoint() and HandleUtility.GUIPointToWorldRay().</li>
<li>Editor: Fix incorrect GameView rendering rect when having multiple GameViews.</li>
<li>Editor: Fix index out of bounds exception in BuildPlayerWindow when opening a project which was previously opened by another Unity Editor which had more platforms in the list.</li>
<li>Editor: Fix MonoBehaviour.OnApplicationFocus() on Windows platform.</li>
<li>Editor: Fix null ref when setting text mesh font with no renderer component.</li>
<li>Editor: Fix that animation window could not expand Transform components.</li>
<li>Editor: Fix that project browser multi-selection was lost when shift-selecting beyond start and end.</li>
<li>Editor: Fix that shift-delete deleted assets while renaming.</li>
<li>Editor: Fix the focus switch problem when the user press 'alt-tab' or 'ctrl-tab'.</li>
<li>Editor: Fixed "Export Package..." failing on OSX in some cases.</li>
<li>Editor: Fixed crash in lightmapping window when multi-selecting renderers.</li>
<li>Editor: Fixed crash when multi-selecting MonoBehaviours with missing scripts.</li>
<li>Editor: Fixed crash when opening scene with a reference to a prefab that has become empty.</li>
<li>Editor: Fixed empty Application.LoadLevelName after loading scene from an assetbundle.</li>
<li>Editor: Fixed forcing texture to be power of two size if PVRTC compression is selected.</li>
<li>Editor: Fixed lightmaps getting wrong compression format on platform change (between mobile and other platforms).</li>
<li>Editor: Fixed out of memory issue when building player with lots of resources files in it. Material texture references are now loaded on first use in the editor. In the player they are always preloaded.</li>
<li>Editor: Fixed Substance texture preview in some cases producing invalid mipmap bias settings.</li>
<li>Editor: Fixed that some keyboard keys could not be used for MenuItem shortcuts (e.g "," and "." can now be used).</li>
<li>Editor: Fixed wireframe scene view rendering not working on some shader model 3.0 shaders on Windows.</li>
<li>Editor: For Add Component window search function, always pick the first search result whenever the search changes.</li>
<li>Editor: Log error if user is calling GUI.Windows nested in window functions.</li>
<li>Editor: Make animated speed of transitions in AddComponent menu not be framerate dependent.</li>
<li>Editor: Make welcome dialog point to new URL for video tutorials.</li>
<li>Editor: Object Selector shows built-in shaders now.</li>
<li>Editor: Opening the Add Component window will now work when adding a MenuItem to the Components menu with priority less than 20.</li>
<li>Editor: Pasting a Particle System as a new component will now properly copy the Renderer values.</li>
<li>Editor: PropertyDrawers now also work for private members in base classes.</li>
<li>Editor: Scene view gizmo picking fixed.</li>
<li>Editor: Texture preview Labels will not be offset and clipped in some cases.</li>
<li>Editor: Throw mono exception (instead of crash), when unwrapping mesh without triangles assigned.</li>
<li>Editor: Fixed target texture size override not storing it's value correclty in the texture importer for the web player target.</li>
<li>Editor: Having a mesh asset preprocessor or doing Reset on mesh import settings no longer turns "Swap UVs" option on.</li>
<li>Fonts: Fixed embedding font data for styled fonts.</li>
<li>Fonts: Duplicating a dynamic font using Instantiate will result in garbage font rendering. User is now notified that duplicating a dynamic font is not allowed.</li>
<li>Graphics: Fix GrabPass when running fullscreen at non-native resolution on Mac and Linux.</li>
<li>Graphics: Fix linear lighting when running fullscreen at non-native resolution on Mac and Linux.</li>
<li>Graphics: Fixed "Use Lightmaps" in the Forward Rendering path, available via Lightmap Display scene view overlay.</li>
<li>Graphics: Fixed Camera.CopyFrom not copying some properties (rendering path, custom projection, layer cull distances etc.).</li>
<li>Graphics: Fixed development standalone players sometimes crashing on Windows when doing Alt-Tab.</li>
<li>Graphics: Fixed dynamic batching not working on meshes that use "Mesh Compression" import setting (regression in 4.0).</li>
<li>Graphics: Fixed incorrect scissoring of point/spot lights when a custom projection matrix is used.</li>
<li>Graphics: Fixed light "Draw Halo" checkbox not working unless there's some Halo component somewhere.</li>
<li>Graphics: Fixed point &amp; spot lights not affecting lightmapped objects in dual-lightmap forward rendering mode.</li>
<li>Graphics: Fixed RenderTextures being invalidated in Windows Standalone player when moving the window.</li>
<li>Graphics: Made the Rendering area in the profiler show proper stats on multithreaded Win-non-dx11, Mac, iOS and Flash.</li>
<li>Graphics: Using BlendOp in a shader doesn't cause the text in the Editor to appear garbled anymore.</li>
<li>Graphics: Fixed crash on Windows standalone player exit exit when using OpenGL.</li>
<li>Graphics: Fixed legacy MeshParticleEmitter crash when the mesh has no vertices.</li>
<li>iOS: Do not render the default cursor as no iOS devices support cursors.</li>
<li>iOS: Fixed CFBundleShortVersionString setting in Info.plist.</li>
<li>iOS: Fixed crash on startup on iPhone 3GS (some versions of iOS5), where empty array of screens is returned.</li>
<li>iOS: Fixed deprecated API usage for Keyboard.</li>
<li>iOS: Fixed gyroscope restart problem.</li>
<li>iOS: Fixed memory leak in GL.InvalidateState.</li>
<li>iOS: Fixed multiline Keyboard not having "done" button.</li>
<li>iOS: Fixed Ping stripping issue.</li>
<li>iOS: Fixed static batching performance regression.</li>
<li>iOS: Fixed various issues with video playback: view stretch after canceling video, second movie in a row cannot be played, status bar is not shown after returning from video, etc.</li>
<li>iOS: Fixed Xcode launching issue when script code supplies relative path.</li>
<li>iOS: Fixed iOS player hangup issue on single core devices.</li>
<li>iOS: Improved Guid API compatibility with managed code stripping.</li>
<li>iOS: Made structs/enums in trampoline be C-style typedefs, for better interop with ObjectiveC plugins.</li>
<li>iOS: Playing two movies in a row will not cause a second movie to disappear.</li>
<li>iOS: Project will not be replaced if doing a silent build and can't append to existing build. Instead, a save dialog will be shown.</li>
<li>iOS: Unity Remote now always will report multitouch supported.</li>
<li>Lightmapping: Fixed crash when a TextMesh has been marked for lightmapping.</li>
<li>Lightmapping: Lightmap atlasing now always tightly packs object UVs based on their bounding rectangles.</li>
<li>Lightmapping: Made baking of terrains much quicker when Color Space is set to Linear.</li>
<li>Linux: Copy StreamingAssets when building player.</li>
<li>Linux: Enable native rendering plugin callbacks.</li>
<li>Linux: Fix Application.CancelQuit() and Application.OpenURL().</li>
<li>Linux: Fix crash when attempting to read a non-readable mesh.</li>
<li>Linux: Fix double-click.</li>
<li>Linux: Fix miscellaneous rendering issues on low-end intel graphics cards.</li>
<li>Linux: Fix plugin detection when the plugin resides in a subfolder (DllImport("foo/bar")).</li>
<li>Linux: Fix pointer offsets when dynamically resizing player windows.</li>
<li>Linux: Fixed keyboard shortcuts for text fields.</li>
<li>Linux: Improve ctrl/alt/shift keypress detection; improved keyboard modifier handling while typing/mousing.</li>
<li>Linux: Make handling of scroll wheel axis more consistent with other platforms.</li>
<li>Mecanim: Fixed crash with interuptible transitions.</li>
<li>Mecanim: AnimationClip.length was not returning the right value for clip created from script.</li>
<li>Mecanim: Blending between two clip with negative scaling was wrongly returning a positive scale.</li>
<li>Mecanim: Check consistency for older avatar asset. Older avatar file pre 4.0 were not valid anymore and could crash in some cases.</li>
<li>Mecanim: Fix Avatar body mask UI accuracy. Selection around the neck and upper torso was not accurate.</li>
<li>Mecanim: Fix Avatar with scale on root not reaching IK goal.</li>
<li>Mecanim: Fix Blend Tree type selector in inspector.</li>
<li>Mecanim: Fix broken blend tree visualization when using Freeform Directional blending with no motion in the center.</li>
<li>Mecanim: Fix clip's additionnal curve binding to controller's parameter when type doesn't match.</li>
<li>Mecanim: Fix crash if you set a small speed value for a state and then preview any transition going from or to this state.</li>
<li>Mecanim: Fix culling bug, at runtime if you add a new renderer it was not added to the animator's list of renderer to compute if it should update the Animator.</li>
<li>Mecanim: Fix error message UnityEngine.Transform.get_position when creating an Avatar whose mesh is not skinned.</li>
<li>Mecanim: Fix IK hand moving on Y axis on iOS.</li>
<li>Mecanim: Fix iOS precision error for IK and root motion.</li>
<li>Mecanim: Fix MatchTarget function for small characters. The matching was done in the wrong transform space.</li>
<li>Mecanim: Fix memory leak in state machine; fix memory leak with recorder.</li>
<li>Mecanim: Fix multi selection of node in animator window now correctly delete all selected node rather than just the last one.</li>
<li>Mecanim: Fix multi-edition of Animator, avatar and apply root motion field can now be multi-edited too.</li>
<li>Mecanim: Fix NullRefException when selecting a prefab with Animator Controller set to null.</li>
<li>Mecanim: Fix Reset button for Animator.</li>
<li>Mecanim: Fix StateMachine copy-paste.</li>
<li>Mecanim: Fixed crash in transition preview with 1 frame animation.</li>
<li>Mecanim: Fixed crash when building standalone with synchronized layer referencing a layer that was after the synchronized layer in the layer's list.</li>
<li>Mecanim: Fixed crash when previewing empty AnimatorController.</li>
<li>Mecanim: Fixed crash when previewing transition with state with no animation.</li>
<li>Mecanim: Fixed preview state mirror in transition preview.</li>
<li>Mecanim: Fixed transition reordering with different StateMachines.</li>
<li>Mecanim: Fixes crash when deleting or reordering some transitions; and with 0 duration transitions.</li>
<li>Mecanim: Fixes transition previewer being slow.</li>
<li>Mecanim: In some case Avatar mapping was not saved correctly when manually set by a user. Transform not attached to a renderer or without any child attached to a renderer were discarded.</li>
<li>Mecanim: OnAnimatorIK and OnAnimatorMove () won't be call anymore on disabled scripts.</li>
<li>Mecanim: Right-clicking on a state in the Animator window now properly shows the context menu.</li>
<li>Mecanim: When creating a transition from or to a blend tree with no motion, the transition duration was set to Infinity which could produce some crash or hang unity when trying to preview this transition.</li>
<li>Mecanim: Fixed transitions with transforms having negative scales.</li>
<li>Mobile: Fixed occasional crash in Substance system when loading Asset Bundles.</li>
<li>Mobile: Fixed RenderTexture.DiscardContents to correctly use glDiscardFramebufferEXT.</li>
<li>Mobile: Fixed unaligned memory accesses in BitStream.</li>
<li>Native Client: Fixed a bug in color multiplication math which could cause wrong colors to be displayed.</li>
<li>Native Client: Fixed a crash loading PNG files.</li>
<li>Native Client: Fixed asset garbage collection not to incorrectly collect assets which were still being referenced.</li>
<li>Native Client: Fixed some rendering issues with particles when the mouse is clicked.</li>
<li>Native Client: Mono is now built from our own sources and is no longer subject to the LGPL.</li>
<li>Native Client: Fix "Development Player" label always showing.</li>
<li>Native Client: Fix color of Terrain details.</li>
<li>Native Client: Fix File Access error message on start up.</li>
<li>Native Client: Fix incorrect methods being used for http requests in WWW class (POST instead of GET).</li>
<li>Native Client: Fixed a memory leak in the WWW class.</li>
<li>Native Client: Fixed a potential crash when loading unity3d files (including the game main data itself).</li>
<li>NavMesh: Fixed crash when loading scenes while NavMeshAgents are marked by "DontDestroyOnLoad".</li>
<li>NavMesh: Fixed issue where agent move state was affected when calling CompleOffMeshLink while not occupying an OffMeshLink.</li>
<li>NavMesh: Fixed issue where calling ResetPath while occupying an OffMeshLink would leave the OffMeshLink inaccessible.</li>
<li>NavMesh: Fixed issue where NavMesh.SamplePosition could return sub-optimal position for large query radius.</li>
<li>NavMesh: Fixed issue where outstanding agent path requests could get corrupted when adding new agents.</li>
<li>NavMesh: Fixed issue where remainingDistance would return too optimistic value.</li>
<li>NavMesh: Fixed regression where agent would accelerate too fast when doing moves shorter that agent diameter.</li>
<li>Physics: Changing gravity will wake up sleeping Rigidbodies.</li>
<li>Physics: Fixed a crash in raycasts against BoxColliders on 64 bit Windows.</li>
<li>Physics: Fixed a crash related to destroying colliders while Time.timeScale is zero.</li>
<li>Physics: Hinge Joints now have sane range limits.</li>
<li>Scripting: Fixes to Mono GC to avoid 'GetThreadContext' error issue on Windows.</li>
<li>Scripting: Fix constraints for Time.scale so that it cannot be negative.</li>
<li>Scripting: "new Font()" will now produce a valid Font instance (useful when programmatically generating font assets).</li>
<li>Scripting: Avoid crash if behaviors are destroyed from OnDisable.</li>
<li>Scripting: Avoid crash when creating MaterialPropertyBlock in MonoBehaviour constructor.</li>
<li>Scripting: Editor and Windows standalone should now be able to correctly use Mono.Posix assembly.</li>
<li>Scripting: Fix Windows crash on OutOfMemory.</li>
<li>Shaders: Fixed HLSL-to-GLSL shader translation when a shader modifies global variables; regression introduced in 4.1.</li>
<li>Shaders: Fixed tex2Dgrad/texCUBElod/texCUBEgrad support for mobile shaders.</li>
<li>Shaders: Fixed rare bug when a fixed function dot3 texture combiner could get wrong alpha channel state.</li>
<li>Shaders: Fixed shader keywords not being copied for instantiated materials.</li>
<li>Shaders: Fixed some surface shaders not being liked by DX11 shader compiler (errors about structs not being fully initialized).</li>
<li>Shaders: Fixed surface shader code generation if you're trying to output Normal into Emission, and are not writing to normal otherwise.</li>
<li>Shaders: Make sure that vertex shader output is always high precision on mobile; fixes some problems on Mali 6xx GPUs if you accidentally have half4 position.</li>
<li>Shaders: Worked around Cg shader code generation bug that happened on saturate(texture2D(...)); Cg was generating invalid D3D9 shader code on this.</li>
<li>Shuriken: Fix collision module such that trigger objects do not cause particle collisions.</li>
<li>Shuriken: Fixed errors when manually emitting particles with a non-unit axis of rotation.</li>
<li>Shuriken: Fixed horizontal and vertical billboard modes to be properly aligned with coordinate axes.</li>
<li>Shuriken: Fixed issue with particle systems not shutting down properly.</li>
<li>Shuriken: Fixed some gradient settings being lost when upgrading project from Unity 3.5.x to 4.x.</li>
<li>Shuriken: Fixed issue with Emit() function when the particle system has a scaled parent object. The emitter shape would be scaled incorrectly.</li>
<li>Substance: B2M instances should no longer lose their output texture references when entering/leaving Play mode.</li>
<li>Substance: Better strategy for mapping ProceduralTextures to shaders slots and for remembering custom assignments.</li>
<li>Substance: Fix crash due to a race condition on resource deallocation.</li>
<li>Substance: It is now possible to properly clone all substance graphs in a SBSAR (previously the first cloned graph would be instantiated when cloning other graphs).</li>
<li>Substance: Instance names are now properly sorted in the Inspector (B2M_10 would previously be listed before B2M_2).</li>
<li>Substance: Unnecessary reimports of multigraph Substances are no longer performed when leaving Play mode.</li>
<li>Substance: Deletion of the single remaining instance of a ProceduralMaterial in the Inspector is now prevented (this would previously result in an empty SubstanceImporter).</li>
<li>Substance: Option groups for newly cloned/instantiated substances in the Inspector no longer show only the first option from each group.</li>
<li>Substance: ProceduralMaterials attached to prefabs that were loaded in levels other than the first one and that were cloned but not modified themselves are no longer reimported after exiting Play mode.</li>
<li>Substance: ProceduralTexture::GetPixels32 now works on cloned substances.</li>
<li>Substance: SBSAR should now properly auto-refresh when the asset is modified on disk.</li>
<li>Substance: Fixed potential deadlock when using ProceduralMaterial.</li>
<li>Substance: Fixed memory leak.</li>
<li>Substance: DoNothing substances in asset bundles are no longer generated when the assetbundle is loaded, but only when RebuildTextures/Immediately is called instead.</li>
<li>Substance: Resetting a ProceduralMaterial from the Inspector no longer causes the 'Generate All Outputs' checkbox to be checked.</li>
<li>UnityGUI: Fix crash when passing a null GUIContent to various methods.</li>
<li>Web Player: Fixed regression playing back content using old grid fonts.</li>
<li>Web Player: Fixed a bug in PlayerPrefs, which made Firefox crash on close.</li>
<li>Web Player: Fixed some crashes during startup and when entering full-screen mode.</li>
<li>Webcam: Fixed Fatal Error on scene loading when WebCamTexture was used in a scene; and fixed a crash on quitting Windows Standalone players with webcam textures.</li>
<li>Webcam: When requesting user authorization to use microphone Unity was previously asking for permission to the web camera.</li>
<li>Windows: Fixed crash when closing the display resolution dialog of the player.</li>
<li>WWW: Fixed CRC calculation to give correct results.</li>
</ul>
