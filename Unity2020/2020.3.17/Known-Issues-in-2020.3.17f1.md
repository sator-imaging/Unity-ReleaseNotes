# Unity 2020.3.17
https://unity3d.com/unity/whats-new/2020.3.17

## Known Issues in 2020.3.17f1

<ul>
<li><p>Asset Importers: Editor crashes on UnityEditor.Unsupported:IsDestroyScriptableObject when applying changes to a custom asset (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-unityeditor-dot-unsupported-isdestroyscriptableobject-when-applying-changes-to-a-custom-asset">1353925</a>)</p></li>
<li><p>Audio: Crash on AudioMixer_CUSTOM_FindSnapshot when passing null as an argument to FindSnapshot() (<a href="https://issuetracker.unity3d.com/issues/crash-on-audiomixer-custom-findsnapshot-when-passing-null-as-an-argument-to-findsnapshot">1341752</a>)</p></li>
<li><p>Global Illumination: Crash while sculpting Terrain and Baking Lightmaps (<a href="https://issuetracker.unity3d.com/issues/crash-while-sculpting-terrain">1266511</a>)</p></li>
<li><p>Global Illumination: [Enlighten] Fatal Error when closing the Editor while Generating Lighting (<a href="https://issuetracker.unity3d.com/issues/fatal-error-when-closing-the-editor-while-generating-lighting">1354238</a>)</p></li>
<li><p>Global Illumination: [LightProbes] Probes lose their lighting data after entering Play mode when Baked and Realtime GI are enabled (<a href="https://issuetracker.unity3d.com/issues/light-probes-lose-their-lighting-data-after-entering-play-mode-when-baked-and-realtime-gi-are-enabled">1052045</a>)</p></li>
<li><p>Input: Input.GetKey does not trigger when the mouse cursor is outside the Game window (<a href="https://issuetracker.unity3d.com/issues/input-dot-getkey-does-not-trigger-when-the-mouse-cursor-is-outside-the-game-window">1358134</a>)</p></li>
<li><p>Linux: Linux Editor crashes at "_XFreeX11XCBStructure" when loading tutorials (<a href="https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-xfreex11xcbstructure-when-loading-tutorials">1323204</a>)</p></li>
<li><p>Metal: Performance in Game View is significantly impacted by Gfx.WaitForPresentOnGfxThread when a second monitor is connected (<a href="https://issuetracker.unity3d.com/issues/performance-in-game-view-is-significantly-impacted-by-gfx-dot-waitforpresentongfxthread-when-a-second-monitor-is-connected">1327408</a>)</p></li>
<li><p>Mobile: [Android] Video player unable to play video from Asset bundles (<a href="https://issuetracker.unity3d.com/issues/android-video-player-unable-to-play-video-from-asset-bundles">1287770</a>)</p></li>
<li><p>Mono: Crash on "(KERNELBASE) RaiseException" when reloading Mono assemblies for play mode (<a href="https://issuetracker.unity3d.com/issues/crash-when-entering-play-mode-1">1289744</a>)</p></li>
<li><p>Mono: Crash on mono_thread_get_undeniable_exception  (<a href="https://issuetracker.unity3d.com/issues/crash-on-mono-thread-get-undeniable-exception">1308625</a>)</p></li>
<li><p>Mono: [Mono Upgrade] CommandBuffer native plugin events hang in the Editor (<a href="https://issuetracker.unity3d.com/issues/commandbuffer-native-plugin-events-hang-in-the-editor">1308216</a>)</p></li>
<li><p>Packman: User can't easily configure location of both UPM and Asset Store package local cache (<a href="https://issuetracker.unity3d.com/issues/user-cant-easily-configure-location-of-both-upm-and-asset-store-package-local-cache">1317232</a>)</p></li>
<li><p>Profiling: GarbageCollectAssets is triggered frequently when higher frame counts are set (<a href="https://issuetracker.unity3d.com/issues/garbagecollectassets-is-triggered-frequently-when-higher-frame-counts-are-set">1332708</a>)</p></li>
<li><p>Profiling: Poor profiler performance when navigating the timeline view and reviewing data with many threads (<a href="https://issuetracker.unity3d.com/issues/poor-profiler-performance-when-navigating-the-timeline-view-and-reviewing-data-with-many-threads">1339407</a>)</p></li>
<li><p>Quality of Life: Crash on GUIView::DoPaint when selecting color with a color picker (<a href="https://issuetracker.unity3d.com/issues/crash-on-guiview-dopaint-when-selecting-color-with-a-color-picker">1355078</a>)</p></li>
<li><p>Scene Management: Crash on BuildPrefabInstanceCorrespondingObjectMap when overriding nested prefab inside AssetDatabase.StartAssetEditing() block (<a href="https://issuetracker.unity3d.com/issues/crash-on-buildprefabinstancecorrespondingobjectmap-when-overriding-nested-prefab-inside-assetdatabase-dot-startassetediting-block">1324978</a>)</p></li>
<li><p>Scripting: Crashes on mono_class_init when entering Play Mode after recompiling scripts (<a href="https://issuetracker.unity3d.com/issues/crashes-on-mono-class-init-when-entering-play-mode-after-recompiling-scripts">1262671</a>)</p></li>
<li><p>Scripting: Error CS8035 is thrown on opening a project when using rulesets (<a href="https://issuetracker.unity3d.com/issues/error-cs8035">1349517</a>)</p></li>
<li><p>Scripting: Increased Script Assembly reload time (<a href="https://issuetracker.unity3d.com/issues/increased-reload-time">1323490</a>)</p></li>
<li><p>Scripting: Performance degradation when activating or deactivating uGUI GameObject (<a href="https://issuetracker.unity3d.com/issues/performance-degradation-when-activating-or-deactivating-ugui-gameobject">1348763</a>)</p></li>
<li><p>Scripting: Unity does not execute code weavers when the project is opened for the first time (<a href="https://issuetracker.unity3d.com/issues/unity-does-not-execute-code-weavers-when-its-opened-for-the-first-time">1350116</a>)</p></li>
<li><p>Templates: Editor Crashes when performing Undo and Redo after duplicating Game Object with LEGO Model Asset component (<a href="https://issuetracker.unity3d.com/issues/crash-when-redoing-and-undoing-pasting-prefabs-in-scene-in-lego-microgame">1298503</a>)</p></li>
<li><p>Vulkan: Linux Editor using Vulkan crashes at " GfxDeviceVK::EnsureValidBackbuffer" when showing tooltips for ProBuilder buttons (<a href="https://issuetracker.unity3d.com/issues/linux-editor-using-vulkan-crashes-at-gfxdevicevk-ensurevalidbackbuffer-when-showing-tooltips-for-probuilder-buttons">1335846</a>)</p></li>
<li><p>Vulkan: [Editor] The Scene's GameObjects textures are seemingly random and change colours depending on the Scene's Camera pos. (<a href="https://issuetracker.unity3d.com/issues/vulkan-editor-the-scenes-gameobjects-textures-are-seemingly-random-and-change-colours-depending-on-the-scenes-camera-pos">1337772</a>)</p></li>
</ul>
