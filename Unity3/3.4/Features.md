# Unity 3.4
https://unity3d.com/unity/whats-new/unity-3.4

## Features

<ul>
<li>Allegorithmic Substance Integration: 
<ul>
<li>Native support for Allegorithmic procedural Substance materials.</li>
<li>Tweak and change exposed substance parameters right inside of Unity.</li>
<li>Change substance parameters at runtime on PC and Mac.</li>
<li>Gain major file size savings due to the compactness of procedural textures on PC and Mac.</li>
<li>Bake substances into regular textures and materials on mobile platforms.</li>
</ul></li>
<li>Gizmo and Icon Management: 
<ul>
<li>Scene View icons for game objects and script assets can now easily be assigned by using the new Icon Selector opened by clicking on the icon in the Inspector.</li>
<li>Rendering of gizmos and icons can now be controlled using the new 'Gizmos' drop-down window found in the toolbar of the Scene View and the Game View.</li>
<li>Toggling of gizmos is linked to the collapsed or expanded state of the corresponding components, making it simple to only see the gizmos you need.</li>
<li>Support for setting a world size to render all icons with makes it simple to only see nearby icons.</li>
</ul></li>
<li>Scripting Execution Order: 
<ul>
<li>Unity now gives you explicit control over the execution order in your scripts. Awake, OnEnable and Update calls are sorted by execution order. Execution order can be defined on a ‘per script’ basis in an easy-to-understand dialog.</li>
</ul></li>
<li>Downloadable content with caching for complete scenes and asset bundles: 
<ul>
<li>Caching now works on all platforms. PC/Mac Standalone players and iOS/Android players have access to a 4 GiB dedicated cache for each application. The webplayer has a 50mb shared cache. A larger application-specific WebPlayer cache can be acquired from Unity Technologies. Caching of course greatly improves loading time not only due to the removed download, but also because the cached files are stored already decompressed on disk. Using the caching feature also greatly reduces memory usage since Unity doens't need to keep any additional data in memory. It is strongly recommended that you always use the caching API for large assets.</li>
<li>A new function BuildPipeline.BuildStreamedSceneAssetBundle makes it easy to create entire scenes and their dependencies into an asset bundle and download them on demand.</li>
<li>Downloading and streaming with the WWW class uses way less memory now. Especially significant when loading from disc using the file:// protocol. You can now load much bigger AssetBundles from disc without running out of memory.</li>
</ul></li>
<li>Editor: 
<ul>
<li>Debug.DrawLine and Debug.DrawRay now has an optional parameter to control the duration of time a debug line should be rendered.</li>
<li>New mouse event for MonoBehaviour: OnMouseUpAsButton. It is only called when the mouse is released over the same GUIElement or Collider as it was pressed.</li>
<li>New interface for ObjectField that controls if scene objects should be assignable to the object field or not. Old interface marked as obsolete since it allowed invalid references e.g assets with with references to scene objects.</li>
<li>Primitive Colliders can now be modified in Scene View by holding down SHIFT.</li>
<li>The preview in the Inspector is now resizable and no longer part of the scroll-view.</li>
</ul></li>
<li>Shadows: 
<ul>
<li>Directional Lights got new shadow projection mode, Stable Fit (default for new projects; change in Quality Settings). Old behaviour is Close Fit. Stable Fit results in slightly lower resolution, but shadow boundaries do not shimmer/wobble when rotating the camera.</li>
<li>Much improved shadow caster culling (less draw calls). Better sorting of shadow casters for GPU efficiency.</li>
<li>Added Very High shadow resolution option.</li>
</ul></li>
<li>Skinning: 
<ul>
<li>SSE2 optimized skinning for Windows &amp; Intel Macs. Improved multithreaded skinning efficiency on Macs.</li>
</ul></li>
<li>Shaders: 
<ul>
<li>#pragma exclude_renderers/only_renderers can now use "shaderonly" (GLES2.0, 360, PS3 etc.) keyword.</li>
<li>tex2Dgrad and tex2Dlod are supported when cross-compiling shaders into GLSL.</li>
<li>Ability to access per-vertex light data in all platforms including OpenGL ES 2.0. Use float4 unity_LightPosition[4], unity_LightColor[4], unity_LightAtten[4].</li>
<li>Added mobile optimized VertexLit and Unlit shaders.</li>
</ul></li>
<li>Image Effects &amp; Water: 
<ul>
<li>There’s a big upgrade to image effects &amp; water. Both have been optimized for performance and, at the same time, visual quality has been improved. They’re also easier to tweak for artists.</li>
</ul></li>
<li>Graphics: 
<ul>
<li>Deferred Lighting is able to use Occlusion Culling to cull invisible Point &amp; Spot lights.</li>
<li>Explicit control over VBlank Sync Count allows for more stable framerates. Quality Settings - Framesync flags: 'VBlank Sync Count' can now be set to 'Don't Sync' 'Every VBlank' or 'Every Second VBlank'</li>
<li>Faster Point &amp; Spot light rendering in Deferred Lighting (draws a more compact light shape).</li>
<li>Optimized light culling in Forward rendering.</li>
<li>Optimized per-vertex lighting in GLES 2.0 when fixed function shaders are used.</li>
<li>Added Shader.WarmupAllShaders() to help reduce shader loading related hiccups.</li>
<li>Added support for precomputed bounding volumes for Skinned Mesh Renderer and the animation component. This improves performance and lets you better cull animations &amp; skinned meshes with minimal CPU overhead.</li>
</ul></li>
<li>iOS: 
<ul>
<li>Added Terrain support for iOS.</li>
<li>Added Gyroscope support.</li>
<li>EAGLView wrapped into UIViewController / iOS native style of autorotation. Also added non-animated autorotation path. Corresponding option added to PlayerSettings.</li>
<li>Added explicit null check option to the AOT code output, which should produce NullReference exceptions without causing SIGABRT in Xcode. Enabled when development player is selected and script debugging enabled.</li>
<li>Improved automatic plugin inclusion for iOS. Now main.mm / AppController.mm could be substituted by the one supplied in Plugins/iOS.</li>
<li>Mobile Quality Settings default to "Simple".</li>
<li>Improved iOS project postprocessing performance. Runtime libs could be symlinked by checking appropriate option in Build Settings panel.</li>
<li>Parallel AOT cross compilation for faster game build times.</li>
<li>iOS SDK selection defaults to "latest".</li>
</ul></li>
<li>Android: 
<ul>
<li>Terrains are now available on Android.</li>
<li>The new Texture Compression override enables developers to target devices with support for specific GL texture-compression formats. With the new Multiple APK Support in the Android Market it helps to cut the distribution size of the application.</li>
<li>Android now supports AssetBundles built with BuildAdditionalStreamedScenes, to help minimize distribution size and enable streaming of new content from the web.</li>
<li>The mesh animation skinning algorithm now uses multi-threaded processing to harness some of the power of the multi-core CPUs available in new Android devices.</li>
<li>Because a number of critical issues were fixed in this version, we encourage everyone to republish any applications built with previous releases.</li>
</ul></li>
<li>Unity Xbox 360, PS3 and Wii release in parallel: 
<ul>
<li>All console versions are now released at same time as 3.4. Projects can easily be moved between all platforms.</li>
<li>Rochard, our first PS3 game, has succesfully completed the Sony Submission process.</li>
<li>Our first Xbox 360 game has succesfully passed pre-cert. And will soon go through Submission 1.</li>
<li>First Wii game powered by Unity 3.4 is about to go through lotcheck.</li>
</ul></li>
</ul>
