# Unity 4.6

https://unity3d.com/unity/whats-new/unity-4.6

## Fixes

- [Editor Fixes](#editor-fixes)
- [Graphics Fixes](#graphics-fixes)
- [Animation Fixes](#animation-fixes)
- [2D Fixes](#2d-fixes)
- [Mobile Fixes](#mobile-fixes)


### Editor Fixes

*   Fixed occasional argument out of range exceptions when using Scene View tools.
*   Picking of locked scene view layers is now prevented.
*   ObjectSelector is now ensured to default to the Asset tab when selecting PhysicsMaterial2D objects.

### Graphics Fixes

*   Fixed an issue where render texture was not being created due unsupported anti aliasing value on devices like Surface RT.
*   Compressed sprites are no longer deformed on devices that support NPOT textures.

### Animation Fixes

*   Fixed issue where changing the animated property to be Rect Transform Scale and trying to transition between 0 and 1 failed.
*   Fixed crash when creating an AnimationClip on a humanoid rig.
*   Fixes crash when previewing transitions on an Animator with UnscaledTime update mode.

### 2D Fixes

*   Unity no longer crashes if a mesh is dragged onto a SpriteRenderer.
*   Fixed issue where 2D colliders break when used as prefab children.

### Mobile Fixes

*   Windows Phone 8: Fixed a race condition in TouchScreenKeyboard which would cause ".active" to return false just after the keyboard was opened.
*   Windows Phone 8.1: Fixed an issue which caused InputField and GUI.TextArea to always receive capital letters from the on screen keyboard.
*   Android: Disabled shadows for Intel PowerVR devices to avoid graphics artifacts.