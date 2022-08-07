# Unity 3.5.7
https://unity3d.com/unity/whats-new/unity-3.5.7

## Fixes

<ul>
<li>Android: Fixed Resources.Load() of prefabs consuming too much memory.</li>
<li>Android: Prevent NullPointerExceptions when using LVL on a device that is not signed in to Google Play.</li>
<li>Android: Fixed a lot of key store related problems.</li>
<li>Android: Fixed an optimization error which could cause javac to crash/fail when loading UnityPlayer class.</li>
<li>Android: Kindle Fire incorrectly reported having a camera.</li>
<li>Android: Fixed an issue where dictionary pop-ups would close the TouchScreenKeyboard.</li>
<li>Android: Application pause now cancels the TouchScreenKeyboard.</li>
<li>Android: Fixed auto-rotation problem in landscape/reversed landscape on Kindle Fire HD.</li>
<li>Android: Fixed a problem where multiple screen touches would lead to incorrect touch phases (especially during low framerate situations).</li>
<li>Android: The detection zone for screen touches resulting in increased tap count has been made resolution independent.</li>
<li>Android: SystemInfo.deviceUniqueIdentifier didn't automatically add the right permissions in the manifest.</li>
<li>Android: Fixed a problem with non-ASCII characters and keyboard input.</li>
<li>Android: Fixed a performance problem affecting the ARMv6 lib.</li>
<li>Android: Fixed rare crashes with dynamic batching in non-development player on PowerVR GPUs.</li>
<li>Android: Fixed performance regression with selecting egl config with msaa enabled albeit no msaa was selected in quality settings.</li>
<li>Android: Worked around bug in NVIDIA drivers resulting in texture samplers sometimes not being reported.</li>
<li>Android: Worked around compositor issue with DisplayBuffer alpha on pre-GB and kindle devices.</li>
<li>Android: Fixed performance regression when rendering dynamic geometry, like dynamic batching, GUI, particles, etc, on PowerVR / SGX hardware.</li>
<li>Android/iOS: Incorrect mouse hover events stemming from screen touches has been fixed.</li>
<li>iOS: fixed www status code handling.</li>
<li>iOS: fixed gyro accuracy problems when running on iOS 6.0 devices.</li>
<li>iOS: Better performance when setting RenderTexture that has different size from the current one.</li>
<li>iOS: removed unnecessary iPhone 5 splashscreen from iPad-only builds.</li>
<li>Mac OS X Editor: Fixed installing on Mac OS X 10.5.</li>
<li>Mac OS X Editor: Fixed crash on selecting RenderTexture on Mac OS X 10.7.5 with Radeon graphics card.</li>
<li>Editor: Fixed windows standalone icons alpha issues.</li>
<li>Native Client: Fixed Build &amp; Run on Chrome 23.</li>
<li>Fix export bitmap only working when the substance is tweaked right beforehand</li>
<li>Web Player: Fixed fullscreen mode initialization in IE10 on Windows 8. Web Player now tries to detect whether it is running in a sandbox.</li>
</ul>
