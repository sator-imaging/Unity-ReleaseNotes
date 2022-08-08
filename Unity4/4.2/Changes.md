# Unity 4.2

https://unity3d.com/unity/whats-new/unity-4.2

## Changes



*   Asset bundles built in prior versions of Unity are no longer compatible with Unity 4.2 (this has been necessary because of changes to how built-in resources are handled).
*   AssetDatabase.ImportPackage and AssetDatabase.ExportPackage can now be called repeatedly from within the same iteration of the game update loop (previously, successive calls would overwrite the buffered state of the previous one).
*   Audio: 7.1 content can now be loaded in the editor (previously only 5.1 was allowed).
*   Editor: Add MeshRenderer component dependency for TextMesh component.
*   Editor: NavMeshLayers editing is now located as a tab in the Navigation Window.
*   Editor: Terrain menu functionality moved to Terrain Inspector. Now you create a terrain by GameObject > Create Other > Terrain. Terrain settings previously in the menu are under Settings tab in terrain inspector.
*   Font colors are now applied as vertex colors, instead of by setting the color on the material. This makes it work better with markup tags in rich text strings. The color property in the font importer has been removed, and instead there are now color properties on the GUIText and TextMesh components to let you set the color of text objects per instance instead of per font.
*   Graphics: Disabled multisampling on NVIDIA cards on OS X earlier than 10.9 in Mac Web Player, due to driver issues.
*   Graphics: Majority of built-in shaders are now only included into your game data if they are actually used. This saves about 200 kilobytes off your mobile game size if you're not using many built-in ones. If you need some built-in shaders to be available without explicit references to them (to make Shader.Find etc. work), set them up in Edit -> Project Settings -> Graphics (by default Diffuse shader is always included).
*   Mac OS X Editor: The Editor on OS X will now allow symlinks in project folders to match Windows behavior. This can be used to share assets across projects, but is not recommended unless you know exactly what you are doing.
*   Made several Unity API calls which had been undocumented for many years properly deprecated.
*   NavMesh: "Reset" button in navmesh bake window is moved to window menu item.
*   Resources.LoadAll() now permits a trailing slash when given a folder name.
*   Web Player: the "Release Channels" context menu item will now only be visible when the Alt/Option key is pressed when opening the context menu.