# Unity 5.0

https://unity3d.com/unity/whats-new/unity-5.0

## Improvements

- [2D](#2d)
- [AI](#ai)
- [Android](#android)
- [Animation](#animation)
- [Asset Import](#asset-import)
- [Asset Management](#asset-management)
- [Audio](#audio)
- [Blackberry](#blackberry)
- [Documentation](#documentation)
- [Editor](#editor)
- [Fonts](#fonts)
- [Graphics](#graphics)
- [iOS](#ios)
- [Linux](#linux)
- [Networking](#networking)
- [Performance](#performance)
- [Physics](#physics)
- [Players](#players)
- [Plugins](#plugins)
- [Profiler](#profiler)
- [Scripting](#scripting)
- [Shaders](#shaders)
- [Substance](#substance)
- [Terrain](#terrain)
- [Version Control](#version-control)
- [Windows](#windows)
- [Windows Store Apps](#windows-store-apps)


### 2D

*   Added Sprite.pivot getter.
*   Sprite geometry can now be overridden using Sprite.OverrideGeometry(Vector2\[\] vertices, UInt16\[\] triangles).
*   SpritePacker: Atlas texture name will now also contain the atlas name.
*   The new AssetPostprocessor.OnPostprocessSprites(Texture2D texture, Sprite\[\] sprites) is called immediately after OnPostprocessTexture when sprites are generated.

### AI

*   Carving navmesh supports carving the detailed tessellation. Fixes height discontinuities when an undulating region is carved
*   Expose pathfinding iteration limit, and avoidance prediction time to script API
*   In Editor the "Show Avoidance" option for NavMeshAgent will show the sampled velocities for avoidance calculation
*   New icons for navmesh asset and components
*   Warn if agent and obstacle components are placed on the same GameObject
*   Warn if navmesh slope bake setting is unreasonable.

### Android

*   "Android TV Compatibility" checkbox which enables Android TV compatibility checks at build time.
*   Hardware upscaling for Screen.SetResolution().
*   isGame setting for Android TV and Android 5.0 devices
*   JDK detection. Build fails if only JRE is present.
*   Made VRAM estimation somewhat more correct.
*   PlayFullScreenMovie now supports FullScreenMovieScalingMode.AspectFill.
*   Public Java API for attaching custom rendering surfaces.
*   Reconfiguring antialiasing or changing display framebuffer properties should no longer result in a GL context loss.
*   Reduced system memory usage.
*   Support for Android TV banners.
*   Support for MouseDrag event.
*   VSync improvements: using Choreographer on JellyBean+ to get more stable time; and using VSync time when available to hit stable 30FPS when "Every other vblank" is on.
*   WWW responseHeaders now contain STATUS key.

### Animation

*   Added AnimationEvent.animatorInfo and AnimationEvent.animationInfo for Event fired by Animator.
*   Added "Edit" button for imported AnimationClip that selects the ModelImporter with proper clip ![description](/sites/default/files/styles/original/public/animation-10.jpg?itok=DXIma7A1)
*   Added helpbox on StateMachine Transitions
*   Added reset functions to Animator State and Animator Transition
*   Added RuntimeAnimatorController.animationClips property. It returns all the clips in the controller
*   Added tooltips to animation transition settings + added foldout group for settings.
*   Always display numeric values for Transition's duration, offset and exitTime.
*   Better error message on default Blendtree parameters
*   Can now drag and drop FBX files directly in the StateMachine Graph
*   Can now drag AnimatorController directly on GameObject, it will created an Animator component if needed.
*   Clicking on the blend tree background will select the top blend node
*   Copy/paste/duplicate keyboard shortcuts work.
*   Display Animator stats in inspector: Clip count, curve count, etc. ![description](/sites/default/files/styles/original/public/animation-11.jpg?itok=7_-ycJdI)
*   Don't show contextual menu when adding transition to empty StateMachine
*   Double clicking on a State with an imported AnimationClip now shows the Animation Import Settings in the Inspector
*   HelpBox in inspector when root node position/rotation is controller by curves
*   Improved computation of Pivot weight
*   Improved humanoid retargeting. The differences between Generic and Humanoid animation are now less than 0.001 normalized meter and 0.1 degrees on end points.
*   Improved performance when ModelImporter has many AnimationClips
*   In the AnimationClip importer, proper support for 0 duration clips
*   ModelImporter remembers foldout state
*   Ordered Interruption UI is disabled when in Next State
*   Persisted the Settings foldout through a static variable.
*   Runtime access to Animator's parameters (Animator.parameters property).
*   States can now be renamed on synchronized layers
*   Support the case that both SkinnedMeshRenderer and Animator are on the same GameObject (optimised mode).
*   Transition Solo and Mute are now undoable.
*   Trigger parameters now have different UI to distinguish them from Bool parameters.

### Asset Import

*   Added AssetPostProcessor.OnPreProcessAnimation, this new callback is called just before animation clips are created.
*   Added ModelImporter.defaultClipAnimations (list of ModelImportClipAnimation based on TakeInfo) and ModelImporter.importedTakeInfos (list of TakeInfo from the file).
*   Support large bitmaps importing (>4Gb in size)
*   Update PVRTC texture compressor.
*   Updated FBX SDK to 2015.1: better performance; fixes various rare crashes and issues when importing some Collada, OBJ, 3DS files; fixed reversed normals in some DXF files.

### Asset Management

*   Allow to access files with long path (more than 260 characters) on Windows.

### Audio

*   Added more descriptive error message when FMOD fails to initialise on Windows because of sound card drivers configured to give applications exclusive mode access.
*   AudioSources now take up fewer resources. Previously this caused problems when importing projects with a large number of AudioSource contained in prefabs.
*   Improved audio importer interface to be make options more clear
*   Increased default virtual voice count from 100 to 512 and made it user-configurable through project settings.
*   Removed 3D property in AudioClip and moved all 3D audio functionality to the AudioSource.
    *   Renamed AudioSource.panLevel to AudioSource.spatialBlend. This property now controls the 2D / 3D mode of sound playback through this AudioSource. There is no longer a mode toggle, but a continuous interpolation between the two states.
    *   Renamed AudioSource.pan to AudioSound.panStereo. This is to remove confusion about the nature of this property. AudioSource.panStereo pans the audio signal into the left or right speakers. This happens before spatial panning is applied and can be applied in conjunction with 3D panning.

### Blackberry

*   Added "Add Attached Device" to the debug token creation window.
*   Application.systemLanguage now differentiates between Chinese Simplified and Chinese Traditional appropriately.
*   Registration now uses BlackBerry's 10.2 registration system. Currently registered systems do not need to re-register.

### Documentation

*   Default language for code snippets in the Scripting Reference is C#, with many more examples in C# available, with Javascript as a secondary language, and Boo removed.
*   Localized documentation available in Russian, Spanish and Japanese (currently based on 4.6 docs and over time 5.0).
*   Improved handling of namespaces, generics and interfaces.
*   API history improved with information about obsolete members.

### Editor

*   Added 8192 maximum texture size option in import settings.
*   Added deferred diffuse/specular/smoothness/normals scene view rendering modes.
*   Added GetCurrentGroupName() and SetCurrentGroupName() to allow overriding the automatic undo name generation
*   Added Gizmos.DrawMesh and DrawWireMesh (the meshes drawn are pickable too).
*   Added support for importing textures from PVRv3, ASTC, KTX file formats.
*   Added virtual function ScriptableWizard.DrawWizardGUI for customizing GUI of derived wizard classes.
*   Added warning on exiting play mode when objects have been spawned into the scene from OnDestroy().
*   Asset Store: The asset store window is now much faster, more responsive, and looks better.
*   Camera inspector shows camera's depth texture mode. Also, scene view camera makes sure to match main camera's depthTextureMode.
*   Drag-and-drop assigns material to a specific part of the mesh now. Holding Alt key will assign material to all the parts of the mesh.
*   EditorStyles.helpBox is now exposed
*   Ensure controls are not rendered with focus state if the EditorWindow they are in does not have focus.
*   Expose RenderTexture color format in the inspector, just like with depth format.
*   Exposed AssetPreview.SetPreviewTextureCacheSize ().
*   Finished builds will be shown in OS X notification center when Editor in the background.
*   Frame Selected (F key over scene view) now takes point/spot light range into account.
*   Improved build times for textures and AudioClips
*   Improved searching for class names in different namespaces and across different user assemblies.
*   Improved UI display names in Player Settings
*   License: Activate from command-line.
*   License: Added -returnlicense command line option, which returns the currently active license and quits the editor.
*   License: A progress bar will be shown during returning or releasing a license.
*   LightmapParameters now has an icon
*   LightmapSnapshot now has an icon
*   MaterialEditor improvements
    *   Show a foldout arrow for Material inspectors inlined on gameobjects to make it clear that they can be expanded/collapsed.
    *   Added TexturePropertyMiniThumbnail(): Draw a property field for a texture shader property that only takes up a single line height. The thumbnail is shown to the left of the label. Clicking the thumbnail will show a large preview info window.
    *   Added GetTexturePropertyCustomArea():. Returns the free rect below the label and before the large thumb object field. Is used for e.g. tiling and offset properties.
    *   Added TextureScaleOffsetProperty(): Draws tiling and offset properties for a texture.
    *   Texture scaling and offset values can now be dragged.
*   Optimization of Hierarchy Window
*   Prevent tooltips from showing while dragging.
*   Tag editor facelift by removing the empty tag and using Reorderable list to draw tags and layers.
*   When browsing for a location to create or open a project, the dialog starts at the location where a project was last created or opened.
*   When saving scenes, overwrite existing scene file only after successful save.
*   Windows Editor: Native child windows have their title set to the GUIView/EditorWindow class name.
*   Unity will output a proper error regarding incompatible CPU architectures on Mac OS X when failing to load native libraries. For ex., You cannot load 32 bit native libraries on 64 bit Editor.

### Fonts

*   Added easier APIs to access OS Fonts (Font.GetOSInstalledFontNames and Font.CreateDynamicFontFromOSFont).
*   Added new APIs to get font metrics if you want to implement your own font rendering: Font.ascent, Font.lineheight, new fields in CharacterInfo (old fields in CharacterInfo are deprecated).
*   Optimized texture rebuilds to happen less often.

### Graphics

*   Added "#pragma exclude\_renderers nomrt" for platforms not supporting multiple render targets (MRTs).
*   Added Camera.onPreCull, onPreRender, onPostRender delegates.
*   Added RenderTextureFormat.ARGB2101010 and Shadowmap formats.
*   Added Shader.IsKeywordEnabled API.
*   Added SystemInfo.graphicsMultiThreaded API.
*   Added Texture2D.SetPixels32 overload that accepts offset and dimensions.
*   All baked and realtime lightmapping computations are now done in linear space, this makes lighting between gamma & linear space look much closer. When using pure lightmaps, it should in fact look very similar.
*   Allow SkinnedMeshRenderer to accept non-skinned meshes.
*   DDS importer can import Float, Half and 11.11.10 format .dds textures now.
*   Dynamic batching can batch non-uniform scaled objects together when normals/tangents are unused. Helps with shadow caster batching, and unlit shaders.
*   Image Effects: Added Threshold tweak to SunShafts, removed legacy "alpha as mask".
*   Image Effects: GlobalFog image post-processing effect was rewritten. Now it has "distance fog" (matches what is set in lighting settings), and optional "height fog" (linearly increasing fog density below specified height).
*   Increased maximum number of simultaneous render targets (MRT) to 8 on capable platforms.
*   Light intensity now behaves consistently between linear and gamma space rendering mode. Lights in linear mode can now have much higher intensity. The light intensity is now defined to be in gamma space, hence in linear rendering it is converted to linear space when passed to the shader. (In linear space the maximum effective light intensity is now 97 while previously it was 8).
*   Lightmaps & baked probes compressed with RGBM now have an effective range of 5 in gamma space or 32 in linear space. This reduces RGBM compression artifacts for lightmaps. Emissive surfaces for enlighten are encoded with a range of 8 in gamma space and 97 in linear space.
*   Meshes: Mesh compression will now also do lossy compression of vertex colors.
*   Meshes: Added "keep quads" mesh import option; useful for DX11/Console tessellation shaders.
*   Optimized per-object light culling in forward rendering by using multiple CPU cores better.
*   Overhauled stats window to be more compact and profiler rendering stats to be more comprehensive.
*   Reduced memory consumption when loading textures on mobile devices.
*   Rendering code optimized to reduce amount of material SetPass calls. Light probes and lightmap UV transform state changes are now internally applied via MaterialPropertyBlocks without requiring a full SetPass. This reduces cost on the main thread to send commands to the render thread, and on the the render thread the driver overhead is reduced.
*   Scene View: Can drag a cubemap onto empty space in the scene view to assign it as a skybox.
*   Skinned meshes use less memory by sharing index buffers between instances.
*   Support for more shader keywords (128, up from 64).

### iOS

*   Added debug labels for OpenGL objects, useful in Xcode frame capture debugging.
*   Allow to set compile flags for already existing files in Xcode API
*   Better support for Unity view size changes from native side.
*   Enabled basic background processing.
*   Expose font directories to the trampoline
*   Game controller button pressure is now also exposed as axis (float) value.
*   Implement a way to select iOS framework dependencies for native plugins.
*   Improved performance of adding large number of files to Xcode project
*   Optimized Texture2D.LoadImage performance for PNG and JPG files.
*   Tweaked external RenderSurface API to make a bit more sense and be more concise.

### Linux

*   Added Input.IsJoystickPreconfigured for querying 5.0 Linux gamepad detection.
*   Monitor selection
*   Set popupwindow mode via Motif borderless hint when supported
*   Support XDG-compliant path overrides.

### Networking

*   WWW: Populate .bytes and .text on non-200 response.

### Performance

*   Improved multithreaded job system:
    *   Culling & shadow caster culling is multithreaded now.
    *   Internally multithreaded parts (culling, skinning, mecanim, ...) are more efficient now via some lockless magic.
    *   Temporary memory allocations done by some jobs are more efficient now.
*   Improved loading performance. More work has been offloaded to the loading thread, reducing the overhead of asynchronous loading on the main thread.
*   Object.Instantiate performance has been improved.
*   Mecanim optimizations:
    *   Optimized Animator Enable(), 2x speed on complex controllers.
    *   Optimized Animator memory usage per instance, 2x smaller on complex controllers.
    *   Improved performance for Animator Tool.
*   Optimized memory usage and runtime performance when serializing objects with backward compatibility (type-tree) enabled.
*   Optimized texture importing performance.
*   Static batching performance is improved in many cases.
*   Updated occlusion culling (Umbra) version; contains improvements for mobile Umbra culling performance, and improves occlusion culling robustness in some cases.

### Physics

*   Adaptive force is now optional (disabled by default).
*   Changed default cloth coefficient values, and added info boxes to cloth editor
*   Cloth constraint editing UI has been replaced by a more intuitive UI inside the Scene View.
*   Cloth; exposed sleep force parameter to tune minimum force after which cloth will start sleeping.
*   Cloth; exposed tethers flag to improve cloth simulation quality.
*   Cloth inspector is now much faster and capable of dealing with meshes of any vertex count
*   Exposed a function ConfigureVehicleSubsteps in WheelCollider to make it possible for developers to customise vehicle sub-stepping. This helps setting up heavy vehicles, that require different amount of sub-steps to simulate wheels correctly.
*   Make scaling mesh colliders cheaper, by not creating a new mesh with scaling applied to it with every scale change.
*   Redesigned WheelCollider gizmo to show more relevant information.
*   Removed internal lock in PhysXRaycast, particles should now be able to process raycasts in multithreaded mode.
*   Show inconsistent hinge joint constraints in inspector
*   Updated default values for WheelCollider as the old ones did not make any sense with new PhysX.

### Players

*   Add -show-screen-selector command line option for Linux and Windows.
*   Cursor management cleanup
    *   Screen.lockCursor has become Cursor.lockState
    *   Screen.showCursor has become Cursor.visible
    *   Added ConfineCursor state to confine cursor to game window (Linux/Windows)
    *   Cursor lock state and cursor visibility state are now mutually independent.

### Plugins

*   Unity will now verify that plugins don’t collide with each other before building to player. Previous behavior was that you would need to wait until all the scenes were built, and you would only then see that plugin with same filename is trying to overwrite another plugin.
*   (Windows Store Apps/Windows Phone): when picking placeholder plugins only plugins with matching file names as the original plugin will be shown

### Profiler

*   Added total and per frame GC allocated bytes to the Memory chart.
*   Image Effects have profiling blocks with the script name in them, instead of a generic "ImageEffect".
*   Improved accuracy of reported AudioSources in the scene when working with AudioSources in prefabs.
*   Search field for filtering the results in the treeview.
*   Stop collecting GPU data when GPU Profiler chart is closed. Defaults to being closed for performance reasons.
*   Stop collecting profiler's data on Player's side if recording is disabled.

### Scripting

*   64-bit platforms will now accept managed DLLs compiled specifically for x64.
*   Added defines for UNITY\_EDITOR\_64/32, UNITY\_5.
*   Added disposable scope helpers for Begin/End pairs for GUI, GUILayout, EditorGUI and EditorGUILayout.
*   Added formatting overloads to Debug.Log\*.
*   Added generic overloads for AssetBundle.Load\*.
*   All GetComponent paths got much faster, especially GetComponent.
*   GetComponent family of functions now supports interfaces as generic argument.
*   Improve error messages reported by IL2CPP by including managed source code information when it is available.
*   Math: Added SphericalHarmonicsL2 scripting struct.
*   Support serialization of all primitive types.

### Shaders

*   Added \[NoTilingOffset\] property attribute; hides tiling & offset fields in texture property UI.
*   Added \[Gamma\] property attribute; allows Float and Vector properties to be flagged for automatic gamma correction. Tagged Float and Vector properties will function the same way as Color properties do - gamma correction will be applied, if necessary, before sending values to the GPU.
*   Added atmospheric thickness and sky tint controls to Skybox (procedural) shader; also visual appearance in gamma space matches that of linear now.
*   Added exposure slider to "Skybox/Cubemap" and "Skybox/6 Planes" shaders.
*   Added MaterialPropertyDecorators. Similar to MaterialPropertyDrawers, but you can add many of them on a shader property. Added built-in decorators: \[Space\], \[Header(text)\].
*   Added rotation and exposure controls to Skybox (6-sided) and Skybox (cubemap) shaders.
*   Added SHADER\_TARGET define that's based on "#pragma target" version. E.g. it will be 30 for SM3.0.
*   Added UNITY\_NO\_LINEAR\_COLORSPACE define; defined on platforms that never have Linear color space.
*   Better comments in generated surface shader code. Better error messages when surface shader lighting functions aren't consistent.
*   Better handling of texture\*Lod for OpenGL ES 2.0. On devices that don't support it, the generated shader code will automatically do a biased mip lookup approximation.
*   Built-in Fog works on all platforms now (includes WP8/WinRT/consoles).
*   Cleaned up shadow macros for shaders (UNITY\_DECLARE\_SHADOWMAP, UNITY\_SAMPLE\_SHADOW). On platforms that always have "native shadow maps" (e.g. DX11), there's no need for SHADOWS\_NATIVE keyword to be present for these macros to do the right thing. On platforms that don't have native shadow maps (e.g. some GLES2.0 devices, Xbox360), these macros will do comparison of texture & depth manually.
*   Existing user surface shaders with custom lighting functions work with Non-Directional (baked and realtime) and Directional (baked) lightmap types. These lighting functions need to be updated to use the UnityGI structure to take advantage of all the new lightmap types and reflection probes.
*   Improved "compile and show code" functionality in shader inspector. Now has dropdown to select custom set of platforms to compile shaders for. And shows a progress bar while compiling shader variants for display.
*   Improved importing performance, in-editor loading performance and reduced imported file sizes for shaders with really large variant counts.
*   Information about texture format decoding (LDR, dLDR, RGBM, Normals) is passed in %TextureName%\_HDR shader constant.
*   Made it possible to use stencil buffer during deferred shading/lighting g-buffer passes, to some extent. Stencil reference value coming from shader/material will be combined (binary or) with Unity-supplied reference value.
*   Massively improved shader loading performance, and reduced memory consumption.
    *   By default, internal shader variants are only loaded when actually needed (typically a lot of shader variants are never actually needed).
    *   Added ShaderVariantCollection asset type for ability to manually preload/warmup shader variants, to avoid hiccups later on. This is like Shader.WarmupAllShaders, done in a better way.
    *   Editor can track shaders & their variants used in scene or play mode, and create ShaderVariantCollection out of them (button in Graphics Settings).
    *   Graphics Settings have a list of ShaderVariantCollection assets to preload at game startup. Can also warmup them from a script.
*   Optimized shader compilation performance for OpenGL/ES platforms
*   Optimized shader importing performance, particularly for surface shaders with many multi\_compile/shader\_feature variants.
*   Shaders no longer apply a 2x multiply of light intensity. Instead lights are automatically upgraded to be twice as bright. This creates more consistency and simplicity in light rigs. For example a directional light shining on a white diffuse surface will get the exact color of the light.
    *   The upgrade does not affect animation, thus if you have an animated light intensity value you must change your animation curves or script code and make them 2x as large to get the same look.
    *   You might have to adjust your shaders to remove a 2x multiply. This is only the case if you define your own lighting function, in the case of surface shaders this is usually not the case. So most content will not require the change. In most cases the shader code looks like this:
        *   c.rgb = s.Albedo \* \_LightColor0.rgb \* (diff \* atten \* 2); --> c.rgb = s.Albedo \* \_LightColor0.rgb \* (diff \* atten);
*   Skybox shaders (including "Skybox/Procedural") get direction and color of the main light passed in the shader constants.
*   Surface shaders allow more texture interpolators, when targeting shader model 4.0+ (up to 32).
*   Surface shaders can use the UnityGI structure in their lighting functions. UnityGI contains light from all lightmap types, light probes and reflection probes. The built-in Lambert and BlinnPhong were updated to use it as well.
*   Surface shaders use up slightly less samplers on DX11-like platforms. Added UNITY\_SAMPLE\_TEX2D\_SAMPLER helper macro to read a texture, while using sampler from another one.
*   Surface shaders using UnityGI and alpha transparency default to alpha premultiply mode (alpha:premul). Otherwise the default is alpha:blend.

### Substance

*   Consolidation of Substance binary data prior to runtime use now has a much lower peak memory footprint.

### Terrain

*   Added API GetTreeInstance()/SetTreeInstance()/treeInstanceCount on TerrainData class for fast tree updating.
*   Added "Keep existing trees" option when mass-placing trees.
*   Improved rendering performance when tree imposters are requested to be rendered.
*   New terrain materials. You now have 4 options to choose from:
    *   Built-in Standard. PBR material that uses the “standard” lighting model. This is the default option for newly created terrains.
    *   Built-in Legacy Diffuse. This is the legacy built-in terrain material from Unity 4.x and before. It uses Lambert (diffuse term only) lighting model and has optional normal map support.
    *   Built-in Legacy Specular. This built-in material uses BlinnPhong (diffuse and specular term) lighting model and has optional normal map support.
    *   Custom. Use a custom material of your choice to render the terrain.

### Version Control

*   Add shortcut for submit and cancel in submit dialog. Default keyboard focus to textarea when opening submit window.
*   Merging: Improve conflict output to console
*   Merging: Improve premerge by rewriting all of left, right and base.

### Windows

*   Standalone and webplayer: Input subsystem processes touch messages via WM\_TOUCH. Previously it worked with Windows-simulated mouse events.
*   Windows Phone 8/Windows Store Apps
*   Added GetMethod() and GetProperty() to WinRTLegacy.TypeExtensions.
*   Added System.IO.Directory, System.IO.File, System.IO.FileStream, WinRTLegacy.IO.StreamReader, WinRTLegacy.IO.StreamWriter classes to WinRTLegacy
*   Shadows on windows mobile devices now work just like on iOS/Android - no cascaded shadow maps (i.e. not "too slow on mobile" anymore).
*   Significantly improved performance of passing System.Type objects to UnityEngine (for example, GetComponent is affected)
*   UnityPlayer.dll now contains version info.
*   Windows Phone 8: Geolocator initialization code removed from Visual Studio project files. When overwriting existing 4.x projects please remove redundant code.

### Windows Store Apps

*   Added Directory, DirectoryInfo, File, FileStream replacements to WinRTLegacy.
*   Added support for linear color space.
*   Added OnFileActivated handler in App.xaml.\[cs/cpp\].
*   Added UnityEngine.WSA.Application.advertisingIdentifier.
*   Building on top of existing project will now check if a project being overwritten is compatible with newly built one.
*   Chinese Traditional and Simplified languages are now detected and reported, instead of always returning generic Chinese.
*   Handheld class added.
*   PlayerPrefs will be saved whenever application goes into suspend mode.
*   Use joysticks in addition to Xbox 360 controllers, but you have to enable HumanInterfaceDevice capability in PlayerSettings. Note: this capability is not visible in Package.appxmanifest UI interface in Visual Studio.