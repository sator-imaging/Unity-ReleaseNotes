# Unity 4.6
https://unity3d.com/unity/whats-new/unity-4.6

## Fixes


### Editor Fixes
<ul>
<li>Fixed occasional argument out of range exceptions when using Scene View tools.</li>
<li>Picking of locked scene view layers is now prevented.</li>
<li>ObjectSelector is now ensured to default to the Asset tab when selecting PhysicsMaterial2D objects.</li>
</ul>

### Graphics Fixes
<ul>
<li>Fixed an issue where render texture was not being created due unsupported anti aliasing value on devices like Surface RT.</li>
<li>Compressed sprites are no longer deformed on devices that support NPOT textures.</li>
</ul>

### Animation Fixes
<ul>
<li>Fixed issue where changing the animated property to be Rect Transform Scale and trying to transition between 0 and 1 failed.</li>
<li>Fixed crash when creating an AnimationClip on a humanoid rig.</li>
<li>Fixes crash when previewing transitions on an Animator with UnscaledTime update mode.</li>
</ul>

### 2D Fixes
<ul>
<li>Unity no longer crashes if a mesh is dragged onto a SpriteRenderer.</li>
<li>Fixed issue where 2D colliders break when used as prefab children.</li>
</ul>

### Mobile Fixes
<ul>
<li>Windows Phone 8: Fixed a race condition in TouchScreenKeyboard which would cause ".active" to return false just after the keyboard was opened.</li>
<li>Windows Phone 8.1: Fixed an issue which caused InputField and GUI.TextArea to always receive capital letters from the on screen keyboard.</li>
<li>Android: Disabled shadows for Intel PowerVR devices to avoid graphics artifacts.</li>
</ul>
