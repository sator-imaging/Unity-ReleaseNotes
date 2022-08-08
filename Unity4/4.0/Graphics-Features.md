# Unity 4.0

https://unity3d.com/unity/whats-new/unity-4.0

## Graphics Features



*   Terrain: Normal map & custom shader support for Terrain. Added built-in shader Nature/Terrain/Bumped Specular; added "normal map" texture slot to terrain splat maps; added Material field under terrain settings.
*   3D (volume) textures support. Currently no way to import them, but you can create them from script (Texture3D) and use them in shaders (sampler3D and tex3D). Also SystemInfo.supports3DTextures.
*   Shadows on mobile devices!
    *   Only directional lights, no shadow cascades, no soft shadows.
    *   Requires GL\_OES\_depth\_texture extension. Most notably, Tegra 2/3-based devices do not support it.
    *   On Android, requires Honeycomb of later OS.
*   Fonts:
    *   Dynamic font rendering on all platforms (including mobiles) with identical results (via FreeType).
    *   Simple html-style text markup support to have multiple font sizes, styles and colors in a string in UnityGUI, GUIText & TextMesh.
*   Image Effects updates:
    *   Depth of Field (Scatter), an improved version of existing Depth of Field 3.4 effect. Has a DX11 mode that splats bokeh sprites on the bright spots.
    *   Camera Motion Blur, does what it says: camera motion based motion blur. Has DX11-optimized mode for better quality.
    *   Noise and Grain does a fancier film noise simulation (also has a DX11-optimized mode).
    *   Bloom, an improved version of Bloom and Lens Flares. New "High Quality" mode simulates aberration, glint, better treatment of high frequency parts.
    *   Color Correction LUT effect that uses a 3D texture to do arbitrary color correction.
    *   Edge Detection (Geometry) effect got ability to interact nicely with other depth-based effects (DOF, Motion Blur etc.) with new "Sobel Depth Thin" mode.
    *   Color Correction Curves now supports (de)saturation and has a fix for color key correction.
*   Cubemaps:
    *   New Generate Cubemap texture import option that creates a cubemap from vertical/horizontal cross or row/column of images.
    *   Seamless cubemap option that makes sure edges of faces match up. Also runtime scripting API, Cubemap.SmoothEdges.
    *   Cubemap assets reference their original textures in the editor instead of copying their pixels at assign time.
*   Lightmapping: "Bake selected" no longer destroys lightmaps on objects that aren't selected. Instead it updates lightmaps on selected objects, as expected.
*   Lightmapping: Normalmaps are taken into account when lightmapping, which allows to add detail to lightmaps and makes the transition between near and far distance in Dual Lightmaps mode less visible.
*   Lightmapping: FIxed issue with generated lightmap uvs being different across mac/win on some occasions.
*   Render Textures: added RenderTextureFormat.ARGBFloat, RGFloat, RGHalf, RFloat, RHalf formats.
*   Meshes can have a non-triangle topology now. You can create meshes that are lines, points or quads from scripts. See MeshTopology enum, Mesh.GetIndices, SetIndices, GetTopology.
*   Added SkinnedMeshRenderer.BakeMesh to "bake" skinned mesh result into a regular mesh. You can use this to implement semi-instanced crowd rendering schemes.
*   Graphics: Added resizable window support for standalone builds; see Resizable Window option in player settings.
*   LOD: Add an API that allows for the construction / configuration of LODs at runtime. You can now add a LODGroup and configure it without using the UI.
*   Shuriken particle system:
    *   World collision support - world collisions can be high/medium/low quality. High quality raycasts all particles and is expensive. Medium/low quality traces some of the particles, while the rest reuses older collisions. While this is approximate, in many cases where there are a lot of particles it will look fine and perform very well. The ray casting budget is set in quality settings.
    *   Automatic simulation culling support. Particle systems will only update when visible. When it is not possible to support this automatically, Shuriken shows why directly inside the UI.
    *   External forces support - use Wind Zones with particles.
    *   Bent normals support for sprites.
    *   Support for sorting and rendering with immediate children (solving sorting issues for combined systems).
*   Shaders:
    *   Added built-in matrix variables, UNITY\_MATRIX\_V (view matrix), UNITY\_MATRIX\_VP (view\*projection).
    *   Added float4 unity\_DeltaTime, contains (dt, 1/dt, smoothdt, 1/smoothdt).
    *   Shader helper macros added:
        *   UNITY\_DECLARE\_SHADOWMAP(tex), UNITY\_SAMPLE\_SHADOW(tex,uv), UNITY\_SAMPLE\_SHADOW\_PROJ(tex,uv).
        *   UNITY\_NEAR\_CLIP\_VALUE, defined to 0.0 on D3D-like, -1.0 on GL-like platforms.
        *   UNITY\_COMPILER\_HLSL (d3d11, 360), UNITY\_COMPILER\_HLSL2GLSL (gles), UNITY\_COMPILER\_CG if you need to determine which shader compiler is used on a platform.
        *   UNITY\_INITIALIZE\_OUTPUT(type,name) to help with DX11 shader compiler requiring full initialization of "out" parameters.
    *   OpenGL ES 2.0: Supports depth textures on Android.
    *   Scripting API: added Texture.SetGlobalAnisotropicFilteringLimits.