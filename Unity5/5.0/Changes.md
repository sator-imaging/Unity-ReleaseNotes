# Unity 5.0
https://unity3d.com/unity/whats-new/unity-5.0

## Changes


### 2D
<ul>
<li>It's no longer possible to have multiple sprites with same name in Sprite Editor</li>
<li>UnityEditor.Sprites.DataUtility.GetSpriteMesh and GetSpriteIndices functions are now deprecated. Use Sprite.vertices, Sprite.uv and Sprite.triangles instead.</li>
</ul>

### AI
<ul>
<li>NavMesh bake settings: Removed width/height inaccuracy and allow to set voxel size instead.</li>
<li>NavMesh data format has changed - you need to rebuild the NavMesh to use it!</li>
<li>NavMeshLayer is replaced with NavMeshArea: old API is deprecated, area types are now stored in ProjectSettings/NavMeshLayers.asset.</li>
<li>NavMeshObstacle supports two basic shapes - Capsule and Box, for both carving and avoidance.</li>
<li>Setting destination on a NavMeshAgent doesn't resume the agent after calling Stop; call Resume explicitly to resume the agent. </li>
<li>Setting NavMeshAgent.nextPosition will update transform immediately if NavMeshAgent.updatePosition is true. This makes it consistent with the existing baseOffset and Move API.</li>
<li>Use smaller navmesh tile partitioning to improve baking and carving speed.</li>
<li>When NavMeshAgent.updatePosition is false - moving the transform position doesn't affect the internal agent position.</li>
<li>When NavMeshAgent.updatePosition is changed to true from false the transform position is moved to the internal agent position.</li>
</ul>

### Android
<ul>
<li>Disabled hidden input keyboard.</li>
<li>Dropped support for non-NEON CPU devices (e.g. Tegra 2). This gives a significant performance boost to Mecanim and PhysX among other things.</li>
<li>User resolution now gets swapped when the orientation is changed.</li>
<li>Default framebuffer format switched from RGBX to RGBA.</li>
<li>WebCamTexture is no longer supported on Gingerbread (2.3) devices.</li>
<li>Switched default from being a NativeActivity to a regular Java Activity. This should make the default Activity more compatible with 3rdparty Android frameworks.</li>
</ul>

### Animation
<ul>
<li>Added Animator.HasState to be able to query if an animator has a certain State.</li>
<li>Added console warning when an IK function is called when the Animator is not in the IK pass</li>
<li>Animator with Apply root motion ON will always be affected by physic gravity when playing a clip without any root motion curve.</li>
<li>Animator Tool deleting a layer or parameter can now be done with delete key.</li>
<li>AnimationUtility.SetAnimationClipSettings now public</li>
<li>Can now transition to self (State or StateMachine). <img class="ii-original" src="/sites/default/files/styles/original/public/animation-9.jpg?itok=UQehptUG" alt="description"></li>
<li>Changed profiling detail to see more information for the Animator evaluation pipeline.</li>
<li>Renamed Animator.GetCurrent/NextAnimationClipState to Animator.GetCurrent/NextAnimatorClipInfo.</li>
<li>In the character transform hierarchy, if a transform doesn't belong to the skeleton, then we preserve it as it is while doing optimization.</li>
<li>Moved AvatarMask to the Animations namespace.</li>
<li>Moved GameObjectUtility.OptimizetransformHierarchy from Editor code to Runtime class AnimatorUtility.OptimizetransformHierarchy.</li>
<li>Transform scale now blends linear instead of exponential. It allows blending with scale = 0.</li>
<li>Changed Culling Mode for the Animator. We now have “Always Animate”, “Cull Update Transforms” (was Based on Render) and “Cull Completely”.</li>
</ul>

### Asset Bundles
<ul>
<li>New version of WWW.LoadFromCacheOrDownload which can take Hash128 as version.</li>
<li>Rename AssetBundle.Load<strong><em>() to AssetBundle.LoadAsset</em></strong>().</li>
<li>Rename AssetBundle.LoadAll() to AssetBundle.LoadAllAssets().</li>
<li>Provide AssetBundle.LoadAllAssetsAsync() which loads all assets asynchronously.</li>
<li>Provide AssetBundle.LoadAssetWithSubAssets***() which loads the asset with the sub assets.</li>
<li>Provide AssetBundle.AllAssetNames() to return all the assets in the assetBundle.</li>
<li>Support type tree incremental build check.</li>
</ul>

