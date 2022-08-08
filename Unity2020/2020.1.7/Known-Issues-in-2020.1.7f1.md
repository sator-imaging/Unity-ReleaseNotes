# Unity 2020.1.7

https://unity3d.com/unity/whats-new/2020.1.7

## Known Issues in 2020.1.7f1



*   2D: Crash on Tilemap::ValidateAllTileAssets when opening a specific prefab or dropping it into the scene ([1275562](https://issuetracker.unity3d.com/issues/crash-on-tilemap-validatealltileassets-when-opening-a-specific-prefab-or-dropping-it-into-the-scene))
    
*   AI: A NavMeshAgent GameObject teleports to a near NavMeshSurface when collided with a moving NavMeshObstacle ([1072945](https://issuetracker.unity3d.com/issues/a-navmeshagent-gameobject-teleports-to-a-near-navmeshsurface-when-collided-with-a-moving-navmeshobstacle))
    
*   Asset Bundles: \[Performance Regression\] AssetBundleLoadAllAssets - Load\_Prefabs\_AllAssets is significantly slower than 18.4 ([1203512](https://issuetracker.unity3d.com/issues/performance-regression-assetbundleloadallassets-load-prefabs-allassets-is-significantly-slower-than-18-dot-4))
    
*   Asset Bundles: \[Performance Regression\] AssetBundleLoadSingleAssets : LoadAsync\_Prefabs\_SingleAssets is significantly slower than 18.4 ([1203511](https://issuetracker.unity3d.com/issues/assetbundleloadsingleassets-loadasync-prefabs-singleassets-is-significantly-slower-than-18-dot-4))
    
*   Asset Import Pipeline: \[Asset Import\] Errors thrown on creating a project using microgame templates ([1268154](https://issuetracker.unity3d.com/issues/asset-import-errors-thrown-on-creating-a-project-using-microgame-templates))
    
*   Asset Importers: \[Performance Regression\] Importing an fbx model is noticeably slower when the model contains Animations ([1265275](https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations))
    
*   Audio: Unity crashes in Play Mode at FMOD\_Resampler\_Linear ([928576](https://issuetracker.unity3d.com/issues/unity-crashes-in-play-mode-at-fmod-resampler-linear))
    
*   Build Pipeline: Building subscenes without platform package doesn't work ([1270120](https://issuetracker.unity3d.com/issues/building-subscenes-without-platform-package-doesnt-work))
    
*   Global Illumination: \[GPU PLM\] OIDN produces noisy results ([1272954](https://issuetracker.unity3d.com/issues/gpu-plm-oidn-produces-noisy-results))
    
*   Global Illumination: \[GPU PLM\] Optix denoiser produces noisy results ([1272950](https://issuetracker.unity3d.com/issues/gpu-plm-optix-denoiser-produces-noisy-results))
    
*   Global Illumination: \[GPU PLM\]\[macOS\] Baking is stuck on 'Finalizing Bake' stage when baking on OSX with AMD GPU ([1204412](https://issuetracker.unity3d.com/issues/unable-to-bake-after-switching-lightmapper-a-few-times))
    
*   Global Illumination: \[OSX\] Crash on 'Preparing Bake' stage when rebaking GI after changing lighting settings and clearing baked data ([1271626](https://issuetracker.unity3d.com/issues/osx-crash-on-preparing-bake-stage-when-rebaking-gi-after-changing-lighting-settings-and-clearing-baked-data))
    
*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup ([1162775](https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup))
    
*   IL2CPP: UnityLinker strips classes used with the SerializeReference attribute ([1232785](https://issuetracker.unity3d.com/issues/unitylinker-strips-classes-used-with-the-serializereference-attribute))
    
*   Input: \[Linux\] Keypad number keys reporting incorrectly ([1280104](https://issuetracker.unity3d.com/issues/linux-keypad-number-keys-reporting-incorrectly))
    
*   MacOS: Fixed mouse position in fullscreen when black bars are present. ([1254446](https://issuetracker.unity3d.com/issues/mouse-clicks-are-offset-when-using-a-specific-players-screen-aspect-ratio))
    
*   MacOS: \[OSX\] Shader import in an external exFAT drive crashes Unity ([727114](https://issuetracker.unity3d.com/issues/osx-shader-import-in-an-external-exfat-drive-crashes-unity))
    
*   Mobile Rendering: \[Android\]\[URP\] Unpredictable FPS Throttling on a device while rendering an empty Terrain ([1261629](https://issuetracker.unity3d.com/issues/urp-low-performance-on-some-android-devices-when-rendering-only-one-terrain-slash-texture))
    
*   Mobile: \[Android\] Keyboard doesn't show up when trying to input text in an Input Field with Hide Mobile Input checked on Android 11 ([1258071](https://issuetracker.unity3d.com/issues/android-keyboard-doesnt-show-up-when-trying-to-input-text-in-an-input-field-with-hide-mobile-input-checked-on-android-11))
    
*   Mono: Crash with various stack traces when exiting Play Mode after recompiling scripts ([1238859](https://issuetracker.unity3d.com/issues/crash-with-various-stack-traces-when-exiting-play-mode-after-recompiling-scripts))
    
*   Package: \[Reflect\] Standalone build fails with package errors if Unity Reflect is installed ([1266377](https://issuetracker.unity3d.com/issues/reflect-standalone-build-fails-with-package-errors-if-unity-reflect-is-installed))
    
*   Packman: Editor crashes when upgrading/downgrading between 2020.1 and 2020.2 ([1276565](https://issuetracker.unity3d.com/issues/editor-crashes-when-upgrading-slash-downgrading-between-2020-dot-1-and-2020-dot-2))
    
*   Profiling: Hold on window appears and loads infinitely when setting ProfilerDriver.selectedPropertyPath while the Profiler holds no frames ([1278249](https://issuetracker.unity3d.com/issues/hold-on-window-appears-and-loads-infinitely-when-setting-profilerdriver-dot-selectedpropertypath-while-the-profiler-holds-no-frames))
    
*   Project Browser: Crash on using global search patterns ([1267138](https://issuetracker.unity3d.com/issues/crash-on-using-global-search-patterns))
    
*   Scene Management: Allocated memory is not cleared when loading and unloading scenes ([1275751](https://issuetracker.unity3d.com/issues/allocated-memory-is-not-cleared-when-loading-and-unloading-scenes))
    
*   Scene Management: Crash on GameObject::ActivateAwakeRecursivelyInternal when enabling a broken Prefab ([1280054](https://issuetracker.unity3d.com/issues/crash-on-gameobject-activateawakerecursivelyinternal-when-enabling-a-broken-prefab))
    
*   Scripting: Building a project crashes when a Script Component has serialized array of a type that contains a serialized PropertyName field ([1267271](https://issuetracker.unity3d.com/issues/building-a-project-crashes-when-a-script-component-has-serialized-array-of-a-type-that-contains-a-serialized-propertyname-field))
    
*   Scripting: Switching targets in SRP projects will cause XR errors on some platforms ([1196164](https://issuetracker.unity3d.com/issues/osx-switching-an-urp-template-projects-build-target-to-tvos-will-create-reference-errors-to-xrsettings))
    
*   Scripting: \[CompilationPipeline\] Project recompile and package changes takes a long time when Project includes a lot of packages ([1272396](https://issuetracker.unity3d.com/issues/compilationpipeline-project-recompile-and-package-changes-takes-a-long-time-when-project-includes-a-lot-of-packages))
    
*   Scripting: \[SerializedField\] fields produce "Field is never assigned to..." warning ([1080427](https://issuetracker.unity3d.com/issues/serializedfield-fields-produce-field-is-never-assigned-to-dot-dot-dot-warning))
    
*   Serialization: Prefab changes are not applied and an error occurs when changing fields that have SerializeReference attribute ([1237191](https://issuetracker.unity3d.com/issues/prefab-changes-are-not-applied-and-an-error-occurs-when-changing-fields-that-have-serializereference-attribute))
    
*   Serialization: \[Performance\]Console Pro causes Slow asset refresh when modifying any script, 45 seconds on one line change ([1270910](https://issuetracker.unity3d.com/issues/performance-regression-slow-asset-reimport-when-modifying-any-script))
    
*   Serialization: \[SerializeReference\] Polymorphic instances are always recreated when applying _any_ inspector value change ([1193322](https://issuetracker.unity3d.com/issues/serializereference-non-serialized-initialized-fields-lose-their-values-when-entering-play-mode))
    
*   Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked ([1250293](https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene))
    
*   Version Control: Unity crashes when connecting to a perforce server with an invalid workspace name in the Project Settings ([1275466](https://issuetracker.unity3d.com/issues/unity-crashes-when-connecting-to-a-perforce-server-with-an-invalid-workspace-name-in-the-project-settings))
    
*   WebGL: Using XElement.Load(string uri) causes an uncaught abort exception when using dlopen() dynamic linking in Emscripten ([1192963](https://issuetracker.unity3d.com/issues/webgl-built-project-causes-an-uncaught-abort-exception-when-using-dlopen-dynamic-linking-in-emscripten))
    
*   WebGL: \[Linux\] WebGL build always fails and throws a FileNotFoundException ([1268262](https://issuetracker.unity3d.com/issues/linux-webgl-build-always-fails-and-throws-a-filenotfoundexception))
    
*   Window Management: \[window layout\] cannot load editor layout, stuck in infinite loop of "failed to load window layout" ([1275270](https://issuetracker.unity3d.com/issues/window-layout-cannot-load-editor-layout-stuck-in-infinite-loop-of-failed-to-load-window-layout))
    
*   iOS: \[UaaL\] UnityFramework with 3rd party plugins triggers watchdog termination after launch ([1262272](https://issuetracker.unity3d.com/issues/ios-unityframework-with-3rd-party-plugins-triggers-watchdog-termination-after-launch))
    
*   iOS: \[iOS 14\] VideoPlayer crashes on EXC\_BAD\_ACCESS or signal SIGABRT when audioOutputMode is set to APIOnly or Audio Source ([1274837](https://issuetracker.unity3d.com/issues/ios-videoplayer-crashes-when-audiooutputmode-is-set-to-apionly-or-audiosource))