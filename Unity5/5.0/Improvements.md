# Unity 5.0
https://unity3d.com/unity/whats-new/unity-5.0

## Improvements


### 2D
<ul>
<li>Added Sprite.pivot getter.</li>
<li>Sprite geometry can now be overridden using Sprite.OverrideGeometry(Vector2[] vertices, UInt16[] triangles). </li>
<li>SpritePacker: Atlas texture name will now also contain the atlas name.</li>
<li>The new AssetPostprocessor.OnPostprocessSprites(Texture2D texture, Sprite[] sprites) is called immediately after OnPostprocessTexture when sprites are generated.</li>
</ul>

### AI
<ul>
<li>Carving navmesh supports carving the detailed tessellation. Fixes height discontinuities when an undulating region is carved</li>
<li>Expose pathfinding iteration limit, and avoidance prediction time to script API</li>
<li>In Editor the "Show Avoidance" option for NavMeshAgent will show the sampled velocities for avoidance calculation</li>
<li>New icons for navmesh asset and components</li>
<li>Warn if agent and obstacle components are placed on the same GameObject</li>
<li>Warn if navmesh slope bake setting is unreasonable.</li>
</ul>

### Android
<ul>
<li>"Android TV Compatibility" checkbox which enables Android TV compatibility checks at build time.</li>
<li>Hardware upscaling for Screen.SetResolution().</li>
<li>isGame setting for Android TV and Android 5.0 devices</li>
<li>JDK detection. Build fails if only JRE is present.</li>
<li>Made VRAM estimation somewhat more correct.</li>
<li>PlayFullScreenMovie now supports FullScreenMovieScalingMode.AspectFill.</li>
<li>Public Java API for attaching custom rendering surfaces.</li>
<li>Reconfiguring antialiasing or changing display framebuffer properties should no longer result in a GL context loss.</li>
<li>Reduced system memory usage.</li>
<li>Support for Android TV banners.</li>
<li>Support for MouseDrag event.</li>
<li>VSync improvements: using Choreographer on JellyBean+ to get more stable time; and using VSync time when available to hit stable 30FPS when "Every other vblank" is on.</li>
<li>WWW responseHeaders now contain STATUS key.</li>
</ul>

### Animation
<ul>
<li>Added AnimationEvent.animatorInfo and AnimationEvent.animationInfo for Event fired by Animator.</li>
<li>Added "Edit" button for imported AnimationClip that selects the ModelImporter with proper clip <img class="ii-original" src="/sites/default/files/styles/original/public/animation-10.jpg?itok=DXIma7A1" alt="description"></li>
<li>Added helpbox on StateMachine Transitions</li>
<li>Added reset functions to Animator State and Animator Transition</li>
<li>Added RuntimeAnimatorController.animationClips property. It returns all the clips in the controller</li>
<li>Added tooltips to animation transition settings + added foldout group for settings.</li>
<li>Always display numeric values for Transition's duration, offset and exitTime.</li>
<li>Better error message on default Blendtree parameters</li>
<li>Can now drag and drop FBX files directly in the StateMachine Graph</li>
<li>Can now drag AnimatorController directly on GameObject, it will created an Animator component if needed.</li>
<li>Clicking on the blend tree background will select the top blend node</li>
<li>Copy/paste/duplicate keyboard shortcuts work.</li>
<li>Display Animator stats in inspector: Clip count, curve count, etc. <img class="ii-original" src="/sites/default/files/styles/original/public/animation-11.jpg?itok=7_-ycJdI" alt="description"></li>
<li>Don't show contextual menu when adding transition to empty StateMachine</li>
<li>Double clicking on a State with an imported AnimationClip now shows the Animation Import Settings in the Inspector</li>
<li>HelpBox in inspector when root node position/rotation is controller by curves</li>
<li>Improved computation of Pivot weight</li>
<li>Improved humanoid retargeting. The differences between Generic and Humanoid animation are now less than 0.001 normalized meter and 0.1 degrees on end points.</li>
<li>Improved performance when ModelImporter has many AnimationClips</li>
<li>In the AnimationClip importer, proper support for 0 duration clips</li>
<li>ModelImporter remembers foldout state</li>
<li>Ordered Interruption UI is disabled when in Next State</li>
<li>Persisted the Settings foldout through a static variable.</li>
<li>Runtime access to Animator's parameters (Animator.parameters property).</li>
<li>States can now be renamed on synchronized layers</li>
<li>Support the case that both SkinnedMeshRenderer and Animator are on the same GameObject (optimised mode).</li>
<li>Transition Solo and Mute are now undoable.</li>
<li>Trigger parameters now have different UI to distinguish them from Bool parameters.</li>
</ul>

