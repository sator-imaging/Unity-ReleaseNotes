# Unity 3.4

https://unity3d.com/unity/whats-new/unity-3.4

## Unity Android

- [Improvements](#improvements)
- [Fixes](#fixes)


### Improvements

*   Load times with both Scene and Resources have been improved.
*   Mesh skinning utilizes NEON optimizations (if supported by the CPU).
*   Mesh skinning utilizes VFP optimizations also for cases where tangents are needed (NVIDIA Tegra 2).
*   Mesh skinning uses multi-threaded processing.
*   AssetBundle can be loaded from memory with AssetBundle.CreateFromMemory.
*   Added support for autorotation screen orientation.
*   Texture Compression override for DXT/PVRTC/ATC instead of ETC/RGBA16 when targeting a specific device range.
*   Build times have been improved, especially when the Resources folder is populated with prefabs.
*   NativeActivity is selected automatically on devices running Gingerbread (OS 2.3) or above.
*   ATC (Qualcomm Snapdragon) texture compression is now supported.
*   The build process automatically adds elements to the manifest for improved Market filtering.
*   Exposed audio latency (mixing buffer size) setting.

### Fixes

*   Using GLES 1.1 mode on NVIDIA Tegra 2-based devices no longer causes the splash screen to hang.
*   Fixed deadlock problem on multi-core Snapdragon based devices (e.g. HTC Sensation / HTC Evo3D) where most applications would hang.
*   Fixed loading time regression with the Android 3.1 update for Motorola Xoom.
*   Scene loading bug was fixed, improving loading performance in some cases and getting rid of hiccups in other.
*   Fixed hang while "Detecting Android SDK" during Build(&Run).
*   WWW data no longer truncated because of compressed data mismatching the announced content length.
*   Some mesh configurations could cause a crash in the mesh skinning.
*   Added workaround for crashes on Samsung GalaxyS II (ARM Mali-400) due to a bug in the graphics driver.
*   Fixed an illegal reference count of a JNI object, which resulted in a crash under Icecream Sandwich.
*   Custom application icon now works on Unity Android Basic license.
*   Workaround for some Androids not handling glPolygonOffset correctly (fixes blob shadows).
*   Crash when using Object\[\] as return value with AndroidJavaObject has been fixed.
*   Xperia PLAY touchpad Y-coordinates were reported incorrectly. This has been fixed but also means that games need to be recalibrated.
*   Fixed occasional graphical glitches on Qualcomm Snapdragon-based devices.
*   Application.Quit caused application to crash while cleaning up resources.
*   Fixed problem where an empty StreamingAssets folder would fail the project build.
*   Synchronization of PlayerPrefs upon LoadLevel now prevents very rare circumstances of loosing PlayerPrefs data when application is terminated unexpectedly.
*   Fixed bytecode stripping on Windows.
*   Fixed internal profiler using old-frame data, fixing negative values by the way.
*   Fixed CultureInfo stripping.
*   Fixed issue where File.Delete would fail if the file was located on the SD card.
*   Fixed RenderTexture broken after losing/regaining focus when used on GL ES 1.1.
*   Initialization of the Audio subsystem no longer crashes should it fail.
*   A java.util.HashMap assert when using WWW with CheckJNI enabled has been removed.
*   Fixed issue where the "quad" combiner in the shader would cause the output to darken.