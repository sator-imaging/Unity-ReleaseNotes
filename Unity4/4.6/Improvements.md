# Unity 4.6

https://unity3d.com/unity/whats-new/unity-4.6

## Improvements

- [Core Improvements](#core-improvements)
- [Editor Improvements](#editor-improvements)
- [Mecanim Improvements](#mecanim-improvements)
- [2D Improvements](#2d-improvements)
- [Android Improvements](#android-improvements)


### Core Improvements

*   Added smart-allocating GetComponents> method which fetches components of type T and grows the list as needed. Non-generic version that supports interfaces has also been added.
*   Added StopCoroutine(Coroutine) function.
*   Added callback 'OnTransformParentChanged' to MonoBehaviour. This is called whenever a transform, or one of it's parent transforms has been reparented.
*   Added Transform.SetParent method that optionally allows setting the parent transform without changing the local position, rotation or scale. For RectTransform it also doesn't change the sizeDelta.
*   Implemented and exposed Transform.TransformVector and Transform.InverseTransformVector so it's no longer necessary to use localToWorldMatrix and WorldToLocalMatrix just to transform vectors with scaling included.
*   Added Vector2.SmoothDamp to be consistent with Vector3.SmoothDamp, Mathf.SmoothDamp, and others.
*   New API TouchScreenKeyboard.isSupported to check if platform supports on screen keyboard.
*   Added new WillFlushUndoRecord callback to Undo class.
*   Added Input.touchSupported API: it tells whether the device on which application is currently running supports touch input.

### Editor Improvements

*   Reorganized GameObject creation menus with categories such as 3D Object, 2D Object, Light, etc. as well as improved functionality.
    *   "Create Empty" now also appears in the hierarchy Create dropdown.
    *   The context menu for Game Objects in the hierarchy can now be used to create new Game Objects as children.
*   More details on the error message when failing to add a Component due to already having another component that is incompatible.
*   If during play mode a hierarchy window takes too long to fetch new data a warning icon will appear to advise users frame rate could be affected based upon the chosen hierarchy sorting.
*   Editor: Made Scene View camera near and far clip planes use constant multipliers of size rather than four fixed ranges with fixed values that cause popping when transitioning over the thresholds of those ranges. The new ranges are about the same for close and medium zoom but has significantly larger near clip planes when zoomed far out, which reduces z-fighting.
*   Made main Game View used by CameraEditor visualizations and the Canvas be the last focused Game View rather than just the first Game View found.
*   Made sure the screen manager uses the correct game view size in the editor, which is only known on the managed side.
*   Increased Texture anisotropic level limit to 16 in the Texture Inspector.
*   Exposed "Generate Mip Maps" option in the Texture Inspector when in Sprite mode.
*   Renamed TextureImporter spritePixelsToUnits to spritePixelsPerUnit and made old property obsolete. The old name was misleading.
*   Curves can now be renamed in the animation window.
*   Made SerializedProperty.displayName public.
*   Enum options generated from SerializedProperty are now nicified just like for all other enum fields in the Inspector.
*   Added SerializedProperty.enumDisplayNames that return the names for enum values as they're shown in the Inspector.

### Mecanim Improvements

*   Animation of PPtr types are now supported in the animation window (textures, sprites, materials etc).
*   SendTransformChanged is now only sent to transforms that are animated. Siblings with no animation will not receive SendTransformChanged.

### 2D Improvements

*   Default SpritePacker policies will automatically pack mipmapped sprites (padding power - 2).
*   Aniso level for sprites with mip-maps now defaults to 16.
*   SpritePacker will flood the atlas instead of adding 1 pixel borders to sprites.
*   A new pixelsPerUnit property has been exposed on the Sprite class.

### Android Improvements

*   Support for profiling Intel GPU using the Unity Editor.
*   Added support for BGRA textures.