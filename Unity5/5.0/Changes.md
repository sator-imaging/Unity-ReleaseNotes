# Unity 5.0

https://unity3d.com/unity/whats-new/unity-5.0

## Changes

- [2D](#2d)
- [AI](#ai)
- [Android](#android)
- [Animation](#animation)
- [Asset Bundles](#asset-bundles)
- [Asset Import](#asset-import)
- [Asset Management](#asset-management)
- [Audio](#audio)
- [BlackBerry](#blackberry)
- [Editor](#editor)
- [Fonts](#fonts)
- [Graphics](#graphics)
- [iOS](#ios)
- [Linux](#linux)
- [OS X](#os-x)
- [Physics](#physics)
- [Scripting](#scripting)
- [Shaders](#shaders)
- [Shadows](#shadows)
- [Web Player](#web-player)


### 2D

*   It's no longer possible to have multiple sprites with same name in Sprite Editor
*   UnityEditor.Sprites.DataUtility.GetSpriteMesh and GetSpriteIndices functions are now deprecated. Use Sprite.vertices, Sprite.uv and Sprite.triangles instead.

### AI

*   NavMesh bake settings: Removed width/height inaccuracy and allow to set voxel size instead.
*   NavMesh data format has changed - you need to rebuild the NavMesh to use it!
*   NavMeshLayer is replaced with NavMeshArea: old API is deprecated, area types are now stored in ProjectSettings/NavMeshLayers.asset.
*   NavMeshObstacle supports two basic shapes - Capsule and Box, for both carving and avoidance.
*   Setting destination on a NavMeshAgent doesn't resume the agent after calling Stop; call Resume explicitly to resume the agent.
*   Setting NavMeshAgent.nextPosition will update transform immediately if NavMeshAgent.updatePosition is true. This makes it consistent with the existing baseOffset and Move API.
*   Use smaller navmesh tile partitioning to improve baking and carving speed.
*   When NavMeshAgent.updatePosition is false - moving the transform position doesn't affect the internal agent position.
*   When NavMeshAgent.updatePosition is changed to true from false the transform position is moved to the internal agent position.

### Android

*   Disabled hidden input keyboard.
*   Dropped support for non-NEON CPU devices (e.g. Tegra 2). This gives a significant performance boost to Mecanim and PhysX among other things.
*   User resolution now gets swapped when the orientation is changed.
*   Default framebuffer format switched from RGBX to RGBA.
*   WebCamTexture is no longer supported on Gingerbread (2.3) devices.
*   Switched default from being a NativeActivity to a regular Java Activity. This should make the default Activity more compatible with 3rdparty Android frameworks.

### Animation

*   Added Animator.HasState to be able to query if an animator has a certain State.
*   Added console warning when an IK function is called when the Animator is not in the IK pass
*   Animator with Apply root motion ON will always be affected by physic gravity when playing a clip without any root motion curve.
*   Animator Tool deleting a layer or parameter can now be done with delete key.
*   AnimationUtility.SetAnimationClipSettings now public
*   Can now transition to self (State or StateMachine). ![description](/sites/default/files/styles/original/public/animation-9.jpg?itok=UQehptUG)
*   Changed profiling detail to see more information for the Animator evaluation pipeline.
*   Renamed Animator.GetCurrent/NextAnimationClipState to Animator.GetCurrent/NextAnimatorClipInfo.
*   In the character transform hierarchy, if a transform doesn't belong to the skeleton, then we preserve it as it is while doing optimization.
*   Moved AvatarMask to the Animations namespace.
*   Moved GameObjectUtility.OptimizetransformHierarchy from Editor code to Runtime class AnimatorUtility.OptimizetransformHierarchy.
*   Transform scale now blends linear instead of exponential. It allows blending with scale = 0.
*   Changed Culling Mode for the Animator. We now have “Always Animate”, “Cull Update Transforms” (was Based on Render) and “Cull Completely”.

### Asset Bundles

*   New version of WWW.LoadFromCacheOrDownload which can take Hash128 as version.
*   Rename AssetBundle.Load**_() to AssetBundle.LoadAsset_**().
*   Rename AssetBundle.LoadAll() to AssetBundle.LoadAllAssets().
*   Provide AssetBundle.LoadAllAssetsAsync() which loads all assets asynchronously.
*   Provide AssetBundle.LoadAssetWithSubAssets\*\*\*() which loads the asset with the sub assets.
*   Provide AssetBundle.AllAssetNames() to return all the assets in the assetBundle.
*   Support type tree incremental build check.

### Asset Import

*   Unify global scale while importing FBX models.

### Asset Management

*   Resources.LoadAssetAtPath is no longer available outside of the Editor.

### Audio

*   AudioClip.isReadyToPlay is now obsolete and replaced by AudioClip.loadState.
*   AudioSettings.outputSampleRate and AudioSettings.speakerMode can now only be read from, because setting it required a complete restart of the sound system and therefore losing state of all non disk-based AudioClips and filters. SetDSPBufferSize has been declared obsolete for the same reason.
*   The hardware, loopable and compressionBitrate properties of AudioImporter are now obsolete.

### BlackBerry

*   Removed Author ID and Author ID override from publishing settings.
*   Removed obsolete "BB10" scripting targets from API. Please use "BlackBerry" instead.

### Editor

*   Apply build target switch from -buildTarget before initial domain load.
*   Creating, duplicating or instantiating (prefab) in editor generates unique name between siblings. Does not affect renaming, re-parenting, scripting or playmode.
*   Editor always runs in background when a debugger is attached.
*   EditorApplication.NewScene() creates a scene that has a Main Camera, a Directional Light, a default Skybox set and has Enlighten enabled by default. If you need a new scene with no GameObjects in it use EditorApplication.NewEmptyScene().
*   If standalone is current build target, do a full build target switch when setting EditorUserBuildSettings.selectedStandaloneTarget.
*   It is now recommended to derive from ShaderGUI instead of deriving from MaterialEditor to make custom gui for shaders. This ensures that custom shader gui works properly together with the Substance Material Editor (Check the docs for ShaderGUI).
*   Merged two scene view render mode dropdowns into one.
*   New bug reporter
*   Players always run in background when "Script Debugging" is enabled.
*   Prefab instance objects are no longer stored as part of the scene file.
*   Recognize more build target names with -buildTarget switch and remove 32bit/64bit switch for "standalone".
*   Remove warning if using Destroy/DestroyImmediate on objects that are still in the load queue and have not been woken up yet.
*   Removed “Make MMO” button from Edit menu. ;)
*   Renamed "Enable HW Statistics" player setting to "Disable Analytics".
*   Replace EditorUtility.UnloadUnusedAssets() to UnloadUnusedAssetsImmediate().
*   TextMesh and MeshFilter components are not allowed to exist on the same GameObject.
*   When manipulating preview object in Material inspector camera will rotate around the object instead of rotating the object itself, this was needed so you can see different reflections from different angles.

### Fonts

*   Font.textureRebuildCallback has been renamed to Font.textureRebuilt and is now a static event of type Action. Font.textureRebuildCallback continues to work but has been deprecated. This change cannot be upgraded automatically by the script updater.

### Graphics

*   Added GL.invertCulling property; obsoleted old GL.SetRevertBackfacing function.
*   Camera.pixelWidth and Camera.pixelHeight now return int, not float.
*   Changed behavior of what happens with textures that are too large for the GPU to handle, and they don't have mipmaps. Now such textures are displayed in blue color. Before, some platforms were downscaling them in some cases; other platforms were leaving them as garbage; others were crashing.
*   DX11: Uses CPU rendering (WARP device) when running in batch mode without a GPU; can also request WARP with "-force-driver-type-warp" command line argument.
*   GLES: Replaced 16bit depth buffer support with the ability to completely disable depth and stencil buffers.
*   Image Effects:
    *   All built-in image effects were rewritten from JavaScript to C#. You probably want to delete old files and import the fresh Effects package if you want the latest version.
    *   Removed old Glow image effect; use Bloom or Bloom(optimized) instead.
*   Light and Reflection Probes are enabled on Renderer components by default.
*   Made SystemInfo.graphicsPixelFillrate obsolete (it was not being maintained to cover new GPUs, and was not working on most platforms anyway). Now it always returns -1, just like it used to for unknown GPUs.
*   OnPreRender script callback is called before rendering camera's depth texture now.
*   Renamed HDR\_LIGHT\_PREPASS\_ON shader keyword to UNITY\_HDR\_ON (now the keyword is always set when camera is HDR).
*   Renamed VertexLit and DeferredLighting rendering paths to "Legacy" names.
*   RenderTexture.Create now actually does nothing if RenderTexture is already created, just like documentation always said :)
*   Replaced the built-in sphere and capsule meshes with versions that are better suited for lightmapping. Because the topology has changed both UV1 and UV2 are now different.
*   Setting Mesh.colors keeps the colors in float format instead of converting to bytes. This allows you to store higher-precision color values on meshes. Note that it will use more memory so if that is a concern use Mesh.colors32 instead.
*   Skybox geometry was changed for cubemapped and other single-pass skybox shaders. Now instead of a big cube, it's a big and somewhat tessellated sphere, with more polygons near horizon. Allows computing things per-vertex in skybox shaders for performance.
*   Removed TextureUsageMode and TextureImportInstructions editor classes.

### iOS

*   Added specialized ViewControllers for fixed screen orientation. Added methods to AppController to override to provide custom ones.
*   An animated splash screen with a Unity logo is shown for non-Pro license users by the engine itself. Static pre-splash screens can be customized by all users.
*   Automatic Reference Counting (ARC) is enabled.
*   Changed the way UI integration works. Now there are specialized ViewController's for fixed orientation. Also made custom UI integration easier - both for simple and complicated cases (e.g. if you have portrait unity content in landscape ViewController, script side and \_unityView.content orientation will return portrait, while AppController's interface orientation will be landscape). For more details check comments in Classes/UI/UnityAppController+ViewHandling.h in trampoline
*   createUnityViewImpl was deprecated and removed (assert will be fired if you implement this method). Override createUnityView instead.
*   createViewHierarchyImpl was deprecated and removed (assert will be fired if you implement this method). Override willStartWithViewController instead.
*   createViewHierarchy was deprecated and removed. Use createUI instead if you had it called from custom place.
*   Refactored player pausing in the trampoline.
*   Default splash screens set to solid color.
*   Trampoline now uses clang standard library, C++11 is enabled, iOS 7.0 SDK and Xcode5 are enforced, iOS 6.0 is the minimal version supported.
*   Fixed TCP 56000 port in now used by player for script debugging.

### Linux

*   Minimum supported version is now Ubuntu 12.04 LTS.

### OS X

*   Application.persistentPath will now correctly give you a folder in ~/Application Support instead of ~/Library/Caches.
*   Mac OS X Standalone: Data folder has moved to Content/Resources, in accordance with Apple guidelines.

### Physics

*   Disabled MonoBehaviours will no longer receive collision or trigger callbacks.
*   Expose contactOffset both global and per-shape. This comes to replace Physics.minPenetrationForPenalty that lost its original meaning with the upgrade to PhysX3. Contact offset is the value that directly affects the distance at which PhysX starts generating contacts; when the distance between colliders is less than the sum of their respective contact offsets the contacts are generated. The value is useful when you have fast moving ragdolls and observe the not physically correct behaviour of joints when the colliders they connect penetrate other collision geometry.
*   Expose enablePreprocessing on joints. Having this flag unset basically lets PhysX to ignore some of the broken joint constraints in complicated configurations; otherwise such constraints may produce huge impulses that lead to "explosions". A typical usecase would be when upgrading a PhysX-powered Unity 4 2D game where you have 2 rotations frozen on each Rigidbody and joints are attached to some of them.
*   Expose projections on CharacterJoint to help with stretching of limbs. Joint projection is a technique that once enabled makes sure the joint constraints are not violated for more than a tolerance value by adjusting the connected bodies' pose so that they it is always within tolerance. This is not a physical process (it may loose energy) and comes with some performance cost, but can serve as a good last resort in challenging configurations where otherwise ragdolls explode or overstretch.
*   Make CharacterController ignore any child & sibling colliders
*   Physics.maxAngularVelocity has been removed as it is non-functional in PhysX 3.3. You can still use Rigidbody.maxAngularVelocity.

### Scripting

#### Note: Many scripting changes should be handled automatically by our new API upgrade tool, see http://blogs.unity3d.com/2014/06/23/unity5-api-changes-automatic-script-updating/

*   AddComponent(string) is removed. Use AddComponent() instead.
*   Added generic version of Object.Instantiate (has been in the docs since 3.5 but not exposed in the API before).
*   Application.RegisterLogCallback() and RegisterLogCallbackThreaded() have been deprecated and replaced by two new events Application.logMessageReceived and Application.logMessageReceivedThreaded. This allows for multiple subscribers.
*   C# compiler defaults script encoding to UTF8.
*   Deprecated Component.active property has been removed.
*   GameObject.SampleAnimation() moved to AnimationClip.SampleObject().
*   'Metro' keyword was replaced to 'WSA' in most APIs, for ex., BuildTarget.MetroPlayer became BuildTarget.WSAPlayer, PlayerSettings.Metro became PlayerSettings.WSA. Defines in scripts like UNITY\_METRO, UNITY\_METRO\_8\_0, UNITY\_METRO\_8\_1 are still there, but along them there are defines UNITY\_WSA, UNITY\_WSA\_8\_0, UNITY\_WSA\_8\_1.
*   ParticleSystem.safeCollisionEventSize changed to ParticleSystem.GetSafeCollisionEventSize().
*   Removed quick property accessors, like .rigidBody, .rigidbody2D, .camera, .light, .animation, .constantForce, .renderer, .audio, .networkView, .guiTexture, .collider, .collider2D, .particleSystem, .particleEmitter, .guiText, .hingeJoint for modularization. Instead, use GetComponent to get references.
*   Removed obsolete graphics APIs: Camera.mainCamera (use Camera.main), Camera.GetScreenWidth (use Screen.width), Camera.GetScreenHeight (use Screen.height), Camera.DoClear, Camera.isOrthoGraphic (use Camera.orthographic), Camera.orthoGraphicSize (use Camera.orthographicSize), Renderer.Render, Graphics.SetupVertexLights, obsolete Graphics.DrawMesh overloads (use DrawMeshNow), RenderTexture.SetBorderColor, Screen.GetResolution (use currentResolution), Mesh.uv1 (use uv2 instead), SkinnedMeshRenderer.skinNormals, LightmapData.lightmap (use lightmapFar instead).
*   Removed SystemInfo properties deviceName, deviceVendor, deviceVersion and supportsVertexProgram. Use graphicsDeviceName, graphicsDeviceVendor, graphicsDeviceVersion instead. Vertex programs are always supported.
*   TerrainData.physicMaterial changed to TerrainData.GetPhysicMaterial() and TerrainData.SetPhysicMaterial().

### Shaders

*   All opaque & skybox built-in shaders and surface shaders now output 1.0 into the alpha channel. This means that image effects that used "alpha as fake HDR" (e.g. old Glow from Unity 1.x days) will not work with them anymore. Use “keepalpha” surface shader option to keep the old behavior.
*   Alpha blended surfaces do NOT automatically have "Alphatest Greater 0" in generated shader code.
*   Built-in default "gray" shader texture is color space aware now.
*   Built-in functionality for directional lightmaps, dynamic Enlighten GI and soft shadows all require shader model 3.0 now.
*   Built-in lightmaps (unity\_Lightmap etc.) are declared in UnityShaderVariables.cginc now. If you had them declared in your own shader code, you might need to remove them (we'll try to do that automatically).
*   Fog handling in shaders was changed.
    *   For surface shaders and fixed function shaders, nothing to do. Can add "nofog" to surface shader #pragma line to explicitly make it not support fog.
    *   For manual vertex/fragment shaders, fog does not happen automagically now. You need to add #pragma multi\_compile\_fog and fog handling macros to your shader code. Check out built-in shader source, for example Unlit-Normal how to do it.
*   Improved error messages for some shader compilation errors.
*   Removed some fixed-function shader features (use vertex & fragment shaders instead). This makes per-draw-call CPU overhead slightly lower across all platforms.
    *   Removed TexGen. If you have old Projector shaders, they might be using this; upgrade to 4.5/5.0 projector shaders.
    *   Removed texture combiner matrix transforms, i.e. "matrix" command inside a SetTexture.
    *   Removed signed add (a+-b), multiply signed add (a_b+-c), multiply subtract (a_b-c), dot product (dot3, dot3rgba) SetTexture combiner modes.
    *   SetTexture stage count is limited to 4 on all platforms.
*   Renamed "RenderFX/Skybox cubed" and "RenderFX/Skybox" shaders to "Skybox/Cubemap" and "Skybox/6 Planes".
*   Renamed unity\_LightmapIndScale variable to unity\_DynamicLightmapScale
*   Some shader compilers have changed:
    *   Mixing partially fixed function & partially programmable shaders (e.g. fixed function vertex lighting & pixel shader; or a vertex shader and texture combiners) is not supported anymore. It was never working on mobile, consoles or DirectX 11 anyway. This required changing behaviour of Reflective/VertexLit shader to not do that - it lost per-vertex specular support; on the plus side it now behaves consistently between platforms.
    *   Direct3D 9 shader compiler was switched from Cg 2.2 to HLSL, the same compiler that's used for D3D11. This fixes a bunch of issues where Cg was generating invalid D3D9 shader assembly code; and generally produces slightly more efficient shaders. However, HLSL is slightly more picky about syntax; in general you have to do same shader fixes for D3D9 as for D3D11 now (e.g. UNITY\_INITIALIZE\_OUTPUT for “out” structures).
    *   On desktop OpenGL, shaders are always compiled into GLSL instead of ARB\_vertex/fragment\_program target now. You no longer need to write "#pragma glsl" to get to features like vertex textures or derivative instructions. All support for ARB\_vertex/fragment\_programs is removed.

### Shadows

*   All built-in shadow shaders use backface culling now. Use “two sided” cast shadows option if you do not need backface culling.
*   Shadows on D3D9 require "native shadowmap" support in the driver now (pretty much all systems that can do shadows have that, so this should be fairly invisible). Upside: less shader variants are included into game builds now.
*   Shadows on iOS+GLES2.0 require GL\_EXT\_shadow\_samplers now. This means iPhone4 / iPodTouch4 will not support realtime shadows anymore. Upside: less shader variants and faster shader loading times.
*   Removed screenspace directional light shadow blur (PCF 5x5 is used now).
    *   Removed shadow softness & softness fade from Light.
    *   Normal-based shadow bias defaults to 0.4 for lights now
*   When using oblique camera projection, shadows are disabled now.

### Web Player

*   Removed WWW.LoadUnityWeb API. Load additional unity web file from website script code.
*   Windows Store Apps
*   Removed support for C++ Visual Studio projects.