### Asset Import
<ul>
<li>Unify global scale while importing FBX models.</li>
</ul>

### Asset Management
<ul>
<li>Resources.LoadAssetAtPath is no longer available outside of the Editor.</li>
</ul>

### Audio
<ul>
<li>AudioClip.isReadyToPlay is now obsolete and replaced by AudioClip.loadState.</li>
<li>AudioSettings.outputSampleRate and AudioSettings.speakerMode can now only be read from, because setting it required a complete restart of the sound system and therefore losing state of all non disk-based AudioClips and filters. SetDSPBufferSize has been declared obsolete for the same reason.</li>
<li>The hardware, loopable and compressionBitrate properties of AudioImporter are now obsolete.</li>
</ul>

### BlackBerry
<ul>
<li>Removed Author ID and Author ID override from publishing settings.</li>
<li>Removed obsolete "BB10" scripting targets from API. Please use "BlackBerry" instead.</li>
</ul>

### Editor
<ul>
<li>Apply build target switch from -buildTarget before initial domain load.</li>
<li>Creating, duplicating or instantiating (prefab) in editor generates unique name between siblings. Does not affect renaming, re-parenting, scripting or playmode.</li>
<li>Editor always runs in background when a debugger is attached. </li>
<li>EditorApplication.NewScene() creates a scene that has a Main Camera, a Directional Light, a default Skybox set and has Enlighten enabled by default. If you need a new scene with no GameObjects in it use EditorApplication.NewEmptyScene().</li>
<li>If standalone is current build target, do a full build target switch when setting EditorUserBuildSettings.selectedStandaloneTarget.</li>
<li>It is now recommended to derive from ShaderGUI instead of deriving from MaterialEditor to make custom gui for shaders. This ensures that custom shader gui works properly together with the Substance Material Editor (Check the docs for ShaderGUI).</li>
<li>Merged two scene view render mode dropdowns into one.</li>
<li>New bug reporter</li>
<li>Players always run in background when "Script Debugging" is enabled.</li>
<li>Prefab instance objects are no longer stored as part of the scene file.</li>
<li>Recognize more build target names with -buildTarget switch and remove 32bit/64bit switch for "standalone".</li>
<li>Remove warning if using Destroy/DestroyImmediate on objects that are still in the load queue and have not been woken up yet.</li>
<li>Removed “Make MMO” button from Edit menu. ;)</li>
<li>Renamed "Enable HW Statistics" player setting to "Disable Analytics".</li>
<li>Replace EditorUtility.UnloadUnusedAssets() to UnloadUnusedAssetsImmediate().</li>
<li>TextMesh and MeshFilter components are not allowed to exist on the same GameObject.</li>
<li>When manipulating preview object in Material inspector camera will rotate around the object instead of rotating the object itself, this was needed so you can see different reflections from different angles.</li>
</ul>

### Fonts
<ul>
<li>Font.textureRebuildCallback has been renamed to Font.textureRebuilt and is now a static event of type Action. Font.textureRebuildCallback continues to work but has been deprecated. This change cannot be upgraded automatically by the script updater.</li>
</ul>

