# Unity 3.4

https://unity3d.com/unity/whats-new/unity-3.4

## Features



*   Allegorithmic Substance Integration:
    *   Native support for Allegorithmic procedural Substance materials.
    *   Tweak and change exposed substance parameters right inside of Unity.
    *   Change substance parameters at runtime on PC and Mac.
    *   Gain major file size savings due to the compactness of procedural textures on PC and Mac.
    *   Bake substances into regular textures and materials on mobile platforms.
*   Gizmo and Icon Management:
    *   Scene View icons for game objects and script assets can now easily be assigned by using the new Icon Selector opened by clicking on the icon in the Inspector.
    *   Rendering of gizmos and icons can now be controlled using the new 'Gizmos' drop-down window found in the toolbar of the Scene View and the Game View.
    *   Toggling of gizmos is linked to the collapsed or expanded state of the corresponding components, making it simple to only see the gizmos you need.
    *   Support for setting a world size to render all icons with makes it simple to only see nearby icons.
*   Scripting Execution Order:
    *   Unity now gives you explicit control over the execution order in your scripts. Awake, OnEnable and Update calls are sorted by execution order. Execution order can be defined on a ‘per script’ basis in an easy-to-understand dialog.
*   Downloadable content with caching for complete scenes and asset bundles:
    *   Caching now works on all platforms. PC/Mac Standalone players and iOS/Android players have access to a 4 GiB dedicated cache for each application. The webplayer has a 50mb shared cache. A larger application-specific WebPlayer cache can be acquired from Unity Technologies. Caching of course greatly improves loading time not only due to the removed download, but also because the cached files are stored already decompressed on disk. Using the caching feature also greatly reduces memory usage since Unity doens't need to keep any additional data in memory. It is strongly recommended that you always use the caching API for large assets.
    *   A new function BuildPipeline.BuildStreamedSceneAssetBundle makes it easy to create entire scenes and their dependencies into an asset bundle and download them on demand.
    *   Downloading and streaming with the WWW class uses way less memory now. Especially significant when loading from disc using the file:// protocol. You can now load much bigger AssetBundles from disc without running out of memory.
*   Editor:
    *   Debug.DrawLine and Debug.DrawRay now has an optional parameter to control the duration of time a debug line should be rendered.
    *   New mouse event for MonoBehaviour: OnMouseUpAsButton. It is only called when the mouse is released over the same GUIElement or Collider as it was pressed.
    *   New interface for ObjectField that controls if scene objects should be assignable to the object field or not. Old interface marked as obsolete since it allowed invalid references e.g assets with with references to scene objects.
    *   Primitive Colliders can now be modified in Scene View by holding down SHIFT.
    *   The preview in the Inspector is now resizable and no longer part of the scroll-view.
*   Shadows:
    *   Directional Lights got new shadow projection mode, Stable Fit (default for new projects; change in Quality Settings). Old behaviour is Close Fit. Stable Fit results in slightly lower resolution, but shadow boundaries do not shimmer/wobble when rotating the camera.
    *   Much improved shadow caster culling (less draw calls). Better sorting of shadow casters for GPU efficiency.
    *   Added Very High shadow resolution option.
*   Skinning:
    *   SSE2 optimized skinning for Windows & Intel Macs. Improved multithreaded skinning efficiency on Macs.
*   Shaders:
    *   #pragma exclude\_renderers/only\_renderers can now use "shaderonly" (GLES2.0, 360, PS3 etc.) keyword.
    *   tex2Dgrad and tex2Dlod are supported when cross-compiling shaders into GLSL.
    *   Ability to access per-vertex light data in all platforms including OpenGL ES 2.0. Use float4 unity\_LightPosition\[4\], unity\_LightColor\[4\], unity\_LightAtten\[4\].
    *   Added mobile optimized VertexLit and Unlit shaders.
*   Image Effects & Water:
    *   There’s a big upgrade to image effects & water. Both have been optimized for performance and, at the same time, visual quality has been improved. They’re also easier to tweak for artists.
*   Graphics:
    *   Deferred Lighting is able to use Occlusion Culling to cull invisible Point & Spot lights.
    *   Explicit control over VBlank Sync Count allows for more stable framerates. Quality Settings - Framesync flags: 'VBlank Sync Count' can now be set to 'Don't Sync' 'Every VBlank' or 'Every Second VBlank'
    *   Faster Point & Spot light rendering in Deferred Lighting (draws a more compact light shape).
    *   Optimized light culling in Forward rendering.
    *   Optimized per-vertex lighting in GLES 2.0 when fixed function shaders are used.
    *   Added Shader.WarmupAllShaders() to help reduce shader loading related hiccups.
    *   Added support for precomputed bounding volumes for Skinned Mesh Renderer and the animation component. This improves performance and lets you better cull animations & skinned meshes with minimal CPU overhead.
*   iOS:
    *   Added Terrain support for iOS.
    *   Added Gyroscope support.
    *   EAGLView wrapped into UIViewController / iOS native style of autorotation. Also added non-animated autorotation path. Corresponding option added to PlayerSettings.
    *   Added explicit null check option to the AOT code output, which should produce NullReference exceptions without causing SIGABRT in Xcode. Enabled when development player is selected and script debugging enabled.
    *   Improved automatic plugin inclusion for iOS. Now main.mm / AppController.mm could be substituted by the one supplied in Plugins/iOS.
    *   Mobile Quality Settings default to "Simple".
    *   Improved iOS project postprocessing performance. Runtime libs could be symlinked by checking appropriate option in Build Settings panel.
    *   Parallel AOT cross compilation for faster game build times.
    *   iOS SDK selection defaults to "latest".
*   Android:
    *   Terrains are now available on Android.
    *   The new Texture Compression override enables developers to target devices with support for specific GL texture-compression formats. With the new Multiple APK Support in the Android Market it helps to cut the distribution size of the application.
    *   Android now supports AssetBundles built with BuildAdditionalStreamedScenes, to help minimize distribution size and enable streaming of new content from the web.
    *   The mesh animation skinning algorithm now uses multi-threaded processing to harness some of the power of the multi-core CPUs available in new Android devices.
    *   Because a number of critical issues were fixed in this version, we encourage everyone to republish any applications built with previous releases.
*   Unity Xbox 360, PS3 and Wii release in parallel:
    *   All console versions are now released at same time as 3.4. Projects can easily be moved between all platforms.
    *   Rochard, our first PS3 game, has succesfully completed the Sony Submission process.
    *   Our first Xbox 360 game has succesfully passed pre-cert. And will soon go through Submission 1.
    *   First Wii game powered by Unity 3.4 is about to go through lotcheck.