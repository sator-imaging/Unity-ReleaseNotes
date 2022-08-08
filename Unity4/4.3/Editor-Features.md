# Unity 4.3

https://unity3d.com/unity/whats-new/unity-4.3

## Editor Features

- [Editor Controls Overhaul](#editor-controls-overhaul)
- [Other Editor Features](#other-editor-features)


### Editor Controls Overhaul

*   LookLikeControls and LookLikeInspector have been replaced with a single unified look.
*   New look has consistent styles, indentation and layout.
*   Keyboard navigation now works for all components and is improved for sliders and object fields.
*   The Inspector has a new Wide Mode that places controls in a more neatly aligned and vertically compact way.
*   Easier to write Editor GUI with consistent alignment.
*   Relevant new API:
    *   EditorGUIUtility.labelWidth and EditorGUIUtility.fieldWidth replaces the parameters in the now obsolete EditorGUIUtility.LookLikeControls function.
    *   EditorGUI.PrefixLabel has a new overload that doesn't need an id parameter.
    *   EditorGUILayout.GetControlRect is the best way to get a Rect for a standard sized Editor control.

### Other Editor Features

*   Unity now ships with a brand new MonoDevelop 4.0.1!
*   Ability to build iOS target in Windows! It's still necessary to compile resulting Xcode project on a Mac.
*   Added global SortingLayers (see Tags & Layers window). Every Renderer can specify a layer and an in-layer order value for explicit ordering using. SpriteRenderer inspector exposes the two properties.
*   Layer locking for scene view. The layers dropdown in editor toolbar controls visibility or locking of layers (and locking of the new Sorting Layers). Locked layers are visible, but aren't pickable in the scene view.
*   Undo has been optimized for large scenes. Full scene undo support has been removed, all undo operations save only the necessary objects. SnapshotUndo support has been deprecated, instead Undo.RecordObject is to be used for all property modifications. Undo API has been revamped to make it clearer what functions should be used now.
*   Added a "Default behavior" property to Editor Properties to control default texture import behavior and default scene view mode.
*   Added an option to the new project wizard to select default editor behavior (2D/3D).
*   BuildPipeline methods now have parameters to output CRC checksums of generated AssetBundles.
*   New Highlighter editor API for highlighting elements in the editor. Useful for in-editor tutorials and similar.
*   Asset Pipeline: Only new assets or assets where the actual content has change will get imported. Changing the time stamp of an asset will no longer cause a reimport.
*   Asset Pipeline: .meta files are now always turned on. From Project Settings -> Editor you can choose to hide them if you are not using version control.
*   Added ability to specify external script editor's args, including file and line info. (Windows editor only).