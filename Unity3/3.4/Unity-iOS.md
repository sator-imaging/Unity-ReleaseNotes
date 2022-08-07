# Unity 3.4
https://unity3d.com/unity/whats-new/unity-3.4

## Unity iOS


### Improvements
<ul>
<li>Mesh skinning uses multi-threaded processing.</li>
<li>VFP skinning for cases where tangents are needed.</li>
<li>Added AOT options field to the player settings. Let's users to pass some additional AOT options, useful for "running out of trampoline" problem.</li>
<li>Terrain stripping enabled (if you don't use terrains, some Mono code can be stripped).</li>
<li>Implemented Application.systemLanguage.</li>
<li>Correctly detect iPad GSM and other devices.</li>
<li>Improved autorotation by fixing numerous issues with video playback and keyboard.</li>
<li>Trampoline code was refactored for easier reading/changing. Please replace your Xcode projects.</li>
<li>Bundle identifiers of pattern XXX.XXX are now allowed.</li>
</ul>

### Fixes
<ul>
<li>Fixed iOS SDK 4.3 App Store submission problems by working around linker bug: added -all_load linker flag and small code hint to the main.mm.</li>
<li>Moved Xcode autorun phase after user postprocess script execution. Should improve 3rd party plugin integration experience.</li>
<li>Fixed iOS SDK 4.3 warnings about unaligned symbols.</li>
<li>Synchronization PlayerPrefs upon LoadLevel prevents very rare circumstances of loosing PlayerPrefs data when application is terminated unexpectedly.</li>
<li>Improved AOT build size when debugging is enabled.</li>
<li>Prevented GUI.WindowDragState from stripping.</li>
<li>Fixed the case when AOT was emitting debugging code when debugging checkbox is checked, but development build is unchecked.</li>
<li>Updated cpu-waits-gpu internal profiler counter for iOS 4.3.</li>
<li>Fixed VFP 1 bone skinning.</li>
<li>Fixed issue with screenshots not working when MSAA is enabled.</li>
<li>iPhoneSettings.generation now recognises iPad2.</li>
<li>Fixed WWW class memory leak when WWW object is disposed before completing download</li>
<li>Added SDK 4.3 selection in player settings.</li>
<li>Fixed material shader on iOS looks different from the Editor.</li>
<li>Unity projects will be closed in Xcode before updating them, which should fix some Xcode glitches.</li>
<li>Fixed AssetBundleCreateRequest stripping problem.</li>
<li>Fixed WWW out of memory problem when estimated download size is unknown.</li>
<li>Fixed GUIText stripping issue.</li>
<li>Fixed corner cases when libraries weren't symlinked properly. For portability reasons Unity runtime library symlink is off by default.</li>
<li>Fixed .cpp/.c native automatic plugin inclusion. Experimental support for .xib and .png files added.</li>
<li>Fixed WWW.EscapeURL() to escape URLs according to RFC.</li>
<li>Fixed issue on iPad2 with MSAA and alpha-blended geometry resulting in wireframe like artefacts. Please see SL-Reference/SL-AdvancedTopics/SL-PlatformDifferences for more thorough description.</li>
<li>Fixed iOS project postprocessing for Unity iOS Basic license and autorotation.</li>
<li>Fixed internal profiler using old-frame data, fixing negative values by the way.</li>
<li>Fixed simulator support for Xcode 4 + SDK 4.3.</li>
<li>Fixed WWWForm support.</li>
<li>Fixed simulator support for simulators &lt;= 4.2.</li>
<li>Fixed CultureInfo code stripping.</li>
<li>Fixed input lag (accelerometer and touch input).</li>
<li>Fixed darken when "quad" combiner was used in shader.</li>
<li>Fixed crash when CADisplayLink is used with kFPS set to 60.</li>
<li>Fixed touch handling when non-Unity UIViews are used (cases with plugins).</li>
<li>Fixed occasional OpenGL errors being reported on iOS (when shaders that use uniform arrays are involved).</li>
<li>GC deadlock fix for multicore ARM devices.</li>
<li>Fixed invalid assembly names in RegisterMonoModules.cpp</li>
</ul>
