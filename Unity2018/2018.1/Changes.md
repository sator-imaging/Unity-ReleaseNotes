# Unity 2018.1
https://unity3d.com/unity/whats-new/unity-2018.1.0

## Changes

<ul>
<li><p>Android: Input field character now always appears at the end of text when opening keyboard. (<a href="https://issuetracker.unity3d.com/issues/android-caret-is-always-at-the-beginning-of-existing-text-when-selecting-inputfield-with-line-type-set-to-multi-line">966477</a>)</p></li>
<li><p>Android: Newly created projects now default to ARMv7 CPU architecture.</p></li>
<li><p>Android: Removed support for <code>UnityPlayerProxyActivity</code>.</p></li>
<li><p>Android: SDK Platform 26 now required to build for Android.</p></li>
<li><p>Android: Unity now creates a 2048-bit RSA key for signing the APK.</p></li>
<li><p>Android: Updated JDK requirements to JDK 8.  This a requirement from the latest Android SDK.</p></li>
<li><p>Animation: Starting play mode while editing an Avatar configuration will no longer change the current scene. (<a href="https://issuetracker.unity3d.com/issues/entering-play-mode-while-editing-avatar-throws-invalidoperationexception-error">916586</a>)</p></li>
<li><p>Audio: Added error message when calling <code>AudioSource.GetSpectrumData</code> or <code>AudioListener.GetSpectrumData</code> with float arrays that are not a power of 2 or are outside the valid range between 64 and 8192 samples. (<a href="https://issuetracker.unity3d.com/issues/audio-error-executing-m-drygroup-getspectrum-when-using-array-with-a-length-that-is-not-a-power-of-2">827154</a>)</p></li>
<li><p>Editor: Added <code>InspectorWindow.OnPostHeaderGUI</code> callback to allow drawing of custom GUI elements in the inspector window.</p></li>
<li><p>Editor: Compiling 'unsafe' C# code now requires the "Allow 'unsafe' code" option to be enabled in the player settings for predefined assemblies (Assembly-CSharp.dll, etc.) and in the inspector for Assembly Definition Files assemblies. Enabling this option will make Unity pass the <code>/unsafe</code> option to the C# compiler when compiling scripts.</p></li>
<li><p>Editor: Removed MonoDevelop 5.9.6 from macOS and Windows installers and deprecated support for it in Unity. Visual Studio for Mac is installed as the C# code editor on macOS and Visual Studio 2017 Community on Windows.</p></li>
<li><p>Editor: Removed the "Intensity" float field next to HDR texture fields in Material editors. Use the exposure controls in the Color Picker instead.</p></li>
<li><p>Editor: Substituted "intensity" float field in the Static Emissives tab of the Light Explorer for HDR color field; instead use the exposure controls in Color Picker.</p></li>
<li><p>Editor: The plug-in code that creates Textures used in rendering with IMGUI should now avoid specifying them in linear space (i.e. should set the linear parameter to false in the <code>Texture2D</code> constructor). Otherwise, GUI elements drawn with such textures might look washed out when the project is working in Linear space (Player Settings &gt; Color space: Linear). (908904)</p></li>
<li><p>GI: Support for hiding and disabling GI features when making a render pipeline.</p></li>
<li><p>Graphics: Deprecated <code>PlayerSettings.defaultIsFullscreen</code>.  <code>Use PlayerSettings.fullscreenMode</code> instead.</p></li>
<li><p>Graphics: GraphicsSettings shaders are no longer loaded on startup.</p></li>
<li><p>Graphics: Metal tessellation: Improved shader importing error reporting for when features are unsupported.</p></li>
<li><p>IL2CPP: Deprecated <code>BuildOptions.IL2CPP</code>, which never actually did anything. (<a href="https://issuetracker.unity3d.com/issues/buildplayer-with-buildoptions-dot-il2cpp-does-not-output-an-il2cpp-build">986326</a>)</p></li>
<li><p>iOS: Increased min target iOS version to 8.0.</p></li>
<li><p>iOS: iOS now links with Security framework by default. To remove it, set a pre-processor define <code>DISABLE_WEBREQUEST_CERTIFICATE_CALLBACK</code> and remove "Security" from the list of linked frameworks in Xcode.</p></li>
<li><p>iOS: <code>ScreenOrientation.Unknown</code> is deprecated.</p></li>
<li><p>OSX: Metal is now the default graphics backend for Editor.</p></li>
<li><p>Package Manager: Unity Package Manager project sub-folder was moved from <em>UnityPackageManager</em> to <em>Packages</em>. This is to align the physical path with the logical path of packages. Notes:</p> 
<ul>
<li>Projects configured with a <em>NuGet</em> should change their configuration to point to another folder (default repository path for <em>NuGet</em> configuration is \packages). The risk of <em>NuGet</em> and <em>Unity Package Manager</em> sharing the <em>Packages</em> folder is minimal, but we suggest to separate them nonetheless to avoid any issues.</li>
<li>When opening a project created with a previous version, a migration flow will copy the content of the <em>UnityPackageManager</em> folder to the <em>Packages</em> folder.  It is left to the project maintainer to erase the <em>UnityPackageManager</em> folder and update source control configuration.</li>
</ul></li>
<li><p>Services: Replaced web-based Collab history window with improved RMGUI version.</p></li>
<li><p>Substance: Built-in support for Substance Designer materials is deprecated in Unity 2017.3, and will be removed in 2018.1. To continue using Substance Designer materials in Unity 2018.1, you will need to install a suitable third-party external importer from the Asset Store.</p></li>
<li><p>Universal Windows Platform: Build &amp; Run now defaults to 64-bit player when running on local machine.</p></li>
<li><p>Web: AssetBundle-related parts of UnityWebRequest have been split into a new module, allowing UnityWebRequest to be used without pulling in AssetBundle module.  API change: <code>UnityWebRequest.GetAssetBundle</code> -&gt; <code>UnityWebRequestAssetBundle.GetAssetBundle</code>.</p></li>
<li><p>WebGL: Removed experimental label from WebAssembly linker target.</p></li>
<li><p>Windows: Removed support for Windows XP in Standalone Player builds. Windows Vista is the minimum supported OS now.</p></li>
<li><p>Windows: The Build Player location selection dialog now asks for a folder rather than a file name when building Windows standalone player. The <code>BuildPipeline.BuildPlayer</code> API is not affected by this change. (<a href="https://issuetracker.unity3d.com/issues/windows-standalone-build-getting-more-stuff-dumped-into-root-build-folder">995320</a>)</p></li>
<li><p>XR: Standalone UWP applications targeting Windows Mixed Reality now cause the OS to notify you if the Mixed Reality components are not installed or a headset is not connected, rather than silently falling back to non-VR desktop mode.</p></li>
<li><p>XR: Updated Google VR:</p> 
<ul>
<li>to 1.130 for Android</li>
<li>to 1.120 for iOS</li>
</ul></li>
</ul>
