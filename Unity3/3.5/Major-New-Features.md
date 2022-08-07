# Unity 3.5
https://unity3d.com/unity/whats-new/unity-3.5

## Major New Features

<ul>
<li>Adobe Flash: Final version of 3.5 supports a preview of publishing to Adobe SWF format, otherwise known as Flash Export. 
<ul>
<li>A separate FAQ for this release is available at <a href="/unity/publishing/flash">https://unity3d.com/unity/publishing/flash</a>.</li>
</ul></li>
<li>New Particle System - "Shuriken". 
<ul>
<li>Edit, view and playback control in Edit Mode. You can manually scrub time to inspect and fine-tune the particle system using the Scene View playback controls.</li>
<li>Module-based: Each particle system has several modules that can be enabled to control color, size and movement of particles.</li>
<li>Groupable: It is possible to group / compose several particle systems in a hierarchy and their playback will behave as one particle system.</li>
<li>Built-in curve editor for easy curve editing.</li>
</ul></li>
<li>Pathfinding and avoidance sub-system added. 
<ul>
<li>NavMesh: Path-finding API. Bake navigation mesh with markup areas.</li>
<li>NavMeshAgent: Character navigation. Avoidance system.</li>
<li>OffmeshLink: used to create arbitrary connections between NavMesh polygons.</li>
</ul></li>
<li>Built-in LOD management via LOD Groups. 
<ul>
<li>Lightmap baking works for LODed models. The lightmapped objects use a surface transfer algorithm similar to normal map baking.</li>
</ul></li>
<li>Asset Cache server. 
<ul>
<li>Assets imports are shared between project folders and users. Switching Platform takes minutes instead of hours on large scale projects. Grabbing changes from other team members is almost instant.</li>
</ul></li>
<li>Built-in HDR support and adaptive tonemapping. 
<ul>
<li>The 3.5 image effects package comes with adaptive tonemapping, bloom and depth of field image effects that are optimized for HDR.</li>
</ul></li>
<li>Multithreaded rendering. 
<ul>
<li>Most of rendering &amp; driver overhead is put onto another CPU core on multicore systems.</li>
<li>You don't have to do anything, it just works!</li>
<li>Currently only on PC / Mac / Xbox 360; and not in the web player yet.</li>
</ul></li>
<li>Light Probes, which allow for using baked lighting on characters and other dynamic objects.</li>
<li>Directional Lightmaps.</li>
<li>Generic external version control (.meta files) is now available in the free version.</li>
<li>Google Native Client is now supported</li>
<li>It is now possible to select and edit multiple objects simultaneously with the Inspector! 
<ul>
<li>The Inspector preview supports showing the multiple selected objects.</li>
<li>Multi-editing can be enabled for custom editors with a single line of code if they are based on using SerializedProperty.</li>
</ul></li>
<li>Occlusion Culling has been rewritten from scratch, it is much faster to compute and always correct 
<ul>
<li>OcclusionPortal component has been added to allow doors that can be opened and closed at runtime.</li>
<li>Terrains work well with occlusion culling now.</li>
<li>The default mode for occlusion culling is “automatic portal generation”, which is very accurate and works well for dynamic objects.</li>
<li>Introduced the “Occludee Static” flag. This is used to mark objects as statically occludable without making them occluders. For example transparent objects that don't move should be marked as Occludee Static.</li>
</ul></li>
<li>Text-based scene and prefab format can be used for improving team workflows. This can be turned on or off in the Editor Settings for each project.</li>
<li>GPU Profiler: added the ability to see GPU usage to the profiler.</li>
<li>A ton of memory and performance optimizations. Several improvements to multithreading.</li>
</ul>
