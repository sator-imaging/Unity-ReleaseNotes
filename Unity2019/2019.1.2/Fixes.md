# Unity 2019.1.2
https://unity3d.com/unity/whats-new/2019.1.2

## Fixes

<ul>
<li><p>Android: Fixed black bar shown on Android9+ devices without notch when in non-fullscreen mode. (<a href="https://issuetracker.unity3d.com/issues/android-android-9-devices-with-a-notch-are-not-in-full-screen-black-bar-is-visible-at-the-bottom-of-the-screen">1144669</a>, 1148770)</p></li>
<li><p>Android: Fixed occasional crash on Moto G when using split binary and loading Asset Bundles from StreamingAssets. (<a href="https://issuetracker.unity3d.com/issues/android-native-crash-on-moto-g-when-loading-assets-of-an-asset-bundle-from-an-obb">1145139</a>, 1150054)</p></li>
<li><p>Asset Pipeline: Asset Bundles - Fix non-deterministic data in asset bundle when using Prebake Collision Mesh. (<a href="https://issuetracker.unity3d.com/issues/when-prebake-collision-mesh-option-is-on-assetbundle-is-built-differently-each-time-we-rebuild-the-same-project">1116173</a>, 1133370)</p></li>
<li><p>Audio: Fixed clip preview autoplay in the object selector. (<a href="https://issuetracker.unity3d.com/issues/audio-is-not-played-when-selecting-audio-asset-in-asset-selector-with-auto-play-enabled-in-unity-versions-past-2018-dot-3-0b5">1126745</a>, 1151363)</p></li>
<li><p>Audio: Fixed crash when creating Presets of AudioManager settings and then modifying AudioManager. (<a href="https://issuetracker.unity3d.com/issues/fmodmemoryalloc-crash-when-creating-presets-of-audiomanager-settings-and-then-modifying-the-audiomanager">1141203</a>, 1151367)</p></li>
<li><p>Build Pipeline: Fixed AssetBundles being build differently on each rebuild when "Prebake Collision Mesh" option is on. (<a href="https://issuetracker.unity3d.com/issues/when-prebake-collision-mesh-option-is-on-assetbundle-is-built-differently-each-time-we-rebuild-the-same-project">1116173</a>, 1133370)</p></li>
<li><p>Editor: Fix GameObject preview flickering on mac (<a href="https://issuetracker.unity3d.com/issues/prefab-inspector-preview-window-flickers-when-moved">1132433</a>, 1150247)</p></li>
<li><p>Editor: Fixed attempting to move an entire light probe group ends up selecting a single probe instead. (1115849, 1144908)</p></li>
<li><p>Editor: Fixed mouse position in new Input System on mac editor. (1145645, 1151369)</p></li>
<li><p>Editor: Fixed the preview pane in the object selector.</p></li>
<li><p>Editor: Fixed UI value synchronization for audio mixer send effects. (<a href="https://issuetracker.unity3d.com/issues/slider-value-for-audiomixers-send-level-in-the-inspector-window-does-not-match-the-same-value-in-audio-mixer-group">1139634</a>, 1151365)</p></li>
<li><p>GI: Fixed we don't check if a point is behind the camera or not. These point should not be included in the selection. (1129856, 1143127)</p></li>
<li><p>GI: Total Bake Time is shown as 0:00:00 in Progressive Lightmapper when Prioritize View is disabled. (<a href="https://issuetracker.unity3d.com/issues/total-bake-time-is-shown-as-0-00-00-in-progressive-lightmapper-when-prioritize-view-is-disabled">1095980</a>, 1143691)</p></li>
<li><p>Graphics: Fixed bug when SRVs were not correct for Texture2DMSArrays. (<a href="https://issuetracker.unity3d.com/issues/graphics-textures-srvs-are-not-correct-for-texture2dmsarrays">1130212</a>, 1145304)</p></li>
<li><p>Graphics: Fixed crash in CameraStackRenderingState::ReleaseResources when exiting play mode. (<a href="https://issuetracker.unity3d.com/issues/camerastackrenderingstate-releaseresources-crash-when-exiting-play-mode">969092</a>, 1151379)</p></li>
<li><p>Package Manager: Fixed an issue where package tarball files could not be extracted when the target path contained non-latin characters. (<a href="https://issuetracker.unity3d.com/issues/package-manager-fails-to-resolve-packages-when-the-windows-user-name-contains-non-latin-characters">1124257</a>, 1144686)</p></li>
<li><p>Player: Fixed mouse position in new Input System on mac standalone players. (<a href="https://issuetracker.unity3d.com/issues/osx-the-x-value-for-mouse-position-is-off-after-switching-into-fullscreen-mode">1145647</a>, 1151376)</p></li>
<li><p>Player: Libpng library upgraded to version 1.6.36 (1141755, 1148310)</p></li>
<li><p>Player: Zlib library upgraded to version 1.2.11 (1141751, 1148305)</p></li>
<li><p>Prefabs: Fixed Particle System Renderer component appearing when adding a script to prefab instance. (1148619, 1148998)</p></li>
<li><p>Prefabs: Fixed prefab asset with orphan GameObject creating dummy root and showing only one child whilst also outputting errors. (<a href="https://issuetracker.unity3d.com/issues/prefab-asset-with-orphan-gameobject-creates-dummy-root-in-prefab-mode-but-shows-only-one-child-under-it-and-spews-errors">1115859</a>, 1148995)</p></li>
<li><p>Prefabs: Fixed that opening a broken legacy Prefab Asset in Prefab Mode shows a recursive dialog (hangs the Editor). (<a href="https://issuetracker.unity3d.com/issues/prefab-asset-with-orphan-gameobject-creates-dummy-root-in-prefab-mode-but-shows-only-one-child-under-it-and-spews-errors">1115859</a>, 1148994)</p></li>
<li><p>Scripting: Fixed empty project generating a few bytes of garbage every frame. (<a href="https://issuetracker.unity3d.com/issues/gc-allocates-9b-garbage-every-frame-when-executing-nativeinputsystem-dot-shouldrunupdate">1142485</a>, 1148201)</p></li>
<li><p>Services: Ensure CrashReporting doesn't capture log messages that occur after the exception being reported (1134786, 1140381)</p></li>
<li><p>Services: Ensure symbols are captured correctly on Android (<a href="https://issuetracker.unity3d.com/issues/android-error-walking-path-errors-thrown-after-completing-a-build-and-having-crash-and-exception-reporting-enabled">1108365</a>, 1140378)</p></li>
<li><p>Services: Ensure symbols are captured correctly on iOS (<a href="https://issuetracker.unity3d.com/issues/ios-automatic-dsym-uploading-doesnt-log-on-first-build-or-archive">1109548</a>, 1140375)</p></li>
<li><p>Services: Fix crash in signal handler on Android IL2CPP ARM64 (1038107, 1140372)</p></li>
<li><p>Services: Fixed collaborate turning itself off. (<a href="https://issuetracker.unity3d.com/issues/collaborate-turns-itself-off">1095539</a>, 1149137)</p></li>
<li><p>Services: Symbol upload for Cloud Diagnostics will now work in batch mode. (851655, 1140370)</p></li>
<li><p>Shaders: Fixed the compute shader compilation failure in Vulkan. (<a href="https://issuetracker.unity3d.com/issues/vulkan-compute-shader-compilation-failure-with-vulkan-plus-msaa-plus-tex2darray-declaration-slash-operation-macros">1103046</a>, 1138090)</p></li>
<li><p>Terrain: Fix the terrain inspector being disabled even after the initial inspector was closed. (<a href="https://issuetracker.unity3d.com/issues/terrain-paint-functionality-is-disabled-in-second-inspector-when-you-close-initial-inspector">1117658</a>, 1143636)</p></li>
<li><p>UI Elements: fix: Graphview - Panning quickly make nodes or edges enter their hover state (1136318, 1141075)</p></li>
<li><p>UI Elements: Fixed a root cause for a bug causing locked inspectors to not update. (1139302, 1151364)</p></li>
<li><p>UI Elements: Pass wheel events in scrollview to parents when they are unused by the scrollview (1118002, 1131482)</p></li>
<li><p>Unity Test Runner: Fixed a regression where the Test Framework would run TearDown in a base class before the inheriting class. (<a href="https://issuetracker.unity3d.com/issues/testrunner-teardown-and-unityteardown-get-called-on-base-class-first">1142553</a>, 1143353)</p></li>
<li><p>Version Control: Fixed YAMLMerge duplicating chunk in output. (<a href="https://issuetracker.unity3d.com/issues/unityyamlmerge-duplicate-chunk-in-the-output-file">1139083</a>, 1146420)</p></li>
<li><p>Video: Fixed audio sync issues on Windows in VideoPlayer when seeking. (<a href="https://issuetracker.unity3d.com/issues/setting-videoplayer-dot-frame-from-code-offsets-audio">889059</a>, 1146539)</p></li>
<li><p>Windows: Fixes maximized Standalone window going to fullscreen (<a href="https://issuetracker.unity3d.com/issues/fullscreen-mode-maximized-window-functionality-is-broken-and-any-built-player-changes-to-non-window-mode-when-maximizing">1137204</a>, 1148786)</p></li>
<li><p>XR: Fix 2D player window crash on resize when started in non-VR and switched to VR. (<a href="https://issuetracker.unity3d.com/issues/uwp-app-triggers-an-exception-when-resizing-uwp-window-after-exiting-xr-mode">1097224</a>, 1148182)</p></li>
<li><p>XR: Fixed app memory leak when open for extended periods of time. (1138251, 1140775)</p></li>
</ul>