### Asset Import
<ul>
<li>Added AssetPostProcessor.OnPreProcessAnimation, this new callback is called just before animation clips are created.</li>
<li>Added ModelImporter.defaultClipAnimations (list of ModelImportClipAnimation based on TakeInfo) and ModelImporter.importedTakeInfos (list of TakeInfo from the file).</li>
<li>Support large bitmaps importing (&gt;4Gb in size)</li>
<li>Update PVRTC texture compressor.</li>
<li>Updated FBX SDK to 2015.1: better performance; fixes various rare crashes and issues when importing some Collada, OBJ, 3DS files; fixed reversed normals in some DXF files.</li>
</ul>

### Asset Management
<ul>
<li>Allow to access files with long path (more than 260 characters) on Windows.</li>
</ul>

### Audio
<ul>
<li>Added more descriptive error message when FMOD fails to initialise on Windows because of sound card drivers configured to give applications exclusive mode access.</li>
<li>AudioSources now take up fewer resources. Previously this caused problems when importing projects with a large number of AudioSource contained in prefabs.</li>
<li>Improved audio importer interface to be make options more clear</li>
<li>Increased default virtual voice count from 100 to 512 and made it user-configurable through project settings.</li>
<li>Removed 3D property in AudioClip and moved all 3D audio functionality to the AudioSource. 
<ul>
<li>Renamed AudioSource.panLevel to AudioSource.spatialBlend. This property now controls the 2D / 3D mode of sound playback through this AudioSource. There is no longer a mode toggle, but a continuous interpolation between the two states.</li>
<li>Renamed AudioSource.pan to AudioSound.panStereo. This is to remove confusion about the nature of this property. AudioSource.panStereo pans the audio signal into the left or right speakers. This happens before spatial panning is applied and can be applied in conjunction with 3D panning.</li>
</ul></li>
</ul>

### Blackberry
<ul>
<li>Added "Add Attached Device" to the debug token creation window.</li>
<li>Application.systemLanguage now differentiates between Chinese Simplified and Chinese Traditional appropriately.</li>
<li>Registration now uses BlackBerry's 10.2 registration system. Currently registered systems do not need to re-register.</li>
</ul>

### Documentation
<ul>
<li>Default language for code snippets in the Scripting Reference is C#, with many more examples in C# available, with Javascript as a secondary language, and Boo removed.</li>
<li>Localized documentation available in Russian, Spanish and Japanese (currently based on 4.6 docs and over time 5.0).</li>
<li>Improved handling of namespaces, generics and interfaces.</li>
<li>API history improved with information about obsolete members.</li>
</ul>

