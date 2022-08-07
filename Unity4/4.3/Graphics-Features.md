# Unity 4.3
https://unity3d.com/unity/whats-new/unity-4.3

## Graphics Features


### Blendshapes
<ul>
<li>Unity now supports blendshapes (also known as "morph targets").</li>
<li>You can drive the blendshapes using name based binding from Mecanim or legacy animation system.</li>
<li>Blendshape curves are imported from FBX files, but you can also record them in the animation window.</li>
</ul>

### Culling in Unity has been rewritten
<ul>
<li>Now it's much faster across the board. Umbra occlusion culling is used to cull away point lights that don't contribute to the final image; and to drastically reduce number of shadow casters from directional lights.</li>
<li>Umbra: Incremental baking of occlusion culling data.</li>
<li>Umbra: Portal culling occluder rasterization has been greatly optimized.</li>
<li>Umbra: PVS culling has been removed. Occluder rasterization is always used because PVS often gave to inaccurate results and bake times were huge.</li>
<li>Umbra: Directional shadow caster occlusion culling drastically reduces the amount of directional shadow casting objects to be rendered.</li>
<li>Umbra: Point light occlusion culling and connectivity tests are used to remove local lights that do not contribute to the final image.</li>
<li>Vertex point lights that are outside of the frustum are faded out with the range of the light.</li>
<li>General culling performance optimizations, by optimizing data layout, code optimizations etc.</li>
</ul>

### Other graphics features
<ul>
<li>Deferred: A number of light rendering optimizations for deferred rendering, making the light pass faster. Side effect is that only up to 4 bits of the stencil buffer are left available, instead of up to 5.</li>
<li>Render Texture improvements: 
<ul>
<li>Added Camera.SetTargetBuffers for multiple render target (MRT) support.</li>
<li>Ability to render into a specified mip level of a RenderTexture. Create a mipmapped RT, turn off automatic mip generation with RenderTexture. generateMips=false; and use new Graphics.SetRenderTarget overloads to specify mip level to render into.</li>
<li>Ability to render into a speficied cubemap RenderTexture face; new overload in Graphics.SetRenderTarget. Added SystemInfo.supportsRenderToCubemap.</li>
</ul></li>
<li>Graphics: Added Mesh.UploadMeshData, to trigger VBO creation and possibly system-side copy unload.</li>
<li>MaterialPropertyBlock got improved: 
<ul>
<li>Added Renderer.GetPropertyBlock, and MaterialPropertyBlock GetVector,GetFloat etc. functions.</li>
<li>MaterialPropertyBlocks can have texture properties now.</li>
<li>Objects with custom material property blocks (renderer.SetPropertyBlock) can be batched now, if their properties are the same.</li>
</ul></li>
<li>Terrain: Optimized terrain rendering and reduced memory usage.</li>
<li>Android: Enabled multi-threaded rendering on OpenGL ES 2.0 and 3.0. This takes advantage of asynchronous multiprocessing architectures like Qualcomm Snapdragon CPUs and enables more efficient rendering of both OpenGLES 2.0 and 3.0, both currently supported on Adreno GPUs.</li>
<li>Android: ASTC (Adaptive Scalable Texture Compression) format support.</li>
<li>Improved system memory usage of statically batched geometry.</li>
<li>It is now possible to set the fade time on flares. This changes how fast a flare will fade in or out when appearing or disappearing from the screen.</li>
<li>Added Texture2D.LoadRawTextureData for loading already-made (e.g. DXT/PVRTC compressed) raw data.</li>
<li>Allow for overriding Hidden/Internal-Flare, Hidden/Internal-Halo and Hidden/Internal-CombineDepthNormals shaders.</li>
<li>Added Max Particles script binding to Shuriken particle systems.</li>
<li>Dynamic batching support for point, line, and quad mesh topologies.</li>
<li>Added support for some DirectX 11.1 features (low precision shader variables, UAVs in all shader stages, logical blending operations etc.); note this works on DX11.1 runtime only (Windows 8 and up).</li>
<li>Exposed Light.cookieSize to scripts.</li>
</ul>

### Shader related features
<ul>
<li>Material.renderQueue is serialized now. You can change it from custom inspector or script, and it will be saved.</li>
<li>Most of fixed function states (like blend, cull, depth test, stencil modes; polygon offsets etc.) can be driven by material parameters now. For example "Blend [MySrcBlend] [_MyDstBlend]", with _MySrcBlend and _MyDstBlend being float variables. See enums in UnityEngine.Rendering for the mode values. _Note: in this alpha, global shader properties can't drive be used for this.</li>
<li>MaterialPropertyDrawers, just like property drawers, but for shaders and material inspectors! e.g. you can do [MaterialToggle(FANCY_ON)] before a float shader property, and this will display it as a checkbox; and will enable FANCY_ON keyword when checked. </li>
<li>Added "by property ID" functions to set/get material properties; use Shader.PropertyToID to compute ID just once. No need to pass strings all the time.</li>
<li>By enabling SceneFX in the scene view materials in the viewport will update as they would at runtime (taking time into account).</li>
<li>Material inspectors now take time into account. Your materials will update in realtime in the inspector window.</li>
<li>Somewhat more sane error reporting - now gives hints in error messages about #pragma target 3.0 or #pragma glsl, and reports way less almost identical errors when you make typos.</li>
<li>Vertex lit shaders can access all 8 vertex light lights instead of only first 4 in custom shader programs. Also, spot light information (spot direction &amp; spot attenuation) can be accessed.</li>
<li>Added Material.EnableKeyword and DisableKeyword.</li>
<li>Added Material.SetInt/GetInt, and Shader.SetGlobalInt. In ShaderLab Properties block, "Int" can be a property type similar to "Float". Note that all these are just aliases for floats.</li>
<li>Added ShaderUtil.CreateShaderAsset this takes a text shader and returns a compiled shader.</li>
</ul>
