# Unity 2018.3.4
https://unity3d.com/unity/whats-new/2018.3.4

## Fixes

<ul>
<li><p>2D: Disabled Tilemap Focus filter when closing Tile Palette window if enabled. (<a href="https://issuetracker.unity3d.com/issues/tilemap-focus-filter-remains-active-in-scene-view-after-closing-the-tile-palette-window-with-focus-on-set-to-tilemap-or-grid">1098821</a>, 1116141)</p></li>
<li><p>2D: Fixed crash on Tilemap::CompressBounds when calling Tilemap.CompressBounds() on corrupted tilemap. (<a href="https://issuetracker.unity3d.com/issues/crash-on-tilemap-compressbounds-when-calling-tilemap-dot-compressbounds-on-corrupted-tilemap">1090111</a>, 1116143)</p></li>
<li><p>2D: Fixed crash on Tilemap::CopyTileDataToTile&lt;0&gt; when importing corrupted Tilemap prefab. (1116144)</p></li>
<li><p>2D: Fixed crash on TilemapRenderer when rendering with a Material that is destroyed. (1116145)</p></li>
<li><p>2D: Fixed current Active Tilemap selection unable to be deselected when a new GameObject is instantiated on the scene. (1116150)</p></li>
<li><p>2D: Fixed for missing Tiles being created when dragging a spritesheet with empty initial columns or rows into Tile Palette. (<a href="https://issuetracker.unity3d.com/issues/missing-tiles-when-dragging-sprite-sheet-into-tile-palette">1103034</a>, 1116146)</p></li>
<li><p>2D: Fixed Tilemap.SwapTiles when swapping Tiles to other Tiles that already exist on the Tilemap. (<a href="https://issuetracker.unity3d.com/issues/2d-tilemap-tilemap-dot-swaptile-swapping-tiles-to-empty">1108368</a>, 1116147)</p></li>
<li><p>Analytics: Removed all XR dependencies on Analytics and made all events support events. (<a href="https://issuetracker.unity3d.com/issues/disabling-unity-analytics-package-throws-compilation-errors-when-project-is-using-unityengine-dot-xr-namespace">1092403</a>)</p></li>
<li><p>Android: Add '-mstackrealign' compile option for android x86 to fix the crash on some x86 devices. (<a href="https://issuetracker.unity3d.com/issues/android-player-crashes-on-some-specific-devices-with-x86-architecture-and-os-version-around-4-dot-4~4-dot-5">1058255</a>)</p></li>
<li><p>Android: Fixed for Android Dynamic feature crashes the application when running the build via Android Studio. (1102209)</p></li>
<li><p>Asset Pipeline: Fixed Asset Bundles not able to load scenes if the scene had a period in its name. (<a href="https://issuetracker.unity3d.com/issues/cant-load-a-scene-from-asset-bundle-if-scene-has-a-period-in-the-name">1022819</a>, 1115505)</p></li>
<li><p>Build Pipeline: Fixed crash when loading compressed meshes out of asset bundles. (1115334)</p></li>
<li><p>Editor: Fixed textures being imported with the platform-specific format when the platform override property is false. (1104345)</p></li>
<li><p>Graphics: Fixed Rendering a scene with a SpriteRenderer with Graphics Jobs on causes a JobTempAlloc memory leak. (1100859)</p></li>
<li><p>IL2CPP: Allow stack sizes for new threads to be set explicitly larger than 64K with the .NET 4.x Equivalent scripting runtime. (1104843)</p></li>
<li><p>IL2CPP: Fixed IL2CPP compiler configuration setting missing from some platforms player settings (like WebGL). (1099894)</p></li>
<li><p>IL2CPP: Updated the zlib implementation to correct the following security issues: CVE-2016-9840, CVE-2016-9841,CVE-2016-9842, CVE-2016-9843.</p></li>
<li><p>iOS: Fixed iOS Frameworks location is ignored when building Xcode project. (1108970)</p></li>
<li><p>Linux: Fixed GPU skinning. (1117706)</p></li>
<li><p>Linux: Fixed issue where SetResolution cannot programmatically resize Linux player after window has been maximized. (<a href="https://issuetracker.unity3d.com/issues/setresolution-fullscreen-parameter-does-not-work-on-linux">1099286</a>, 1115831)</p></li>
<li><p>Linux: Fixed the graphical corruption in the framebuffer for various games on Nvidia Linux. (<a href="https://issuetracker.unity3d.com/issues/linux-nvidia-graphical-corruption-in-many-games-possible-regression">1108929</a>, 1111474)</p></li>
<li><p>Linux: Fixed using libstdc++ in native plugins crashing (2018.3 no longer links with libstdc++ statically). (1115024)</p></li>
<li><p>Multiplayer: Fixed exception thrown when clicking Lan Client on WebGL build. (<a href="https://issuetracker.unity3d.com/issues/networkmanagerhud-uncaught-typeerror-cannot-read-property-id-of-null-thrown-when-clicking-lan-client-on-webgl-build">860733</a>)</p></li>
<li><p>Particles: Fixed JobTempAlloc memory leaks in the Particle System Trails Module on WebGL. (1114502)</p></li>
<li><p>Physics: Added a message with a reference to the Rigidbody component when the CCD mode is incompatible with the kinematic setting. (1064491)</p></li>
<li><p>Physics: Fixed crash due to auto-sync-transforms during Rigidbody2D.Cast query when changing transform prior to query being executed. (<a href="https://issuetracker.unity3d.com/issues/physicsquery2d-collidercastall-crash-when-calling-rigidbody2d-dot-cast">1099642</a>)</p></li>
<li><p>Physics: Fixed crash due to multi-scene physics when destroying an object during a 2D collision/trigger callback. (1110897)</p></li>
<li><p>Plugins: Fixed an issue where CPU information was respected on non-native libs for android plugins. Since users could potentially change these CPU properties on a Plugin Importer via PluginImporter.SetPlatformData() we should eliminate the possibility of  problems occurring due to wrongful modifications of the plugin importer's properties. (<a href="https://issuetracker.unity3d.com/issues/android-plugin-stored-in-universal-aar-is-not-copied-to-apk-properly">1076868</a>)</p></li>
<li><p>Prefabs: Fixed crash when applying changes from Prefab Instance to asset, when assets contains disconnected nested prefabs. (1104595)</p></li>
<li><p>Prefabs: Fixed crash when creating a Prefab Asset in Awake when entering Play Mode. (<a href="https://issuetracker.unity3d.com/issues/getmanagerfromcontext-pointer-to-object-of-manager-lightmapsettings-is-null-table-index-22-when-entering-play-mode">1085577</a>, 1115008)</p></li>
<li><p>Prefabs: Fixed crash when undo'ing after applying a disconnected prefab. (1110703)</p></li>
<li><p>Prefabs: Fixed crash when using Undo wrongly on Prefab asset objects. (1099646)</p></li>
<li><p>Prefabs: Fixed MonoBehaviour cannot be dragged to the Inspector after ParticleSystem on a Prefab Instance (1110704)</p></li>
<li><p>Scripting: Fixed an issue with static members such as generic classes with their argument being an array type not being reported the memory snapshot API. (<a href="https://issuetracker.unity3d.com/issues/packedmemorysnapshot-type-contains-staticfieldbytes-but-has-no-static-field">984330</a>)</p></li>
<li><p>Scripting: Fixed issue where processing SynchronizationContext tasks would allocate. (<a href="https://issuetracker.unity3d.com/issues/unitysynchronizationcontext-dot-executetasks-causes-per-frame-gc-alloc">1114295</a>)</p></li>
<li><p>Scripting: Fixed random crash in Asset GC. (1091878)</p></li>
<li><p>XR: Fixed an issue with a black screen occuring after resuming from pause on some Oculus devices. (<a href="https://issuetracker.unity3d.com/issues/oculus-black-screen-when-resume-from-sleeping-mode-on-quest">1115358</a>)</p></li>
</ul>

#### Changeset: 1d952368ca3a
