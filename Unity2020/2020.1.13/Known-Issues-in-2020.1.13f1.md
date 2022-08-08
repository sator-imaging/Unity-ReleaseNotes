# Unity 2020.1.13

https://unity3d.com/unity/whats-new/2020.1.13

## Known Issues in 2020.1.13f1



*   Animation: The Inspector is empty when selecting the Blend Tree that has been copied and pasted of other Blend Tree ([1274572](https://issuetracker.unity3d.com/issues/the-inspector-is-empty-when-selecting-the-blend-tree-that-has-been-copied-and-pasted-of-other-blend-tree))
    
*   Asset Import Pipeline: Crash on mdb\_txn\_begin when SourceAssetDB has a lock on it from another process ([1208749](https://issuetracker.unity3d.com/issues/crash-on-mdb-txn-begin-when-sourceassetdb-has-a-lock-on-it-from-another-process))
    
*   Asset Import Pipeline: Project Startup time slow due to unmatched Custom Dependencies ([1276078](https://issuetracker.unity3d.com/issues/project-startup-time-slow-due-to-unmatched-custom-dependencies))
    
*   Asset Import Pipeline: Texture Assets are reimported when the launched Editor is recovering from an unexpected close if there were compilation errors ([1264055](https://issuetracker.unity3d.com/issues/texture-assets-are-reimported-when-the-launched-editor-is-recovering-from-an-unexpected-close-if-there-were-compilation-errors))
    
*   Asset Importers: \[Performance Regression\] Importing an fbx model is noticeably slower when the model contains Animations ([1265275](https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations))
    
*   Collab: Collab crashes on clicking Update calling ConflictsManager::AddConflict ([913690](https://issuetracker.unity3d.com/issues/collab-crashes-on-clicking-update-calling-conflictsmanager-addconflict))
    
*   Global Illumination: \[OSX\] Crash on 'Preparing Bake' stage when rebaking GI after changing lighting settings and clearing baked data ([1271626](https://issuetracker.unity3d.com/issues/osx-crash-on-preparing-bake-stage-when-rebaking-gi-after-changing-lighting-settings-and-clearing-baked-data))
    
*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup ([1162775](https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup))
    
*   IL2CPP: UnityLinker strips classes used with the SerializeReference attribute ([1232785](https://issuetracker.unity3d.com/issues/unitylinker-strips-classes-used-with-the-serializereference-attribute))
    
*   IMGUI: Editor performance loss when selecting an object in the Select Object window ([1285342](https://issuetracker.unity3d.com/issues/editor-performance-loss-when-selecting-an-object-in-the-select-object-window))
    
*   Linux: InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked ([1248389](https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked))
    
*   Mobile: \[Android\]\[IL2CPP\] App crashes during launch with "Using memoryadresses from more than 16GB of memory" messages on Android 11 ([1284525](https://issuetracker.unity3d.com/issues/android-il2cpp-empty-project-crashes-on-launch-with-using-memoryadresses-from-more-than-16gb-of-memory-messages))
    
*   Package: \[Reflect\] Standalone build fails with package errors if Unity Reflect is installed ([1266377](https://issuetracker.unity3d.com/issues/reflect-standalone-build-fails-with-package-errors-if-unity-reflect-is-installed))
    
*   Profiling: \[Profiler\] "GetInt is not allowed error" is thrown when entering the Play Mode while Profiler is recording the Editor ([1289794](https://issuetracker.unity3d.com/issues/profiler-getint-is-not-allowed-error-is-thrown-when-entering-the-play-mode-while-profiler-is-recording-the-editor))
    
*   Scene Management: Allocated memory is not cleared when loading and unloading scenes ([1275751](https://issuetracker.unity3d.com/issues/allocated-memory-is-not-cleared-when-loading-and-unloading-scenes))
    
*   Scene/Game View: Editor locks up when applying a material to a prefab in isolation mode after renaming the prefab ([1284799](https://issuetracker.unity3d.com/issues/editor-locks-up-when-applying-a-material-to-a-prefab-in-isolation-mode-after-renaming-the-prefab))
    
*   Serialization: \[SerializeReference\] Polymorphic instances are always recreated when applying _any_ inspector value change ([1193322](https://issuetracker.unity3d.com/issues/serializereference-non-serialized-initialized-fields-lose-their-values-when-entering-play-mode))
    
*   Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked ([1250293](https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene))
    
*   Shortcut Management: ShortcutManager window columns can't be resized anymore ([1288083](https://issuetracker.unity3d.com/issues/shortcutmanager-window-columns-cant-be-resized-anymore))
    
*   WebGL: \[Linux\] WebGL build always fails and throws a FileNotFoundException ([1268262](https://issuetracker.unity3d.com/issues/linux-webgl-build-always-fails-and-throws-a-filenotfoundexception))
    
*   Window Management: \[window layout\] cannot load editor layout, stuck in infinite loop of "failed to load window layout" ([1275270](https://issuetracker.unity3d.com/issues/window-layout-cannot-load-editor-layout-stuck-in-infinite-loop-of-failed-to-load-window-layout))
    
*   iOS: Crash on il2cpp::vm::LivenessState::AddProcessObject when using Social.LoadUsers and then changing scenes ([1270230](https://issuetracker.unity3d.com/issues/ios-il2cpp-crash-on-il2cpp-vm-livenessstate-addprocessobject-when-using-social-dot-loadusers-and-then-changing-scenes))
    
*   iOS: \[UaaL\] UnityFramework with 3rd party plugins triggers watchdog termination after launch ([1262272](https://issuetracker.unity3d.com/issues/ios-unityframework-with-3rd-party-plugins-triggers-watchdog-termination-after-launch))
    
*   iOS: \[iOS 14\] VideoPlayer crashes on EXC\_BAD\_ACCESS or signal SIGABRT when audioOutputMode is set to APIOnly or Audio Source ([1274837](https://issuetracker.unity3d.com/issues/ios-videoplayer-crashes-when-audiooutputmode-is-set-to-apionly-or-audiosource))