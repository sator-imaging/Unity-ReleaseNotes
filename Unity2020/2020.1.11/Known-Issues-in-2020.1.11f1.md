# Unity 2020.1.11
https://unity3d.com/unity/whats-new/2020.1.11

## Known Issues in 2020.1.11f1

<ul>
<li><p>AI: A NavMeshAgent GameObject teleports to a near NavMeshSurface when collided with a moving NavMeshObstacle (<a href="https://issuetracker.unity3d.com/issues/a-navmeshagent-gameobject-teleports-to-a-near-navmeshsurface-when-collided-with-a-moving-navmeshobstacle">1072945</a>)</p></li>
<li><p>Animation: The Inspector is empty when selecting the Blend Tree that has been copied and pasted of other Blend Tree (<a href="https://issuetracker.unity3d.com/issues/the-inspector-is-empty-when-selecting-the-blend-tree-that-has-been-copied-and-pasted-of-other-blend-tree">1274572</a>)</p></li>
<li><p>Asset Import Pipeline: Crash on mdb_txn_begin when SourceAssetDB has a lock on it from another process (<a href="https://issuetracker.unity3d.com/issues/crash-on-mdb-txn-begin-when-sourceassetdb-has-a-lock-on-it-from-another-process">1208749</a>)</p></li>
<li><p>Asset Import Pipeline: Project Startup time slow due to unmatched Custom Dependencies (<a href="https://issuetracker.unity3d.com/issues/project-startup-time-slow-due-to-unmatched-custom-dependencies">1276078</a>)</p></li>
<li><p>Asset Importers: [Performance Regression] Importing an fbx model is noticeably slower when the model contains Animations (<a href="https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations">1265275</a>)</p></li>
<li><p>Audio: "Unknown platform passed to AudioImporter" error is thrown when selecting an audio file and UWP support is installed (<a href="https://issuetracker.unity3d.com/issues/unknown-platform-passed-to-audioimporter-error-is-thrown-when-selecting-an-audio-file-and-uwp-support-is-installed">1279810</a>)</p></li>
<li><p>Global Illumination: Crashing with progressive GPU when baking lighting with the AZURE Nature demo scene (<a href="https://issuetracker.unity3d.com/issues/crashing-with-progressive-gpu-when-baking-lighting-with-the-azure-nature-demo-scene">1277383</a>)</p></li>
<li><p>Global Illumination: [OSX] Crash on 'Preparing Bake' stage when rebaking GI after changing lighting settings and clearing baked data (<a href="https://issuetracker.unity3d.com/issues/osx-crash-on-preparing-bake-stage-when-rebaking-gi-after-changing-lighting-settings-and-clearing-baked-data">1271626</a>)</p></li>
<li><p>Global Illumination: [PLM] Viewport progressively updating, even with progressive updates toggle unchecked (<a href="https://issuetracker.unity3d.com/issues/viewport-progressively-updating-even-with-progressive-updated-toggle-checked-off">1284697</a>)</p></li>
<li><p>Global Illumination: [macOS] BugReporter doesn't get invoked when the project crashes (<a href="https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes">1219458</a>)</p></li>
<li><p>Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup (<a href="https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup">1162775</a>)</p></li>
<li><p>IL2CPP: UnityLinker strips classes used with the SerializeReference attribute (<a href="https://issuetracker.unity3d.com/issues/unitylinker-strips-classes-used-with-the-serializereference-attribute">1232785</a>)</p></li>
<li><p>Linux: InputSystem not mapping keyboard keys properly on Linux (<a href="https://issuetracker.unity3d.com/issues/inputsystem-not-mapping-keyboard-keys-properly-on-linux">1275964</a>)</p></li>
<li><p>Package: [Reflect] Standalone build fails with package errors if Unity Reflect is installed (<a href="https://issuetracker.unity3d.com/issues/reflect-standalone-build-fails-with-package-errors-if-unity-reflect-is-installed">1266377</a>)</p></li>
<li><p>Packman: Editor crashes when upgrading/downgrading between 2020.1 and 2020.2 (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-upgrading-slash-downgrading-between-2020-dot-1-and-2020-dot-2">1276565</a>)</p></li>
<li><p>Profiling: Profiler - RawFrameDataIterator ThreadID will always return 0 for profiler frame data loaded from .data files (<a href="https://issuetracker.unity3d.com/issues/profiler-rawframedataiterator-threadid-will-always-return-0-for-profiler-frame-data-loaded-from-data-files">1279213</a>)</p></li>
<li><p>Scene Management: Allocated memory is not cleared when loading and unloading scenes (<a href="https://issuetracker.unity3d.com/issues/allocated-memory-is-not-cleared-when-loading-and-unloading-scenes">1275751</a>)</p></li>
<li><p>Scene Management: Crash on GameObject::ActivateAwakeRecursivelyInternal when enabling a broken Prefab (<a href="https://issuetracker.unity3d.com/issues/crash-on-gameobject-activateawakerecursivelyinternal-when-enabling-a-broken-prefab">1280054</a>)</p></li>
<li><p>Scene/Game View: Editor locks up when applying a material to a prefab in isolation mode after renaming the prefab (<a href="https://issuetracker.unity3d.com/issues/editor-locks-up-when-applying-a-material-to-a-prefab-in-isolation-mode-after-renaming-the-prefab">1284799</a>)</p></li>
<li><p>Scripting: Switching targets in SRP projects will cause XR errors on some platforms (<a href="https://issuetracker.unity3d.com/issues/osx-switching-an-urp-template-projects-build-target-to-tvos-will-create-reference-errors-to-xrsettings">1196164</a>)</p></li>
<li><p>Scripting: [CompilationPipeline] Project recompile and package changes takes a long time when Project includes a lot of packages (<a href="https://issuetracker.unity3d.com/issues/compilationpipeline-project-recompile-and-package-changes-takes-a-long-time-when-project-includes-a-lot-of-packages">1272396</a>)</p></li>
<li><p>Serialization: [SerializeReference] Polymorphic instances are always recreated when applying <em>any</em> inspector value change (<a href="https://issuetracker.unity3d.com/issues/serializereference-non-serialized-initialized-fields-lose-their-values-when-entering-play-mode">1193322</a>)</p></li>
<li><p>Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked (<a href="https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene">1250293</a>)</p></li>
<li><p>Vulkan: Right-clicking panels turns them black when Vulkan is the selected Graphics API (<a href="https://issuetracker.unity3d.com/issues/right-clicking-panels-turns-them-black-when-vulkan-is-the-selected-graphics-api">1283290</a>)</p></li>
<li><p>WebGL: [Linux] WebGL build always fails and throws a FileNotFoundException (<a href="https://issuetracker.unity3d.com/issues/linux-webgl-build-always-fails-and-throws-a-filenotfoundexception">1268262</a>)</p></li>
<li><p>Window Management: [window layout] cannot load editor layout, stuck in infinite loop of "failed to load window layout" (<a href="https://issuetracker.unity3d.com/issues/window-layout-cannot-load-editor-layout-stuck-in-infinite-loop-of-failed-to-load-window-layout">1275270</a>)</p></li>
<li><p>iOS: [UaaL] UnityFramework with 3rd party plugins triggers watchdog termination after launch (<a href="https://issuetracker.unity3d.com/issues/ios-unityframework-with-3rd-party-plugins-triggers-watchdog-termination-after-launch">1262272</a>)</p></li>
<li><p>iOS: [iOS 14] VideoPlayer crashes on EXC_BAD_ACCESS or signal SIGABRT when audioOutputMode is set to APIOnly or Audio Source (<a href="https://issuetracker.unity3d.com/issues/ios-videoplayer-crashes-when-audiooutputmode-is-set-to-apionly-or-audiosource">1274837</a>)</p></li>
</ul>