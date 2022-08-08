# Unity 2020.1.6

https://unity3d.com/unity/whats-new/2020.1.6

## Known Issues in 2020.1.6f1



*   AI: A NavMeshAgent GameObject teleports to a near NavMeshSurface when collided with a moving NavMeshObstacle ([1072945](https://issuetracker.unity3d.com/issues/a-navmeshagent-gameobject-teleports-to-a-near-navmeshsurface-when-collided-with-a-moving-navmeshobstacle))
    
*   Asset Bundles: \[Performance Regression\] AssetBundleLoadAllAssets - Load\_Prefabs\_AllAssets is significantly slower than 18.4 ([1203512](https://issuetracker.unity3d.com/issues/performance-regression-assetbundleloadallassets-load-prefabs-allassets-is-significantly-slower-than-18-dot-4))
    
*   Asset Bundles: \[Performance Regression\] AssetBundleLoadSingleAssets : LoadAsync\_Prefabs\_SingleAssets is significantly slower than 18.4 ([1203511](https://issuetracker.unity3d.com/issues/assetbundleloadsingleassets-loadasync-prefabs-singleassets-is-significantly-slower-than-18-dot-4))
    
*   Asset Importers: \[Performance Regression\] Importing an fbx model is noticeably slower when the model contains Animations ([1265275](https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations))
    
*   Audio: Unity crashes in Play Mode at FMOD\_Resampler\_Linear ([928576](https://issuetracker.unity3d.com/issues/unity-crashes-in-play-mode-at-fmod-resampler-linear))
    
*   Build Pipeline: Building subscenes without platform package doesn't work ([1270120](https://issuetracker.unity3d.com/issues/building-subscenes-without-platform-package-doesnt-work))
    
*   Global Illumination: \[GPU PLM\] OIDN produces noisy results ([1272954](https://issuetracker.unity3d.com/issues/gpu-plm-oidn-produces-noisy-results))
    
*   Global Illumination: \[GPU PLM\] Optix denoiser produces noisy results ([1272950](https://issuetracker.unity3d.com/issues/gpu-plm-optix-denoiser-produces-noisy-results))
    
*   Global Illumination: \[GPU PLM\]\[macOS\] Baking is stuck on 'Finalizing Bake' stage when baking on OSX with AMD GPU ([1204412](https://issuetracker.unity3d.com/issues/unable-to-bake-after-switching-lightmapper-a-few-times))
    
*   Global Illumination: \[OSX\] Crash on 'Preparing Bake' stage when rebaking GI after changing lighting settings and clearing baked data ([1271626](https://issuetracker.unity3d.com/issues/osx-crash-on-preparing-bake-stage-when-rebaking-gi-after-changing-lighting-settings-and-clearing-baked-data))
    
*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup ([1162775](https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup))
    
*   Graphics - LowLevel: Gfx.WaitForPresent / Gfx.WaitForPresentOnGfxThread huge spikes in Profiler when in Play Mode with vSync set to "Don't Sync" ([1108469](https://issuetracker.unity3d.com/issues/gfx-dot-waitforpresent-huge-spikes-in-profiler-when-vsync-is-off))
    
*   IL2CPP: UnityLinker strips classes used with the SerializeReference attribute ([1232785](https://issuetracker.unity3d.com/issues/unitylinker-strips-classes-used-with-the-serializereference-attribute))
    
*   Linux: \[Editor\] Color picker does not work ([1174814](https://issuetracker.unity3d.com/issues/linux-editor-color-picker-does-not-work))
    
*   MacOS: \[OSX\] Shader import in an external exFAT drive crashes Unity ([727114](https://issuetracker.unity3d.com/issues/osx-shader-import-in-an-external-exfat-drive-crashes-unity))
    
*   Mobile Rendering: \[URP\] Low performance on some Android devices when rendering only one terrain/texture ([1261629](https://issuetracker.unity3d.com/issues/urp-low-performance-on-some-android-devices-when-rendering-only-one-terrain-slash-texture))
    
*   Mono: Crash with various stack traces when exiting Play Mode after recompiling scripts ([1238859](https://issuetracker.unity3d.com/issues/crash-with-various-stack-traces-when-exiting-play-mode-after-recompiling-scripts))
    
*   Package: \[Reflect\] Standalone build fails with package errors if Unity Reflect is installed ([1266377](https://issuetracker.unity3d.com/issues/reflect-standalone-build-fails-with-package-errors-if-unity-reflect-is-installed))
    
*   Packman: Editor crashes when upgrading/downgrading between 2020.1 and 2020.2 ([1276565](https://issuetracker.unity3d.com/issues/editor-crashes-when-upgrading-slash-downgrading-between-2020-dot-1-and-2020-dot-2))
    
*   Project Browser: Crash on using global search patterns ([1267138](https://issuetracker.unity3d.com/issues/crash-on-using-global-search-patterns))
    
*   Scene Management: Allocated memory is not cleared when loading and unloading scenes ([1275751](https://issuetracker.unity3d.com/issues/allocated-memory-is-not-cleared-when-loading-and-unloading-scenes))
    
*   Scene Management: Building project when two identical scenes are open crashes the editor ([1266194](https://issuetracker.unity3d.com/issues/building-project-when-two-identical-scenes-are-open-crashes-the-editor))
    
*   Scripting: Building a project crashes when a Script Component has serialized array of a type that contains a serialized PropertyName field ([1267271](https://issuetracker.unity3d.com/issues/building-a-project-crashes-when-a-script-component-has-serialized-array-of-a-type-that-contains-a-serialized-propertyname-field))
    
*   Scripting: Switching targets in SRP projects will cause XR errors on some platforms ([1196164](https://issuetracker.unity3d.com/issues/osx-switching-an-urp-template-projects-build-target-to-tvos-will-create-reference-errors-to-xrsettings))
    
*   Scripting: \[CompilationPipeline\] Project recompile and package changes takes a long time when Project includes a lot of packages ([1272396](https://issuetracker.unity3d.com/issues/compilationpipeline-project-recompile-and-package-changes-takes-a-long-time-when-project-includes-a-lot-of-packages))
    
*   Scripting: \[SerializedField\] fields produce "Field is never assigned to..." warning ([1080427](https://issuetracker.unity3d.com/issues/serializedfield-fields-produce-field-is-never-assigned-to-dot-dot-dot-warning))
    
*   Serialization: Prefab changes are not applied and an error occurs when changing fields that have SerializeReference attribute ([1237191](https://issuetracker.unity3d.com/issues/prefab-changes-are-not-applied-and-an-error-occurs-when-changing-fields-that-have-serializereference-attribute))
    
*   Serialization: \[Performance\] Slow asset refresh when modifying any script, 45 seconds on one line change ([1270910](https://issuetracker.unity3d.com/issues/performance-regression-slow-asset-reimport-when-modifying-any-script))
    
*   Serialization: \[SerializeReference\] Polymorphic instances are always recreated when applying _any_ inspector value change ([1193322](https://issuetracker.unity3d.com/issues/serializereference-non-serialized-initialized-fields-lose-their-values-when-entering-play-mode))
    
*   Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked ([1250293](https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene))
    
*   Shadows/Lights: \[Regression\] Directional light shadow artefacts in 2020.2.0a21 ([1271048](https://issuetracker.unity3d.com/issues/hdrp-directional-light-artefacts-in-2020-dot-2-0a21))
    
*   Version Control: Unity crashes when connecting to a perforce server with an invalid workspace name in the Project Settings ([1275466](https://issuetracker.unity3d.com/issues/unity-crashes-when-connecting-to-a-perforce-server-with-an-invalid-workspace-name-in-the-project-settings))
    
*   WebGL: Using XElement.Load(string uri) causes an uncaught abort exception when using dlopen() dynamic linking in Emscripten ([1192963](https://issuetracker.unity3d.com/issues/webgl-built-project-causes-an-uncaught-abort-exception-when-using-dlopen-dynamic-linking-in-emscripten))
    
*   WebGL: \[Linux\] WebGL build always fails and throws a FileNotFoundException ([1268262](https://issuetracker.unity3d.com/issues/linux-webgl-build-always-fails-and-throws-a-filenotfoundexception))
    
*   Window Management: \[window layout\] cannot load editor layout, stuck in infinite loop of "failed to load window layout" ([1275270](https://issuetracker.unity3d.com/issues/window-layout-cannot-load-editor-layout-stuck-in-infinite-loop-of-failed-to-load-window-layout))
    
*   iOS: Images.xcassets folder does not contain LaunchImage files ([1254927](https://issuetracker.unity3d.com/issues/ios-images-dot-xcassets-folder-does-not-contain-launchimage-files))
    
*   iOS: \[UaaL\] UnityFramework with 3rd party plugins triggers watchdog termination after launch ([1262272](https://issuetracker.unity3d.com/issues/ios-unityframework-with-3rd-party-plugins-triggers-watchdog-termination-after-launch))
    
*   iOS: \[iOS 14\] VideoPlayer crashes on EXC\_BAD\_ACCESS or signal SIGABRT when audioOutputMode is set to APIOnly or Audio Source ([1274837](https://issuetracker.unity3d.com/issues/ios-videoplayer-crashes-when-audiooutputmode-is-set-to-apionly-or-audiosource))