### Editor
<ul>
<li>Added 8192 maximum texture size option in import settings.</li>
<li>Added deferred diffuse/specular/smoothness/normals scene view rendering modes.</li>
<li>Added GetCurrentGroupName() and SetCurrentGroupName() to allow overriding the automatic undo name generation</li>
<li>Added Gizmos.DrawMesh and DrawWireMesh (the meshes drawn are pickable too).</li>
<li>Added support for importing textures from PVRv3, ASTC, KTX file formats.</li>
<li>Added virtual function ScriptableWizard.DrawWizardGUI for customizing GUI of derived wizard classes.</li>
<li>Added warning on exiting play mode when objects have been spawned into the scene from OnDestroy().</li>
<li>Asset Store: The asset store window is now much faster, more responsive, and looks better.</li>
<li>Camera inspector shows camera's depth texture mode. Also, scene view camera makes sure to match main camera's depthTextureMode.</li>
<li>Drag-and-drop assigns material to a specific part of the mesh now. Holding Alt key will assign material to all the parts of the mesh.</li>
<li>EditorStyles.helpBox is now exposed</li>
<li>Ensure controls are not rendered with focus state if the EditorWindow they are in does not have focus.</li>
<li>Expose RenderTexture color format in the inspector, just like with depth format.</li>
<li>Exposed AssetPreview.SetPreviewTextureCacheSize ().</li>
<li>Finished builds will be shown in OS X notification center when Editor in the background.</li>
<li>Frame Selected (F key over scene view) now takes point/spot light range into account.</li>
<li>Improved build times for textures and AudioClips</li>
<li>Improved searching for class names in different namespaces and across different user assemblies.</li>
<li>Improved UI display names in Player Settings</li>
<li>License: Activate from command-line.</li>
<li>License: Added -returnlicense command line option, which returns the currently active license and quits the editor.</li>
<li>License: A progress bar will be shown during returning or releasing a license.</li>
<li>LightmapParameters now has an icon</li>
<li>LightmapSnapshot now has an icon</li>
<li>MaterialEditor improvements 
<ul>
<li>Show a foldout arrow for Material inspectors inlined on gameobjects to make it clear that they can be expanded/collapsed.</li>
<li>Added TexturePropertyMiniThumbnail(): Draw a property field for a texture shader property that only takes up a single line height. The thumbnail is shown to the left of the label. Clicking the thumbnail will show a large preview info window.</li>
<li>Added GetTexturePropertyCustomArea():. Returns the free rect below the label and before the large thumb object field. Is used for e.g. tiling and offset properties.</li>
<li>Added TextureScaleOffsetProperty(): Draws tiling and offset properties for a texture.</li>
<li>Texture scaling and offset values can now be dragged.</li>
</ul></li>
<li>Optimization of Hierarchy Window</li>
<li>Prevent tooltips from showing while dragging.</li>
<li>Tag editor facelift by removing the empty tag and using Reorderable list to draw tags and layers.</li>
<li>When browsing for a location to create or open a project, the dialog starts at the location where a project was last created or opened.</li>
<li>When saving scenes, overwrite existing scene file only after successful save.</li>
<li>Windows Editor: Native child windows have their title set to the GUIView/EditorWindow class name.</li>
<li>Unity will output a proper error regarding incompatible CPU architectures on Mac OS X when failing to load native libraries. For ex., You cannot load 32 bit native libraries on 64 bit Editor.</li>
</ul>

### Fonts
<ul>
<li>Added easier APIs to access OS Fonts (Font.GetOSInstalledFontNames and Font.CreateDynamicFontFromOSFont).</li>
<li>Added new APIs to get font metrics if you want to implement your own font rendering: Font.ascent, Font.lineheight, new fields in CharacterInfo (old fields in CharacterInfo are deprecated).</li>
<li>Optimized texture rebuilds to happen less often.</li>
</ul>

