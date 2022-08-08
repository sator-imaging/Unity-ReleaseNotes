# Unity 3.4

https://unity3d.com/unity/whats-new/unity-3.4

## Unity iOS

- [Improvements](#improvements)
- [Fixes](#fixes)


### Improvements

*   Mesh skinning uses multi-threaded processing.
*   VFP skinning for cases where tangents are needed.
*   Added AOT options field to the player settings. Let's users to pass some additional AOT options, useful for "running out of trampoline" problem.
*   Terrain stripping enabled (if you don't use terrains, some Mono code can be stripped).
*   Implemented Application.systemLanguage.
*   Correctly detect iPad GSM and other devices.
*   Improved autorotation by fixing numerous issues with video playback and keyboard.
*   Trampoline code was refactored for easier reading/changing. Please replace your Xcode projects.
*   Bundle identifiers of pattern XXX.XXX are now allowed.

### Fixes

*   Fixed iOS SDK 4.3 App Store submission problems by working around linker bug: added -all\_load linker flag and small code hint to the main.mm.
*   Moved Xcode autorun phase after user postprocess script execution. Should improve 3rd party plugin integration experience.
*   Fixed iOS SDK 4.3 warnings about unaligned symbols.
*   Synchronization PlayerPrefs upon LoadLevel prevents very rare circumstances of loosing PlayerPrefs data when application is terminated unexpectedly.
*   Improved AOT build size when debugging is enabled.
*   Prevented GUI.WindowDragState from stripping.
*   Fixed the case when AOT was emitting debugging code when debugging checkbox is checked, but development build is unchecked.
*   Updated cpu-waits-gpu internal profiler counter for iOS 4.3.
*   Fixed VFP 1 bone skinning.
*   Fixed issue with screenshots not working when MSAA is enabled.
*   iPhoneSettings.generation now recognises iPad2.
*   Fixed WWW class memory leak when WWW object is disposed before completing download
*   Added SDK 4.3 selection in player settings.
*   Fixed material shader on iOS looks different from the Editor.
*   Unity projects will be closed in Xcode before updating them, which should fix some Xcode glitches.
*   Fixed AssetBundleCreateRequest stripping problem.
*   Fixed WWW out of memory problem when estimated download size is unknown.
*   Fixed GUIText stripping issue.
*   Fixed corner cases when libraries weren't symlinked properly. For portability reasons Unity runtime library symlink is off by default.
*   Fixed .cpp/.c native automatic plugin inclusion. Experimental support for .xib and .png files added.
*   Fixed WWW.EscapeURL() to escape URLs according to RFC.
*   Fixed issue on iPad2 with MSAA and alpha-blended geometry resulting in wireframe like artefacts. Please see SL-Reference/SL-AdvancedTopics/SL-PlatformDifferences for more thorough description.
*   Fixed iOS project postprocessing for Unity iOS Basic license and autorotation.
*   Fixed internal profiler using old-frame data, fixing negative values by the way.
*   Fixed simulator support for Xcode 4 + SDK 4.3.
*   Fixed WWWForm support.
*   Fixed simulator support for simulators <= 4.2.
*   Fixed CultureInfo code stripping.
*   Fixed input lag (accelerometer and touch input).
*   Fixed darken when "quad" combiner was used in shader.
*   Fixed crash when CADisplayLink is used with kFPS set to 60.
*   Fixed touch handling when non-Unity UIViews are used (cases with plugins).
*   Fixed occasional OpenGL errors being reported on iOS (when shaders that use uniform arrays are involved).
*   GC deadlock fix for multicore ARM devices.
*   Fixed invalid assembly names in RegisterMonoModules.cpp