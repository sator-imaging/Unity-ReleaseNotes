# Unity 3.4

https://unity3d.com/unity/whats-new/unity-3.4

## Graphics

- [Improvements](#improvements)
- [Fixes](#fixes)


### Improvements

*   Anti-aliasing choices now are None, 2x, 4x, 8x (new). Removed 6x and 16x since no GPUs support them.
*   Fixed Camera.RenderToCubemap rendering skybox wrong (unless the camera incidentally had 90 FOV and 1:1 aspect set).
*   Fixed error messages when spotlighs with very small range were used.
*   Better prevention of "out of video memory" situations with crazy high resolutions + MSAA levels. For example, fixes some cases when using 8xMSAA on 2560x1440 screen.
*   Prevent scripts from setting invalid Particle values (Min/Max Size, Min/Max Energy, Min/Max Emission on Emitter; UV Animation on Renderer).
*   Fixed Particle Renderer UV Animation not being updated when changing it from a script.
*   Fixed Particle Renderer sometimes using wrong UV Animation frame when spawning a particle.
*   Per-layer culling distances are properly handled for shadow casters of non-directional lights.
*   Added information for more GPUs to SystemInfo.graphicsPixelFillrate.
*   Fixed Application.CaptureScreenshot() grabbing parts of Game View UI on Windows.
*   Mesh Compression setting was wrongly displayed in the Mesh Inspector.
*   Realtime shadows over single lightmaps no longer incorrectly darken lightmaps brighter than 2.
*   When creating RenderTexture from script it is no longer needed to set isPowerOfTwo; it will be set automatically based on RenderTexture size.
*   Implemented AnimationState.RemoveMixingTransform function.
*   Shadows:
    *   Tweaked shadow related default quality settings.
    *   Shadow Projection is now chosen in Quality Settings (no longer in the Light component).
*   Shaders:
    *   Fixed D3D9 Debug Runtime validation failures on some shaders.
    *   Fixed some bugs in Cg to GLSL cross-compiler.
    *   Multiple objects using a shader with GrabPass can share the same texture, see GrabPass docs.
    *   Added ComputeGrabScreenPos helper function to UnityCG.cginc, for use in shaders with GrabPass.
    *   Added Mobile optimized Diffuse, Bumped, VertexLit (only directional lights), Unlit Lightmap shaders.
*   Lightmaps:
    *   Clearing lightmaps properly resets lightmap tiling/offset on objects, making them batchable again.
    *   Fixed for shaders that do not have \_Color property (like some Mobile shaders).

### Fixes

*   Fixed VRAM amount detection on some Windows Vista/7 systems.
*   Fixed some built-in matrices (\_Object2World etc.) only working in vertex shaders.
*   Fixed camera.RenderToCubemap not working when using deferred lighting (now falls back to forward).
*   Texture scale and translate (name\_ST) properties now work properly even when material's texture is not actually sampled in the shader.
*   Fixed Flares sometimes using wrong UVs in OpenGL ES 2.0.
*   Dynamic batching on normal mapped objects was incorrectly disabled on Direct3D9 (it's still disabled on OpenGL due to driver bugs).
*   Worked around driver performance issue in latest MacBook Pros (with Radeon HD 6xxx) caused by batching.
*   Fixed dynamic batching ending batch too early.
*   Fixed dynamic batching breaking if GUI.DrawTexture was used.
*   Fixed Spot light shadows from large triangles that are partly behind the light.
*   Fixed crash when creating textures with zero length on one side.
*   Lightmaps:
    *   Beast on Mac shouldn't misbehave anymore if objects' transforms contain subnormal floats.
    *   Fixed a lot of bugs with mac/win differences in generated texture uv’s for lightmaps. Please reimport your meshes.
    *   Fixed bug where baking lightmaps would randomly force reimports of 3D models and dirty prefabs.
*   Animation:
    *   Fixed error message when layers and mixing transforms are used.
    *   When you use animation splitting in model@animation file all animations will be attached to the model, not just the main animation.
    *   Fixed dereferencing of null pointer when list of AnimationClips contains null reference.
*   Standard assets:
    *   Added, optimized and improved image effects (e.g. Antialiasing, Fog, TiltShift, Depth of Field).
    *   Added Water4 scripts and example prefabs.
    *   Water: fixed upside down reflections in scene view and game view (windows) and water mesh normals generation.
    *   Image Effects: fixed DLAA corner cases (and added a sharp setting) re-enabled support for additive blending (sun shafts, bloom).
    *   Fixed scripts SmoothFollow and ThirdPersonController.
    *   Depth of field now using more suitable blend modes.
    *   Water got a simpler wave model.
*   Fixes for handhelds:
    *   GLES 2.0: specular is disabled when SeparateSpecular is set to Off.
    *   GLES 1.1: fixed support for anisotropic filtering.
    *   Worked around iPad 2 driver crash on some shaders (mostly ones that involved loops).
    *   Fixed overbright specular highlights on iOS with some shaders.
    *   Worked around iPad 2 driver crash on some shaders (mostly ones that use Fog).
*   Movies:
    *   Time.captureFramerate is respected by movie playback when movie does not have audio.