### Graphics
<ul>
<li>Added "#pragma exclude_renderers nomrt" for platforms not supporting multiple render targets (MRTs).</li>
<li>Added Camera.onPreCull, onPreRender, onPostRender delegates.</li>
<li>Added RenderTextureFormat.ARGB2101010 and Shadowmap formats.</li>
<li>Added Shader.IsKeywordEnabled API.</li>
<li>Added SystemInfo.graphicsMultiThreaded API.</li>
<li>Added Texture2D.SetPixels32 overload that accepts offset and dimensions.</li>
<li>All baked and realtime lightmapping computations are now done in linear space, this makes lighting between gamma &amp; linear space look much closer. When using pure lightmaps, it should in fact look very similar.</li>
<li>Allow SkinnedMeshRenderer to accept non-skinned meshes.</li>
<li>DDS importer can import Float, Half and 11.11.10 format .dds textures now.</li>
<li>Dynamic batching can batch non-uniform scaled objects together when normals/tangents are unused. Helps with shadow caster batching, and unlit shaders.</li>
<li>Image Effects: Added Threshold tweak to SunShafts, removed legacy "alpha as mask".</li>
<li>Image Effects: GlobalFog image post-processing effect was rewritten. Now it has "distance fog" (matches what is set in lighting settings), and optional "height fog" (linearly increasing fog density below specified height).</li>
<li>Increased maximum number of simultaneous render targets (MRT) to 8 on capable platforms.</li>
<li>Light intensity now behaves consistently between linear and gamma space rendering mode. Lights in linear mode can now have much higher intensity. The light intensity is now defined to be in gamma space, hence in linear rendering it is converted to linear space when passed to the shader. (In linear space the maximum effective light intensity is now 97 while previously it was 8).</li>
<li>Lightmaps &amp; baked probes compressed with RGBM now have an effective range of 5 in gamma space or 32 in linear space. This reduces RGBM compression artifacts for lightmaps. Emissive surfaces for enlighten are encoded with a range of 8 in gamma space and 97 in linear space.</li>
<li>Meshes: Mesh compression will now also do lossy compression of vertex colors.</li>
<li>Meshes: Added "keep quads" mesh import option; useful for DX11/Console tessellation shaders.</li>
<li>Optimized per-object light culling in forward rendering by using multiple CPU cores better.</li>
<li>Overhauled stats window to be more compact and profiler rendering stats to be more comprehensive.</li>
<li>Reduced memory consumption when loading textures on mobile devices.</li>
<li>Rendering code optimized to reduce amount of material SetPass calls. Light probes and lightmap UV transform state changes are now internally applied via MaterialPropertyBlocks without requiring a full SetPass. This reduces cost on the main thread to send commands to the render thread, and on the the render thread the driver overhead is reduced.</li>
<li>Scene View: Can drag a cubemap onto empty space in the scene view to assign it as a skybox.</li>
<li>Skinned meshes use less memory by sharing index buffers between instances.</li>
<li>Support for more shader keywords (128, up from 64). </li>
</ul>

### iOS
<ul>
<li>Added debug labels for OpenGL objects, useful in Xcode frame capture debugging.</li>
<li>Allow to set compile flags for already existing files in Xcode API</li>
<li>Better support for Unity view size changes from native side.</li>
<li>Enabled basic background processing.</li>
<li>Expose font directories to the trampoline</li>
<li>Game controller button pressure is now also exposed as axis (float) value.</li>
<li>Implement a way to select iOS framework dependencies for native plugins.</li>
<li>Improved performance of adding large number of files to Xcode project</li>
<li>Optimized Texture2D.LoadImage performance for PNG and JPG files.</li>
<li>Tweaked external RenderSurface API to make a bit more sense and be more concise.</li>
</ul>

### Linux
<ul>
<li>Added Input.IsJoystickPreconfigured for querying 5.0 Linux gamepad detection.</li>
<li>Monitor selection</li>
<li>Set popupwindow mode via Motif borderless hint when supported</li>
<li>Support XDG-compliant path overrides.</li>
</ul>

### Networking
<ul>
<li>WWW: Populate .bytes and .text on non-200 response.</li>
</ul>

### Performance
<ul>
<li>Improved multithreaded job system: 
<ul>
<li>Culling &amp; shadow caster culling is multithreaded now.</li>
<li>Internally multithreaded parts (culling, skinning, mecanim, ...) are more efficient now via some lockless magic.</li>
<li>Temporary memory allocations done by some jobs are more efficient now.</li>
</ul></li>
<li>Improved loading performance. More work has been offloaded to the loading thread, reducing the overhead of asynchronous loading on the main thread.</li>
<li>Object.Instantiate performance has been improved.</li>
<li>Mecanim optimizations: 
<ul>
<li>Optimized Animator Enable(), 2x speed on complex controllers.</li>
<li>Optimized Animator memory usage per instance, 2x smaller on complex controllers.</li>
<li>Improved performance for Animator Tool.</li>
</ul></li>
<li>Optimized memory usage and runtime performance when serializing objects with backward compatibility (type-tree) enabled.</li>
<li>Optimized texture importing performance.</li>
<li>Static batching performance is improved in many cases.</li>
<li>Updated occlusion culling (Umbra) version; contains improvements for mobile Umbra culling performance, and improves occlusion culling robustness in some cases.</li>
</ul>