### Graphics
<ul>
<li>Added GL.invertCulling property; obsoleted old GL.SetRevertBackfacing function.</li>
<li>Camera.pixelWidth and Camera.pixelHeight now return int, not float.</li>
<li>Changed behavior of what happens with textures that are too large for the GPU to handle, and they don't have mipmaps. Now such textures are displayed in blue color. Before, some platforms were downscaling them in some cases; other platforms were leaving them as garbage; others were crashing.</li>
<li>DX11: Uses CPU rendering (WARP device) when running in batch mode without a GPU; can also request WARP with "-force-driver-type-warp" command line argument.</li>
<li>GLES: Replaced 16bit depth buffer support with the ability to completely disable depth and stencil buffers.</li>
<li>Image Effects: 
<ul>
<li>All built-in image effects were rewritten from JavaScript to C#. You probably want to delete old files and import the fresh Effects package if you want the latest version.</li>
<li>Removed old Glow image effect; use Bloom or Bloom(optimized) instead.</li>
</ul></li>
<li>Light and Reflection Probes are enabled on Renderer components by default.</li>
<li>Made SystemInfo.graphicsPixelFillrate obsolete (it was not being maintained to cover new GPUs, and was not working on most platforms anyway). Now it always returns -1, just like it used to for unknown GPUs.</li>
<li>OnPreRender script callback is called before rendering camera's depth texture now.</li>
<li>Renamed HDR_LIGHT_PREPASS_ON shader keyword to UNITY_HDR_ON (now the keyword is always set when camera is HDR).</li>
<li>Renamed VertexLit and DeferredLighting rendering paths to "Legacy" names.</li>
<li>RenderTexture.Create now actually does nothing if RenderTexture is already created, just like documentation always said :)</li>
<li>Replaced the built-in sphere and capsule meshes with versions that are better suited for lightmapping. Because the topology has changed both UV1 and UV2 are now different.</li>
<li>Setting Mesh.colors keeps the colors in float format instead of converting to bytes. This allows you to store higher-precision color values on meshes. Note that it will use more memory so if that is a concern use Mesh.colors32 instead.</li>
<li>Skybox geometry was changed for cubemapped and other single-pass skybox shaders. Now instead of a big cube, it's a big and somewhat tessellated sphere, with more polygons near horizon. Allows computing things per-vertex in skybox shaders for performance.</li>
<li>Removed TextureUsageMode and TextureImportInstructions editor classes.</li>
</ul>

### iOS
<ul>
<li>Added specialized ViewControllers for fixed screen orientation. Added methods to AppController to override to provide custom ones.</li>
<li>An animated splash screen with a Unity logo is shown for non-Pro license users by the engine itself. Static pre-splash screens can be customized by all users.</li>
<li>Automatic Reference Counting (ARC) is enabled.</li>
<li>Changed the way UI integration works. Now there are specialized ViewController's for fixed orientation. Also made custom UI integration easier - both for simple and complicated cases (e.g. if you have portrait unity content in landscape ViewController, script side and _unityView.content orientation will return portrait, while AppController's interface orientation will be landscape). For more details check comments in Classes/UI/UnityAppController+ViewHandling.h in trampoline</li>
<li>createUnityViewImpl was deprecated and removed (assert will be fired if you implement this method). Override createUnityView instead.</li>
<li>createViewHierarchyImpl was deprecated and removed (assert will be fired if you implement this method). Override willStartWithViewController instead.</li>
<li>createViewHierarchy was deprecated and removed. Use createUI instead if you had it called from custom place.</li>
<li>Refactored player pausing in the trampoline.</li>
<li>Default splash screens set to solid color.</li>
<li>Trampoline now uses clang standard library, C++11 is enabled, iOS 7.0 SDK and Xcode5 are enforced, iOS 6.0 is the minimal version supported.</li>
<li>Fixed TCP 56000 port in now used by player for script debugging.</li>
</ul>

### Linux
<ul>
<li>Minimum supported version is now Ubuntu 12.04 LTS.</li>
</ul>

### OS X
<ul>
<li>Application.persistentPath will now correctly give you a folder in ~/Application Support instead of ~/Library/Caches.</li>
<li>Mac OS X Standalone: Data folder has moved to Content/Resources, in accordance with Apple guidelines.</li>
</ul>

