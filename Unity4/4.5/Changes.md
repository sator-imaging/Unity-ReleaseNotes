# Unity 4.5
https://unity3d.com/unity/whats-new/unity-4.5

## Changes

<ul>
<li>2D: Atlas packer DefaultPackerPolicy will now pack Sprites as rectangles unless packing tags begin with "[TIGHT]". The new TightPackerPolicy will tightly pack Sprites with a Tight Mesh unless packing tags begin with "[RECT]". </li>
<li>2D: Sprite Packer is no longer a preview feature.</li>
<li>Android: Disabled GPU profiling on Adrenos for now, due to unstable drivers. </li>
<li>Asset Bundles: Trying to build a bundle from within an AssetPostprocessor will now throw an error.</li>
<li>BlackBerry: BuildTarget.BB10, BuildTargetGroup.BB10, and BaseClass.BB10Player have been deprecated. Please use BuildTarget.BlackBerry, BuildTargetGroup.BlackBerry and BaseClass.BlackBerryPlayer</li>
<li>Editor: Components with OnSceneGUI calls will now show up in scene view Gizmos popup.</li>
<li>Editor: Data consistency checks for objects loaded from disk are now performed on all objects before waking up the first one of them instead of interleaving the two operations.</li>
<li>Editor: Newly created projects default to DirectX 11 on Windows now (you can still make DX9 be the default in project settings).</li>
<li>Editor: Utility Editor windows no longer have 10 pixels automatically added at the top when using GUILayout.</li>
<li>Editor: Removed SpriteRenderer preview.</li>
<li>Editor: Show overlay label in Game View with actual used resolution if actual used resolution is smaller than the selected fixed resolution.</li>
<li>iOS: Added iOS7 target.</li>
<li>iOS: Refactored trampoline; extracted view handling and rendering categories from UnityAppController.</li>
<li>Mac: Rewrote Mac web cam support to use AVFoundation framework, so you can publish to the Mac App Store without using deprecated APIs.</li>
<li>Mecanim: Introduced Animator Update Mode which replaces Animator.animatePhysics. Adds the possibility to update Mecanim independently of Time.timeScale.</li>
<li>Physics: All existing joints are now derived from AnchoredJoint2D component rather than the Joint2D component.</li>
<li>Physics: Collision and trigger callbacks now occur on both the GameObject containing the 2D collider as well as the GameObject containing the 2D rigid-body.</li>
<li>Physics: Updated Box2D to v2.3.0.</li>
<li>Sprite Editor: Now an undockable utility window and can only be opened from the sprite inspector.</li>
<li>Sprite Editor: Removed 'Minimum size' from automatic slicing dialog. </li>
<li>Substance: A new 'DoNothingAndCache' loading behaviour is now available. Substances are no longer automatically generated when loaded but are still cached to non-volatile storage after the first call to RebuildTextures() / RebuildTexturesImmediately().</li>
<li>Substance: ProceduralMaterial.isCachedDataAvailable was added to check if cache data will be used for a cached ProceduralMaterial or if its outputs will have to be rebuilt. Coupled with DoNothingAndCache, this allows for interactive "installer / substance decompressors" scenes to be created.</li>
<li>Windows Store Apps / WP8: Unity won't spam warnings for incorrectly unloaded assets, unless explicitly specified.</li>
<li>Windows Store Apps: Independent Input Source is disabled again by default due to delays in Windows Update. </li>
<li>WWW: deprecated 'WWW(string url, byte[] postData, Hashtable headers)', use 'public WWW(string url, byte[] postData, Dictionary headers)' instead. </li>
</ul>
