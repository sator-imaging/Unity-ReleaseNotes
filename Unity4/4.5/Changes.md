# Unity 4.5

https://unity3d.com/unity/whats-new/unity-4.5

## Changes



*   2D: Atlas packer DefaultPackerPolicy will now pack Sprites as rectangles unless packing tags begin with "\[TIGHT\]". The new TightPackerPolicy will tightly pack Sprites with a Tight Mesh unless packing tags begin with "\[RECT\]".
*   2D: Sprite Packer is no longer a preview feature.
*   Android: Disabled GPU profiling on Adrenos for now, due to unstable drivers.
*   Asset Bundles: Trying to build a bundle from within an AssetPostprocessor will now throw an error.
*   BlackBerry: BuildTarget.BB10, BuildTargetGroup.BB10, and BaseClass.BB10Player have been deprecated. Please use BuildTarget.BlackBerry, BuildTargetGroup.BlackBerry and BaseClass.BlackBerryPlayer
*   Editor: Components with OnSceneGUI calls will now show up in scene view Gizmos popup.
*   Editor: Data consistency checks for objects loaded from disk are now performed on all objects before waking up the first one of them instead of interleaving the two operations.
*   Editor: Newly created projects default to DirectX 11 on Windows now (you can still make DX9 be the default in project settings).
*   Editor: Utility Editor windows no longer have 10 pixels automatically added at the top when using GUILayout.
*   Editor: Removed SpriteRenderer preview.
*   Editor: Show overlay label in Game View with actual used resolution if actual used resolution is smaller than the selected fixed resolution.
*   iOS: Added iOS7 target.
*   iOS: Refactored trampoline; extracted view handling and rendering categories from UnityAppController.
*   Mac: Rewrote Mac web cam support to use AVFoundation framework, so you can publish to the Mac App Store without using deprecated APIs.
*   Mecanim: Introduced Animator Update Mode which replaces Animator.animatePhysics. Adds the possibility to update Mecanim independently of Time.timeScale.
*   Physics: All existing joints are now derived from AnchoredJoint2D component rather than the Joint2D component.
*   Physics: Collision and trigger callbacks now occur on both the GameObject containing the 2D collider as well as the GameObject containing the 2D rigid-body.
*   Physics: Updated Box2D to v2.3.0.
*   Sprite Editor: Now an undockable utility window and can only be opened from the sprite inspector.
*   Sprite Editor: Removed 'Minimum size' from automatic slicing dialog.
*   Substance: A new 'DoNothingAndCache' loading behaviour is now available. Substances are no longer automatically generated when loaded but are still cached to non-volatile storage after the first call to RebuildTextures() / RebuildTexturesImmediately().
*   Substance: ProceduralMaterial.isCachedDataAvailable was added to check if cache data will be used for a cached ProceduralMaterial or if its outputs will have to be rebuilt. Coupled with DoNothingAndCache, this allows for interactive "installer / substance decompressors" scenes to be created.
*   Windows Store Apps / WP8: Unity won't spam warnings for incorrectly unloaded assets, unless explicitly specified.
*   Windows Store Apps: Independent Input Source is disabled again by default due to delays in Windows Update.
*   WWW: deprecated 'WWW(string url, byte\[\] postData, Hashtable headers)', use 'public WWW(string url, byte\[\] postData, Dictionary headers)' instead.