### Physics
<ul>
<li>Disabled MonoBehaviours will no longer receive collision or trigger callbacks.</li>
<li>Expose contactOffset both global and per-shape. This comes to replace Physics.minPenetrationForPenalty that lost its original meaning with the upgrade to PhysX3. Contact offset is the value that directly affects the distance at which PhysX starts generating contacts; when the distance between colliders is  less than the sum of their respective contact offsets the contacts are generated. The value is useful when you have fast moving ragdolls and observe the not physically correct behaviour of joints when the colliders they connect penetrate other collision geometry.</li>
<li>Expose enablePreprocessing on joints. Having this flag unset basically lets PhysX to ignore some of the broken joint constraints in complicated configurations; otherwise such constraints may produce huge impulses that lead to "explosions". A typical usecase would be when upgrading a PhysX-powered Unity 4 2D game where you have 2 rotations frozen on each Rigidbody and joints are attached to some of them.</li>
<li>Expose projections on CharacterJoint to help with stretching of limbs. Joint projection is a technique that once enabled makes sure the joint constraints are not violated for more than a tolerance value by adjusting the connected bodies' pose so that they it is always within tolerance. This is not a physical process (it may loose energy) and comes with some performance cost, but can serve as a good last resort in challenging configurations where otherwise ragdolls explode or overstretch.</li>
<li>Make CharacterController ignore any child &amp; sibling colliders</li>
<li>Physics.maxAngularVelocity has been removed as it is non-functional in PhysX 3.3. You can still use Rigidbody.maxAngularVelocity.</li>
</ul>

### Scripting

#### Note: Many scripting changes should be handled automatically by our new API upgrade tool, see http://blogs.unity3d.com/2014/06/23/unity5-api-changes-automatic-script-updating/
<ul>
<li>AddComponent(string) is removed. Use AddComponent() instead.</li>
<li>Added generic version of Object.Instantiate (has been in the docs since 3.5 but not exposed in the API before).</li>
<li>Application.RegisterLogCallback() and RegisterLogCallbackThreaded() have been deprecated and replaced by two new events Application.logMessageReceived and Application.logMessageReceivedThreaded. This allows for multiple subscribers.</li>
<li>C# compiler defaults script encoding to UTF8.</li>
<li>Deprecated Component.active property has been removed.</li>
<li>GameObject.SampleAnimation() moved to AnimationClip.SampleObject().</li>
<li>'Metro' keyword was replaced to 'WSA' in most APIs, for ex., BuildTarget.MetroPlayer became BuildTarget.WSAPlayer, PlayerSettings.Metro became PlayerSettings.WSA. Defines in scripts like UNITY_METRO, UNITY_METRO_8_0, UNITY_METRO_8_1 are still there, but along them there are defines UNITY_WSA, UNITY_WSA_8_0, UNITY_WSA_8_1.</li>
<li>ParticleSystem.safeCollisionEventSize changed to ParticleSystem.GetSafeCollisionEventSize().</li>
<li>Removed quick property accessors, like .rigidBody, .rigidbody2D, .camera, .light, .animation, .constantForce, .renderer, .audio, .networkView, .guiTexture, .collider, .collider2D, .particleSystem, .particleEmitter, .guiText, .hingeJoint for modularization. Instead, use GetComponent to get references.</li>
<li>Removed obsolete graphics APIs: Camera.mainCamera (use Camera.main), Camera.GetScreenWidth (use Screen.width), Camera.GetScreenHeight (use Screen.height), Camera.DoClear, Camera.isOrthoGraphic (use Camera.orthographic), Camera.orthoGraphicSize (use Camera.orthographicSize), Renderer.Render, Graphics.SetupVertexLights, obsolete Graphics.DrawMesh overloads (use DrawMeshNow), RenderTexture.SetBorderColor, Screen.GetResolution (use currentResolution), Mesh.uv1 (use uv2 instead), SkinnedMeshRenderer.skinNormals, LightmapData.lightmap (use lightmapFar instead).</li>
<li>Removed SystemInfo properties deviceName, deviceVendor, deviceVersion and supportsVertexProgram. Use graphicsDeviceName, graphicsDeviceVendor, graphicsDeviceVersion instead. Vertex programs are always supported.</li>
<li>TerrainData.physicMaterial changed to TerrainData.GetPhysicMaterial() and TerrainData.SetPhysicMaterial().</li>
</ul>

