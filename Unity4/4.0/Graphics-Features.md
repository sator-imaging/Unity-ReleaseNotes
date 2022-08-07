# Unity 4.0
https://unity3d.com/unity/whats-new/unity-4.0

## Graphics Features

<ul>
<li>Terrain: Normal map &amp; custom shader support for Terrain. Added built-in shader Nature/Terrain/Bumped Specular; added "normal map" texture slot to terrain splat maps; added Material field under terrain settings.</li>
<li>3D (volume) textures support. Currently no way to import them, but you can create them from script (Texture3D) and use them in shaders (sampler3D and tex3D). Also SystemInfo.supports3DTextures.</li>
<li>Shadows on mobile devices! 
<ul>
<li>Only directional lights, no shadow cascades, no soft shadows.</li>
<li>Requires GL_OES_depth_texture extension. Most notably, Tegra 2/3-based devices do not support it.</li>
<li>On Android, requires Honeycomb of later OS.</li>
</ul></li>
<li>Fonts: 
<ul>
<li>Dynamic font rendering on all platforms (including mobiles) with identical results (via FreeType).</li>
<li>Simple html-style text markup support to have multiple font sizes, styles and colors in a string in UnityGUI, GUIText &amp; TextMesh.</li>
</ul></li>
<li>Image Effects updates: 
<ul>
<li>Depth of Field (Scatter), an improved version of existing Depth of Field 3.4 effect. Has a DX11 mode that splats bokeh sprites on the bright spots.</li>
<li>Camera Motion Blur, does what it says: camera motion based motion blur. Has DX11-optimized mode for better quality.</li>
<li>Noise and Grain does a fancier film noise simulation (also has a DX11-optimized mode).</li>
<li>Bloom, an improved version of Bloom and Lens Flares. New "High Quality" mode simulates aberration, glint, better treatment of high frequency parts.</li>
<li>Color Correction LUT effect that uses a 3D texture to do arbitrary color correction.</li>
<li>Edge Detection (Geometry) effect got ability to interact nicely with other depth-based effects (DOF, Motion Blur etc.) with new "Sobel Depth Thin" mode.</li>
<li>Color Correction Curves now supports (de)saturation and has a fix for color key correction.</li>
</ul></li>
<li>Cubemaps: 
<ul>
<li>New Generate Cubemap texture import option that creates a cubemap from vertical/horizontal cross or row/column of images.</li>
<li>Seamless cubemap option that makes sure edges of faces match up. Also runtime scripting API, Cubemap.SmoothEdges.</li>
<li>Cubemap assets reference their original textures in the editor instead of copying their pixels at assign time.</li>
</ul></li>
<li>Lightmapping: "Bake selected" no longer destroys lightmaps on objects that aren't selected. Instead it updates lightmaps on selected objects, as expected.</li>
<li>Lightmapping: Normalmaps are taken into account when lightmapping, which allows to add detail to lightmaps and makes the transition between near and far distance in Dual Lightmaps mode less visible.</li>
<li>Lightmapping: FIxed issue with generated lightmap uvs being different across mac/win on some occasions.</li>
<li>Render Textures: added RenderTextureFormat.ARGBFloat, RGFloat, RGHalf, RFloat, RHalf formats.</li>
<li>Meshes can have a non-triangle topology now. You can create meshes that are lines, points or quads from scripts. See MeshTopology enum, Mesh.GetIndices, SetIndices, GetTopology.</li>
<li>Added SkinnedMeshRenderer.BakeMesh to "bake" skinned mesh result into a regular mesh. You can use this to implement semi-instanced crowd rendering schemes.</li>
<li>Graphics: Added resizable window support for standalone builds; see Resizable Window option in player settings.</li>
<li>LOD: Add an API that allows for the construction / configuration of LODs at runtime. You can now add a LODGroup and configure it without using the UI.</li>
<li>Shuriken particle system: 
<ul>
<li>World collision support - world collisions can be high/medium/low quality. High quality raycasts all particles and is expensive. Medium/low quality traces some of the particles, while the rest reuses older collisions. While this is approximate, in many cases where there are a lot of particles it will look fine and perform very well. The ray casting budget is set in quality settings.</li>
<li>Automatic simulation culling support. Particle systems will only update when visible. When it is not possible to support this automatically, Shuriken shows why directly inside the UI.</li>
<li>External forces support - use Wind Zones with particles.</li>
<li>Bent normals support for sprites.</li>
<li>Support for sorting and rendering with immediate children (solving sorting issues for combined systems).</li>
</ul></li>
<li>Shaders: 
<ul>
<li>Added built-in matrix variables, UNITY_MATRIX_V (view matrix), UNITY_MATRIX_VP (view*projection).</li>
<li>Added float4 unity_DeltaTime, contains (dt, 1/dt, smoothdt, 1/smoothdt).</li>
<li>Shader helper macros added:

<ul>
<li>UNITY_DECLARE_SHADOWMAP(tex), UNITY_SAMPLE_SHADOW(tex,uv), UNITY_SAMPLE_SHADOW_PROJ(tex,uv).</li>
<li>UNITY_NEAR_CLIP_VALUE, defined to 0.0 on D3D-like, -1.0 on GL-like platforms.</li>
<li>UNITY_COMPILER_HLSL (d3d11, 360), UNITY_COMPILER_HLSL2GLSL (gles), UNITY_COMPILER_CG if you need to determine which shader compiler is used on a platform.</li>
<li>UNITY_INITIALIZE_OUTPUT(type,name) to help with DX11 shader compiler requiring full initialization of "out" parameters.</li>
</ul></li>
<li>OpenGL ES 2.0: Supports depth textures on Android.</li>
<li>Scripting API: added Texture.SetGlobalAnisotropicFilteringLimits.</li>
</ul></li>
</ul>
