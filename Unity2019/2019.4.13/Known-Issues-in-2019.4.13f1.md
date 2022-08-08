# Unity 2019.4.13

https://unity3d.com/unity/whats-new/2019.4.13

## Known Issues in 2019.4.13f1



*   AI: A NavMeshAgent GameObject teleports to a near NavMeshSurface when collided with a moving NavMeshObstacle ([1072945](https://issuetracker.unity3d.com/issues/a-navmeshagent-gameobject-teleports-to-a-near-navmeshsurface-when-collided-with-a-moving-navmeshobstacle))
    
*   Asset Bundles: \[Performance Regression\] AssetBundleLoadAllAssets - Load\_Prefabs\_AllAssets is significantly slower than 18.4 ([1203512](https://issuetracker.unity3d.com/issues/performance-regression-assetbundleloadallassets-load-prefabs-allassets-is-significantly-slower-than-18-dot-4))
    
*   Asset Bundles: \[Performance Regression\] AssetBundleLoadSingleAssets : LoadAsync\_Prefabs\_SingleAssets is significantly slower than 18.4 ([1203511](https://issuetracker.unity3d.com/issues/assetbundleloadsingleassets-loadasync-prefabs-singleassets-is-significantly-slower-than-18-dot-4))
    
*   Asset Import Pipeline: Project Startup time slow due to unmatched Custom Dependencies ([1276078](https://issuetracker.unity3d.com/issues/project-startup-time-slow-due-to-unmatched-custom-dependencies))
    
*   Asset Import Pipeline: \[Asset Import\] Errors thrown on creating a project using microgame templates ([1268154](https://issuetracker.unity3d.com/issues/asset-import-errors-thrown-on-creating-a-project-using-microgame-templates))
    
*   Audio: "Unknown platform passed to AudioImporter" error is thrown when selecting an audio file and UWP support is installed ([1279810](https://issuetracker.unity3d.com/issues/unknown-platform-passed-to-audioimporter-error-is-thrown-when-selecting-an-audio-file-and-uwp-support-is-installed))
    
*   Global Illumination: \[URP\] Transparencies are ignored because URP uses \_BaseMap as main texture identifier ([1246262](https://issuetracker.unity3d.com/issues/urp-shadows-from-alpha-materials-are-not-baked-into-a-lightmap-when-using-baked-lit-shader))
    
*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup ([1162775](https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup))
    
*   Graphics - LowLevel: FPS drops when the Camera is on the right side of the instantiated GameObject with Graphics.DrawMeshInstancedIndirect method ([1278749](https://issuetracker.unity3d.com/issues/fps-drops-when-the-camera-is-on-the-right-side-of-the-instantiated-gameobject-with-graphics-dot-drawmeshinstancedindirect-method))
    
*   IAP: Disabling and re-enabling IAP in services window throws multiple errors about failing to find assemblies ([1193774](https://issuetracker.unity3d.com/issues/disabling-and-re-enabling-iap-in-services-window-throws-multiple-errors-about-failing-to-find-assemblies))
    
*   IL2CPP: UnityLinker strips classes used with the SerializeReference attribute ([1232785](https://issuetracker.unity3d.com/issues/unitylinker-strips-classes-used-with-the-serializereference-attribute))
    
*   Mono: Crash with various stack traces when exiting Play Mode after recompiling scripts ([1238859](https://issuetracker.unity3d.com/issues/crash-with-various-stack-traces-when-exiting-play-mode-after-recompiling-scripts))
    
*   Packman: \[Performance\] Compilation and refresh time increases after each script change - Packman ([1274461](https://issuetracker.unity3d.com/issues/compilation-and-refresh-time-increases-after-each-script-change))
    
*   Profiling: Profiler - RawFrameDataIterator ThreadID will always return 0 for profiler frame data loaded from .data files ([1279213](https://issuetracker.unity3d.com/issues/profiler-rawframedataiterator-threadid-will-always-return-0-for-profiler-frame-data-loaded-from-data-files))
    
*   Scripting: Switching targets in SRP projects will cause XR errors on some platforms ([1196164](https://issuetracker.unity3d.com/issues/osx-switching-an-urp-template-projects-build-target-to-tvos-will-create-reference-errors-to-xrsettings))
    
*   Scripting: \[CompilationPipeline\] Project recompile and package changes takes a long time when Project includes a lot of packages ([1272396](https://issuetracker.unity3d.com/issues/compilationpipeline-project-recompile-and-package-changes-takes-a-long-time-when-project-includes-a-lot-of-packages))
    
*   Scripting: \[SerializedField\] fields produce "Field is never assigned to..." warning ([1080427](https://issuetracker.unity3d.com/issues/serializedfield-fields-produce-field-is-never-assigned-to-dot-dot-dot-warning))
    
*   Serialization: \[Performance\]Console Pro in non-collapse mode and with large logs causes Slow asset refresh when modifying any script, 45 second ([1270910](https://issuetracker.unity3d.com/issues/performance-regression-slow-asset-reimport-when-modifying-any-script))
    
*   Serialization: \[SerializeReference\] Polymorphic instances are always recreated when applying _any_ inspector value change ([1193322](https://issuetracker.unity3d.com/issues/serializereference-non-serialized-initialized-fields-lose-their-values-when-entering-play-mode))
    
*   Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked ([1250293](https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene))
    
*   Shadows/Lights: \[Regression\] Directional light shadow artefacts in 2020.2.0a21 ([1271048](https://issuetracker.unity3d.com/issues/hdrp-directional-light-artefacts-in-2020-dot-2-0a21))
    
*   iOS: \[UaaL\] UnityFramework with 3rd party plugins triggers watchdog termination after launch ([1262272](https://issuetracker.unity3d.com/issues/ios-unityframework-with-3rd-party-plugins-triggers-watchdog-termination-after-launch))
    
*   iOS: \[iOS 14\] VideoPlayer crashes on EXC\_BAD\_ACCESS or signal SIGABRT when audioOutputMode is set to APIOnly or Audio Source ([1274837](https://issuetracker.unity3d.com/issues/ios-videoplayer-crashes-when-audiooutputmode-is-set-to-apionly-or-audiosource))