### Shaders
<ul>
<li>All opaque &amp; skybox built-in shaders and surface shaders now output 1.0 into the alpha channel. This means that image effects that used "alpha as fake HDR" (e.g. old Glow from Unity 1.x days) will not work with them anymore. Use “keepalpha” surface shader option to keep the old behavior.</li>
<li>Alpha blended surfaces do NOT automatically have "Alphatest Greater 0" in generated shader code.</li>
<li>Built-in default "gray" shader texture is color space aware now.</li>
<li>Built-in functionality for directional lightmaps, dynamic Enlighten GI and soft shadows all require shader model 3.0 now.</li>
<li>Built-in lightmaps (unity_Lightmap etc.) are declared in UnityShaderVariables.cginc now. If you had them declared in your own shader code, you might need to remove them (we'll try to do that automatically).</li>
<li>Fog handling in shaders was changed. 
<ul>
<li>For surface shaders and fixed function shaders, nothing to do. Can add "nofog" to surface shader #pragma line to explicitly make it not support fog.</li>
<li>For manual vertex/fragment shaders, fog does not happen automagically now. You need to add #pragma multi_compile_fog and fog handling macros to your shader code. Check out built-in shader source, for example Unlit-Normal how to do it.</li>
</ul></li>
<li>Improved error messages for some shader compilation errors.</li>
<li>Removed some fixed-function shader features (use vertex &amp; fragment shaders instead). This makes per-draw-call CPU overhead slightly lower across all platforms. 
<ul>
<li>Removed TexGen. If you have old Projector shaders, they might be using this; upgrade to 4.5/5.0 projector shaders.</li>
<li>Removed texture combiner matrix transforms, i.e. "matrix" command inside a SetTexture.</li>
<li>Removed signed add (a+-b), multiply signed add (a<em>b+-c), multiply subtract (a</em>b-c), dot product (dot3, dot3rgba) SetTexture combiner modes.</li>
<li>SetTexture stage count is limited to 4 on all platforms.</li>
</ul></li>
<li>Renamed "RenderFX/Skybox cubed" and "RenderFX/Skybox" shaders to "Skybox/Cubemap" and "Skybox/6 Planes".</li>
<li>Renamed unity_LightmapIndScale variable to unity_DynamicLightmapScale</li>
<li>Some shader compilers have changed: 
<ul>
<li>Mixing partially fixed function &amp; partially programmable shaders (e.g. fixed function vertex lighting &amp; pixel shader; or a vertex shader and texture combiners) is not supported anymore. It was never working on mobile, consoles or DirectX 11 anyway. This required changing behaviour of Reflective/VertexLit shader to not do that - it lost per-vertex specular support; on the plus side it now behaves consistently between platforms.</li>
<li>Direct3D 9 shader compiler was switched from Cg 2.2 to HLSL, the same compiler that's used for D3D11. This fixes a bunch of issues where Cg was generating invalid D3D9 shader assembly code; and generally produces slightly more efficient shaders. However, HLSL is slightly more picky about syntax; in general you have to do same shader fixes for D3D9 as for D3D11 now (e.g. UNITY_INITIALIZE_OUTPUT for “out” structures).</li>
<li>On desktop OpenGL, shaders are always compiled into GLSL instead of ARB_vertex/fragment_program target now. You no longer need to write "#pragma glsl" to get to features like vertex textures or derivative instructions. All support for ARB_vertex/fragment_programs is removed.</li>
</ul></li>
</ul>

### Shadows
<ul>
<li>All built-in shadow shaders use backface culling now. Use “two sided” cast shadows option if you do not need backface culling.</li>
<li>Shadows on D3D9 require "native shadowmap" support in the driver now (pretty much all systems that can do shadows have that, so this should be fairly invisible). Upside: less shader variants are included into game builds now.</li>
<li>Shadows on iOS+GLES2.0 require GL_EXT_shadow_samplers now. This means iPhone4 / iPodTouch4 will not support realtime shadows anymore. Upside: less shader variants and faster shader loading times.</li>
<li>Removed screenspace directional light shadow blur (PCF 5x5 is used now). 
<ul>
<li>Removed shadow softness &amp; softness fade from Light.</li>
<li>Normal-based shadow bias defaults to 0.4 for lights now</li>
</ul></li>
<li>When using oblique camera projection, shadows are disabled now.</li>
</ul>

### Web Player
<ul>
<li>Removed WWW.LoadUnityWeb API. Load additional unity web file from website script code.</li>
<li>Windows Store Apps</li>
<li>Removed support for C++ Visual Studio projects.</li>
</ul>
