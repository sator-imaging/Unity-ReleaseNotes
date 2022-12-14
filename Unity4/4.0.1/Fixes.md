# Unity 4.0.1

https://unity3d.com/unity/whats-new/unity-4.0.1

## Fixes



*   Android: Improved build times for projects with lots of resources.
*   Android: Fixed Resources.Load() of prefabs consuming too much memory.
*   Android: Prevent NullPointerExceptions when using LVL on a device that is not signed in to Google Play.
*   Android: Detect manifest permissions for Application.genuine / .genuineCheckAvailable.
*   Android: Stereo sound enforced to avoid garbled audio when Mono is selected as speaker mode.
*   Android: TouchScreenKeyboard.text is now set to initial value on cancel.
*   Android: Touches outside TouchScreenKeyboard no longer result in a cancelation event.
*   Android: Fixed an issue where async updates of the TouchScreenKeyboard.text property would void any input from the keyboard.
*   Android: Fixed an issue with missing features/permissions in the AndroidManifest.
*   Android: Added workaround for Tegra shader compiler bug when texture samplers are not reported.
*   Android: Fixed issue on Adreno with skinning on gles11.
*   Android: Made sure correct screen resolution is set before Awake is called on scripts.
*   Android: Fixed error message when current build is aborted by the user.
*   Android: Fixed an issue where dictionary pop-ups would close the TouchScreenKeyboard.
*   Android: Application pause now cancels the TouchScreenKeyboard.
*   Android: Fixed Build&Run with Split Application Binary enabled, when running on a device with JB MR1 (OS 4.2) or later.
*   Android: Fixed a problem with non-ascii characters and keyboard input.
*   Documentation: Fixed iOS specific API docs, now they are back.
*   Editor: Fixed leak in the editor when loading a scene
*   Editor: Fixed rare crash when updating from 3.5 project
*   Editor: Fixed missing references to animation when updating from 3.5 project
*   Graphics: Fixed !IsNormalized error message when rendering a Camera with a skewed transform.
*   Graphics: Fixed reporting of TextureFormat.RGBA4444.
*   iOS: fix WWW class crash when loading files via file:// on iOS 4.x devices
*   iOS: Fixed reporting of GPS location data.
*   iOS: Better performance when setting RenderTexture that has different size from the current one.
*   iOS: Fixed gyro accuracy issue.
*   Lightmapping: Fixed lightmapping in some cases being much slower than 3.5.x.
*   Mac OS X and Linux Standalone: Fix free version splash screen rendering correctly in full screen mode.
*   Mac OS X Standalone: Fix window resolution not correctly restoring after going in and out of full screen mode.
*   Mac OS X Web Player: Fix Input.inputString when a text field is focused (this caused problems with NGUI).
*   Mecanim: Fixed a crash when you preview an animation on an avatar and the file containing this avatar is updated in an External tools.
*   Mecanim: Fix problem with deltaPosition and deltaRotation not being updated for Generic Rigs.
*   Mecanim: Fix crash when previewing transitions with a BlendTree that as a 0 speed child.
*   Mecanim: Fix getting NaN root transform in MatchTarget on IOS devices.
*   Shuriken: Fixed emitter shape being wrong shape when parented to another game object with scale.
*   Substance: fixed bitmap export.
*   Web Player: Fixed crash with 3.x content containing font data with invalid TrueType font names.
*   Web Player: Fixed fullscreen mode initialization in IE10 on Windows 8. Web Player now tries to detect whether it is running in a sandbox.
*   Windows Web Player: Fix the Web Player ticking code, so that it works smoother, fixing a performance regression from 3.5.5.
*   Fixed mesh assets created with 3.5.0 crashing newer versions of Unity when mixing compressed and non-compressed meshes.
*   Fixed a crash in which garbage collection of assets could cause broken references to those assets in script code.