# Unity 4.2

https://unity3d.com/unity/whats-new/unity-4.2

## Fixes

- [](#)


*   Android: Support for Android SDK rev22.
*   Android: Added a workaround for ANR when using Apple magic mouse; fixed ANR caused by deadlock when using touch enabled controllers.
*   Android: Added exception checks to avoid crashes in AndroidJNI.
*   Android: Added JDK version detection.
*   Android: Application no longer quits if joystick button 'A' is pressed before the first level has loaded.
*   Android: Disabled shader cache on pre-Honeycomb devices due to buggy drivers; also disabled it on all Immersion GPUs due to driver bugs.
*   Android: Editor; when switching between building a project and an actual apk, project is no longer replaced by the apk.
*   Android: Fixed a problem with streaming assets in exported android project.
*   Android: Fixed an issue where it was impossible to delete a project on windows due to adb keeping a lock in the project directory.
*   Android: Fixed crash on GL context recreate.
*   Android: Fixed crash when trying to read a non-existent string field through JNI.
*   Android: Fixed IndexOutOfRangeException on faulty package name.
*   Android: Fixed occasional crash on Nexus4 in shader compilation.
*   Android: Fixed problem with crashing video player on 1st gen Kindle Fire.
*   Android: Fixed propagation of key input events to OnGUI().
*   Android: Fixed touch and stylus input on devices having a single surface emitting both at the same time.
*   Android: Re-initialization of UnityPlayer is now possible.
*   Android: Removed black screen rendered while loading first level using Unity free.
*   Android: Reworked LocationService and Compass, to only compensate the magnetic declination when location is updated.
*   Animation: Added error when assigning too few bind poses so mesh skin indexes would index out of bounds.
*   Animation: Fix null reference exception in Clip tab of Model Importer.
*   Audio: Fixed memory leak when attempting realtime streamed playback of tracker files (XM/MOD/IT/S3M). Realtime streamed playback is not supported for these files, but streams may still be used for loading the files fully before playing them.
*   Audio: Fixed some down-mixing issues when compressing multi-channel material for Android/iOS.
*   Audio: Fixed upside-down rendering of channels in previews.
*   Audio: Use of OnAudioFilterRead should no longer causes random crashes.
*   Audio: Fixed a memory leak when importing a large number of audio files at once.
*   Building: When list of included assets is printed to editor console, built-in resources have proper names now, instead of empty strings.
*   Caching: AssetBundles with a CRC not matching the request will be removed from the asset bundle cache.
*   CacheServer: Improved robustness of LRU size calculation when replacing files in the cache server.
*   Core: Fixed a crash where AsyncOperation.allowSceneActivation = false would cause an infinite loop when exiting playmode.
*   Core: Fixed crash when exiting playmode and allowSceneActivation being disabled.
*   Core: Fixed deadlock that could occur when asset bundles failed to load.
*   Core: Assets referenced by GUISkin are now corectly retained.
*   DX11: Fixed dynamic Meshes being inefficient on DirectX 11, mostly observable on WSA/WP8.
*   DX11: Fix crash when setting ComputeBuffer stride to zero.
*   DX11: Fixed Asset Store window not working on some machines when in DirectX 11 mode.
*   DX11: Fixed crash with stacked cameras, HDR and some image effect combinations.
*   DX11: Fixed some normal maps being decoded wrong (if the normal length has exceeded 1.0).
*   DX11: Make Raw compute buffer types actually work.
*   DX11: RenderTextures properly respect depthBits now; fixes really confusing behavior when a depth buffer was always created for a RenderTexture even if no depth buffer was requested.
*   DX11: Fixed some fixed function shaders (AlphaTest or projected textures), and some Fog combinations not working properly on Intel GPUs.

*   Editor: Improved importing of semitransparent PSD texture files. They are premultiplied with white color; this will be accounted for in Unity now.
*   Editor: Active toolbar button rendered with correct style without a delay.
*   Editor: Animation preview rendering problems fixed.
*   Editor: AnimationWindow: Notify user if animating invalid game object hierarchy: When animating a object hiearchy user needs to ensure that names of object siblings are unique.
*   Editor: Calling Focus() on an invisible EditorWindow no longer crashes.
*   Editor: Camera frustum gizmo in Scene View now renders correctly when using normalized viewport rect.
*   Editor: Dark skin loads correctly after upgrading/activating a Pro license.
*   Editor: Displayed number of Asset Store previews in Project browser is consistent when zooming/resizing view.
*   Editor: Do not force RGBA format for normal maps when building for OpenGL ES targets.
*   Editor: Fix \[HideInInspector\] not working for shader properties.
*   Editor: Fix Aux Windows causing assert when closed on OS X.
*   Editor: Fix bad texture previews / mesh previews in linear lighting mode.
*   Editor: Fix broken occlusion culling overlay window.
*   Editor: Fix build target not updating correctly when switching between standalone platforms.
*   Editor: Fix color picker zoomed preview being upside down on OS X.
*   Editor: Fix copying of text in SelectableLabel in windows.
*   Editor: Fix crash if terrain alpha map textures get out of sync with the alpha map resolution setting.
*   Editor: Fix crash when loading assemblies with invalid references.
*   Editor: Fix crash while attempting to deserialize abstractly typed fields.
*   Editor: Fix flicker of progress bar when reserializing all assets to switch between text and binary serialization.
*   Editor: Fix inaccuracy caused by window margins in HandleUtility.WorldToGUIPoint() and HandleUtility.GUIPointToWorldRay().
*   Editor: Fix incorrect GameView rendering rect when having multiple GameViews.
*   Editor: Fix index out of bounds exception in BuildPlayerWindow when opening a project which was previously opened by another Unity Editor which had more platforms in the list.
*   Editor: Fix MonoBehaviour.OnApplicationFocus() on Windows platform.
*   Editor: Fix null ref when setting text mesh font with no renderer component.
*   Editor: Fix that animation window could not expand Transform components.
*   Editor: Fix that project browser multi-selection was lost when shift-selecting beyond start and end.
*   Editor: Fix that shift-delete deleted assets while renaming.
*   Editor: Fix the focus switch problem when the user press 'alt-tab' or 'ctrl-tab'.
*   Editor: Fixed "Export Package..." failing on OSX in some cases.
*   Editor: Fixed crash in lightmapping window when multi-selecting renderers.
*   Editor: Fixed crash when multi-selecting MonoBehaviours with missing scripts.
*   Editor: Fixed crash when opening scene with a reference to a prefab that has become empty.
*   Editor: Fixed empty Application.LoadLevelName after loading scene from an assetbundle.
*   Editor: Fixed forcing texture to be power of two size if PVRTC compression is selected.
*   Editor: Fixed lightmaps getting wrong compression format on platform change (between mobile and other platforms).
*   Editor: Fixed out of memory issue when building player with lots of resources files in it. Material texture references are now loaded on first use in the editor. In the player they are always preloaded.
*   Editor: Fixed Substance texture preview in some cases producing invalid mipmap bias settings.
*   Editor: Fixed that some keyboard keys could not be used for MenuItem shortcuts (e.g "," and "." can now be used).
*   Editor: Fixed wireframe scene view rendering not working on some shader model 3.0 shaders on Windows.
*   Editor: For Add Component window search function, always pick the first search result whenever the search changes.
*   Editor: Log error if user is calling GUI.Windows nested in window functions.
*   Editor: Make animated speed of transitions in AddComponent menu not be framerate dependent.
*   Editor: Make welcome dialog point to new URL for video tutorials.
*   Editor: Object Selector shows built-in shaders now.
*   Editor: Opening the Add Component window will now work when adding a MenuItem to the Components menu with priority less than 20.
*   Editor: Pasting a Particle System as a new component will now properly copy the Renderer values.
*   Editor: PropertyDrawers now also work for private members in base classes.
*   Editor: Scene view gizmo picking fixed.
*   Editor: Texture preview Labels will not be offset and clipped in some cases.
*   Editor: Throw mono exception (instead of crash), when unwrapping mesh without triangles assigned.
*   Editor: Fixed target texture size override not storing it's value correclty in the texture importer for the web player target.
*   Editor: Having a mesh asset preprocessor or doing Reset on mesh import settings no longer turns "Swap UVs" option on.
*   Fonts: Fixed embedding font data for styled fonts.
*   Fonts: Duplicating a dynamic font using Instantiate will result in garbage font rendering. User is now notified that duplicating a dynamic font is not allowed.
*   Graphics: Fix GrabPass when running fullscreen at non-native resolution on Mac and Linux.
*   Graphics: Fix linear lighting when running fullscreen at non-native resolution on Mac and Linux.
*   Graphics: Fixed "Use Lightmaps" in the Forward Rendering path, available via Lightmap Display scene view overlay.
*   Graphics: Fixed Camera.CopyFrom not copying some properties (rendering path, custom projection, layer cull distances etc.).
*   Graphics: Fixed development standalone players sometimes crashing on Windows when doing Alt-Tab.
*   Graphics: Fixed dynamic batching not working on meshes that use "Mesh Compression" import setting (regression in 4.0).
*   Graphics: Fixed incorrect scissoring of point/spot lights when a custom projection matrix is used.
*   Graphics: Fixed light "Draw Halo" checkbox not working unless there's some Halo component somewhere.
*   Graphics: Fixed point & spot lights not affecting lightmapped objects in dual-lightmap forward rendering mode.
*   Graphics: Fixed RenderTextures being invalidated in Windows Standalone player when moving the window.
*   Graphics: Made the Rendering area in the profiler show proper stats on multithreaded Win-non-dx11, Mac, iOS and Flash.
*   Graphics: Using BlendOp in a shader doesn't cause the text in the Editor to appear garbled anymore.
*   Graphics: Fixed crash on Windows standalone player exit exit when using OpenGL.
*   Graphics: Fixed legacy MeshParticleEmitter crash when the mesh has no vertices.
*   iOS: Do not render the default cursor as no iOS devices support cursors.
*   iOS: Fixed CFBundleShortVersionString setting in Info.plist.
*   iOS: Fixed crash on startup on iPhone 3GS (some versions of iOS5), where empty array of screens is returned.
*   iOS: Fixed deprecated API usage for Keyboard.
*   iOS: Fixed gyroscope restart problem.
*   iOS: Fixed memory leak in GL.InvalidateState.
*   iOS: Fixed multiline Keyboard not having "done" button.
*   iOS: Fixed Ping stripping issue.
*   iOS: Fixed static batching performance regression.
*   iOS: Fixed various issues with video playback: view stretch after canceling video, second movie in a row cannot be played, status bar is not shown after returning from video, etc.
*   iOS: Fixed Xcode launching issue when script code supplies relative path.
*   iOS: Fixed iOS player hangup issue on single core devices.
*   iOS: Improved Guid API compatibility with managed code stripping.
*   iOS: Made structs/enums in trampoline be C-style typedefs, for better interop with ObjectiveC plugins.
*   iOS: Playing two movies in a row will not cause a second movie to disappear.
*   iOS: Project will not be replaced if doing a silent build and can't append to existing build. Instead, a save dialog will be shown.
*   iOS: Unity Remote now always will report multitouch supported.
*   Lightmapping: Fixed crash when a TextMesh has been marked for lightmapping.
*   Lightmapping: Lightmap atlasing now always tightly packs object UVs based on their bounding rectangles.
*   Lightmapping: Made baking of terrains much quicker when Color Space is set to Linear.
*   Linux: Copy StreamingAssets when building player.
*   Linux: Enable native rendering plugin callbacks.
*   Linux: Fix Application.CancelQuit() and Application.OpenURL().
*   Linux: Fix crash when attempting to read a non-readable mesh.
*   Linux: Fix double-click.
*   Linux: Fix miscellaneous rendering issues on low-end intel graphics cards.
*   Linux: Fix plugin detection when the plugin resides in a subfolder (DllImport("foo/bar")).
*   Linux: Fix pointer offsets when dynamically resizing player windows.
*   Linux: Fixed keyboard shortcuts for text fields.
*   Linux: Improve ctrl/alt/shift keypress detection; improved keyboard modifier handling while typing/mousing.
*   Linux: Make handling of scroll wheel axis more consistent with other platforms.
*   Mecanim: Fixed crash with interuptible transitions.
*   Mecanim: AnimationClip.length was not returning the right value for clip created from script.
*   Mecanim: Blending between two clip with negative scaling was wrongly returning a positive scale.
*   Mecanim: Check consistency for older avatar asset. Older avatar file pre 4.0 were not valid anymore and could crash in some cases.
*   Mecanim: Fix Avatar body mask UI accuracy. Selection around the neck and upper torso was not accurate.
*   Mecanim: Fix Avatar with scale on root not reaching IK goal.
*   Mecanim: Fix Blend Tree type selector in inspector.
*   Mecanim: Fix broken blend tree visualization when using Freeform Directional blending with no motion in the center.
*   Mecanim: Fix clip's additionnal curve binding to controller's parameter when type doesn't match.
*   Mecanim: Fix crash if you set a small speed value for a state and then preview any transition going from or to this state.
*   Mecanim: Fix culling bug, at runtime if you add a new renderer it was not added to the animator's list of renderer to compute if it should update the Animator.
*   Mecanim: Fix error message UnityEngine.Transform.get\_position when creating an Avatar whose mesh is not skinned.
*   Mecanim: Fix IK hand moving on Y axis on iOS.
*   Mecanim: Fix iOS precision error for IK and root motion.
*   Mecanim: Fix MatchTarget function for small characters. The matching was done in the wrong transform space.
*   Mecanim: Fix memory leak in state machine; fix memory leak with recorder.
*   Mecanim: Fix multi selection of node in animator window now correctly delete all selected node rather than just the last one.
*   Mecanim: Fix multi-edition of Animator, avatar and apply root motion field can now be multi-edited too.
*   Mecanim: Fix NullRefException when selecting a prefab with Animator Controller set to null.
*   Mecanim: Fix Reset button for Animator.
*   Mecanim: Fix StateMachine copy-paste.
*   Mecanim: Fixed crash in transition preview with 1 frame animation.
*   Mecanim: Fixed crash when building standalone with synchronized layer referencing a layer that was after the synchronized layer in the layer's list.
*   Mecanim: Fixed crash when previewing empty AnimatorController.
*   Mecanim: Fixed crash when previewing transition with state with no animation.
*   Mecanim: Fixed preview state mirror in transition preview.
*   Mecanim: Fixed transition reordering with different StateMachines.
*   Mecanim: Fixes crash when deleting or reordering some transitions; and with 0 duration transitions.
*   Mecanim: Fixes transition previewer being slow.
*   Mecanim: In some case Avatar mapping was not saved correctly when manually set by a user. Transform not attached to a renderer or without any child attached to a renderer were discarded.
*   Mecanim: OnAnimatorIK and OnAnimatorMove () won't be call anymore on disabled scripts.
*   Mecanim: Right-clicking on a state in the Animator window now properly shows the context menu.
*   Mecanim: When creating a transition from or to a blend tree with no motion, the transition duration was set to Infinity which could produce some crash or hang unity when trying to preview this transition.
*   Mecanim: Fixed transitions with transforms having negative scales.
*   Mobile: Fixed occasional crash in Substance system when loading Asset Bundles.
*   Mobile: Fixed RenderTexture.DiscardContents to correctly use glDiscardFramebufferEXT.
*   Mobile: Fixed unaligned memory accesses in BitStream.
*   Native Client: Fixed a bug in color multiplication math which could cause wrong colors to be displayed.
*   Native Client: Fixed a crash loading PNG files.
*   Native Client: Fixed asset garbage collection not to incorrectly collect assets which were still being referenced.
*   Native Client: Fixed some rendering issues with particles when the mouse is clicked.
*   Native Client: Mono is now built from our own sources and is no longer subject to the LGPL.
*   Native Client: Fix "Development Player" label always showing.
*   Native Client: Fix color of Terrain details.
*   Native Client: Fix File Access error message on start up.
*   Native Client: Fix incorrect methods being used for http requests in WWW class (POST instead of GET).
*   Native Client: Fixed a memory leak in the WWW class.
*   Native Client: Fixed a potential crash when loading unity3d files (including the game main data itself).
*   NavMesh: Fixed crash when loading scenes while NavMeshAgents are marked by "DontDestroyOnLoad".
*   NavMesh: Fixed issue where agent move state was affected when calling CompleOffMeshLink while not occupying an OffMeshLink.
*   NavMesh: Fixed issue where calling ResetPath while occupying an OffMeshLink would leave the OffMeshLink inaccessible.
*   NavMesh: Fixed issue where NavMesh.SamplePosition could return sub-optimal position for large query radius.
*   NavMesh: Fixed issue where outstanding agent path requests could get corrupted when adding new agents.
*   NavMesh: Fixed issue where remainingDistance would return too optimistic value.
*   NavMesh: Fixed regression where agent would accelerate too fast when doing moves shorter that agent diameter.
*   Physics: Changing gravity will wake up sleeping Rigidbodies.
*   Physics: Fixed a crash in raycasts against BoxColliders on 64 bit Windows.
*   Physics: Fixed a crash related to destroying colliders while Time.timeScale is zero.
*   Physics: Hinge Joints now have sane range limits.
*   Scripting: Fixes to Mono GC to avoid 'GetThreadContext' error issue on Windows.
*   Scripting: Fix constraints for Time.scale so that it cannot be negative.
*   Scripting: "new Font()" will now produce a valid Font instance (useful when programmatically generating font assets).
*   Scripting: Avoid crash if behaviors are destroyed from OnDisable.
*   Scripting: Avoid crash when creating MaterialPropertyBlock in MonoBehaviour constructor.
*   Scripting: Editor and Windows standalone should now be able to correctly use Mono.Posix assembly.
*   Scripting: Fix Windows crash on OutOfMemory.
*   Shaders: Fixed HLSL-to-GLSL shader translation when a shader modifies global variables; regression introduced in 4.1.
*   Shaders: Fixed tex2Dgrad/texCUBElod/texCUBEgrad support for mobile shaders.
*   Shaders: Fixed rare bug when a fixed function dot3 texture combiner could get wrong alpha channel state.
*   Shaders: Fixed shader keywords not being copied for instantiated materials.
*   Shaders: Fixed some surface shaders not being liked by DX11 shader compiler (errors about structs not being fully initialized).
*   Shaders: Fixed surface shader code generation if you're trying to output Normal into Emission, and are not writing to normal otherwise.
*   Shaders: Make sure that vertex shader output is always high precision on mobile; fixes some problems on Mali 6xx GPUs if you accidentally have half4 position.
*   Shaders: Worked around Cg shader code generation bug that happened on saturate(texture2D(...)); Cg was generating invalid D3D9 shader code on this.
*   Shuriken: Fix collision module such that trigger objects do not cause particle collisions.
*   Shuriken: Fixed errors when manually emitting particles with a non-unit axis of rotation.
*   Shuriken: Fixed horizontal and vertical billboard modes to be properly aligned with coordinate axes.
*   Shuriken: Fixed issue with particle systems not shutting down properly.
*   Shuriken: Fixed some gradient settings being lost when upgrading project from Unity 3.5.x to 4.x.
*   Shuriken: Fixed issue with Emit() function when the particle system has a scaled parent object. The emitter shape would be scaled incorrectly.
*   Substance: B2M instances should no longer lose their output texture references when entering/leaving Play mode.
*   Substance: Better strategy for mapping ProceduralTextures to shaders slots and for remembering custom assignments.
*   Substance: Fix crash due to a race condition on resource deallocation.
*   Substance: It is now possible to properly clone all substance graphs in a SBSAR (previously the first cloned graph would be instantiated when cloning other graphs).
*   Substance: Instance names are now properly sorted in the Inspector (B2M\_10 would previously be listed before B2M\_2).
*   Substance: Unnecessary reimports of multigraph Substances are no longer performed when leaving Play mode.
*   Substance: Deletion of the single remaining instance of a ProceduralMaterial in the Inspector is now prevented (this would previously result in an empty SubstanceImporter).
*   Substance: Option groups for newly cloned/instantiated substances in the Inspector no longer show only the first option from each group.
*   Substance: ProceduralMaterials attached to prefabs that were loaded in levels other than the first one and that were cloned but not modified themselves are no longer reimported after exiting Play mode.
*   Substance: ProceduralTexture::GetPixels32 now works on cloned substances.
*   Substance: SBSAR should now properly auto-refresh when the asset is modified on disk.
*   Substance: Fixed potential deadlock when using ProceduralMaterial.
*   Substance: Fixed memory leak.
*   Substance: DoNothing substances in asset bundles are no longer generated when the assetbundle is loaded, but only when RebuildTextures/Immediately is called instead.
*   Substance: Resetting a ProceduralMaterial from the Inspector no longer causes the 'Generate All Outputs' checkbox to be checked.
*   UnityGUI: Fix crash when passing a null GUIContent to various methods.
*   Web Player: Fixed regression playing back content using old grid fonts.
*   Web Player: Fixed a bug in PlayerPrefs, which made Firefox crash on close.
*   Web Player: Fixed some crashes during startup and when entering full-screen mode.
*   Webcam: Fixed Fatal Error on scene loading when WebCamTexture was used in a scene; and fixed a crash on quitting Windows Standalone players with webcam textures.
*   Webcam: When requesting user authorization to use microphone Unity was previously asking for permission to the web camera.
*   Windows: Fixed crash when closing the display resolution dialog of the player.
*   WWW: Fixed CRC calculation to give correct results.