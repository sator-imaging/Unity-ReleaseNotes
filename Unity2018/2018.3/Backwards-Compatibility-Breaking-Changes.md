# Unity 2018.3

https://unity3d.com/unity/whats-new/unity-2018.3.0

## Backwards Compatibility Breaking Changes



*   AI: Set the maximum number of OffMeshLinks that Unity can autogenerate and load in a static Scene NavMesh to 65535.
    
*   Android: Deprecated the Internal build system.
    
*   Android: On Adreno 4xx devices, Vulkan is now only used when it is the only selected Graphics API.
    
*   Android: Removed fastzip support.
    
*   Asset Import: Reorganized the Model tab of the Model Import Settings window to improve usability.
    
*   Audio: Simplified the Audio Profiler so that it is consistent with other profiler panes. The detailed view enables audio profiling so that Unity only carries this out when you need it.
    
*   Editor: Added 'Find references in Scene' to Component context menus.
    
*   Editor: Changed File menu item names. 'Save Scenes' is now 'Save' and 'Save Scene As' is now 'Save As', because they now save either a Prefab or Scenes depending on whether Prefab Mode is active. Unity still saves any dirty Assets when you use Ctrl/Cmd + S.
    
*   Editor: Changed Particle System module headers to only track the enabled state property instead of all properties. Also added Property menu choices to the context menu that appears when you right-click on the headers.
    
*   Editor: In USS files, `flex N` now means `flex N 0 auto`. It previously meant `flex N 0 0`.
    
*   Editor: Unity no longer automatically shows the Services window.
    
*   Editor: Updated event queueing in UIElements. When an event occurs that generates subsequent events, Unity now processes those subsequent events only when it has finished processing the current event.
    
*   Editor: Updated the UXML factory-related API. The old API is now marked obsolete.
    
*   Editor: When Unity builds assemblies in the Editor for the .NET 4.x scripting runtime, they now have .NET 4.6 (`NET_4_6 define`) set, regardless of when the .NET Standard 2.0 scripting profile is set (`NET_STANDARD_2_0 define`). This is because the scripting profile setting only affects players, and the Editor always uses the .NET 4.6 scripting profile.
    
*   GI: Renamed 'Recompile RSLS Shaders' menu item to "Recompile Lightmapping Shaders".
    
*   Graphics: Graphics emulation is now disabled whenever a Scriptable Render Pipeline is active.
    
*   Package Manager: Hid Assets subfolders for Packages from the Object Picker.
    
*   Particles: Added option to start Android app in non-fullscreen mode.
    
*   Scripting: Marked the **.NET 3.5 Equivalent** **Scripting Runtime Version** as deprecated.
    
*   Scripting Upgrade: Updated the default **Api Compatibility Level** to **.NET Standard 2.0**.
    
*   Web: WWW is now obsolete. Use UnityWebRequest instead.
    
*   WebGL: Added asm.js deprecation warning.
    
*   WebGL: Enabled WebAssembly traps in Development builds.
    
*   WebGL: Removed caching support for compiled WebAssembly module.
    
*   WebGL: Unity no longer uses glGetProcAddress internally.
    
*   WebGL: WebAssembly is now the default Linker Target on new WebGL projects.
    
*   XR: Moved Oculus support to a package. The package automatically downloads when you add Oculus to the Virtual Reality SDKs list.
    
*   XR: Moved OpenVR support to a package. The package automatically downloads when you add OpenVR to the Virtual Reality SDKs list.
    
*   XR: Moved Windows Mixed Reality support to a package. The package automatically downloads when you add Hololens/WindowsMR to the Virtual Reality SDKs list.
    
*   XR: Oculus Dash and Shared Depth Buffer options are now enabled by default in the Oculus XR settings.