# Unity 5.2

https://unity3d.com/unity/whats-new/unity-5.2

## Features



*   2D: Ability to rotate sprites while Sprite Packing to save atlas space ![description](/sites/default/files/5.2.0-relnotes-sprite-rotation.png)
*   Android: Experimental support for IL2CPP scripting backend
*   Android: Audio - Enable OpenSL fast path for devices that support FEATURE\_AUDIO\_LOW\_LATENCY
*   Android: ETC1 Compression for Sprite Atlases. The texture is split into two RGB parts (second part containing alpha information as a grayscale) and combined in the shader. The option can be set on a per texture level, which affects the final atlas the texture lands in
*   Audio: Ability to set custom rolloff curves for an AudioSource at runtime via script. The following curves will be able to be set at runtime: Volume Rolloff, Spatial Blend (2D / 3D), Reverb Zone Mix, Spread, LowPass Filter Cutoff Frequency
*   Audio: Spatialization API for audio plugins, see (SDK and example)\[https://bitbucket.org/Unity-Technologies/nativeaudioplugins\]

*   Cloud Services: Access control list support
*   Core: Application.UnloadLevel. Unloading scenes is now possible while the game is running. References to lightmaps are cleared but you have to call Resources.UnloadUnusedAssets() to actually unload them. Enlighten data is unloaded immediately. This feature is especially useful in conjunction with Lightmapping.BakeMultipleLevels()
*   Graphics: Added CullingGroup API, which allows you to specify a large set of bounding spheres that are integrated into the culling pipeline and subjected to frustum and occlusion culling
*   Graphics: Added option in player settings for configurable vertex compression. Default values: position and UV1 is uncompressed, the rest of the channels are compressed ![description](/sites/default/files/5.2.0-relnotes-vertex-compression.png)
    
*   Mecanim: Playable API. Supports creating Animation blending graphs at runtime, providing the capacity to have full control over the AnimationClips and AnimationControllers played by the engine.
    
*   Mecanim: 3ds Max Auto Mapping and T-Pose. When setting an Avatar Animation Type to Humanoid, the Auto-Configure will try to detect if it is a Biped. If the hierarchy and naming of Biped is found, then default mapping and t-pose for biped will be used. Translation DoF will also be automatically activated for that avatar. The avatar can still be re-configured from this point, but usually default Biped mapping, t-pose and translation DoF will give the best results. Note that only Bipeds with no “Triangle Pelvis” and using default naming are supported
*   Mecanim: Translation DoF for Humanoid. Some animation files come with translation animation on humanoid bones. For example, it is the case with 3ds Max Biped that comes with translation on 1st Spine bone. Translation DoF can be activated on those humanoid avatar to convert translation animation to retargetable translation DoFs. Translation DoF affects Spine, Shoulders, Upper Legs and Neck bones. Translation DoFs usually represent small amount of translation that improves retargeting quality. Translation DoF may also be used to improve retargeting quality when animation has more than two animated spine bones. Translation DoF can be activated in Muscle & Setting tab of Humanoid configure window ![description](/sites/default/files/5.2.0-relnotes-mecanim-translation-humanoid.png)
    
*   Multi Scene Lighting baking. Lightmapping.BakeMultipleScenes lets you bake lightmaps, reflection probes and realtime lightmaps for multiple scenes together, which can be loaded additively. Data is automatically split on bake per scene
    
*   Plugins: Expanded low-level graphics plugin API
*   Out of the box support for VisualStudio Tools for Unity (aka UnityVS)
*   Performance: CPU side rendering performance optimizations across the board. We've seen between 5% and 30% lower CPU cost for rendering, depending on the setup. Sorting of the renderable objects is now multithreaded too

*   Performance: Improved performance of LoadAssetAsync. Allow multiple AsyncOperations to be completed in a single frame
*   Performance: Particle rendering optimizations (especially for VR), with speed improvements varying from 15% to 50% depending on geometry type
*   Performance: Rendering on Linux uses the same main+render thread setup as on other platforms
*   Performance: UI now uses multithreaded batching & geometry generation backend. This leads to a performance increase of up 4x in our stress test scenes
*   Physics: Added parameter QueryTriggerInteraction to all physics queries (raycast, spherecast, overlap) to allow any query to override whether or not the query should hit Triggers
*   Physics: Expose CharacterController.skinWidth parameter to scripts
*   Physics: Expose impulse applied at contact (see Collision.impulse)
*   Physics: Support scaling of vehicles
*   Shaders: Fixed Function shaders work on all platforms now (including consoles). They are always generated at shader import time (a button "show generated code" in shader inspector shows the code); removed all runtime support. All rendering got slightly faster (even when not using fixed function shaders); and executable sizes got slightly smaller. MaterialPropertyBlocks work with them now (which means Sprites and animated materials work too). Behave more consistently across platforms (specular highlights and light attenuation was slightly different before). Fixed function shaders aren't rasterized at a half-pixel shift on WP8 anymore. However, can not create fixed function shaders using "new Material(string)" at runtime anymore; see Changes section
*   UI: 2D Rect Mask. A mask for 2D UI elements. Performs faster than the previous stencil buffer mask and does not require additional draw calls to prime the stencil buffer. When an element is outside the bounds of the mask the canvas renderer is also culled which leads to faster batching performance
*   UI: Dropdown control. The Dropdown can be used to let the user choose a single option from a list of options. ![description](/sites/default/files/5.2.0-relnotes-ui-dropdown.png)
    
*   UI: New Scroll View menu item and improved support in ScrollRect component for scrollbars.
    
*   Unity Ads: Enable and configure Ads from the Unity Connect window in the Editor
*   WebGL: allow .jspre files to be added to the project to be prefixed to the generated JavaScript
*   WebGL: Experimental support for WebGL 2.0 (not yet supported in any released browser)
*   Windows Store Apps: Universal Windows Platform app (Windows 10) support