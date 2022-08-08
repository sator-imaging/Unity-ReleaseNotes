# Unity 5.3

https://unity3d.com/unity/whats-new/unity-5.3

## The following are changes and fixes to 5.3 features and regressions...

- [Change](#change)
- [Improvement](#improvement)
- [Fixes](#fixes)


### Change

*   Animation: Changed ModelImporter.resampleRotations to ModelImporter.resampleCurves
*   MSE: Lightmap baking now work with multi-scene edit from the Lighting window UI. Simply opening multiple scenes, then pressing bake, will bake data for all open scenes at the same time. Lightmaps and Enlighten data is separated out into separate chunks / atlases per scene. At runtime it is loaded / unloaded separately from each other via the normal scene loading / unloading API's.
*   MSE: Navmesh baking now work with multi-scene edit from the Navmesh window UI. Simply opening multiple scenes, then pressing bake, will bake data for all open scenes at the same time. Navmeshes will be baked and stored for all geometry together and the resulting navmesh is assigned to each scene.

### Improvement

*   OSX / new OpenGL renderer: Performance improvement when rendering small batches on immediate GL (or via Handles.DrawLine)

### Fixes

*   Android: Fixed increase in APK size comparing to 5.2 (Disable texture streaming for Android)
*   FrameDebugger: Fixed crash in remote frame debugger in cases where scene has statically batched geometry
*   GI: Fixed crash when switching scene view from baked to clustering.
*   iOS: Fix crash for devices that didn’t support NPOT Textures with GLES2
*   Mecanim: Event key in animation window is not movable if keyframe is added
*   Mecanim: Fixed a bug where errors would pop when using resampleRotations/resampleCurves with optimized Game Objects
*   Mecanim: Fixed a crash when using resampleRotations/resampleCurves with optimized Game Objects
*   Mecanim: Fixed an issue where an event with the wrong parameter type would throw an exception
*   Mecanim: Fixed an unreported issue where animation events using enums would never get fired
*   Mecanim: Fixed crash when deleting AnimatorController asset
*   Mecanim: Setting AnimatorController on a GameObject does not dirty the scene.
*   MSE: Fix the crash that when performing an undo after pasting a GO to the implied active scene.
*   MSE: Fix the crash when starting up Unity if last active scene was a Untitled scene (in multi scene setup)
*   MSE: Fix the error about loading an unloaded scene during runtime/play mode
*   MSE: Fix the Window title bar not updating when scene were opened
*   OSX / New OpenGL: Fix for garbled rendering on older Macs with NVidia GT 8x00 or 9x00
*   OSX / New OpenGL: Fix missing VSync
*   OSX / New OpenGL: Fix normal map encoding in the editor when targeting iOS or Android
*   WebPlayer: Fix webplayer content to work with prior versions of web plugin