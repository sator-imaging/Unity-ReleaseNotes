# Unity 3.5.7

https://unity3d.com/unity/whats-new/unity-3.5.7

## Fixes



*   Android: Fixed Resources.Load() of prefabs consuming too much memory.
*   Android: Prevent NullPointerExceptions when using LVL on a device that is not signed in to Google Play.
*   Android: Fixed a lot of key store related problems.
*   Android: Fixed an optimization error which could cause javac to crash/fail when loading UnityPlayer class.
*   Android: Kindle Fire incorrectly reported having a camera.
*   Android: Fixed an issue where dictionary pop-ups would close the TouchScreenKeyboard.
*   Android: Application pause now cancels the TouchScreenKeyboard.
*   Android: Fixed auto-rotation problem in landscape/reversed landscape on Kindle Fire HD.
*   Android: Fixed a problem where multiple screen touches would lead to incorrect touch phases (especially during low framerate situations).
*   Android: The detection zone for screen touches resulting in increased tap count has been made resolution independent.
*   Android: SystemInfo.deviceUniqueIdentifier didn't automatically add the right permissions in the manifest.
*   Android: Fixed a problem with non-ASCII characters and keyboard input.
*   Android: Fixed a performance problem affecting the ARMv6 lib.
*   Android: Fixed rare crashes with dynamic batching in non-development player on PowerVR GPUs.
*   Android: Fixed performance regression with selecting egl config with msaa enabled albeit no msaa was selected in quality settings.
*   Android: Worked around bug in NVIDIA drivers resulting in texture samplers sometimes not being reported.
*   Android: Worked around compositor issue with DisplayBuffer alpha on pre-GB and kindle devices.
*   Android: Fixed performance regression when rendering dynamic geometry, like dynamic batching, GUI, particles, etc, on PowerVR / SGX hardware.
*   Android/iOS: Incorrect mouse hover events stemming from screen touches has been fixed.
*   iOS: fixed www status code handling.
*   iOS: fixed gyro accuracy problems when running on iOS 6.0 devices.
*   iOS: Better performance when setting RenderTexture that has different size from the current one.
*   iOS: removed unnecessary iPhone 5 splashscreen from iPad-only builds.
*   Mac OS X Editor: Fixed installing on Mac OS X 10.5.
*   Mac OS X Editor: Fixed crash on selecting RenderTexture on Mac OS X 10.7.5 with Radeon graphics card.
*   Editor: Fixed windows standalone icons alpha issues.
*   Native Client: Fixed Build & Run on Chrome 23.
*   Fix export bitmap only working when the substance is tweaked right beforehand
*   Web Player: Fixed fullscreen mode initialization in IE10 on Windows 8. Web Player now tries to detect whether it is running in a sandbox.