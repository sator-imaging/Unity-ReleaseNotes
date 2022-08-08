# Unity 4.3

https://unity3d.com/unity/whats-new/unity-4.3

## Graphics Features

- [Blendshapes](#blendshapes)
- [Culling in Unity has been rewritten](#culling-in-unity-has-been-rewritten)
- [Other graphics features](#other-graphics-features)
- [Shader related features](#shader-related-features)


### Blendshapes

*   Unity now supports blendshapes (also known as "morph targets").
*   You can drive the blendshapes using name based binding from Mecanim or legacy animation system.
*   Blendshape curves are imported from FBX files, but you can also record them in the animation window.

### Culling in Unity has been rewritten

*   Now it's much faster across the board. Umbra occlusion culling is used to cull away point lights that don't contribute to the final image; and to drastically reduce number of shadow casters from directional lights.
*   Umbra: Incremental baking of occlusion culling data.
*   Umbra: Portal culling occluder rasterization has been greatly optimized.
*   Umbra: PVS culling has been removed. Occluder rasterization is always used because PVS often gave to inaccurate results and bake times were huge.
*   Umbra: Directional shadow caster occlusion culling drastically reduces the amount of directional shadow casting objects to be rendered.
*   Umbra: Point light occlusion culling and connectivity tests are used to remove local lights that do not contribute to the final image.
*   Vertex point lights that are outside of the frustum are faded out with the range of the light.
*   General culling performance optimizations, by optimizing data layout, code optimizations etc.

### Other graphics features

*   Deferred: A number of light rendering optimizations for deferred rendering, making the light pass faster. Side effect is that only up to 4 bits of the stencil buffer are left available, instead of up to 5.
*   Render Texture improvements:
    *   Added Camera.SetTargetBuffers for multiple render target (MRT) support.
    *   Ability to render into a specified mip level of a RenderTexture. Create a mipmapped RT, turn off automatic mip generation with RenderTexture. generateMips=false; and use new Graphics.SetRenderTarget overloads to specify mip level to render into.
    *   Ability to render into a speficied cubemap RenderTexture face; new overload in Graphics.SetRenderTarget. Added SystemInfo.supportsRenderToCubemap.
*   Graphics: Added Mesh.UploadMeshData, to trigger VBO creation and possibly system-side copy unload.
*   MaterialPropertyBlock got improved:
    *   Added Renderer.GetPropertyBlock, and MaterialPropertyBlock GetVector,GetFloat etc. functions.
    *   MaterialPropertyBlocks can have texture properties now.
    *   Objects with custom material property blocks (renderer.SetPropertyBlock) can be batched now, if their properties are the same.
*   Terrain: Optimized terrain rendering and reduced memory usage.
*   Android: Enabled multi-threaded rendering on OpenGL ES 2.0 and 3.0. This takes advantage of asynchronous multiprocessing architectures like Qualcomm Snapdragon CPUs and enables more efficient rendering of both OpenGLES 2.0 and 3.0, both currently supported on Adreno GPUs.
*   Android: ASTC (Adaptive Scalable Texture Compression) format support.
*   Improved system memory usage of statically batched geometry.
*   It is now possible to set the fade time on flares. This changes how fast a flare will fade in or out when appearing or disappearing from the screen.
*   Added Texture2D.LoadRawTextureData for loading already-made (e.g. DXT/PVRTC compressed) raw data.
*   Allow for overriding Hidden/Internal-Flare, Hidden/Internal-Halo and Hidden/Internal-CombineDepthNormals shaders.
*   Added Max Particles script binding to Shuriken particle systems.
*   Dynamic batching support for point, line, and quad mesh topologies.
*   Added support for some DirectX 11.1 features (low precision shader variables, UAVs in all shader stages, logical blending operations etc.); note this works on DX11.1 runtime only (Windows 8 and up).
*   Exposed Light.cookieSize to scripts.

### Shader related features

*   Material.renderQueue is serialized now. You can change it from custom inspector or script, and it will be saved.
*   Most of fixed function states (like blend, cull, depth test, stencil modes; polygon offsets etc.) can be driven by material parameters now. For example "Blend \[MySrcBlend\] \[\_MyDstBlend\]", with \_MySrcBlend and \_MyDstBlend being float variables. See enums in UnityEngine.Rendering for the mode values. \_Note: in this alpha, global shader properties can't drive be used for this.
*   MaterialPropertyDrawers, just like property drawers, but for shaders and material inspectors! e.g. you can do \[MaterialToggle(FANCY\_ON)\] before a float shader property, and this will display it as a checkbox; and will enable FANCY\_ON keyword when checked.
*   Added "by property ID" functions to set/get material properties; use Shader.PropertyToID to compute ID just once. No need to pass strings all the time.
*   By enabling SceneFX in the scene view materials in the viewport will update as they would at runtime (taking time into account).
*   Material inspectors now take time into account. Your materials will update in realtime in the inspector window.
*   Somewhat more sane error reporting - now gives hints in error messages about #pragma target 3.0 or #pragma glsl, and reports way less almost identical errors when you make typos.
*   Vertex lit shaders can access all 8 vertex light lights instead of only first 4 in custom shader programs. Also, spot light information (spot direction & spot attenuation) can be accessed.
*   Added Material.EnableKeyword and DisableKeyword.
*   Added Material.SetInt/GetInt, and Shader.SetGlobalInt. In ShaderLab Properties block, "Int" can be a property type similar to "Float". Note that all these are just aliases for floats.
*   Added ShaderUtil.CreateShaderAsset this takes a text shader and returns a compiled shader.