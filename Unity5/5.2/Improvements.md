# Unity 5.2
https://unity3d.com/unity/whats-new/unity-5.2

## Improvements


### 2D Improvements
<ul>
<li>Allow sprites to be dragged into scene view in 3d mode. Add temp GO while dragging for visual feedback similar to when dragging prefabs/model into scene view</li>
<li>Frame selected command (F) now works in the sprite editor window for the selected sprite rect</li>
<li>Implement undo functionality for sprite editor window's slice menu</li>
<li>New grid slicing method that uses column and row count</li>
<li>Pivot snapping on sprite frame rect in sprite editor window only happens when Ctrl is pressed while mouse dragging the pivot handle</li>
<li>Provide a custom pivot field in the slicing menu for the sprite editor window</li>
<li>Zooming on sprite editor window’s texture will zoom towards mouse cursor</li>
</ul>

### Editor Improvements
<ul>
<li>Added RunOpenPanelWithFilters API</li>
<li>Better error message when "The classes in the module cannot be loaded" is thrown</li>
<li>Improved Compute Shader inspector; now lists errors &amp; warnings similar to regular shader inspector</li>
<li>Improved Export Package window (now uses a proper tree view)</li>
<li>Improved shader inspector performance when there are many errors shown</li>
<li>Make sure ObjectField and Object Selector shows icons for game objects and prefabs</li>
<li>More "create new shader" templates under assets create menu (PBS surface shader, unlit shader, image effect shader)</li>
<li>Selection.selectionChange callback triggered when selection changes</li>
<li>Show proper cubemap preview instead of icon in large preview ObjectField</li>
<li>When in 2D mode, the camera bounds for the main camera is always visible when it is in orthographic mode</li>
</ul>

### Graphics, Lightmapping and Shader Improvements
<ul>
<li>GI: Added progress bar for GI Cache -&gt; Clean Cache progress status</li>
<li>GI: Allow ambient intensity higher than 1</li>
<li>GI: Size of the last lightmap is now reduced to pack the instances more tightly and not waste space</li>
<li>Graphics: Add SetUVs to Mesh API, it takes a UV channel, and a List of either Vector2, Vector3, or Vector4 as arguments</li>
<li>Graphics: Added a quality setting 'Shadow near plane offset' to allow working around shadow pancaking artifacts</li>
<li>Graphics: Added CommandBuffer.IssuePluginEvent to allow invoking native code plugin from a command buffer</li>
<li>Graphics: Added Cubemap.mipmapCount</li>
<li>Graphics: Implemented object naming for D3D11, so textures and meshes will pick up the correct name in external graphics debuggers (e.g. RenderDoc, NSight etc.)</li>
<li>Graphics: Memory saving for meshes with &lt; 300 vertices if dynamic batching is off</li>
<li>Graphics: New GL.IssuePluginEvent override allows invoking a specific callback in a specific native plugin</li>
<li>Graphics: Windows Store Apps 8.1 and Windows Phone 8.1 now support MSAA</li>
<li>Image Effects: Added option to disable 'no fog on skybox pixels' behaviour in GlobalFog effect</li>
<li>OpenGL: Added -force-clamped argument that prevents use of all available extensions when used together with -force-glcoreXX or -force-glesXX</li>
<li>OpenGL: Added -force-gles editor and standalone player to automatically run with the best version of ES supported by the platform</li>
<li>Particles: Mesh particles now support the Texture Sheet Animation settings</li>
<li>Reflection Probes: when using Deferred Shading, the reflection probes are now rendered per-pixel (instead of each object only being affected by one or two probes)</li>
<li>Shaders: Added finalgbuffer and finalprepass modifiers. They work in the same way as finalcolor does, but are used by the deferred and prepass base paths respectively for altering what would be written into the gbuffer</li>
<li>Shaders: decal:add surface shaders now generate code for deferred and legacy deferred paths if finalgbuffer and finalprepass modifiers are specified</li>
<li>Shaders: Now #pragma skip_variants skips user variants as well</li>
<li>Shaders: Procedural Skybox shader now has selectable options for Sun Disk: None (fastest), Simple (should be close to the current sun disk), High Quality</li>
<li>Shaders: Make it possible to use UNITY_SAMPLE_SHADOW macros when SHADOWS_NATIVE keyword is not explicitly defined</li>
</ul>

