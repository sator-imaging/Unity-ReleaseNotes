# Unity 4.0.1
https://unity3d.com/unity/whats-new/unity-4.0.1

## Fixes

<ul>
<li>Android: Improved build times for projects with lots of resources.</li>
<li>Android: Fixed Resources.Load() of prefabs consuming too much memory.</li>
<li>Android: Prevent NullPointerExceptions when using LVL on a device that is not signed in to Google Play.</li>
<li>Android: Detect manifest permissions for Application.genuine / .genuineCheckAvailable.</li>
<li>Android: Stereo sound enforced to avoid garbled audio when Mono is selected as speaker mode.</li>
<li>Android: TouchScreenKeyboard.text is now set to initial value on cancel.</li>
<li>Android: Touches outside TouchScreenKeyboard no longer result in a cancelation event.</li>
<li>Android: Fixed an issue where async updates of the TouchScreenKeyboard.text property would void any input from the keyboard.</li>
<li>Android: Fixed an issue with missing features/permissions in the AndroidManifest.</li>
<li>Android: Added workaround for Tegra shader compiler bug when texture samplers are not reported.</li>
<li>Android: Fixed issue on Adreno with skinning on gles11.</li>
<li>Android: Made sure correct screen resolution is set before Awake is called on scripts.</li>
<li>Android: Fixed error message when current build is aborted by the user.</li>
<li>Android: Fixed an issue where dictionary pop-ups would close the TouchScreenKeyboard.</li>
<li>Android: Application pause now cancels the TouchScreenKeyboard.</li>
<li>Android: Fixed Build&amp;Run with Split Application Binary enabled, when running on a device with JB MR1 (OS 4.2) or later.</li>
<li>Android: Fixed a problem with non-ascii characters and keyboard input.</li>
<li>Documentation: Fixed iOS specific API docs, now they are back.</li>
<li>Editor: Fixed leak in the editor when loading a scene</li>
<li>Editor: Fixed rare crash when updating from 3.5 project</li>
<li>Editor: Fixed missing references to animation when updating from 3.5 project</li>
<li>Graphics: Fixed !IsNormalized error message when rendering a Camera with a skewed transform.</li>
<li>Graphics: Fixed reporting of TextureFormat.RGBA4444.</li>
<li>iOS: fix WWW class crash when loading files via file:// on iOS 4.x devices</li>
<li>iOS: Fixed reporting of GPS location data.</li>
<li>iOS: Better performance when setting RenderTexture that has different size from the current one.</li>
<li>iOS: Fixed gyro accuracy issue.</li>
<li>Lightmapping: Fixed lightmapping in some cases being much slower than 3.5.x.</li>
<li>Mac OS X and Linux Standalone: Fix free version splash screen rendering correctly in full screen mode.</li>
<li>Mac OS X Standalone: Fix window resolution not correctly restoring after going in and out of full screen mode.</li>
<li>Mac OS X Web Player: Fix Input.inputString when a text field is focused (this caused problems with NGUI).</li>
<li>Mecanim: Fixed a crash when you preview an animation on an avatar and the file containing this avatar is updated in an External tools.</li>
<li>Mecanim: Fix problem with deltaPosition and deltaRotation not being updated for Generic Rigs.</li>
<li>Mecanim: Fix crash when previewing transitions with a BlendTree that as a 0 speed child.</li>
<li>Mecanim: Fix getting NaN root transform in MatchTarget on IOS devices.</li>
<li>Shuriken: Fixed emitter shape being wrong shape when parented to another game object with scale.</li>
<li>Substance: fixed bitmap export.</li>
<li>Web Player: Fixed crash with 3.x content containing font data with invalid TrueType font names.</li>
<li>Web Player: Fixed fullscreen mode initialization in IE10 on Windows 8. Web Player now tries to detect whether it is running in a sandbox.</li>
<li>Windows Web Player: Fix the Web Player ticking code, so that it works smoother, fixing a performance regression from 3.5.5.</li>
<li>Fixed mesh assets created with 3.5.0 crashing newer versions of Unity when mixing compressed and non-compressed meshes.</li>
<li>Fixed a crash in which garbage collection of assets could cause broken references to those assets in script code.</li>
</ul>
