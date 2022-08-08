# Unity 5.5

https://unity3d.com/unity/whats-new/unity-5.5.0

## The following are changes and fixes to 5.5.0 features and regressions...

- [Fixes](#fixes)


### Fixes

*   Core: Fixed Library folder corruption when opening project in previous versions of Unity (851782)
*   Editor: Fixed undoing Transform changes when multiselection includes prefab instance and share a common ancestor [(822868)](https://issuetracker.unity3d.com/issues/ctrl-plus-z-does-not-revert-all-objects-position-when-prefab-is-present-and-objects-are-empty-gameobjects-children)
*   GI: Clearing baked data at certain lighting calculation stages causes uninformative errors in the console [(757816)](https://issuetracker.unity3d.com/issues/editor-clearbakeddata-clearing-baked-data-at-certain-lighting-calculation-stages-causes-uninformative-errors-in-the-console)
*   GI: Fixed broken GI Previews on Retina Mac [(836815)](https://issuetracker.unity3d.com/issues/gi-previews-are-broken-on-retina-mac)
*   Graphics: Fixed a crash in the renderloop, caused by incorrect memlabel when releasing shared LightmapSettings data. (834235)
*   Graphics: Fixed issue where occlusion mesh was incorrectly displayed when using single pass stereo [(850170)](https://issuetracker.unity3d.com/issues/singlepassstereo-scene-with-reflections-renders-occlusion-mesh-artifacts)
*   Graphics: Fixed Reflection Probes artifacts when multiple overlapping lights are captured by the Reflection Probe (835423)
*   Graphics: Fixed several issues regarding single pass stereo with Image effects and deferred rendering (832185, 830612 ,832283, 814290, 821746)
*   Graphics: LightProbes are sometimes applied incorrectly, depending on object use/don't use probes flag, and object render order (840641)
*   Serialization: Fix rare issue where prefab references from scene objects would be show as missing when using text serialization. (850947)
*   UI: Fixed issue where calculation of Text perferred height was incorrect. [(850077)](https://issuetracker.unity3d.com/issues/ui-incorrect-preferred-height-for-text-component-if-pivot-x-is-set-to-0)
*   VR: Fixed MsHRTFSpatializer load failure. No longer requires external dependencies to Unity and Windows. (847470)

#### Revision: 38b4efef76f0