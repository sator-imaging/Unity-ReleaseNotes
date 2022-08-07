# Unity 3.4
https://unity3d.com/unity/whats-new/unity-3.4

## Unity Android


### Improvements
<ul>
<li>Load times with both Scene and Resources have been improved.</li>
<li>Mesh skinning utilizes NEON optimizations (if supported by the CPU).</li>
<li>Mesh skinning utilizes VFP optimizations also for cases where tangents are needed (NVIDIA Tegra 2).</li>
<li>Mesh skinning uses multi-threaded processing.</li>
<li>AssetBundle can be loaded from memory with AssetBundle.CreateFromMemory.</li>
<li>Added support for autorotation screen orientation.</li>
<li>Texture Compression override for DXT/PVRTC/ATC instead of ETC/RGBA16 when targeting a specific device range.</li>
<li>Build times have been improved, especially when the Resources folder is populated with prefabs.</li>
<li>NativeActivity is selected automatically on devices running Gingerbread (OS 2.3) or above.</li>
<li>ATC (Qualcomm Snapdragon) texture compression is now supported.</li>
<li>The build process automatically adds elements to the manifest for improved Market filtering.</li>
<li>Exposed audio latency (mixing buffer size) setting.</li>
</ul>

### Fixes
<ul>
<li>Using GLES 1.1 mode on NVIDIA Tegra 2-based devices no longer causes the splash screen to hang.</li>
<li>Fixed deadlock problem on multi-core Snapdragon based devices (e.g. HTC Sensation / HTC Evo3D) where most applications would hang.</li>
<li>Fixed loading time regression with the Android 3.1 update for Motorola Xoom.</li>
<li>Scene loading bug was fixed, improving loading performance in some cases and getting rid of hiccups in other.</li>
<li>Fixed hang while "Detecting Android SDK" during Build(&amp;Run).</li>
<li>WWW data no longer truncated because of compressed data mismatching the announced content length.</li>
<li>Some mesh configurations could cause a crash in the mesh skinning.</li>
<li>Added workaround for crashes on Samsung GalaxyS II (ARM Mali-400) due to a bug in the graphics driver.</li>
<li>Fixed an illegal reference count of a JNI object, which resulted in a crash under Icecream Sandwich.</li>
<li>Custom application icon now works on Unity Android Basic license.</li>
<li>Workaround for some Androids not handling glPolygonOffset correctly (fixes blob shadows).</li>
<li>Crash when using Object[] as return value with AndroidJavaObject has been fixed.</li>
<li>Xperia PLAY touchpad Y-coordinates were reported incorrectly. This has been fixed but also means that games need to be recalibrated.</li>
<li>Fixed occasional graphical glitches on Qualcomm Snapdragon-based devices.</li>
<li>Application.Quit caused application to crash while cleaning up resources.</li>
<li>Fixed problem where an empty StreamingAssets folder would fail the project build.</li>
<li>Synchronization of PlayerPrefs upon LoadLevel now prevents very rare circumstances of loosing PlayerPrefs data when application is terminated unexpectedly.</li>
<li>Fixed bytecode stripping on Windows.</li>
<li>Fixed internal profiler using old-frame data, fixing negative values by the way.</li>
<li>Fixed CultureInfo stripping.</li>
<li>Fixed issue where File.Delete would fail if the file was located on the SD card.</li>
<li>Fixed RenderTexture broken after losing/regaining focus when used on GL ES 1.1.</li>
<li>Initialization of the Audio subsystem no longer crashes should it fail.</li>
<li>A java.util.HashMap assert when using WWW with CheckJNI enabled has been removed.</li>
<li>Fixed issue where the "quad" combiner in the shader would cause the output to darken.</li>
</ul>