### Physics
<ul>
<li>Adaptive force is now optional (disabled by default).</li>
<li>Changed default cloth coefficient values, and added info boxes to cloth editor</li>
<li>Cloth constraint editing UI has been replaced by a more intuitive UI inside the Scene View.</li>
<li>Cloth; exposed sleep force parameter to tune minimum force after which cloth will start sleeping.</li>
<li>Cloth; exposed tethers flag to improve cloth simulation quality.</li>
<li>Cloth inspector is now much faster and capable of dealing with meshes of any vertex count</li>
<li>Exposed a function ConfigureVehicleSubsteps in WheelCollider to make it possible for developers to customise vehicle sub-stepping. This helps setting up heavy vehicles, that require different amount of sub-steps to simulate wheels correctly.</li>
<li>Make scaling mesh colliders cheaper, by not creating a new mesh with scaling applied to it with every scale change.</li>
<li>Redesigned WheelCollider gizmo to show more relevant information.</li>
<li>Removed internal lock in PhysXRaycast, particles should now be able to process raycasts in multithreaded mode.</li>
<li>Show inconsistent hinge joint constraints in inspector</li>
<li>Updated default values for WheelCollider as the old ones did not make any sense with new PhysX.</li>
</ul>

### Players
<ul>
<li>Add -show-screen-selector command line option for Linux and Windows.</li>
<li>Cursor management cleanup 
<ul>
<li>Screen.lockCursor has become Cursor.lockState</li>
<li>Screen.showCursor has become Cursor.visible</li>
<li>Added ConfineCursor state to confine cursor to game window (Linux/Windows)</li>
<li>Cursor lock state and cursor visibility state are now mutually independent.</li>
</ul></li>
</ul>

### Plugins
<ul>
<li>Unity will now verify that plugins don’t collide with each other before building to player. Previous behavior was that you would need to wait until all the scenes were built, and you would only then see that plugin with same filename is trying to overwrite another plugin.</li>
<li>(Windows Store Apps/Windows Phone): when picking placeholder plugins only plugins with matching file names as the original plugin will be shown</li>
</ul>

### Profiler
<ul>
<li>Added total and per frame GC allocated bytes to the Memory chart.</li>
<li>Image Effects have profiling blocks with the script name in them, instead of a generic "ImageEffect".</li>
<li>Improved accuracy of reported AudioSources in the scene when working with AudioSources in prefabs.</li>
<li>Search field for filtering the results in the treeview.</li>
<li>Stop collecting GPU data when GPU Profiler chart is closed. Defaults to being closed for performance reasons.</li>
<li>Stop collecting profiler's data on Player's side if recording is disabled.</li>
</ul>

### Scripting
<ul>
<li>64-bit platforms will now accept managed DLLs compiled specifically for x64.</li>
<li>Added defines for UNITY_EDITOR_64/32, UNITY_5.</li>
<li>Added disposable scope helpers for Begin/End pairs for GUI, GUILayout, EditorGUI and EditorGUILayout.</li>
<li>Added formatting overloads to Debug.Log*.</li>
<li>Added generic overloads for AssetBundle.Load*.</li>
<li>All GetComponent paths got much faster, especially GetComponent.</li>
<li>GetComponent family of functions now supports interfaces as generic argument.</li>
<li>Improve error messages reported by IL2CPP by including managed source code information when it is available.</li>
<li>Math: Added SphericalHarmonicsL2 scripting struct.</li>
<li>Support serialization of all primitive types.</li>
</ul>

