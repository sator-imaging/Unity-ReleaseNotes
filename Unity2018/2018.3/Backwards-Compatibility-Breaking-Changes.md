# Unity 2018.3
https://unity3d.com/unity/whats-new/unity-2018.3.0

## Backwards Compatibility Breaking Changes

<ul>
<li><p>AI: Set the maximum number of OffMeshLinks that Unity can autogenerate and load in a static Scene NavMesh to 65535.</p></li>
<li><p>Android: Deprecated the Internal build system.</p></li>
<li><p>Android: On Adreno 4xx devices, Vulkan is now only used when it is the only selected Graphics API.</p></li>
<li><p>Android: Removed fastzip support.</p></li>
<li><p>Asset Import: Reorganized the Model tab of the Model Import Settings window to improve usability.</p></li>
<li><p>Audio: Simplified the Audio Profiler so that it is consistent with other profiler panes. The detailed view enables audio profiling so that Unity only carries this out when you need it.</p></li>
<li><p>Editor: Added 'Find references in Scene' to Component context menus.</p></li>
<li><p>Editor: Changed File menu item names. 'Save Scenes' is now 'Save' and 'Save Scene As' is now 'Save As', because they now save either a Prefab or Scenes depending on whether Prefab Mode is active. Unity still saves any dirty Assets when you use Ctrl/Cmd + S.</p></li>
<li><p>Editor: Changed Particle System module headers to only track the enabled state property instead of all properties. Also added Property menu choices to the context menu that appears when you right-click on the headers.</p></li>
<li><p>Editor: In USS files, <code>flex N</code> now means <code>flex N 0 auto</code>. It previously meant <code>flex N 0 0</code>.</p></li>
<li><p>Editor: Unity no longer automatically shows the Services window.</p></li>
<li><p>Editor: Updated event queueing in UIElements. When an event occurs that generates subsequent events, Unity now processes those subsequent events only when it has finished processing the current event.</p></li>
<li><p>Editor: Updated the UXML factory-related API. The old API is now marked obsolete.</p></li>
<li><p>Editor: When Unity builds assemblies in the Editor for the .NET 4.x scripting runtime, they now have .NET 4.6 (<code>NET_4_6 define</code>) set, regardless of when the .NET Standard 2.0 scripting profile is set (<code>NET_STANDARD_2_0 define</code>). This is because the scripting profile setting only affects players, and the Editor always uses the .NET 4.6 scripting profile.</p></li>
<li><p>GI: Renamed 'Recompile RSLS Shaders' menu item to "Recompile Lightmapping Shaders".</p></li>
<li><p>Graphics: Graphics emulation is now disabled whenever a Scriptable Render Pipeline is active.</p></li>
<li><p>Package Manager: Hid Assets subfolders for Packages from the Object Picker.</p></li>
<li><p>Particles: Added option to start Android app in non-fullscreen mode.</p></li>
<li><p>Scripting: Marked the <strong>.NET 3.5 Equivalent</strong> <strong>Scripting Runtime Version</strong> as deprecated.</p></li>
<li><p>Scripting Upgrade: Updated the default <strong>Api Compatibility Level</strong> to <strong>.NET Standard 2.0</strong>.</p></li>
<li><p>Web: WWW is now obsolete. Use UnityWebRequest instead.</p></li>
<li><p>WebGL: Added asm.js deprecation warning.</p></li>
<li><p>WebGL: Enabled WebAssembly traps in Development builds.</p></li>
<li><p>WebGL: Removed caching support for compiled WebAssembly module.</p></li>
<li><p>WebGL: Unity no longer uses glGetProcAddress internally.</p></li>
<li><p>WebGL: WebAssembly is now the default Linker Target on new WebGL projects.</p></li>
<li><p>XR: Moved Oculus support to a package. The package automatically downloads when you add Oculus to the Virtual Reality SDKs list.</p></li>
<li><p>XR: Moved OpenVR support to a package. The package automatically downloads when you add OpenVR to the Virtual Reality SDKs list.</p></li>
<li><p>XR: Moved Windows Mixed Reality support to a package. The package automatically downloads when you add Hololens/WindowsMR to the Virtual Reality SDKs list.</p></li>
<li><p>XR: Oculus Dash and Shared Depth Buffer options are now enabled by default in the Oculus XR settings.</p></li>
</ul>
