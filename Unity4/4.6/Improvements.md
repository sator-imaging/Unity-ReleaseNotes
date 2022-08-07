# Unity 4.6
https://unity3d.com/unity/whats-new/unity-4.6

## Improvements


### Core Improvements
<ul>
<li>Added smart-allocating GetComponents&gt; method which fetches components of type T and grows the list as needed. Non-generic version that supports interfaces has also been added.</li>
<li>Added StopCoroutine(Coroutine) function.</li>
<li>Added callback 'OnTransformParentChanged' to MonoBehaviour. This is called whenever a transform, or one of it's parent transforms has been reparented.</li>
<li>Added Transform.SetParent method that optionally allows setting the parent transform without changing the local position, rotation or scale. For RectTransform it also doesn't change the sizeDelta.</li>
<li>Implemented and exposed Transform.TransformVector and Transform.InverseTransformVector so it's no longer necessary to use localToWorldMatrix and WorldToLocalMatrix just to transform vectors with scaling included. </li>
<li>Added Vector2.SmoothDamp to be consistent with Vector3.SmoothDamp, Mathf.SmoothDamp, and others.</li>
<li>New API TouchScreenKeyboard.isSupported to check if platform supports on screen keyboard.</li>
<li>Added new WillFlushUndoRecord callback to Undo class.</li>
<li>Added Input.touchSupported API: it tells whether the device on which application is currently running supports touch input.</li>
</ul>

### Editor Improvements
<ul>
<li>Reorganized GameObject creation menus with categories such as 3D Object, 2D Object, Light, etc. as well as improved functionality. 
<ul>
<li>"Create Empty" now also appears in the hierarchy Create dropdown.</li>
<li>The context menu for Game Objects in the hierarchy can now be used to create new Game Objects as children.</li>
</ul></li>
<li>More details on the error message when failing to add a Component due to already having another component that is incompatible. </li>
<li>If during play mode a hierarchy window takes too long to fetch new data a warning icon will appear to advise users frame rate could be affected based upon the chosen hierarchy sorting.</li>
<li>Editor: Made Scene View camera near and far clip planes use constant multipliers of size rather than four fixed ranges with fixed values that cause popping when transitioning over the thresholds of those ranges. The new ranges are about the same for close and medium zoom but has significantly larger near clip planes when zoomed far out, which reduces z-fighting.</li>
<li>Made main Game View used by CameraEditor visualizations and the Canvas be the last focused Game View rather than just the first Game View found.</li>
<li>Made sure the screen manager uses the correct game view size in the editor, which is only known on the managed side.</li>
<li>Increased Texture anisotropic level limit to 16 in the Texture Inspector.</li>
<li>Exposed "Generate Mip Maps" option in the Texture Inspector when in Sprite mode.</li>
<li>Renamed TextureImporter spritePixelsToUnits to spritePixelsPerUnit and made old property obsolete. The old name was misleading.</li>
<li>Curves can now be renamed in the animation window.</li>
<li>Made SerializedProperty.displayName public.</li>
<li>Enum options generated from SerializedProperty are now nicified just like for all other enum fields in the Inspector.</li>
<li>Added SerializedProperty.enumDisplayNames that return the names for enum values as they're shown in the Inspector.</li>
</ul>

### Mecanim Improvements
<ul>
<li>Animation of PPtr types are now supported in the animation window (textures, sprites, materials etc).</li>
<li>SendTransformChanged is now only sent to transforms that are animated. Siblings with no animation will not receive SendTransformChanged.</li>
</ul>

### 2D Improvements
<ul>
<li>Default SpritePacker policies will automatically pack mipmapped sprites (padding power - 2).</li>
<li>Aniso level for sprites with mip-maps now defaults to 16.</li>
<li>SpritePacker will flood the atlas instead of adding 1 pixel borders to sprites.</li>
<li>A new pixelsPerUnit property has been exposed on the Sprite class.</li>
</ul>

### Android Improvements
<ul>
<li>Support for profiling Intel GPU using the Unity Editor.</li>
<li>Added support for BGRA textures.</li>
</ul>
