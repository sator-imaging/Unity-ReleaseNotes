# Unity 2019.4.13
https://unity3d.com/unity/whats-new/2019.4.13

## Known Issues in 2019.4.13f1

<ul>
<li><p>AI: A NavMeshAgent GameObject teleports to a near NavMeshSurface when collided with a moving NavMeshObstacle (<a href="https://issuetracker.unity3d.com/issues/a-navmeshagent-gameobject-teleports-to-a-near-navmeshsurface-when-collided-with-a-moving-navmeshobstacle">1072945</a>)</p></li>
<li><p>Asset Bundles: [Performance Regression] AssetBundleLoadAllAssets - Load_Prefabs_AllAssets is significantly slower than 18.4 (<a href="https://issuetracker.unity3d.com/issues/performance-regression-assetbundleloadallassets-load-prefabs-allassets-is-significantly-slower-than-18-dot-4">1203512</a>)</p></li>
<li><p>Asset Bundles: [Performance Regression] AssetBundleLoadSingleAssets : LoadAsync_Prefabs_SingleAssets is significantly slower than 18.4 (<a href="https://issuetracker.unity3d.com/issues/assetbundleloadsingleassets-loadasync-prefabs-singleassets-is-significantly-slower-than-18-dot-4">1203511</a>)</p></li>
<li><p>Asset Import Pipeline: Project Startup time slow due to unmatched Custom Dependencies (<a href="https://issuetracker.unity3d.com/issues/project-startup-time-slow-due-to-unmatched-custom-dependencies">1276078</a>)</p></li>
<li><p>Asset Import Pipeline: [Asset Import] Errors thrown on creating a project using microgame templates (<a href="https://issuetracker.unity3d.com/issues/asset-import-errors-thrown-on-creating-a-project-using-microgame-templates">1268154</a>)</p></li>
<li><p>Audio: "Unknown platform passed to AudioImporter" error is thrown when selecting an audio file and UWP support is installed (<a href="https://issuetracker.unity3d.com/issues/unknown-platform-passed-to-audioimporter-error-is-thrown-when-selecting-an-audio-file-and-uwp-support-is-installed">1279810</a>)</p></li>
<li><p>Global Illumination: [URP] Transparencies are ignored because URP uses _BaseMap as main texture identifier (<a href="https://issuetracker.unity3d.com/issues/urp-shadows-from-alpha-materials-are-not-baked-into-a-lightmap-when-using-baked-lit-shader">1246262</a>)</p></li>
<li><p>Global Illumination: [macOS] BugReporter doesn't get invoked when the project crashes (<a href="https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes">1219458</a>)</p></li>
<li><p>Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup (<a href="https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup">1162775</a>)</p></li>
<li><p>Graphics - LowLevel: FPS drops when the Camera is on the right side of the instantiated GameObject with Graphics.DrawMeshInstancedIndirect method (<a href="https://issuetracker.unity3d.com/issues/fps-drops-when-the-camera-is-on-the-right-side-of-the-instantiated-gameobject-with-graphics-dot-drawmeshinstancedindirect-method">1278749</a>)</p></li>
<li><p>IAP: Disabling and re-enabling IAP in services window throws multiple errors about failing to find assemblies (<a href="https://issuetracker.unity3d.com/issues/disabling-and-re-enabling-iap-in-services-window-throws-multiple-errors-about-failing-to-find-assemblies">1193774</a>)</p></li>
<li><p>IL2CPP: UnityLinker strips classes used with the SerializeReference attribute (<a href="https://issuetracker.unity3d.com/issues/unitylinker-strips-classes-used-with-the-serializereference-attribute">1232785</a>)</p></li>
<li><p>Mono: Crash with various stack traces when exiting Play Mode after recompiling scripts (<a href="https://issuetracker.unity3d.com/issues/crash-with-various-stack-traces-when-exiting-play-mode-after-recompiling-scripts">1238859</a>)</p></li>
<li><p>Packman: [Performance] Compilation and refresh time increases after each script change - Packman (<a href="https://issuetracker.unity3d.com/issues/compilation-and-refresh-time-increases-after-each-script-change">1274461</a>)</p></li>
<li><p>Profiling: Profiler - RawFrameDataIterator ThreadID will always return 0 for profiler frame data loaded from .data files (<a href="https://issuetracker.unity3d.com/issues/profiler-rawframedataiterator-threadid-will-always-return-0-for-profiler-frame-data-loaded-from-data-files">1279213</a>)</p></li>
<li><p>Scripting: Switching targets in SRP projects will cause XR errors on some platforms (<a href="https://issuetracker.unity3d.com/issues/osx-switching-an-urp-template-projects-build-target-to-tvos-will-create-reference-errors-to-xrsettings">1196164</a>)</p></li>
<li><p>Scripting: [CompilationPipeline] Project recompile and package changes takes a long time when Project includes a lot of packages (<a href="https://issuetracker.unity3d.com/issues/compilationpipeline-project-recompile-and-package-changes-takes-a-long-time-when-project-includes-a-lot-of-packages">1272396</a>)</p></li>
<li><p>Scripting: [SerializedField] fields produce "Field is never assigned to..." warning (<a href="https://issuetracker.unity3d.com/issues/serializedfield-fields-produce-field-is-never-assigned-to-dot-dot-dot-warning">1080427</a>)</p></li>
<li><p>Serialization: [Performance]Console Pro in non-collapse mode and with large logs causes Slow asset refresh when modifying any script, 45 second (<a href="https://issuetracker.unity3d.com/issues/performance-regression-slow-asset-reimport-when-modifying-any-script">1270910</a>)</p></li>
<li><p>Serialization: [SerializeReference] Polymorphic instances are always recreated when applying <em>any</em> inspector value change (<a href="https://issuetracker.unity3d.com/issues/serializereference-non-serialized-initialized-fields-lose-their-values-when-entering-play-mode">1193322</a>)</p></li>
<li><p>Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked (<a href="https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene">1250293</a>)</p></li>
<li><p>Shadows/Lights: [Regression] Directional light shadow artefacts in 2020.2.0a21 (<a href="https://issuetracker.unity3d.com/issues/hdrp-directional-light-artefacts-in-2020-dot-2-0a21">1271048</a>)</p></li>
<li><p>iOS: [UaaL] UnityFramework with 3rd party plugins triggers watchdog termination after launch (<a href="https://issuetracker.unity3d.com/issues/ios-unityframework-with-3rd-party-plugins-triggers-watchdog-termination-after-launch">1262272</a>)</p></li>
<li><p>iOS: [iOS 14] VideoPlayer crashes on EXC_BAD_ACCESS or signal SIGABRT when audioOutputMode is set to APIOnly or Audio Source (<a href="https://issuetracker.unity3d.com/issues/ios-videoplayer-crashes-when-audiooutputmode-is-set-to-apionly-or-audiosource">1274837</a>)</p></li>
</ul>