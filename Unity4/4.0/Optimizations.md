# Unity 4.0
https://unity3d.com/unity/whats-new/unity-4.0

## Optimizations

<ul>
<li>Editor: Optimize Console window memory usage with high log entry counts.</li>
<li>Editor: Optimized Hierarchy View for very large number of root objects.</li>
<li>Editor: Optimized DXT compression of textures; better uses all CPU cores now.</li>
<li>Editor: Detecting if assets need to be reimported when switching platforms is much much faster.</li>
<li>Editor: Made entering playmode faster by reducing the number of domain reloads.</li>
<li>Flash: Made performance improvements when calling functions taking or returning an array of structs.</li>
<li>Flash: Made dramatic memory usage reduction.</li>
<li>Flash: Optimizations were done by recycling actionscript objects for value types such as Vector3, and by being smarter about when to not have to copy them.</li>
<li>Mac OS X: Dynamic geometry optimization via ARB_map_buffer_range &amp; APPLE_flush_buffer_range.</li>
<li>Meshes: Mesh.MarkDynamic; use this for meshes which you modify from scripts a lot.</li>
<li>Mobile: added RenderTexture.DiscardContents - discards previous RT contents via EXT_discard_framebuffer or explicit clear.</li>
<li>Particles: Optimized legacy particle systems via prefetching.</li>
<li>Physics: Physics simulation is now using SSE2 on windows for better performance and to make simulation consistent with Mac OS X.</li>
<li>Rendering: Point &amp; spot lights in forward rendering use scissor rectangle optimization.</li>
<li>Rendering: Unity skips rendering lights that have intensity smaller than 0.01.</li>
<li>Rendering: Optimized Color32 multiplications (particles, lightmapping, …).</li>
<li>Skinned Meshes: Optimized performance &amp; memory usage by keeping static data (UVs &amp; colors) in a separate vertex stream.</li>
<li>Static batching: Compress vertex data to half-precision floats on platforms that support them; and save memory by unloading batched geometry after it's sent to the graphics card.</li>
<li>Static batching: Optimized static batching code.</li>
<li>Threading: Optimized multithreaded job scheduler (used for skinning, Mecanim, Shuriken, shader compilation, texture compression). It “multithreads more efficiently” now.</li>
</ul>
