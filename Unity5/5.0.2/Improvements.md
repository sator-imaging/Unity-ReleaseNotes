# Unity 5.0.2

https://unity3d.com/unity/whats-new/unity-5.0.2

## Improvements



*   Editor: Added Android 5.0 and 5.1 to "Minimum API Level" list.
*   GI: Don't add lights to Enlighten at runtime if they don't contribute to GI (bounce intensity at 0).
*   GI: Made pig assert message human readable.
*   iOS: Enabled thumb instruction support for IL2CPP ARMv7 slice. Should improve ARMv7 slice code size by 10-20%.
*   iOS/IL2CPP: Avoid generating NullReference checks on value types.
*   iOS/IL2CPP: Improve performance of finally blocks.
*   iOS/Metal: Better support for native rendering plugins when using Metal.
*   Mecanim: Fix direct blendtree editor slow down when there is too much motion.
*   Physics 2D: Added 'AreaEffector2D.useGlobalAngle' to allow the selection of whether the force-angle is global or local.
*   Physics 2D: Added 'Effector2D.useColliderMask' to allow the selection of whether the effector collider mask is used or the global collision matrix.
*   Physics 2D: Added 'Rigidbody2D.IsTouching' and 'Rigidbody2D.IsTouchingLayers' to complement the same on 'Collider2D' and 'Physics2D'.
*   Physics 2D: Renamed 'AreaEffector2D.forceDirection' to 'AreaEffector2D.forceAngle' (sciprts are automaticallly updated).
*   Physics: Report detailed error when generating collision meshes, also during asset import. Simplifies troubleshooting creation of non-triangle collision meshes.
*   Substance: New Substance features introduced by Substance Designer 5.0 are now supported.
*   Terrain: TerrainData.alphamapTextures is now public.
*   Windows Standalone: Hint to AMD driver that discrete GPU should be used, rather than integrated GPU.
*   XboxOne: Lightmap files are now listed in the package manifest in the same chunk as the scene that uses them.
*   XboxOne: Unity is now built with the April 2015 XDK. You will need to install the April 2015 XDK on your PC and use the same or later recovery on your console.
*   XboxOne: Updated docs to reflect terminology and tools in latest XDK, and added a section on Packaging.
*   XboxOne: Worker threads created by Unity's core systems (Physics, AI) will no longer run on cores 0 and 1, which are reserved for the Rendering thread and Unity's main thread respectively. This will be a performance gain in most cases by avoiding thread context switches.