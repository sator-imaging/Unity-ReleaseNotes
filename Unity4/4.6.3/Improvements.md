# Unity 4.6.3

https://unity3d.com/unity/whats-new/unity-4.6.3

## Improvements



*   Asset Loading: Added names of affected assets to the error message when a hash collision occurs while generating asset bundles.
*   BlackBerry: Passport device now supports landscape orientation.
*   Documentation: Fixed broken links, particularly in UI docs.
*   Documentation: Updated documentation for iOS 64-bit and UI.
*   iOS: Added launch screen support for iPhones.
*   iOS: Added PlayerSettings.shortBundleVersion which is linked to the CFBundleShortVersionString stored in the Info.plist file; this relates to short public version string. PlayerSettings.bundleVersion can now be used for full incremental build version and is linked to CFBundleVersion.
*   iOS: Allow to set compile flags for already existing files in Xcode API.
*   iOS/IL2CPP: Added support for async delegates (BeginInvoke/EndInvoke).
*   iOS/IL2CPP: Disabled Script Debugging option when building iOS projects with IL2CPP scripting backend.
*   iOS/IL2CPP: Implemented .NET classes: for ThreadPool, Asynchronous Sockets, WebRequest.
*   iOS/IL2CPP: Optimize methods that use string literals and memory used for string literals.
*   Shaders: Added UNITY\_NO\_SCREENSPACE\_SHADOWS, UNITY\_NO\_RGBM, UNITY\_NO\_DXT5nm macros; better to check for these instead of hardcoding checks for "GLES or GLES3" and similar.
*   Shaders: MRT support on OpenGL ES 2.0 via GL\_EXT\_draw\_buffers.
*   Shaders: Support for GL\_EXT\_shader\_framebuffer\_fetch. If you have a pixel shader with an "inout" color, it gets translated to use shader framebuffer fetch on GLES2/GLES3/Metal. Use UNITY\_FRAMEBUFFER\_FETCH\_AVAILABLE macro in shaders to conditionally enclose that.
*   UI: Exposed IsAddedToManager on Behaviour.
*   UI: Improved ordering for the EventOrdering.
*   UI: Optimized adding/removing Graphics to a Canvas. It should be much cheaper to enable and disable Graphics now.