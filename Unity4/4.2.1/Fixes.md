# Unity 4.2.1
https://unity3d.com/unity/whats-new/unity-4.2.1

## Fixes

<ul>
<li>Android: Fixed an issue where a KeyNotFoundException was thrown when trying to deploy to the android emulator.</li>
<li>Android: Renamed exported .jar file from untiy-classes.jar to unity-classes.jar</li>
<li>Android: .meta files are now dropped before compilation of android libraries.</li>
<li>Android: Fixed for "Unable to find suitable jdk installation" on windows.</li>
<li>BlackBerry: Fixed issue where windows xp BlackBerry registration file path was not supported.</li>
<li>Fixed issue where windows xp BlackBerry registration file path was not supported.</li>
<li>Bugreporter: Fixed crash when submitting documentation bugs from OS X.</li>
<li>Documentation: Fixed that some editor classes were not showing up in the table of contents (Editor, EditorWindow).</li>
<li>Documentation: Monobehaviour page no longer has a dead link.</li>
<li>Documentation: "Inherited from ..." is showing for classes that inherit from other Unity classes.</li>
<li>Editor: Fixed editor crashing on older (SM2.0) GPUs.</li>
<li>Editor: Fixed that clicking cancel on the build progress bar would loose any unsaved work and would fail to load original scene.</li>
<li>Editor: Fixed memory leak occurring during Play/Stop and script compilation.</li>
<li>Editor: Fixed nested property drawers finding the wrong property drawer to use for rendering.</li>
<li>Editor: Asset store doesn't hang after downloading and importing assets.</li>
<li>Graphics: Fixed incorrect rendering order on meshes with multiple materials, introduced in Unity 4.2.</li>
<li>Graphics: Fixed multiple texture coordinate handling in immediate mode on OpenGL ES 3.0.</li>
<li>iOS: Fixed Input.compensateSensors not working with autorotation.</li>
<li>iOS: Fixed SystemInfo.deviceUniqueIdentifier returning udid on pre-iOS 7 devices that is different from the one returned in Unity 4.1.</li>
<li>iOS: Fixed status bar appearance on iOS 7.</li>
<li>iOS: Enforced proper screen mode and overscan compensation for AirPlay Displays.</li>
<li>iOS: Fixed PLCrashReporter name clash with Crittercism plugin.</li>
<li>iOS: Fixed crash when using SystemInfo.deviceUniqueIdentifier repeatedely.</li>
<li>Mecanim: Fixed culling crash bug happening in visibility callback.</li>
<li>Memory Profiler: Fixed freed textures in OpenGL showing up as a memory leak.</li>
<li>Mobile: Fixed Camera rendering to RenderTexture outside of normal rendering loop.</li>
<li>Mobile: Fixed possible OpenGL ES objects leaks when using several RenderTextures and destroying them.</li>
<li>Particles: Fixed editor crash when exiting playmode with particle system inspector showing.</li>
<li>Physics: Fixed incorrect collider/trigger exit messages being sent when paused.</li>
<li>Windows Store Apps: Fixed the leaked exceptions from sensors (typically happens when the system reports that a gyroscope exists but fails to set the properties) that break the rendering loop.</li>
<li>Windows Phone: Implemented Application.OpenURL.</li>
<li>Windows Phone: Fixed editor lock up when profiling and deploying new build at the same time.</li>
<li>Windows Phone: Fixed reloading of assets from bundles on fast resume.</li>
<li>Windows Phone and Windows Store Apps: 
<ul>
<li>Fixed WWW class constructor - now it never throws exceptions.</li>
<li>Fixed crash on accessing WheelHit.collider after calling WheelCollider.GetGroundHit().</li>
<li>Arrays with dimension bigger than one won't be serialized. For ex., byte [,]</li>
<li>Unity splash screen will be shown if you have a basic license, this is not a splash screen shown by OS, it's the one shown by Unity engine.</li>
</ul></li>
<li>Windows Store Apps: PlayerPrefs will correctly store huge strings.</li>
<li>OpenGL ES 3.0: Made various fixes and stability improvements.</li>
<li>OS X Web Player: Fixed crash when starting up the web player when an IME input mode is enabled.</li>
</ul>