### Shaders
<ul>
<li>Added [NoTilingOffset] property attribute; hides tiling &amp; offset fields in texture property UI.</li>
<li>Added [Gamma] property attribute; allows Float and Vector properties to be flagged for automatic gamma correction. Tagged Float and Vector properties will function the same way as Color properties do - gamma correction will be applied, if necessary, before sending values to the GPU.</li>
<li>Added atmospheric thickness and sky tint controls to Skybox (procedural) shader; also visual appearance in gamma space matches that of linear now.</li>
<li>Added exposure slider to  "Skybox/Cubemap" and "Skybox/6 Planes" shaders.</li>
<li>Added MaterialPropertyDecorators. Similar to MaterialPropertyDrawers, but you can add many of them on a shader property. Added built-in decorators: [Space], [Header(text)].</li>
<li>Added rotation and exposure controls to Skybox (6-sided) and Skybox (cubemap) shaders.</li>
<li>Added SHADER_TARGET define that's based on "#pragma target" version. E.g. it will be 30 for SM3.0.</li>
<li>Added UNITY_NO_LINEAR_COLORSPACE define; defined on platforms that never have Linear color space.</li>
<li>Better comments in generated surface shader code. Better error messages when surface shader lighting functions aren't consistent.</li>
<li>Better handling of texture*Lod for OpenGL ES 2.0. On devices that don't support it, the generated shader code will automatically do a biased mip lookup approximation.</li>
<li>Built-in Fog works on all platforms now (includes WP8/WinRT/consoles).</li>
<li>Cleaned up shadow macros for shaders (UNITY_DECLARE_SHADOWMAP, UNITY_SAMPLE_SHADOW). On platforms that always have "native shadow maps" (e.g. DX11), there's no need for SHADOWS_NATIVE keyword to be present for these macros to do the right thing. On platforms that don't have native shadow maps (e.g. some GLES2.0 devices, Xbox360), these macros will do comparison of texture &amp; depth manually.</li>
<li>Existing user surface shaders with custom lighting functions work with Non-Directional (baked and realtime) and Directional (baked) lightmap types. These lighting functions need to be updated to use the UnityGI structure to take advantage of all the new lightmap types and reflection probes.</li>
<li>Improved "compile and show code" functionality in shader inspector. Now has dropdown to select custom set of platforms to compile shaders for. And shows a progress bar while compiling shader variants for display.</li>
<li>Improved importing performance, in-editor loading performance and reduced imported file sizes for shaders with really large variant counts.</li>
<li>Information about texture format decoding (LDR, dLDR, RGBM, Normals) is passed in %TextureName%_HDR shader constant.</li>
<li>Made it possible to use stencil buffer during deferred shading/lighting g-buffer passes, to some extent. Stencil reference value coming from shader/material will be combined (binary or) with Unity-supplied reference value.</li>
<li>Massively improved shader loading performance, and reduced memory consumption. 
<ul>
<li>By default, internal shader variants are only loaded when actually needed (typically a lot of shader variants are never actually needed).</li>
<li>Added ShaderVariantCollection asset type for ability to manually preload/warmup shader variants, to avoid hiccups later on. This is like Shader.WarmupAllShaders, done in a better way.</li>
<li>Editor can track shaders &amp; their variants used in scene or play mode, and create ShaderVariantCollection out of them (button in Graphics Settings).</li>
<li>Graphics Settings have a list of ShaderVariantCollection assets to preload at game startup. Can also warmup them from a script. </li>
</ul></li>
<li>Optimized shader compilation performance for OpenGL/ES platforms</li>
<li>Optimized shader importing performance, particularly for surface shaders with many multi_compile/shader_feature variants.</li>
<li>Shaders no longer apply a 2x multiply of light intensity. Instead lights are automatically upgraded to be twice as bright. This creates more consistency and simplicity in light rigs. For example a directional light shining on a white diffuse surface will get the exact color of the light. 
<ul>
<li>The upgrade does not affect animation, thus if you have an animated light intensity value you must change your animation curves or script code and make them 2x as large to get the same look.</li>
<li>You might have to adjust your shaders to remove a 2x multiply. This is only the case if you define your own lighting function, in the case of surface shaders this is usually not the case. So most content will not require the change. In most cases the shader code looks like this:

