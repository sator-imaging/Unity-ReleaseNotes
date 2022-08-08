# Unity 3.5

https://unity3d.com/unity/whats-new/unity-3.5

## Major New Features



*   Adobe Flash: Final version of 3.5 supports a preview of publishing to Adobe SWF format, otherwise known as Flash Export.
    *   A separate FAQ for this release is available at [https://unity3d.com/unity/publishing/flash](/unity/publishing/flash).
*   New Particle System - "Shuriken".
    *   Edit, view and playback control in Edit Mode. You can manually scrub time to inspect and fine-tune the particle system using the Scene View playback controls.
    *   Module-based: Each particle system has several modules that can be enabled to control color, size and movement of particles.
    *   Groupable: It is possible to group / compose several particle systems in a hierarchy and their playback will behave as one particle system.
    *   Built-in curve editor for easy curve editing.
*   Pathfinding and avoidance sub-system added.
    *   NavMesh: Path-finding API. Bake navigation mesh with markup areas.
    *   NavMeshAgent: Character navigation. Avoidance system.
    *   OffmeshLink: used to create arbitrary connections between NavMesh polygons.
*   Built-in LOD management via LOD Groups.
    *   Lightmap baking works for LODed models. The lightmapped objects use a surface transfer algorithm similar to normal map baking.
*   Asset Cache server.
    *   Assets imports are shared between project folders and users. Switching Platform takes minutes instead of hours on large scale projects. Grabbing changes from other team members is almost instant.
*   Built-in HDR support and adaptive tonemapping.
    *   The 3.5 image effects package comes with adaptive tonemapping, bloom and depth of field image effects that are optimized for HDR.
*   Multithreaded rendering.
    *   Most of rendering & driver overhead is put onto another CPU core on multicore systems.
    *   You don't have to do anything, it just works!
    *   Currently only on PC / Mac / Xbox 360; and not in the web player yet.
*   Light Probes, which allow for using baked lighting on characters and other dynamic objects.
*   Directional Lightmaps.
*   Generic external version control (.meta files) is now available in the free version.
*   Google Native Client is now supported
*   It is now possible to select and edit multiple objects simultaneously with the Inspector!
    *   The Inspector preview supports showing the multiple selected objects.
    *   Multi-editing can be enabled for custom editors with a single line of code if they are based on using SerializedProperty.
*   Occlusion Culling has been rewritten from scratch, it is much faster to compute and always correct
    *   OcclusionPortal component has been added to allow doors that can be opened and closed at runtime.
    *   Terrains work well with occlusion culling now.
    *   The default mode for occlusion culling is “automatic portal generation”, which is very accurate and works well for dynamic objects.
    *   Introduced the “Occludee Static” flag. This is used to mark objects as statically occludable without making them occluders. For example transparent objects that don't move should be marked as Occludee Static.
*   Text-based scene and prefab format can be used for improving team workflows. This can be turned on or off in the Editor Settings for each project.
*   GPU Profiler: added the ability to see GPU usage to the profiler.
*   A ton of memory and performance optimizations. Several improvements to multithreading.