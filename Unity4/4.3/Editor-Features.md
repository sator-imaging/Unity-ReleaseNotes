# Unity 4.3
https://unity3d.com/unity/whats-new/unity-4.3

## Editor Features


### Editor Controls Overhaul
<ul>
<li>LookLikeControls and LookLikeInspector have been replaced with a single unified look.</li>
<li>New look has consistent styles, indentation and layout.</li>
<li>Keyboard navigation now works for all components and is improved for sliders and object fields.</li>
<li>The Inspector has a new Wide Mode that places controls in a more neatly aligned and vertically compact way.</li>
<li>Easier to write Editor GUI with consistent alignment.</li>
<li>Relevant new API: 
<ul>
<li>EditorGUIUtility.labelWidth and EditorGUIUtility.fieldWidth replaces the parameters in the now obsolete EditorGUIUtility.LookLikeControls function.</li>
<li>EditorGUI.PrefixLabel has a new overload that doesn't need an id parameter.</li>
<li>EditorGUILayout.GetControlRect is the best way to get a Rect for a standard sized Editor control.</li>
</ul></li>
</ul>

### Other Editor Features
<ul>
<li>Unity now ships with a brand new MonoDevelop 4.0.1!</li>
<li>Ability to build iOS target in Windows! It's still necessary to compile resulting Xcode project on a Mac.</li>
<li>Added global SortingLayers (see Tags &amp; Layers window). Every Renderer can specify a layer and an in-layer order value for explicit ordering using. SpriteRenderer inspector exposes the two properties.</li>
<li>Layer locking for scene view. The layers dropdown in editor toolbar controls visibility or locking of layers (and locking of the new Sorting Layers). Locked layers are visible, but aren't pickable in the scene view.</li>
<li>Undo has been optimized for large scenes. Full scene undo support has been removed, all undo operations save only the necessary objects. SnapshotUndo support has been deprecated, instead Undo.RecordObject is to be used for all property modifications. Undo API has been revamped to make it clearer what functions should be used now.</li>
<li>Added a "Default behavior" property to Editor Properties to control default texture import behavior and default scene view mode.</li>
<li>Added an option to the new project wizard to select default editor behavior (2D/3D).</li>
<li>BuildPipeline methods now have parameters to output CRC checksums of generated AssetBundles.</li>
<li>New Highlighter editor API for highlighting elements in the editor. Useful for in-editor tutorials and similar.</li>
<li>Asset Pipeline: Only new assets or assets where the actual content has change will get imported. Changing the time stamp of an asset will no longer cause a reimport.</li>
<li>Asset Pipeline: .meta files are now always turned on. From Project Settings -&gt; Editor you can choose to hide them if you are not using version control.</li>
<li>Added ability to specify external script editor's args, including file and line info. (Windows editor only).</li>
</ul>