### Mecanim Improvements
<ul>
<li>Added a "destructive action" prompt when deleting blend tree nodes, so that the behaviour is consistent between StateMachine and BlendTree graphs</li>
<li>Added AnimatorStateInfo.speed and AnimatorStateInfo.speedMultiplier</li>
<li>Added the possibility to create AnyState Transitions to the entry node of a state machine. In a sub state machine, this is essentially the same as creating an AnyState Transition to a sub state machine from the parent state machine. This also adds a straightforward way to add an AnyState Transition to the top-level state machine, which was previously only possible through roundabout methods</li>
<li>Added tracking of missing or invalid StateMachineBehaviours in the StateMachine and State inspectors. Missing or Invalid StateMachineBehaviours shouldn't disappear anymore from the inspector</li>
<li>Adding a child blend tree will use the default blend tree parameter, not the blend parameter of the parent</li>
<li>Alt-drag works in BlendTree graph view now</li>
<li>BlendTree API publishes useAutomaticThresholds</li>
<li>Can create new clip from selected clip/take in Animation importer</li>
<li>Creating a blend tree in a controller with no float parameter will now automatically add a new float parameter named Blend</li>
<li>Expose Animator.IsInitialized in scripting API</li>
<li>Fixing empty State Machine Behaviour after compilation error</li>
<li>Import humanoid animation warnings have been cleaned and improved. A “Warning” summary box has been added at the top of Animation Inspector to prevent warnings to be left unnoticed. Warnings are reported per take when animation file contains multiple takes. Warnings have been added when in-between humanoid bones rotation differs in Source Avatar and Animation. Text has been reformatted so that is easier to consult the warning report</li>
<li>Improved default IK Hint for legs. Default IK Hint for knee now points towards foot direction. It gives a more natural IK solving for leg when IK correction needed gets bigger</li>
<li>Improved display of transition previewer</li>
<li>Improved Humanoid animation jitters (Humanoid Oversampling). For some animations, usually those with fast motion, the Humanoid interpolation may differ from original Euler rotation interpolation. In those rare cases, use animator.humanoidOversampling to increase sampling rate. ModelImporterHumanoidOversampling.X2 up to X8 can be used. Usually 2 will do the job! Default is X1 or no oversampling. Key reducing can be used conjointly to only keep Humanoid animation oversampled keys where it is needed while reducing asset size</li>
<li>Renaming Animator parameters updates transitions using those parameters</li>
<li>Retargeting quality for humanoid import animation. The retargeting quality compares original generic animation with humanoid retargeted animation. An average or maximum position error greater than 1.0 “normalized” mm will be reported. An average or maximum error greater than 0.5 degree will be reported. The time (and frame number) in full take of maximum errors is also reported. The position and rotation errors are reported per human body parts. The Retargeting Quality report can be turned on or off in Import Message foldout of Animation Inspector. It is off by default as it makes file import slower</li>
<li>SetBoneLocalRotation. Animator.SetBoneLocalRotation let you modify the local rotation of humanoid bone during IK passes/OnAnimatorIK() callback. It can be used to modify the pose of a humanoid avatar after Animation Blending, but that will still be taken in account by IK Solving. Ex: Adjust Hips and Spine rotation to drive lower and upper body independently on top of animation</li>
</ul>

### Networking Improvements
<ul>
<li>Added OnLobbyServerPlayersReady callback to the NetworkLobbyManager to allow users to perform custom behaviour when all the players in the lobby are ready</li>
<li>Added support for client-side authority for non-player objects. The new function NetworkServer.SpawnWithClientAuthority allows authority to be assigned to a client by its connection when an object is created</li>
<li>Networking: Added support for network [Command] calls from non-player objects with authority on a client</li>
<li>Networking: Added the ability for the NetworkTransform to validate on the server, the movement of authoritative client objects. There are now clientMoveCallback delegates on the NetworkTransform that allow user code to process 2D and 3D movement updates from clients before they are applied</li>
<li>Networking: Added NetworkDiscovery component to network HLAPI. This exposes the network transport layer local discovery function to HLAPI code, and allows Unity games on a local network to find each other</li>
</ul>

### Terrain Improvements
<ul>
<li>A warning message will be printed onto the console window if there are too many vertices in a detail patch. Increased the vertex limit to from 50k to 65k.</li>
<li>Deferred and legacy deferred rendering paths work again with Terrain</li>
<li>Made it easier to work with height maps created by World Machine. The default value of Byte Order option is now Windows (little endian). Added an option to vertically flip the height map when importing or exporting a raw file</li>
<li>Now 4097x4097 raw heightmap can be imported</li>
<li>Now a TerrainData object embedded into a scene (created by script) allows scene objects being selected as tree prefabs</li>
<li>SpeedTree: Negated tangent vectors to match those in the SpeedTree Modeler</li>
<li>SpeedTree: Now shader has less variants due to the merge of some geometry types</li>
<li>Trees painted on the terrain now are scaled by the prototype's transform scaling</li>
</ul>

