# Unity 4.2
https://unity3d.com/unity/whats-new/unity-4.2

## Graphics Features

<ul>
<li>Anti-aliased RenderTextures. Implemented on D3D9, D3D11, OpenGL, OpenGL ES 2.0 (iOS and some Android devices via GL_IMG_multisampled_render_to_texture), OpenGL ES 3.0.</li>
<li>Image Effects, a batch of new goodies and improvements (update Image Effects package!) 
<ul>
<li>Ambient Obscurance: Added "Screen Space Ambient Obscurance" effect, like old SSAO but better quality, faster and scales better to large resolutions.</li>
<li>Bloom: Added mobile oriented "Bloom (Optimized)" effect; not as fancy as Bloom one but faster.</li>
<li>Blur: Added mobile oriented "Blur (Optimized)" effect.</li>
<li>Tilt Shift: Replaced old effect with "Tilt Shift (Lens Blur)" one; better quality and HDR support.</li>
<li>Camera Motion Blur: Added "Reconstruction Disc" mode, quality tweaks to existing modes.</li>
<li>Vignetting: Optimized performance and improved UI.</li>
<li>Edge detection: Removed old simple "Edge Detection (Color)" effect, added it as a new mode into Edge Detection effect.</li>
<li>Reorganized image effects menu structure to be more logical.</li>
</ul></li>
<li>Stencil buffer access (requires Unity Pro). Shaders can define stencil buffer operations that they perform, for optimizations or special effects.</li>
<li>Shadows: Implemented static &amp; dynamic batching for shadow casters &amp; shadow collector pass. Note: many shadow casters can be batched even if they use different materials! They will be batched as long as the actual shadow caster shader &amp; material properties affecting it are the same.</li>
<li>Shuriken: Collision event callback scripting interface. Efficient callbacks on GameObjects and ParticleSystems are issued when Shuriken particle collisions occur. Per particle callback data include collision positions, incident velocities, surface normals and Collider references allowing developers to, say, cause + damage to GameObjects and apply forces to RigidBodies.v</li>
<li>GPU Skinning! (requires Unity Pro) 
<ul>
<li>Completely automatic, no custom shaders needed.</li>
<li>Works on DirectX 11 (via stream-out), OpenGL ES 3.0 (via transform feedback) and Xbox 360 (via memexport). Other platforms will continue to use CPU skinning.</li>
</ul></li>
<li>OpenGL ES 3.0 support for Android: 
<ul>
<li>ES3 has nicer shadow filtering, ETC2 texture compression, GPU skinning via transform feedback, HDR rendering, multiple render targets, derivative instructions in shaders etc.</li>
<li>A new option in Player Settings, next to ES1.x and 2.0 devices.</li>
<li>Requires a GPU that can do ES3, for example Qualcomm Adreno 3xx or ARM Mali T6xx.</li>
<li>Note that the official Android version does not support ES3 yet. So to test it you should install ES3 drivers directly from GPU makers (e.g. Qualcomm).</li>
</ul></li>
<li>Deferred Lighting is now enabled on Android and iOS. 
<ul>
<li>Requires depth texture support and at least a 512MB RAM device.</li>
<li>Note, it might still be too slow for big games scenes on anything but latest devices, so use with care.</li>
</ul></li>
<li>Added possibility to create Texture2D directly from native texture; Texture2D.CreateExternalTexture. This is mostly useful when your native code plugin creates textures itself.</li>
</ul>
