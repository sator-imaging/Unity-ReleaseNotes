# Unity 4.2

https://unity3d.com/unity/whats-new/unity-4.2

## Mobile Features



*   Android: Added support for Android Library Projects (no compilation support, so the libraries have to be pre-compiled).
*   Android: AndroidJavaProxy - Support for implementing Java interfaces in C#.
*   Android: Editor can now update the Android SDK if it does not match the required dependencies.
*   iOS: Added CrashReporter API for crash detection and extraction (requires Unity Pro).
*   iOS: Now you can setup iOS PlayerSettings, texture import overrides and build iOS AssetBundles from Windows Editor. Building an actual iOS player still requires Mac OS X & Xcode.
*   iOS: WebCamTexture can be set non-readable (prior to playback), which allows it to output from camera directly to texture, avoiding extra memory copies.
*   Editor: When in mobile graphics emulation mode, editor will show a warning when RenderTexture usage is not optimal for tile-based or multi-GPU systems. Use RenderTexture.MarkRestoreExpected() to suppress the warning if needed.