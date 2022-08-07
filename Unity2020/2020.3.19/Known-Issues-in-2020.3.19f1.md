# Unity 2020.3.19
https://unity3d.com/unity/whats-new/2020.3.19

## Known Issues in 2020.3.19f1

<ul>
<li><p>Asset Bundles: Building process of the AssetBundles is slow when the file count is huge (<a href="https://issuetracker.unity3d.com/issues/building-process-of-the-assetbundles-is-slow-when-the-file-count-is-huge">1358059</a>)</p></li>
<li><p>Asset Importers: Editor crashes on UnityEditor.Unsupported:IsDestroyScriptableObject when applying changes to a custom asset (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-unityeditor-dot-unsupported-isdestroyscriptableobject-when-applying-changes-to-a-custom-asset">1353925</a>)</p></li>
<li><p>Audio: Crash on AudioCustomFilter::GetOrCreateDSP when recompiling scripts while in Play Mode (<a href="https://issuetracker.unity3d.com/issues/crash-on-audiocustomfilter-getorcreatedsp-when-recompiling-scripts-while-in-play-mode">1354002</a>)</p></li>
<li><p>Global Illumination: Crash while sculpting Terrain and Baking Lightmaps (<a href="https://issuetracker.unity3d.com/issues/crash-while-sculpting-terrain">1266511</a>)</p></li>
<li><p>Global Illumination: [Enlighten] Fatal Error when closing the Editor while Generating Lighting (<a href="https://issuetracker.unity3d.com/issues/fatal-error-when-closing-the-editor-while-generating-lighting">1354238</a>)</p></li>
<li><p>Global Illumination: [LightProbes] Probes lose their lighting data after entering Play mode when Baked and Realtime GI are enabled (<a href="https://issuetracker.unity3d.com/issues/light-probes-lose-their-lighting-data-after-entering-play-mode-when-baked-and-realtime-gi-are-enabled">1052045</a>)</p></li>
<li><p>IL2CPP: [Android] [IL2CPP] Old build artifacts are used when ARMv7 and ARM64 build follows a ARM64 only build from different git branch (<a href="https://issuetracker.unity3d.com/issues/android-il2cpp-old-build-artifacts-are-used-when-armv7-and-arm64-build-follows-a-arm64-only-build-from-different-git-branch">1347245</a>)</p></li>
<li><p>Input: Input.GetKey does not trigger when the mouse cursor is outside the Game window (<a href="https://issuetracker.unity3d.com/issues/input-dot-getkey-does-not-trigger-when-the-mouse-cursor-is-outside-the-game-window">1358134</a>)</p></li>
<li><p>Linux: Linux Editor crashes at "_XFreeX11XCBStructure" when loading tutorials (<a href="https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-xfreex11xcbstructure-when-loading-tutorials">1323204</a>)</p></li>
<li><p>MacOS: Port count never stops increasing in Standalone build on Mac Standalone (<a href="https://issuetracker.unity3d.com/issues/port-count-never-stops-increasing-in-standalone-build-on-mac-standalone">1365570</a>)</p></li>
<li><p>Mono: Crash on "(KERNELBASE) RaiseException" when reloading Mono assemblies for play mode (<a href="https://issuetracker.unity3d.com/issues/crash-when-entering-play-mode-1">1289744</a>)</p></li>
<li><p>Mono: Crash on mono_thread_get_undeniable_exception  (<a href="https://issuetracker.unity3d.com/issues/crash-on-mono-thread-get-undeniable-exception">1308625</a>)</p></li>
<li><p>Packman: User can't easily configure location of both UPM and Asset Store package local cache (<a href="https://issuetracker.unity3d.com/issues/user-cant-easily-configure-location-of-both-upm-and-asset-store-package-local-cache">1317232</a>)</p></li>
<li><p>Profiling: GarbageCollectAssets is triggered frequently when higher frame counts are set (<a href="https://issuetracker.unity3d.com/issues/garbagecollectassets-is-triggered-frequently-when-higher-frame-counts-are-set">1332708</a>)</p></li>
<li><p>Profiling: Profiler.GetTotalAllocatedMemoryLong increases when Scene is loaded and unloaded (<a href="https://issuetracker.unity3d.com/issues/profiler-dot-gettotalallocatedmemorylong-increases-when-scene-is-loaded-and-unloaded">1364643</a>)</p></li>
<li><p>Quality of Life: Crash on GUIView::DoPaint when selecting color with a color picker (<a href="https://issuetracker.unity3d.com/issues/crash-on-guiview-dopaint-when-selecting-color-with-a-color-picker">1355078</a>)</p></li>
<li><p>Scene Management: Poor performance when loading or unloading a large Scene  (<a href="https://issuetracker.unity3d.com/issues/poor-performance-when-loading-or-unloading-a-large-scene">1360901</a>)</p></li>
<li><p>Scripting: Crashes on mono_class_init when entering Play Mode after recompiling scripts (<a href="https://issuetracker.unity3d.com/issues/crashes-on-mono-class-init-when-entering-play-mode-after-recompiling-scripts">1262671</a>)</p></li>
<li><p>Scripting: Increased Script Assembly reload time (<a href="https://issuetracker.unity3d.com/issues/increased-reload-time">1323490</a>)</p></li>
<li><p>Scripting: Unity does not execute code weavers when the project is opened for the first time (<a href="https://issuetracker.unity3d.com/issues/unity-does-not-execute-code-weavers-when-its-opened-for-the-first-time">1350116</a>)</p></li>
<li><p>Templates: Crash when quickly duplicating prefab with Behaviour Brick attached and undoing duplicate in LEGO Microgame (<a href="https://issuetracker.unity3d.com/issues/i-was-ctrl-plus-z-lego-microgame-blocks">1362660</a>)</p></li>
<li><p>Templates: Editor Crashes when performing Undo and Redo after duplicating Game Object with LEGO Model Asset component (<a href="https://issuetracker.unity3d.com/issues/crash-when-redoing-and-undoing-pasting-prefabs-in-scene-in-lego-microgame">1298503</a>)</p></li>
<li><p>Windows: Editor crashes when exiting and keeping a tutorial project (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-exiting-and-keeping-a-new-micrograme-project">1338299</a>)</p></li>
<li><p>XR: [Linux] Scene View doesn't render when opening new AR or VR Template project or pressing "Show Tutorials" (<a href="https://issuetracker.unity3d.com/issues/xr-linux-scene-view-doesnt-render-when-opening-new-ar-or-vr-template-project-or-pressing-show-tutorials">1362435</a>)</p></li>
</ul>
