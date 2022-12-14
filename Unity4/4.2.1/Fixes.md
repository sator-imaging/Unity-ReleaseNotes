# Unity 4.2.1

https://unity3d.com/unity/whats-new/unity-4.2.1

## Fixes



*   Android: Fixed an issue where a KeyNotFoundException was thrown when trying to deploy to the android emulator.
*   Android: Renamed exported .jar file from untiy-classes.jar to unity-classes.jar
*   Android: .meta files are now dropped before compilation of android libraries.
*   Android: Fixed for "Unable to find suitable jdk installation" on windows.
*   BlackBerry: Fixed issue where windows xp BlackBerry registration file path was not supported.
*   Fixed issue where windows xp BlackBerry registration file path was not supported.
*   Bugreporter: Fixed crash when submitting documentation bugs from OS X.
*   Documentation: Fixed that some editor classes were not showing up in the table of contents (Editor, EditorWindow).
*   Documentation: Monobehaviour page no longer has a dead link.
*   Documentation: "Inherited from ..." is showing for classes that inherit from other Unity classes.
*   Editor: Fixed editor crashing on older (SM2.0) GPUs.
*   Editor: Fixed that clicking cancel on the build progress bar would loose any unsaved work and would fail to load original scene.
*   Editor: Fixed memory leak occurring during Play/Stop and script compilation.
*   Editor: Fixed nested property drawers finding the wrong property drawer to use for rendering.
*   Editor: Asset store doesn't hang after downloading and importing assets.
*   Graphics: Fixed incorrect rendering order on meshes with multiple materials, introduced in Unity 4.2.
*   Graphics: Fixed multiple texture coordinate handling in immediate mode on OpenGL ES 3.0.
*   iOS: Fixed Input.compensateSensors not working with autorotation.
*   iOS: Fixed SystemInfo.deviceUniqueIdentifier returning udid on pre-iOS 7 devices that is different from the one returned in Unity 4.1.
*   iOS: Fixed status bar appearance on iOS 7.
*   iOS: Enforced proper screen mode and overscan compensation for AirPlay Displays.
*   iOS: Fixed PLCrashReporter name clash with Crittercism plugin.
*   iOS: Fixed crash when using SystemInfo.deviceUniqueIdentifier repeatedely.
*   Mecanim: Fixed culling crash bug happening in visibility callback.
*   Memory Profiler: Fixed freed textures in OpenGL showing up as a memory leak.
*   Mobile: Fixed Camera rendering to RenderTexture outside of normal rendering loop.
*   Mobile: Fixed possible OpenGL ES objects leaks when using several RenderTextures and destroying them.
*   Particles: Fixed editor crash when exiting playmode with particle system inspector showing.
*   Physics: Fixed incorrect collider/trigger exit messages being sent when paused.
*   Windows Store Apps: Fixed the leaked exceptions from sensors (typically happens when the system reports that a gyroscope exists but fails to set the properties) that break the rendering loop.
*   Windows Phone: Implemented Application.OpenURL.
*   Windows Phone: Fixed editor lock up when profiling and deploying new build at the same time.
*   Windows Phone: Fixed reloading of assets from bundles on fast resume.
*   Windows Phone and Windows Store Apps:
    *   Fixed WWW class constructor - now it never throws exceptions.
    *   Fixed crash on accessing WheelHit.collider after calling WheelCollider.GetGroundHit().
    *   Arrays with dimension bigger than one won't be serialized. For ex., byte \[,\]
    *   Unity splash screen will be shown if you have a basic license, this is not a splash screen shown by OS, it's the one shown by Unity engine.
*   Windows Store Apps: PlayerPrefs will correctly store huge strings.
*   OpenGL ES 3.0: Made various fixes and stability improvements.
*   OS X Web Player: Fixed crash when starting up the web player when an IME input mode is enabled.