### Other Improvements
<ul>
<li>Android: ETC2 is now the default compressed texture format for RGBA textures instead of RGBA4444</li>
<li>Audio: Improved preview rendering of audio clips, especially for clips that are very short</li>
<li>Audio: Improved inspector of AudioMixer performance parameters</li>
<li>Audio: One-shot sounds now also contribute to the data read by AudioSource.GetAudioData/GetSpectrumData</li>
<li>C# Project Generation: included extensions and rootnamespace now configurable in ProjectSettings-&gt;EditorSettings</li>
<li>C# Project Generation: only one set of project files will be generated, based on what the preferred external editor is</li>
<li>Fonts: CharacterInfo properties are now writeable</li>
<li>iOS/IL2CPP: Enable generic sharing for types and methods whose generic parameters have constraints</li>
<li>iOS/IL2CPP: Enable MakeGenericType and MakeGenericMethod for types and methods whose generic parameters have constraints</li>
<li>iOS/IL2CPP: Improve conversion time of IL2CPP, especially in generics heavy code</li>
<li>iOS: Added build number to Player Settings</li>
<li>iOS: Added onBannerFailedToLoad delegate to iOS.AdBannerView</li>
<li>iOS: Added support of asset tags and folder references to the Xcode API</li>
<li>Linux: Enable experimental GL core profile mode (via -force-glcore and friends)</li>
<li>Physics: Now you can set negative WheelCollider.forceAppPointDistance. This allows to adjust forceAppPointDistance in order to have suspension and tire forces applied at the wheel base</li>
<li>Physics: Renamed 'CollisionDetectionMode2D.None' to 'CollisionDetectionMode2D.Discrete' (scripts will be auto-updated)</li>
<li>Scripting: Application.isShowingSplashScreen checks if Unity is currently showing a splash screen</li>
<li>Stacktrace logging: Allow to log full (native/managed) stack trace when log is printed, the option is available in the console window in top right corner popup menu. Also check Application.stackTraceLogType API. Works in Editor and Windows/OSX standalone players</li>
<li>Substance: "visibleIf" expressions set in Substance Designer are now properly evaluated (for inputs only) and inputs are now displayed or hidden accordingly</li>
<li>Substance: Dynamic parameter in Substance graphs are now evaluated using native code instead of bytecode on Windows / OSX / Linux, resulting in faster texture generation</li>
<li>Substance: Feature parity with Substance Designer 5.1</li>
<li>Substance: Runtime generation of procedural materials is now supported on PS4 and XboxOne consoles</li>
<li>TrueTypeFontImporter: References to other font assets to be used in the project as fallback are now shown in the TrueTypeFontImporter inspector</li>
<li>UI: Add callback to MaskableGraphic for when it becomes culled via the 2D culling API</li>
<li>UI: Added support for EventType.ExecuteCommand "SelectAll" to InputField so that it works in the Editor</li>
<li>UI: Added underloaded function call for RectTransformUntility.RectangleContainsScreenPoint so a camera is not required</li>
<li>UI: Make the default value for a slider / scrollbar be 0</li>
<li>UI: Remove (Pro Only) from UI shaders as they can be used on any version of Unity 5</li>
<li>Version Control: Bottom most version control info bar in inspector shows separate state for meta file if different from asset</li>
<li>Version Control: Icon overlays for version control is surrounded by parenthesis in case an asset and its meta file's state is out of sync</li>
<li>Version Control: Reduce unnecessary checkouts</li>
<li>WebGL/IL2CPP: Improved stripping resulting in smaller build sizes</li>
<li>WebGL: Resolution set in HTML file will no longer be overridden by PlayerSettings</li>
<li>Windows Store Apps/Phone 8.1/Universal Apps: Unity will generate projects in a consistent way with Visual Studio. For ex., When specifying project names with whitespaces or symbols like '-', '.', Unity will no longer strip those symbols when creating folders, note this might break existing projects if you're building on top of old directory and your project name contains one of these symbols</li>
<li>Windows Store Apps/Phone 8.1/Universal Apps: Unity will properly use project name instead of hardcoded "Template" word, when creating App.xaml, App.xaml.cs, MainPage.xaml, MainPage.xaml.cs, AssemblyInfo.cs files</li>
<li>Windows Store Apps: InvokeOnAppThread/InvokeOnUIThread now will not cause deadlock, when called with sync=true multiple times in one chain</li>
<li>Windows Store Apps: supported orientations are now populated to manifest</li>
<li>Windows Store/Phone will now show animated Unity splashscreen instead of the static one</li>
<li>XboxOne: Improved performance for certain audio operations: converting float to PCM16 formats, mixing audio for one speaker configuration to another, and linear resampling</li>
<li>XboxOne: Unity is now build using the June 2015 QFE 1 XDK. You will need to have this XDK installed on your PC and use the matching or a later recovery</li>
</ul>
