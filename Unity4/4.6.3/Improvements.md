# Unity 4.6.3
https://unity3d.com/unity/whats-new/unity-4.6.3

## Improvements

<ul>
<li>Asset Loading: Added names of affected assets to the error message when a hash collision occurs while generating asset bundles.</li>
<li>BlackBerry: Passport device now supports landscape orientation.</li>
<li>Documentation: Fixed broken links, particularly in UI docs.</li>
<li>Documentation: Updated documentation for iOS 64-bit and UI.</li>
<li>iOS: Added launch screen support for iPhones.</li>
<li>iOS: Added PlayerSettings.shortBundleVersion which is linked to the CFBundleShortVersionString stored in the Info.plist file; this relates to short public version string. PlayerSettings.bundleVersion can now be used for full incremental build version and is linked to CFBundleVersion.</li>
<li>iOS: Allow to set compile flags for already existing files in Xcode API.</li>
<li>iOS/IL2CPP: Added support for async delegates (BeginInvoke/EndInvoke).</li>
<li>iOS/IL2CPP: Disabled Script Debugging option when building iOS projects with IL2CPP scripting backend.</li>
<li>iOS/IL2CPP: Implemented .NET classes: for ThreadPool, Asynchronous Sockets, WebRequest.</li>
<li>iOS/IL2CPP: Optimize methods that use string literals and memory used for string literals.</li>
<li>Shaders: Added UNITY_NO_SCREENSPACE_SHADOWS, UNITY_NO_RGBM, UNITY_NO_DXT5nm macros; better to check for these instead of hardcoding checks for "GLES or GLES3" and similar.</li>
<li>Shaders: MRT support on OpenGL ES 2.0 via GL_EXT_draw_buffers.</li>
<li>Shaders: Support for GL_EXT_shader_framebuffer_fetch. If you have a pixel shader with an "inout" color, it gets translated to use shader framebuffer fetch on GLES2/GLES3/Metal. Use UNITY_FRAMEBUFFER_FETCH_AVAILABLE macro in shaders to conditionally enclose that.</li>
<li>UI: Exposed IsAddedToManager on Behaviour.</li>
<li>UI: Improved ordering for the EventOrdering.</li>
<li>UI: Optimized adding/removing Graphics to a Canvas. It should be much cheaper to enable and disable Graphics now.</li>
</ul>