<ul>
<li>c.rgb = s.Albedo * _LightColor0.rgb * (diff * atten * 2); --&gt; c.rgb = s.Albedo * _LightColor0.rgb * (diff * atten);</li>
</ul></li>
</ul></li>
<li>Skybox shaders (including "Skybox/Procedural") get direction and color of the main light passed in the shader constants.</li>
<li>Surface shaders allow more texture interpolators, when targeting shader model 4.0+ (up to 32).</li>
<li>Surface shaders can use the UnityGI structure in their lighting functions. UnityGI contains light from all lightmap types, light probes and reflection probes. The built-in Lambert and BlinnPhong were updated to use it as well.</li>
<li>Surface shaders use up slightly less samplers on DX11-like platforms. Added UNITY_SAMPLE_TEX2D_SAMPLER helper macro to read a texture, while using sampler from another one.</li>
<li>Surface shaders using UnityGI and alpha transparency default to alpha premultiply mode (alpha:premul). Otherwise the default is alpha:blend.</li>
</ul>

### Substance
<ul>
<li>Consolidation of Substance binary data prior to runtime use now has a much lower peak memory footprint.</li>
</ul>

### Terrain
<ul>
<li>Added API GetTreeInstance()/SetTreeInstance()/treeInstanceCount on TerrainData class for fast tree updating.</li>
<li>Added "Keep existing trees" option when mass-placing trees.</li>
<li>Improved rendering performance when tree imposters are requested to be rendered.</li>
<li>New terrain materials. You now have 4 options to choose from: 
<ul>
<li>Built-in Standard. PBR material that uses the “standard” lighting model. This is the default option for newly created terrains.</li>
<li>Built-in Legacy Diffuse. This is the legacy built-in terrain material from Unity 4.x and before. It uses Lambert (diffuse term only) lighting model and has optional normal map support.</li>
<li>Built-in Legacy Specular. This built-in material uses BlinnPhong (diffuse and specular term) lighting model and has optional normal map support.</li>
<li>Custom. Use a custom material of your choice to render the terrain.</li>
</ul></li>
</ul>

### Version Control
<ul>
<li>Add shortcut for submit and cancel in submit dialog. Default keyboard focus to textarea when opening submit window.</li>
<li>Merging: Improve conflict output to console</li>
<li>Merging: Improve premerge by rewriting all of left, right and base.</li>
</ul>

### Windows
<ul>
<li>Standalone and webplayer: Input subsystem processes touch messages via WM_TOUCH. Previously it worked with Windows-simulated mouse events.</li>
<li>Windows Phone 8/Windows Store Apps</li>
<li>Added GetMethod() and GetProperty() to WinRTLegacy.TypeExtensions.</li>
<li>Added System.IO.Directory, System.IO.File, System.IO.FileStream, WinRTLegacy.IO.StreamReader, WinRTLegacy.IO.StreamWriter classes to WinRTLegacy</li>
<li>Shadows on windows mobile devices now work just like on iOS/Android - no cascaded shadow maps (i.e. not "too slow on mobile" anymore).</li>
<li>Significantly improved performance of passing System.Type objects to UnityEngine (for example, GetComponent is affected)</li>
<li>UnityPlayer.dll now contains version info.</li>
<li>Windows Phone 8: Geolocator initialization code removed from Visual Studio project files. When overwriting existing 4.x projects please remove redundant code.</li>
</ul>

### Windows Store Apps
<ul>
<li>Added Directory, DirectoryInfo, File, FileStream replacements to WinRTLegacy.</li>
<li>Added support for linear color space.</li>
<li>Added OnFileActivated handler in App.xaml.[cs/cpp].</li>
<li>Added UnityEngine.WSA.Application.advertisingIdentifier.</li>
<li>Building on top of existing project will now check if a project being overwritten is compatible with newly built one.</li>
<li>Chinese Traditional and Simplified languages are now detected and reported, instead of always returning generic Chinese.</li>
<li>Handheld class added.</li>
<li>PlayerPrefs will be saved whenever application goes into suspend mode.</li>
<li>Use joysticks in addition to Xbox 360 controllers, but you have to enable HumanInterfaceDevice capability in PlayerSettings. Note: this capability is not visible in Package.appxmanifest UI interface in Visual Studio.</li>
</ul>
