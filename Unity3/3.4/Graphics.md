# Unity 3.4
https://unity3d.com/unity/whats-new/unity-3.4

## Graphics


### Improvements
<ul>
<li>Anti-aliasing choices now are None, 2x, 4x, 8x (new). Removed 6x and 16x since no GPUs support them.</li>
<li>Fixed Camera.RenderToCubemap rendering skybox wrong (unless the camera incidentally had 90 FOV and 1:1 aspect set).</li>
<li>Fixed error messages when spotlighs with very small range were used.</li>
<li>Better prevention of "out of video memory" situations with crazy high resolutions + MSAA levels. For example, fixes some cases when using 8xMSAA on 2560x1440 screen.</li>
<li>Prevent scripts from setting invalid Particle values (Min/Max Size, Min/Max Energy, Min/Max Emission on Emitter; UV Animation on Renderer).</li>
<li>Fixed Particle Renderer UV Animation not being updated when changing it from a script.</li>
<li>Fixed Particle Renderer sometimes using wrong UV Animation frame when spawning a particle.</li>
<li>Per-layer culling distances are properly handled for shadow casters of non-directional lights.</li>
<li>Added information for more GPUs to SystemInfo.graphicsPixelFillrate.</li>
<li>Fixed Application.CaptureScreenshot() grabbing parts of Game View UI on Windows.</li>
<li>Mesh Compression setting was wrongly displayed in the Mesh Inspector.</li>
<li>Realtime shadows over single lightmaps no longer incorrectly darken lightmaps brighter than 2.</li>
<li>When creating RenderTexture from script it is no longer needed to set isPowerOfTwo; it will be set automatically based on RenderTexture size.</li>
<li>Implemented AnimationState.RemoveMixingTransform function.</li>
<li>Shadows: 
<ul>
<li>Tweaked shadow related default quality settings.</li>
<li>Shadow Projection is now chosen in Quality Settings (no longer in the Light component).</li>
</ul></li>
<li>Shaders: 
<ul>
<li>Fixed D3D9 Debug Runtime validation failures on some shaders.</li>
<li>Fixed some bugs in Cg to GLSL cross-compiler.</li>
<li>Multiple objects using a shader with GrabPass can share the same texture, see GrabPass docs.</li>
<li>Added ComputeGrabScreenPos helper function to UnityCG.cginc, for use in shaders with GrabPass.</li>
<li>Added Mobile optimized Diffuse, Bumped, VertexLit (only directional lights), Unlit Lightmap shaders.</li>
</ul></li>
<li>Lightmaps: 
<ul>
<li>Clearing lightmaps properly resets lightmap tiling/offset on objects, making them batchable again.</li>
<li>Fixed for shaders that do not have _Color property (like some Mobile shaders).</li>
</ul></li>
</ul>

### Fixes
<ul>
<li>Fixed VRAM amount detection on some Windows Vista/7 systems.</li>
<li>Fixed some built-in matrices (_Object2World etc.) only working in vertex shaders.</li>
<li>Fixed camera.RenderToCubemap not working when using deferred lighting (now falls back to forward).</li>
<li>Texture scale and translate (name_ST) properties now work properly even when material's texture is not actually sampled in the shader.</li>
<li>Fixed Flares sometimes using wrong UVs in OpenGL ES 2.0.</li>
<li>Dynamic batching on normal mapped objects was incorrectly disabled on Direct3D9 (it's still disabled on OpenGL due to driver bugs).</li>
<li>Worked around driver performance issue in latest MacBook Pros (with Radeon HD 6xxx) caused by batching.</li>
<li>Fixed dynamic batching ending batch too early.</li>
<li>Fixed dynamic batching breaking if GUI.DrawTexture was used.</li>
<li>Fixed Spot light shadows from large triangles that are partly behind the light.</li>
<li>Fixed crash when creating textures with zero length on one side.</li>
<li>Lightmaps: 
<ul>
<li>Beast on Mac shouldn't misbehave anymore if objects' transforms contain subnormal floats.</li>
<li>Fixed a lot of bugs with mac/win differences in generated texture uv’s for lightmaps. Please reimport your meshes.</li>
<li>Fixed bug where baking lightmaps would randomly force reimports of 3D models and dirty prefabs.</li>
</ul></li>
<li>Animation: 
<ul>
<li>Fixed error message when layers and mixing transforms are used.</li>
<li>When you use animation splitting in model@animation file all animations will be attached to the model, not just the main animation.</li>
<li>Fixed dereferencing of null pointer when list of AnimationClips contains null reference.</li>
</ul></li>
<li>Standard assets: 
<ul>
<li>Added, optimized and improved image effects (e.g. Antialiasing, Fog, TiltShift, Depth of Field).</li>
<li>Added Water4 scripts and example prefabs.</li>
<li>Water: fixed upside down reflections in scene view and game view (windows) and water mesh normals generation.</li>
<li>Image Effects: fixed DLAA corner cases (and added a sharp setting) re-enabled support for additive blending (sun shafts, bloom).</li>
<li>Fixed scripts SmoothFollow and ThirdPersonController.</li>
<li>Depth of field now using more suitable blend modes.</li>
<li>Water got a simpler wave model.</li>
</ul></li>
<li>Fixes for handhelds: 
<ul>
<li>GLES 2.0: specular is disabled when SeparateSpecular is set to Off.</li>
<li>GLES 1.1: fixed support for anisotropic filtering.</li>
<li>Worked around iPad 2 driver crash on some shaders (mostly ones that involved loops).</li>
<li>Fixed overbright specular highlights on iOS with some shaders.</li>
<li>Worked around iPad 2 driver crash on some shaders (mostly ones that use Fog).</li>
</ul></li>
<li>Movies: 
<ul>
<li>Time.captureFramerate is respected by movie playback when movie does not have audio.</li>
</ul></li>
</ul>
