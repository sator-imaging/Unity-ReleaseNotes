# Unity 2021.1.22
https://unity3d.com/unity/whats-new/2021.1.22

## Known Issues in 2021.1.22f1

<ul>
<li><p>Asset Bundles: Building process of the AssetBundles is slow when the file count is huge (<a href="https://issuetracker.unity3d.com/issues/building-process-of-the-assetbundles-is-slow-when-the-file-count-is-huge">1358059</a>)</p></li>
<li><p>Asset Import Pipeline: Editor crashes with out of memory while importing a lot of assets (mostly textures) at once, on Windows/DX11 (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-with-system-out-of-memory-error-when-importing-size-heavy-textures">1324536</a>)</p></li>
<li><p>Asset Importers: Editor crashes on UnityEditor.Unsupported:IsDestroyScriptableObject when applying changes to a custom asset (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-unityeditor-dot-unsupported-isdestroyscriptableobject-when-applying-changes-to-a-custom-asset">1353925</a>)</p></li>
<li><p>Asset Importers: [MacOS] Second Unity instance in Activity Monitor is "not responding” after importing (<a href="https://issuetracker.unity3d.com/issues/macos-second-unity-instance-in-activity-monitor-is-not-responding-after-importing">1331736</a>)</p></li>
<li><p>Audio: Crash on AudioCustomFilter::GetOrCreateDSP when recompiling scripts while in Play Mode (<a href="https://issuetracker.unity3d.com/issues/crash-on-audiocustomfilter-getorcreatedsp-when-recompiling-scripts-while-in-play-mode">1354002</a>)</p></li>
<li><p>Global Illumination: Crash while sculpting Terrain and Baking Lightmaps (<a href="https://issuetracker.unity3d.com/issues/crash-while-sculpting-terrain">1266511</a>)</p></li>
<li><p>Global Illumination: [Enlighten] Fatal Error when closing the Editor while Generating Lighting (<a href="https://issuetracker.unity3d.com/issues/fatal-error-when-closing-the-editor-while-generating-lighting">1354238</a>)</p></li>
<li><p>Global Illumination: [LightProbes] Probes lose their lighting data after entering Play mode when Baked and Realtime GI are enabled (<a href="https://issuetracker.unity3d.com/issues/light-probes-lose-their-lighting-data-after-entering-play-mode-when-baked-and-realtime-gi-are-enabled">1052045</a>)</p></li>
<li><p>IMGUI: Scrolling is jumping when scrolling in the Input Manager (<a href="https://issuetracker.unity3d.com/issues/scrolling-is-jumping-when-scrolling-in-the-input-manager">1362327</a>)</p></li>
<li><p>Input: Input.GetKey does not trigger when the mouse cursor is outside the Game window (<a href="https://issuetracker.unity3d.com/issues/input-dot-getkey-does-not-trigger-when-the-mouse-cursor-is-outside-the-game-window">1358134</a>)</p></li>
<li><p>Linux: Linux Editor crashes at "_XFreeX11XCBStructure" when loading tutorials (<a href="https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-xfreex11xcbstructure-when-loading-tutorials">1323204</a>)</p></li>
<li><p>MacOS: Port count never stops increasing in Standalone build on Mac Standalone (<a href="https://issuetracker.unity3d.com/issues/port-count-never-stops-increasing-in-standalone-build-on-mac-standalone">1365570</a>)</p></li>
<li><p>Mobile: [Android] App stops due to OnPixelCopyFinishedListener not being supported on devices with lower than 24 SDK (<a href="https://issuetracker.unity3d.com/issues/app-stops-due-to-onpixelcopyfinishedlistener-not-being-supported-on-devices-with-lower-than-24-sdk">1331290</a>)</p></li>
<li><p>Packman: User can't easily configure location of both UPM and Asset Store package local cache (<a href="https://issuetracker.unity3d.com/issues/user-cant-easily-configure-location-of-both-upm-and-asset-store-package-local-cache">1317232</a>)</p></li>
<li><p>Profiling: GUIStyle errors are thrown when entering Play mode with docked Profiler and the "Maximize On Play" option Enabled (<a href="https://issuetracker.unity3d.com/issues/guistyle-errors-are-thrown-when-entering-play-mode-with-docked-profiler-and-the-maximize-on-play-option-enabled">1364443</a>)</p></li>
<li><p>Profiling: Profiler.GetTotalAllocatedMemoryLong increases when Scene is loaded and unloaded (<a href="https://issuetracker.unity3d.com/issues/profiler-dot-gettotalallocatedmemorylong-increases-when-scene-is-loaded-and-unloaded">1364643</a>)</p></li>
<li><p>Quality of Life: Crash on GUIView::DoPaint when selecting color with a color picker (<a href="https://issuetracker.unity3d.com/issues/crash-on-guiview-dopaint-when-selecting-color-with-a-color-picker">1355078</a>)</p></li>
<li><p>Scene Management: Poor performance when loading or unloading a large Scene  (<a href="https://issuetracker.unity3d.com/issues/poor-performance-when-loading-or-unloading-a-large-scene">1360901</a>)</p></li>
<li><p>Scripting: Crashes on mono_class_init when entering Play Mode after recompiling scripts (<a href="https://issuetracker.unity3d.com/issues/crashes-on-mono-class-init-when-entering-play-mode-after-recompiling-scripts">1262671</a>)</p></li>
<li><p>Scripting: Increased Script Assembly reload time (<a href="https://issuetracker.unity3d.com/issues/increased-reload-time">1323490</a>)</p></li>
<li><p>Scripting: Performance degradation when activating or deactivating uGUI GameObject (<a href="https://issuetracker.unity3d.com/issues/performance-degradation-when-activating-or-deactivating-ugui-gameobject">1348763</a>)</p></li>
<li><p>Scripting: Unity does not execute code weavers when the project is opened for the first time (<a href="https://issuetracker.unity3d.com/issues/unity-does-not-execute-code-weavers-when-its-opened-for-the-first-time">1350116</a>)</p></li>
<li><p>Vulkan: [Editor] The Scene's GameObjects textures are seemingly random and change colours depending on the Scene's Camera pos. (<a href="https://issuetracker.unity3d.com/issues/vulkan-editor-the-scenes-gameobjects-textures-are-seemingly-random-and-change-colours-depending-on-the-scenes-camera-pos">1337772</a>)</p></li>
<li><p>XR: [Linux] Scene View doesn't render when opening new AR or VR Template project or pressing "Show Tutorials" (<a href="https://issuetracker.unity3d.com/issues/xr-linux-scene-view-doesnt-render-when-opening-new-ar-or-vr-template-project-or-pressing-show-tutorials">1362435</a>)</p></li>
</ul>
