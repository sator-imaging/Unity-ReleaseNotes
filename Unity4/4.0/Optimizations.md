# Unity 4.0

https://unity3d.com/unity/whats-new/unity-4.0

## Optimizations



*   Editor: Optimize Console window memory usage with high log entry counts.
*   Editor: Optimized Hierarchy View for very large number of root objects.
*   Editor: Optimized DXT compression of textures; better uses all CPU cores now.
*   Editor: Detecting if assets need to be reimported when switching platforms is much much faster.
*   Editor: Made entering playmode faster by reducing the number of domain reloads.
*   Flash: Made performance improvements when calling functions taking or returning an array of structs.
*   Flash: Made dramatic memory usage reduction.
*   Flash: Optimizations were done by recycling actionscript objects for value types such as Vector3, and by being smarter about when to not have to copy them.
*   Mac OS X: Dynamic geometry optimization via ARB\_map\_buffer\_range & APPLE\_flush\_buffer\_range.
*   Meshes: Mesh.MarkDynamic; use this for meshes which you modify from scripts a lot.
*   Mobile: added RenderTexture.DiscardContents - discards previous RT contents via EXT\_discard\_framebuffer or explicit clear.
*   Particles: Optimized legacy particle systems via prefetching.
*   Physics: Physics simulation is now using SSE2 on windows for better performance and to make simulation consistent with Mac OS X.
*   Rendering: Point & spot lights in forward rendering use scissor rectangle optimization.
*   Rendering: Unity skips rendering lights that have intensity smaller than 0.01.
*   Rendering: Optimized Color32 multiplications (particles, lightmapping, …).
*   Skinned Meshes: Optimized performance & memory usage by keeping static data (UVs & colors) in a separate vertex stream.
*   Static batching: Compress vertex data to half-precision floats on platforms that support them; and save memory by unloading batched geometry after it's sent to the graphics card.
*   Static batching: Optimized static batching code.
*   Threading: Optimized multithreaded job scheduler (used for skinning, Mecanim, Shuriken, shader compilation, texture compression). It “multithreads more efficiently” now.