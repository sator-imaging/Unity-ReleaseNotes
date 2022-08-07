# Unity 2018.3.8
https://unity3d.com/unity/whats-new/2018.3.8

## Fixes

<ul>
<li><p>2D: Fixed case of Editor crashing on <code>WorldContactFilter2D::ShouldCollide</code> when trying to destroy Tilemap. (1126791)</p></li>
<li><p>2D: Fixed case of Tile Animation showing a wrong Sprite when Tilemap is deactivated and reactivated. (1126772)</p></li>
<li><p>2D: Fixed issue where Tilemap Collider Physics Shape/s were not updating when a single Tile was removed. (1126789)</p></li>
<li><p>2D: Fixed to clean up Preview Tiles when painting on a Tilemap when an asset is saved. (1126776)</p></li>
<li><p>2D: Fixed <code>NullReferenceException</code> when painting with a Tile Palette without a valid Tilemap component. (<a href="https://issuetracker.unity3d.com/issues/2d-painting-in-tile-palette-window-after-deleting-child-gameobject-from-tile-palette-prefab-throws-nullreferenceexception">1120310</a>, 1126781)</p></li>
<li><p>2D: We now use Grid Cell Layout instead of Tile Orientation for doing Grid Cell picking when painting on a Tilemap. (1126779)</p></li>
<li><p>Android: Fixed null exception on GC when Java class is not found. (1128659)</p></li>
<li><p>Android: UnityWebRequest: Relaxed format requirements for jar:file uris. (<a href="https://issuetracker.unity3d.com/issues/accessing-nonexistent-streaming-asset-on-android-with-incorrect-number-of-slashes-in-the-url-produces-incorrect-error">1117525</a>, 1128887)</p></li>
<li><p>Asset Import: Fixed crash when reading a meta file with a "Byte Order Mark". (1128853)</p></li>
<li><p>Editor: Fixed Instability in IConnectionStateInternal_HasAtLeastTheDefaultAmountOfAvailableConnections . (1103431)</p></li>
<li><p>GI: Fixed an issue were newly loaded scenes with bounce count 3 would not bake any indirect light. (1129335)</p></li>
<li><p>Graphics: Fixed for [ASAN] Memory use after free in GpuProgramMetal::ApplyGpuProgram. (1127838)</p></li>
<li><p>Graphics: Fixed issue where  "GetGfxDevice() should only be called from main thread" errors are thrown and crashes in Play Mode later on. (1124135)</p></li>
<li><p>Graphics: Fixed memory leak in batchmode when rendering on desktop platforms . (<a href="https://issuetracker.unity3d.com/issues/unity-runtime-has-huge-memory-leak-while-rendering-in-batchmode-on-desktop-platforms">1093649</a>, 1102280)</p></li>
<li><p>Graphics: Vulkan: Fixed a crash when draw call was made without an active GPU program. (1126841)</p></li>
<li><p>IL2CPP: Fixed correct flow control code not generated for try/catch/finally handling with async methods in C#. (1122868)</p></li>
<li><p>IL2CPP: Fixed step-into debugging for some generic methods. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-failing-to-step-into-generic-methods-while-debugging-il2cpp-build">1124177</a>)</p></li>
<li><p>IL2CPP: Improved the performance of WaitOne, WaitAny, and WaitAll on Windows platforms. (1111339)</p></li>
<li><p>IMGUI: Maximizing the player in the windowed mode sets it to Maximized Window mode. (<a href="https://issuetracker.unity3d.com/issues/buttons-dont-record-input-when-the-window-is-maximized-and-then-set-to-2560x1080-resolution">1085673</a>, 1127910)</p></li>
<li><p>iOS: Fixed background audio stopping when startin an Unity app on iOS. (1115948)</p></li>
<li><p>iOS: Fixed issue where an App won't be automatically deployed to Device when building project via Build and Run. (1114541)</p></li>
<li><p>Linux: Fixed editor UI breaking with Screen.SetResolution is called. (<a href="https://issuetracker.unity3d.com/issues/editor-ui-breaks-when-screen-dot-setresolution-is-called">1057513</a>, 1128667)</p></li>
<li><p>Mobile: Fixed il2cpp player build when engine stripping is enable and AssetImporter log is not empty. (1115957)</p></li>
<li><p>Multiplayer: Fixed memory leak in TLS connections, affecting Windows/Linux/Mac/UWP. (1121523)</p></li>
<li><p>OSX: Fixed an issue where older Macs could incorrectly report that they support GPU instancing. (1126530)</p></li>
<li><p>OSX: Fixed the fullscreen menu item in the standalone player. (1120105)</p></li>
<li><p>Package Manager: Fixed incorrect build settings on Project Templates in packages. (<a href="https://issuetracker.unity3d.com/issues/build-settings-window-has-a-deleted-scene-in-it-upon-new-project-creation">1114141</a>)</p></li>
<li><p>Prefabs: Fixed crashes when instantiating prefab with certain user scripts. (1113205, 1125019)</p></li>
<li><p>Prefabs: Fixed drag and drop not unpacking the Prefab instance under some circumstances. (1117374)</p></li>
<li><p>Prefabs: Fixed object IDs changing when saving a prefab after building a player. (1106345)</p></li>
<li><p>Profiler: Fixed an issue where chart data would be inconsistent from hierarchy data. (<a href="https://issuetracker.unity3d.com/issues/profiler-data-does-not-match-the-numeric-data-in-its-hierarchy">1080435</a>)</p></li>
<li><p>Scripting: Fixed MissingMethodException when calling bindings methods in VRModule on XBox One. (1109347)</p></li>
<li><p>Scripting: Removed allocation in every frame from ScriptableRuntimeReflectionSystemWrapper.TickRealtimeProbes. (1097039)</p></li>
<li><p>Scripting Upgrade: Fixed an issue where some C# class libaries would fail to load. (1116475)</p></li>
<li><p>Scripting Upgrade: Fixed ReflectionTypeLoadException when getting types from assembly. (1127900)</p></li>
<li><p>Services: Fixed crash when an unhandled exception occurs on a background thread with Cloud Diagnostics enabled. (<a href="https://issuetracker.unity3d.com/issues/android-apk-build-crashes-on-an-android-device-when-iap-placement-is-enabled-but-sdk-is-not-included-in-a-build">1114571</a>, 1122097)</p></li>
<li><p>Shaders: Fixed out-of-memory when trying to compile shader that uses self-referencing macro. (1119490)</p></li>
<li><p>Timeline: Fixed issue where a timeline would not play on AOT platforms using Mono and .NET 3.5 (1129165)</p></li>
<li><p>UI: Fixed issue with CanvasGroup.Alpha not affecting nested Canvas's UI elements. (1127613)</p></li>
<li><p>Unity Test Runner: Fixed Exception not handled properly in PlayTests when a custom Enumerator is used as a Coroutine and throws an Exception. (1120096)</p></li>
<li><p>Universal Windows Platform: Fixed incorrect mouse position for NewInput. (1091493)</p></li>
<li><p>Universal Windows Platform: Fixed rapid triggering of OnClick() events in UI when multiple Xbox controllers connected. (<a href="https://issuetracker.unity3d.com/issues/uwp-xbox-one-controller-button-triggers-rapidly-only-when-two-controllers-are-connected">1099111</a>)</p></li>
<li><p>Universal Windows Platform: Prevented an error from the reference rewriter about the missing method 'ConfigurationElement::get_Item' when the EntityFramework.dll assembly is used. (1124092)</p></li>
<li><p>Video: Fixed a crash on quit, and on end of playmode, when using a VideoPlayer in a prefab. (1126578)</p></li>
<li><p>Video: Fixed Android Video doesn't start to play in the application when Android OS is 4.1 or 4.2. (1124979)</p></li>
<li><p>Web: UnityWebRequest: Better document SetRequestHeader regarding cookie. (1128889)</p></li>
<li><p>Windows: Fixed Multidisplay always reverting to native resolution on primary display. (<a href="https://issuetracker.unity3d.com/issues/primary-screen-window-size-turns-to-native-when-using-more-than-one-display">1040726</a>)</p></li>
</ul>
