# Unity 2018.1

https://unity3d.com/unity/whats-new/unity-2018.1.0

## Changes



*   Android: Input field character now always appears at the end of text when opening keyboard. ([966477](https://issuetracker.unity3d.com/issues/android-caret-is-always-at-the-beginning-of-existing-text-when-selecting-inputfield-with-line-type-set-to-multi-line))
    
*   Android: Newly created projects now default to ARMv7 CPU architecture.
    
*   Android: Removed support for `UnityPlayerProxyActivity`.
    
*   Android: SDK Platform 26 now required to build for Android.
    
*   Android: Unity now creates a 2048-bit RSA key for signing the APK.
    
*   Android: Updated JDK requirements to JDK 8. This a requirement from the latest Android SDK.
    
*   Animation: Starting play mode while editing an Avatar configuration will no longer change the current scene. ([916586](https://issuetracker.unity3d.com/issues/entering-play-mode-while-editing-avatar-throws-invalidoperationexception-error))
    
*   Audio: Added error message when calling `AudioSource.GetSpectrumData` or `AudioListener.GetSpectrumData` with float arrays that are not a power of 2 or are outside the valid range between 64 and 8192 samples. ([827154](https://issuetracker.unity3d.com/issues/audio-error-executing-m-drygroup-getspectrum-when-using-array-with-a-length-that-is-not-a-power-of-2))
    
*   Editor: Added `InspectorWindow.OnPostHeaderGUI` callback to allow drawing of custom GUI elements in the inspector window.
    
*   Editor: Compiling 'unsafe' C# code now requires the "Allow 'unsafe' code" option to be enabled in the player settings for predefined assemblies (Assembly-CSharp.dll, etc.) and in the inspector for Assembly Definition Files assemblies. Enabling this option will make Unity pass the `/unsafe` option to the C# compiler when compiling scripts.
    
*   Editor: Removed MonoDevelop 5.9.6 from macOS and Windows installers and deprecated support for it in Unity. Visual Studio for Mac is installed as the C# code editor on macOS and Visual Studio 2017 Community on Windows.
    
*   Editor: Removed the "Intensity" float field next to HDR texture fields in Material editors. Use the exposure controls in the Color Picker instead.
    
*   Editor: Substituted "intensity" float field in the Static Emissives tab of the Light Explorer for HDR color field; instead use the exposure controls in Color Picker.
    
*   Editor: The plug-in code that creates Textures used in rendering with IMGUI should now avoid specifying them in linear space (i.e. should set the linear parameter to false in the `Texture2D` constructor). Otherwise, GUI elements drawn with such textures might look washed out when the project is working in Linear space (Player Settings > Color space: Linear). (908904)
    
*   GI: Support for hiding and disabling GI features when making a render pipeline.
    
*   Graphics: Deprecated `PlayerSettings.defaultIsFullscreen`. `Use PlayerSettings.fullscreenMode` instead.
    
*   Graphics: GraphicsSettings shaders are no longer loaded on startup.
    
*   Graphics: Metal tessellation: Improved shader importing error reporting for when features are unsupported.
    
*   IL2CPP: Deprecated `BuildOptions.IL2CPP`, which never actually did anything. ([986326](https://issuetracker.unity3d.com/issues/buildplayer-with-buildoptions-dot-il2cpp-does-not-output-an-il2cpp-build))
    
*   iOS: Increased min target iOS version to 8.0.
    
*   iOS: iOS now links with Security framework by default. To remove it, set a pre-processor define `DISABLE_WEBREQUEST_CERTIFICATE_CALLBACK` and remove "Security" from the list of linked frameworks in Xcode.
    
*   iOS: `ScreenOrientation.Unknown` is deprecated.
    
*   OSX: Metal is now the default graphics backend for Editor.
    
*   Package Manager: Unity Package Manager project sub-folder was moved from _UnityPackageManager_ to _Packages_. This is to align the physical path with the logical path of packages. Notes:
    
    *   Projects configured with a _NuGet_ should change their configuration to point to another folder (default repository path for _NuGet_ configuration is \\packages). The risk of _NuGet_ and _Unity Package Manager_ sharing the _Packages_ folder is minimal, but we suggest to separate them nonetheless to avoid any issues.
    *   When opening a project created with a previous version, a migration flow will copy the content of the _UnityPackageManager_ folder to the _Packages_ folder. It is left to the project maintainer to erase the _UnityPackageManager_ folder and update source control configuration.
*   Services: Replaced web-based Collab history window with improved RMGUI version.
    
*   Substance: Built-in support for Substance Designer materials is deprecated in Unity 2017.3, and will be removed in 2018.1. To continue using Substance Designer materials in Unity 2018.1, you will need to install a suitable third-party external importer from the Asset Store.
    
*   Universal Windows Platform: Build & Run now defaults to 64-bit player when running on local machine.
    
*   Web: AssetBundle-related parts of UnityWebRequest have been split into a new module, allowing UnityWebRequest to be used without pulling in AssetBundle module. API change: `UnityWebRequest.GetAssetBundle` -> `UnityWebRequestAssetBundle.GetAssetBundle`.
    
*   WebGL: Removed experimental label from WebAssembly linker target.
    
*   Windows: Removed support for Windows XP in Standalone Player builds. Windows Vista is the minimum supported OS now.
    
*   Windows: The Build Player location selection dialog now asks for a folder rather than a file name when building Windows standalone player. The `BuildPipeline.BuildPlayer` API is not affected by this change. ([995320](https://issuetracker.unity3d.com/issues/windows-standalone-build-getting-more-stuff-dumped-into-root-build-folder))
    
*   XR: Standalone UWP applications targeting Windows Mixed Reality now cause the OS to notify you if the Mixed Reality components are not installed or a headset is not connected, rather than silently falling back to non-VR desktop mode.
    
*   XR: Updated Google VR:
    
    *   to 1.130 for Android
    *   to 1.120 for iOS