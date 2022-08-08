# Unity 5.0

https://unity3d.com/unity/whats-new/unity-5.0

## Features

- [AI](#ai)
- [Android](#android)
- [Animation](#animation)
- [Audio](#audio)
- [Consoles](#consoles)
- [Editor](#editor)
- [Graphics](#graphics)
- [iOS](#ios)
- [Linux & SteamOS](#linux--steamos)
- [Physics](#physics)
- [Scripting](#scripting)
- [Shaders](#shaders)
- [Standard Assets](#standard-assets)
- [Unity Download Assistant](#unity-download-assistant)
- [WebGL](#webgl)


### AI

*   NavMesh supports LoadLevelAdditive
*   Improved performance and reduced memory consumption:
    *   NavMeshObstacles update is multi-threaded now. Carving speed generally improved 2-4x.
    *   NavMesh data for non-carved regions takes ~2x less memory now.
    *   Performance improvements for multi-threaded NavMeshAgent updates.
    *   HeightMeshes bake faster, work faster at runtime, and use ~35% less memory.
    *   Path replanning in presence of many carving obstacles is faster and more accurate.
*   Improved inspectors and debug visualizations:
    *   NavMesh Areas inspector (previously NavMesh Layers) got a facelift.
    *   Reorganized parameters NavMeshAgent inspector.
    *   Added carve hull debug visualisation for NavMeshObstacles.
    *   Added visualisation on how NavMesh bake settings relate to each other.

#### Improved inspectors and debug visualizations

*   Improved accuracy and raised limits:
    *   NavMeshObstacle supports two basic shapes - cylinder and box for both carving and avoidance.
    *   Improved automatic Off-Mesh Link collision detection accuracy. Note that this will change how off-mesh links placement on existing scenes.
    *   Improved navmesh point location/mapping when height mesh is used.
    *   Increased the height range of NavMesh baking (can build meshes for taller scenes).
    *   Made Height Mesh query more resilient to small holes in input geometry.
    *   NavMesh obstacle rotation is take into account when carving and avoiding.
    *   NavMesh tile count limit lifted from 216 to 228.
    *   NavMeshPath and NavMeshAgent paths removed 256 polygon limit.
    *   OffMeshLink - removed restriction on tile span - previously connected only up to neighbouring tiles.

### Android

*   KitKat Immersive Fullscreen Mode. Applied by default.
*   Rendering to multiple displays.
*   Rendering to custom java surfaces. Exposed in Unity as additional displays.
*   AAR Support. AAR files can now be used as a replacement for Android Library Project folders.

### Animation

*   State Machine Behaviours
    *   StateMachineBehaviours is a new MonoBehaviour-like Component that can be added to a StateMachine state to attach callbacks
    *   Available callbacks are : OnStateEnter, OnStateExit, OnStateUpdate, OnStateMove, OnStateIK, OnStateMachineEnter and OnStateMachineExit
    *   Animator.GetBehaviour(). This function return the first StateMachineBehaviour that match type T

#### State Machine Behaviours

*   StateMachine Transitions
    *   Can now add higher level transitions from StateMachine to StateMachine
    *   Entry and Exit nodes define how the StateMachine behaves upon entering and exiting.

#### StateMachine Transitions

*   Asset API
    *   Allows to create and edit, in Editor, all types of Mecanim assets ( Controllers, StateMachines, BlendTree etc.)
    *   Added API for Avatar, Motion Nodes, Events and Curve in the Model Importer
*   Direct Blend Tree.
    *   New type of blend tree to control the weight of each child independently

#### Direct Blend Tree (Character by Mixamo)

*   Root Motion authoring
    *   Can convert animation on the parent transform into Root Motion (Delta Animation)

#### Root Motion authoring

*   Animator Tool revamp
    *   Improved workflow
    *   Re-orderable layers and parameters

#### Animator Tool revamp

*   Transition interruption source.
    *   Replaces the Atomic setting on transitions. You can now decide if a transition is interrupted by transitions in the source state, the destination state or both.
    *   Also possible to be interrupted by transitions independently of their order by disabling "ordered interruption" setting on transitions.

#### Transition interruption source

*   Added Animator Gizmo that show up upon selection: you can see the mass center, avatar root and the pivot.
*   IK Hint for knees and elbows.

#### IK Hint for knees and elbows (Character by Mixamo)

*   Improved animation previewer camera.
    *   Camera can now Pan, Orbit and Scale with the same control than the scene viewer.
    *   The camera can also frame on the previewed Object with shortcut F and frame on the cursor position with shortcut G.
*   AnimationEvents are now fully editable at runtime, see AnimationClip.events to query, add and delete them at runtime
*   Keep last evaluated value when a property stops to be animated.
    *   Activated per State
    *   By default it is writing default value when a property stops to be evaluated
*   Linear Velocity Blending
    *   Advanced feature for users requiring linear speed interpolation during blending.
    *   Root Motion Speed and Angular Speed now blend linearly in Blend Trees, Transition or Layers
    *   Choose between Linear Velocity Blending or Linear Position Blending in Animator with animator.linearVelocityBlending. It is false by default.
    *   You can now get Animator root motion velocity and angular velocity with animator.velocity and animator.angularVelocity

### Audio

*   Added a new AudioMixer asset type! Create one or more AudioMixers in a project. ![description](/sites/default/files/styles/original/public/audio-1.jpg?itok=1Bx36-_T)
    *   Use the Audio Mixer window to create complex mixing hierarchies and effect processing chains.
    *   Mix and master all audio within Unity by tweaking all parameters during edit mode and play mode.
    *   VU meters for the outputs of all AudioGroup and at attenuation points within the AudioGroup.
    *   Allow AudioSources to route their signal into any AudioMixer.
    *   The audio output of one AudioMixer can be routed into any AudioGroup of any other AudioMixer, allowing complex re-configurable Audio processing.
    *   Audio "Sends" and "Receives" can be inserted anywhere into the signal chain of an AudioGroup.
    *   The attenuation of an AudioGroup can be applied at any point in the AudioGroup (allowing pre and post fader effects).
    *   Snapshots of mixer state (on all parameters) can be created for AudioMixers. These snapshots can be interpolated between during play through a set of per-parameter transition curves.
    *   Snapshots can also be weighted blended (2 or more snapshots).
    *   Any parameter (volume / pitch / effect parameter etc) can be exposed via a name to the runtime API allowing very precise tweaking of any parameter in a mixer during game play.
    *   Mixer "Views" can be created so that complex mixer hierarchies can be narrowed down in the GUI allowing focus on tweaking certain parts of the mix (music / foley / etc).
    *   AudioGroups can be Soloed, Muted and have their effects bypassed.
    *   Built-in side-chain volume ducking. ![description](/sites/default/files/styles/original/public/audio-2.jpg?itok=4JXnYNzJ)
    *   Support for custom high-performance native audio plugins through a new SDK. [![description](/sites/default/files/styles/developer_profile_thumb/public/audio-3.jpg?itok=mMM46QR2)](/sites/default/files/audio-3.jpg)
*   Reverb Zone Mix slider and curve in order to be able to control amount of signal routed to the global reverb associated with Audio Reverb Zones. This allows setting up natural transitions between near field and distant sounds and also allows routing 2D sounds into the reverb.
*   Rewritten Audio asset pipeline and AudioClip backend.
    *   AudioClip settings now support multi-editing.
    *   Per-platform compression setting overrides for AudioClip import, much like texture importing. This includes an API change. Users will now be able to enable override settings per platform and have unity have different compression characteristics for different platforms. ![description](/sites/default/files/styles/original/public/audio-4.jpg?itok=Glia30PC)
    *   Audio transcoding and packing now happens in a separate tool, removing risk of crashing Unity on import.
    *   No double loading of sounds during import processing.
    *   Better handling of huge audio files. If a sound is set to streaming, it is never fully loaded in the editor or player now.
    *   Editor profiling of Audio is now accurate and reflects how it would be in the game.
    *   Streaming (file handle) resources are now freed immediately after playback of sound.
    *   Much improved audio formats in terms of memory and CPU usage. The Format property no longer refers to a specific platform-specific file format, but to a encoding method (Uncompressed, Compressed, ADPCM).
    *   The audio data of an AudioClip can now be loaded on demand by scripts, and loading can happen in the background without blocking the main game thread. Memory management can now be performed much easier of AudioClips in the project.
*   Improved Audio Profiler with better statistics and detailed information. To view it, open the Profiler window, click the Audio pane and press the “Channels”, “Groups” or “Channels and groups” button..

#### Improved Audio Profiler

*   AudioSettings.GetConfiguration / AudioSettings.Reset API as an alternative to the now deprecated AudioSettings.outputSampleRate/AudioSettings.speakerMode property setters and the AudioSettings.SetDSPBufferSize function. The new API allows querying the current configuration and applying all changes at once.
*   Notification callback AudioSettings.OnAudioConfigurationChanged(deviceChanged) callback which can be used to get notifications when sound system reinitialisation happens. This can then be used to adapt audio device settings further or reload volatile AudioClips such as generated PCM clips and restore other audio system state.

### Consoles

*   Unity 5.0 has day one support for XBox 360, XBox One, PS Vita, PS3 and PS4, with Wii-U arriving later in the spring.
*   A custom editor is no longer required for any console. The console extensions are compatible with the general Unity editor!
*   Many developers are already building their games with Unity 5.0 on console having taken part in a Beta release program.

### Editor

*   Unity editor is now 64-bit!
    *   A separate 32-bit installer is available for Windows; on Mac OS X we only ship 64-bit now.
    *   Note that this affects native plugins used in the editor, which now also need to be 64-bit.
*   New AssetBundle build system.
    *   Adds simple UI to mark assets into assetBundles, provides simple API to build assetBundles without having to write complex custom scripts (no need for Push/Pop).
    *   Supports incremental build, which only rebuilds AssetBundles that actually change.
    *   AssetBundle dependencies don't force the rebuild of all the bundles in the dependency chain.
    *   Provides AppendHashToAssetBundleName option to allow to append the hash to the bundle name.
    *   Provides AssetBundleManifest which can be used to get the dependent AssetBundles at runtime.
    *   By default includes type tree in the assetBundle on all the platform except metro.
*   New Project Wizard dialog.
    *   Recent projects list shows "Last Saved With" version number for each project (if available - this information is only saved starting with 5.0).
*   Timeline Profiler:
    *   New view in the CPU Profiler that shows the frame samples laid out on a Timeline. Each thread has its own timeline; This is mostly useful for multi-threaded profiling.

#### Timeline Profiler

*   Version Control: Scene and Prefab Merging
    *   Command line merge tool that understands the scene and prefab formats in order to do semantic merges.
    *   Merge tool integration with Unity's existing version control integration. Can be enabled from EditorSettings.
*   Plugin Inspector: new native plugin importing system. You're no longer required to place platform specific plugins into special folders like Assets/Plugins/iOS, Assets/Plugins/X64, etc. From now on, you can place them anywhere.
    *   You can set platform compatibility settings by clicking on the plugin (files with extensions \*.dll, \*.so, etc, and folders with extension \*.bundle), this include both managed and native files. Plugins can be set for “Any” platform, “Editor only” or a specific platform.
    *   Platform specific settings can also be set, e.g. CPU type. Different platforms may have different settings.

### Graphics

*   Integrated Enlighten real-time global illumination (GI) technology, and improved lightmapping workflow. ![description](/sites/default/files/styles/original/public/graphics-1b.jpg?itok=x2khckJX)
    *   In “Continuous baking” mode scene changes are automatically picked up and tasks are spawned to precompute data for dynamic GI, calculate static lightmaps, light probes, reflection probes etc.
    *   Runtime Dynamic GI for lights:
        *   Changes to lights marked as "Dynamic GI" and skylight changes are picked up automatically.
        *   Emissive surfaces can emit light into GI at runtime. Emissive colors can be changed affect static and dynamic objects in realtime.
        *   Material changes can be triggered via DynamicGI API.
    *   Directional lightmaps can now be baked in a "directional specular" mode (which allows materials to retain their specular look) or in a cheaper "directional" mode (materials get a normal-mapped diffuse look). "Non-directional" mode is the cheapest and results in a flat diffuse appearance. All 3 options are available for both baked and realtime lightmaps. ![description](/sites/default/files/styles/original/public/graphics-2c.jpg?itok=Eh1Xf7pP)
*   New Lighting window
    *   Single place to specify lightmapping, GI and scene render (ambient/reflection/fog) settings.
    *   UI grouped by logical areas.
    *   When real-time lightmaps are disabled and baked lightmaps enabled, indirect lighting of real-time lights is automatically baked into baked lightmaps. If you don't want this behavior, set indirect lighting to 0.
*   HDR workflow improvements:
    *   HDR scene view. When main camera is HDR, then scene view rendering is done in HDR too using the same Tonemapper settings as the main camera.
    *   Support for .hdr and .exr texture formats.
    *   HDR textures (from .exr/.hdr files) are automatically encoded into RGBM format. You can alter this behavior in advanced texture import settings.
    *   Reflection Probes
    *   New "ReflectionProbe" component that captures its surroundings into a cubemap. Cubemap is assigned to Renderers in the proximity from the probe and can be used to produce glossy reflections.
    *   Reflection probes are baked similar to light probes and are stored as cubemap assets. Specular convolution is applied automatically to achieve high-quality glossy reflections.
    *   Reflection probes can also be rendered in realtime, with optional timeslicing across multiple frames.
    *   Added global reflection cubemap in Lighting settings; by default matches the skybox.

#### Reflection Probes

*   Skybox and ambient improvements:
    *   New scenes are now set with directional light, procedural skybox and a reflection probe by default.
    *   Added "Skybox/Procedural" shader that allows setting up simple skies easily.
    *   Built-in Skybox shaders now support HDR (RGBM encoded) textures.
    *   Skybox materials can be assigned by drag-and-drop on the background in the Scene View.
    *   Cubemap textures can be assigned to skybox by drag-and-drop on the background in the Scene View. Material with Skybox/Cubed shader is created automatically.
    *   Improved inspector preview & thumbnails of Skybox materials.
    *   Ambient lighting automatically matches to a skybox. This behavior can be turned off by specifying ambient colors explicitly in Lighting settings.

#### Skybox and ambient improvements

*   New "Deferred Shading" rendering path:
    *   Single pass, multiple-rendertarget G-buffer shading.
    *   Fully supported by the new Standard shader.
    *   Overriding of DeferredShading (and DeferredLighting) shaders is in the UI now, under GraphicsSettings. Possible to even exclude the shaders from game build, in case you don't need them at all.
    *   Surface shaders can generate code for new Deferred Shading rendering path. All 4.x builtin shaders also got support for that.

#### Deferred G-buffer

*   Improved and extended cubemap workflow.
    *   Renamed “Reflection” texture import type to “Cubemap”. Automatic detection of the mapping mode for spherical, cylindrical and 6 image layouts; removed 2 obscure spherical mappings which were rarely used.
    *   Textures imported as cubemaps can use texture compression now!
    *   Added specular and diffuse convolution options to cubemap textures.
    *   Cubemap inspector was improved, can now show alpha channel & mipmaps properly; also understands RGBM encoded HDR cubemaps.
    *   Improved seamless cubemap edge fixup.
    *   Moved old Cubemap menu entry from Assets into Assets | Legacy. Instead to import cubemap textures use “Cubemap” type in texture importer settings.
*   Meshes:
    *   More than two UV coordinates! Up to 4 UVs are imported from model files; and Mesh class gained uv3 & uv4.
    *   Non-uniformly scaled meshes no longer incur any memory cost or performance hit. Instead of being scaled on the CPU they are scaled and lit correctly in shaders.
    *   MeshRenderer has a new additionalVertexStreams property for per-instance mesh data overrides. For example just vertex color for one instance. This is currently used by Enlighten for per-instance UVs.
*   SpeedTree integration: ![description](/sites/default/files/styles/original/public/speedtree.jpg?itok=9w9CXSnf)
    *   SpeedTree models (.SPM files) now can be recognized, imported and rendered by Unity. The workflow is very similar to other mesh formats like FBX.
    *   SpeedTree features like smooth LOD transition, billboards, wind animation and physics colliders are fully supported by specialized SpeedTree shaders.
    *   SpeedTree models are selectable as tree prototypes on terrain.
*   Frame Debugger. See how exactly frame is rendered by stepping through draw calls. See [http://blogs.unity3d.com/2014/07/29/frame-debugger-in-unity-5-0/](http://blogs.unity3d.com/2014/07/29/frame-debugger-in-unity-5-0/)

#### Frame Debugger

*   Added scriptable "Command Buffers" for more extensible rendering pipeline.
    *   Create command buffers ("draw mesh, set render target, ...") from a script, and set them up to be executed from inside camera rendering.
    *   Command buffers can be executed from a bunch of places during rendering, e.g. immediately after deferred G-buffer; or right after skybox; etc. See this blog post: [http://blogs.unity3d.com/2015/02/06/extending-unity-5-rendering-pipeline-command-buffers/](http://blogs.unity3d.com/2015/02/06/extending-unity-5-rendering-pipeline-command-buffers/)

#### Blurred refraction implemented through command buffers

*   Shadows: ![description](/sites/default/files/styles/original/public/graphics-8.jpg?itok=6bjrx6eL)
    *   Much better directional light soft shadows (5x5 PCF filter replaces the old screenspace blur).
    *   Ability to control directional light shadow cascade split ratios in Quality Settings; and added a shadow cascade scene view visualization mode. ![description](/sites/default/files/styles/original/public/graphics-9.jpg?itok=xMurprUF)
    *   Replaced "cast shadows" checkbox in Renderer component with a popup. Additional modes: Two Sided - casts two-sided shadows even from single-sided geometry; Shadows Only - cast shadows, but make the object invisible otherwise.
    *   In Forward rendering, directional light shadows are computed from camera's depth texture instead of a separate "shadow collector" rendering pass. Saves a bunch of draw calls, especially when depth texture is needed for image effects anyway.
        *   This means that ShadowCollector shader passes aren't used for anything; you can just remove them if you had any.
        *   Camera’s DepthTexture is not generated using shader replacement anymore. Now it is generated using same shaders as used for shadowmap rendering (ShadowCaster pass types). Camera-DepthTexture.shader is not used for anything now.
        *   Normal-offset shadows to help reduce self-shadowing artifacts (“normal bias” setting on Light). Manually written shaders should use TRANSFER\_SHADOW\_CASTER\_NORMALOFFSET in the vertex shader, which is similar to the old TRANSFER\_SHADOW\_CASTER but it requires v.normal to be present.
        *   Most platforms now internally use floating point (RFloat) format for point light shadows, instead of custom encoded ARGB32 format. Saves shader instructions and has better precision.
*   Particles: Added a Circle emitter (with an option to specify an arc) and one-way Edge emitter.
*   LOD Group was improved. A "fade mode" can be set on each level and a value of "how current LOD be blended/faded to the next LOD" will be passed to shader in unity\_LODFade.x.

### iOS

*   Support deep plugin folder structure.
*   Support for XIB launch screens.
*   Xcode manipulation API for editor scripts, and rewritten Xcode project generator.
*   iOS 64-bit support via IL2CPP scripting backend. You can switch to it in Player Settings.
*   Metal graphics API support. Picked automatically on eligible devices. Can be controlled in Player Settings.

### Linux & SteamOS

*   Gamepad configuration via Steam Big Picture mode (See upgrade guide).
*   Gamepad hot plugging.
*   Includes default configurations for several common gamepads.

### Physics

*   PhysX 3 integration!
    *   Better performance on multi-core processors, and especially on mobile. See [http://physxinfo.com/news/11297/the-evolution-of-physx-sdk-performance-wise/](http://physxinfo.com/news/11297/the-evolution-of-physx-sdk-performance-wise/)
    *   Moving static colliders does not cause performance penalty anymore.
    *   Better simulation quality, e.g. stacking stability.
    *   Cleaner codebase, which does not contain some of the long standing issues.
    *   See [http://blogs.unity3d.com/2014/07/08/high-performance-physics-in-unity-5/](http://blogs.unity3d.com/2014/07/08/high-performance-physics-in-unity-5/)
*   2D physics:
    *   Added ConstantForce2D, PointEffector2D, AreaEffector2D, PlatformEffector2D and SurfaceEffector2D components. ![description](/sites/default/files/styles/original/public/physics-1.jpg?itok=l6QbO1GP)
    *   Added Physics2D.IsTouching, IsTouchingLayer and Collider2D.IsTouching, IsTouchingLayer methods.
    *   All 2D colliders now have a 2D ‘offset’ property that replaces the ‘center’ property on BoxCollider2D and CircleCollider2D. ![description](/sites/default/files/styles/original/public/physics-2.jpg?itok=FueX1j-8)
*   Added Rigidbody.maxDepenetrationVelocity to make possible to tune the velocity of the colliding rigidbodies when they are pushing each other away.
*   Added TerrainData.thickness to control the thickness of TerrainColliders.
*   Add Cloth.ClearTransformMotion method to allow teleportation of cloth instances.
*   Exposed WheelCollider.sprungMass to C# as a read-only property. Sprung mass can have a wide range of applications like being able to configure suspension springs using natural frequency & damping ratio or having custom forces added to suspension based on the weight supported by particular wheels.

### Scripting

*   Auto-update obsolete Unity API usage in scripts & assemblies. Majority of API upgrades are done automatically, see this post for details: [http://blogs.unity3d.com/2014/06/23/unity5-api-changes-automatic-script-updating/](http://blogs.unity3d.com/2014/06/23/unity5-api-changes-automatic-script-updating/)

### Shaders

*   New built-in "Standard" shader. ![description](/sites/default/files/styles/original/public/shaders-1.jpg?itok=Opt13CS-)
    *   Physically based shader, suitable for most everyday surfaces (metals, plastics, wood, stone etc.).
    *   Comes in both “metallic workflow” and “specular workflow” variants.
    *   Introduce detail normalmaps and ambient occlusion support.
    *   Support two modes of alpha blending - physically plausible “Transparent” mode (suitable for glass, ice, etc) and “Fade” mode which allows to shade fading out objects and decals.
    *   Features driven by what you enable in the inspector (e.g. when no normal map assigned, the shader will internally use a faster variant without a normal map).
    *   Approximate and optimized path for mobile & shader model 2.0.
    *   This is a default shader for newly created objects now. Most of Unity 4.x shaders were moved to “Legacy” shader popup menu.
    *   Surface shaders can also use the same physically based BRDF (Standard and StandardSpecular lighting functions).
*   Build-time stripping of unused shader features, and shader variant compilation improvements.
    *   Added #pragma shader\_feature; similar to multi\_compile but unused ones are removed from the game builds. If no materials use a particular shader feature variant, shader code for it is not included into game data.
    *   #pragma shader\_feature can be provided just one parameter, e.g. #pragma shader\_feature FANCY\_ON. This expands to two shader variants (without and with the parameter defined).
    *   Can specify vertex- or fragment-only shader variants. For example, #pragma shader\_feature\_vertex A B C will add 3x more shader variants, but to the vertex shader only.
    *   Underscore-only names in shader\_feature and multi\_compile are treated as "dummy" and don't consume shader keyword names. Useful for defining default shader behavior.
    *   Shader variants for unused lightmap modes aren’t included into build. E.g. if you don't use directional lightmaps in any of your scenes, then shader variants that handle directional lightmaps will be removed from game build data. No need to manually add "nolightmap" and friends to shader code now.
*   Single CGPROGRAM block can target multiple "shader models" at once. For example, you can base it for SM2.0, but have fancier multi\_compile variants that require SM3.0. Syntax:
    *   #pragma target 3.0 // base is SM3.0
    *   #pragma target 4.0 FOO BAR // FOO or BAR require SM4.0
*   Custom Shader GUI can now be defined by implementing the IShaderGUI interface instead of deriving from MaterialEditor. Using this approach makes the custom shader GUI show within the inspector for Substance materials.

### Standard Assets

*   A new suite of Standard Assets including cameras, first and third person controllers, car controller, aeroplane controller and sample particle systems.
*   A cross platform input helper.
*   New mobile control prefabs based on the new UI system.
*   Image effects have been converted to C#.
*   New sample project based on the Standard assets shows how to best utilize them.

### Unity Download Assistant

*   As part of optimizing download, we're shipping Unity 5 as multiple installers. The Download Assistant lets the user select which components to download and install.
*   The individual installers can be downloaded separately and installed silently, as described in the documentation.

### WebGL

*   WebGL support: a new target in the build player window!
*   Currently marked as “Preview” state; official support for latest Firefox & Chrome.
*   Uses the same il2cpp scripting backend as 64-bit iOS.
*   See blog post: [http://blogs.unity3d.com/2014/04/29/on-the-future-of-web-publishing-in-unity/](http://blogs.unity3d.com/2014/04/29/on-the-future-of-web-publishing-in-unity/)