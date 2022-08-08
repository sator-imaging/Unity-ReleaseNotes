# Unity 3.5

https://unity3d.com/unity/whats-new/unity-3.5

## Editor Features



*   Middle-click on any surface in the Scene View to focus on the clicked point.
*   AssetModificationProcessor class created with custom VCS systems in mind.
    *   Adds IsOpenForEdit check on assets which can prevent assets from being edited.
*   The preview in the Inspector can be detached to a separate window.
*   Implemented support for C4D file import from Cinema4D R13.
*   Implemented better detection of imported material types. Unity uses normal-map and transparency properties (texture or factor) to apply one of the following shaders: "Bumped Diffuse", "Transparent/Diffuse" or "Transparent/Bumped Diffuse".
*   Implemented import of texture Tiling and Offset values.
*   Implemented support for baking animation through FBX exporter during C4D file import (supported only from Cinema 4D R13, the old version uses our native IK baker).
*   Mac: Added support for full-screen mode in the new Mac OS X Lion 10.7.
*   Improved preferences window that users can extend by using the PreferenceItem attribute.
*   Gizmos can have world-space sizes. Nice, hi-res gizmos were added.
*   The Transform gizmo has a new planar transform tool for performing two-axis translations, which replaces the Free Transform tool. Hold the 'shift' key to switch back to the Free Transform tool.
*   GUI class now has a DrawTextureWithTexCoords function for specifying texture coordinates.
*   Entire curves can now be dragged vertically.
*   Gizmos are now depth-tested, and exist in world space. The gizmo size can be adjusted using the existing gizmos size slider.
*   Introduced a more advanced Static checkbox: It is now possible to mark objects static for different situations (lightmapping, navigation, occlusion etc).
*   Made it possible to find objects in scene that reference the selected asset.
*   Texture Importer for pvrtc-enabled platforms allows to select compression quality.
*   New Prefab system allows adding / removing components from instances without breaking the prefab connection.
    *   Backwards compatibility with old prefabs is maintained.
    *   Made sure prefabs do not show up as “missing” in play mode.