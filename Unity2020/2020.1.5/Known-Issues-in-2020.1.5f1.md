# Unity 2020.1.5
https://unity3d.com/unity/whats-new/2020.1.5

## Known Issues in 2020.1.5f1

<ul>
<li><p>AI: A NavMeshAgent GameObject teleports to a near NavMeshSurface when collided with a moving NavMeshObstacle (<a href="https://issuetracker.unity3d.com/issues/a-navmeshagent-gameobject-teleports-to-a-near-navmeshsurface-when-collided-with-a-moving-navmeshobstacle">1072945</a>)</p></li>
<li><p>Asset Bundles: [Performance Regression] AssetBundleLoadAllAssets - Load_Prefabs_AllAssets is significantly slower than 18.4 (<a href="https://issuetracker.unity3d.com/issues/performance-regression-assetbundleloadallassets-load-prefabs-allassets-is-significantly-slower-than-18-dot-4">1203512</a>)</p></li>
<li><p>Asset Bundles: [Performance Regression] AssetBundleLoadSingleAssets : LoadAsync_Prefabs_SingleAssets is significantly slower than 18.4 (<a href="https://issuetracker.unity3d.com/issues/assetbundleloadsingleassets-loadasync-prefabs-singleassets-is-significantly-slower-than-18-dot-4">1203511</a>)</p></li>
<li><p>Asset Importers: [Performance Regression] Importing an fbx model is noticeably slower when the model contains Animations (<a href="https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations">1265275</a>)</p></li>
<li><p>Audio: Crash on StackAllocator::WalkAllocations when there's a memory leak in Play mode (<a href="https://issuetracker.unity3d.com/issues/crash-on-stackallocator-walkallocations-when-theres-a-memory-leak-in-play-mode">1225987</a>)</p></li>
<li><p>Audio: Unity crashes in Play Mode at FMOD_Resampler_Linear (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-in-play-mode-at-fmod-resampler-linear">928576</a>)</p></li>
<li><p>Build Pipeline: Building subscenes without platform package doesn't work (<a href="https://issuetracker.unity3d.com/issues/building-subscenes-without-platform-package-doesnt-work">1270120</a>)</p></li>
<li><p>Global Illumination: [GPU PLM] OIDN produces noisy results (<a href="https://issuetracker.unity3d.com/issues/gpu-plm-oidn-produces-noisy-results">1272954</a>)</p></li>
<li><p>Global Illumination: [GPU PLM] Optix denoiser produces noisy results (<a href="https://issuetracker.unity3d.com/issues/gpu-plm-optix-denoiser-produces-noisy-results">1272950</a>)</p></li>
<li><p>Global Illumination: [GPU PLM][macOS] Baking is stuck on 'Finalizing Bake' stage when baking on OSX with AMD GPU (<a href="https://issuetracker.unity3d.com/issues/unable-to-bake-after-switching-lightmapper-a-few-times">1204412</a>)</p></li>
<li><p>Global Illumination: [OSX] Crash on 'Preparing Bake' stage when rebaking GI after changing lighting settings and clearing baked data (<a href="https://issuetracker.unity3d.com/issues/osx-crash-on-preparing-bake-stage-when-rebaking-gi-after-changing-lighting-settings-and-clearing-baked-data">1271626</a>)</p></li>
<li><p>Global Illumination: [macOS] BugReporter doesn't get invoked when the project crashes (<a href="https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes">1219458</a>)</p></li>
<li><p>Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup (<a href="https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup">1162775</a>)</p></li>
<li><p>Graphics - LowLevel: Gfx.WaitForPresent / Gfx.WaitForPresentOnGfxThread huge spikes in Profiler when in Play Mode with vSync set to "Don't Sync" (<a href="https://issuetracker.unity3d.com/issues/gfx-dot-waitforpresent-huge-spikes-in-profiler-when-vsync-is-off">1108469</a>)</p></li>
<li><p>IL2CPP: UnityLinker strips classes used with the SerializeReference attribute (<a href="https://issuetracker.unity3d.com/issues/unitylinker-strips-classes-used-with-the-serializereference-attribute">1232785</a>)</p></li>
<li><p>Linux: [Editor] Color picker does not work (<a href="https://issuetracker.unity3d.com/issues/linux-editor-color-picker-does-not-work">1174814</a>)</p></li>
<li><p>MacOS: [OSX] Shader import in an external exFAT drive crashes Unity (<a href="https://issuetracker.unity3d.com/issues/osx-shader-import-in-an-external-exfat-drive-crashes-unity">727114</a>)</p></li>
<li><p>Mobile Rendering: [URP] Low performance on some Android devices when rendering only one terrain/texture (<a href="https://issuetracker.unity3d.com/issues/urp-low-performance-on-some-android-devices-when-rendering-only-one-terrain-slash-texture">1261629</a>)</p></li>
<li><p>Mono: Crash with various stack traces when exiting Play Mode after recompiling scripts (<a href="https://issuetracker.unity3d.com/issues/crash-with-various-stack-traces-when-exiting-play-mode-after-recompiling-scripts">1238859</a>)</p></li>
<li><p>Package: [Reflect] Standalone build fails with package errors if Unity Reflect is installed (<a href="https://issuetracker.unity3d.com/issues/reflect-standalone-build-fails-with-package-errors-if-unity-reflect-is-installed">1266377</a>)</p></li>
<li><p>Project Browser: Crash on using global search patterns (<a href="https://issuetracker.unity3d.com/issues/crash-on-using-global-search-patterns">1267138</a>)</p></li>
<li><p>Scene Management: Building project when two identical scenes are open crashes the editor (<a href="https://issuetracker.unity3d.com/issues/building-project-when-two-identical-scenes-are-open-crashes-the-editor">1266194</a>)</p></li>
<li><p>Scripting: Building a project crashes when a Script Component has serialized array of a type that contains a serialized PropertyName field (<a href="https://issuetracker.unity3d.com/issues/building-a-project-crashes-when-a-script-component-has-serialized-array-of-a-type-that-contains-a-serialized-propertyname-field">1267271</a>)</p></li>
<li><p>Scripting: [CompilationPipeline] Project recompile and package changes takes a long time when Project includes a lot of packages (<a href="https://issuetracker.unity3d.com/issues/compilationpipeline-project-recompile-and-package-changes-takes-a-long-time-when-project-includes-a-lot-of-packages">1272396</a>)</p></li>
<li><p>Scripting: [SerializedField] fields produce "Field is never assigned to..." warning (<a href="https://issuetracker.unity3d.com/issues/serializedfield-fields-produce-field-is-never-assigned-to-dot-dot-dot-warning">1080427</a>)</p></li>
<li><p>Serialization: Prefab changes are not applied and an error occurs when changing fields that have SerializeReference attribute (<a href="https://issuetracker.unity3d.com/issues/prefab-changes-are-not-applied-and-an-error-occurs-when-changing-fields-that-have-serializereference-attribute">1237191</a>)</p></li>
<li><p>Serialization: [SerializeReference] Polymorphic instances are always recreated when applying <em>any</em> inspector value change (<a href="https://issuetracker.unity3d.com/issues/serializereference-non-serialized-initialized-fields-lose-their-values-when-entering-play-mode">1193322</a>)</p></li>
<li><p>Shader System: [Bug] "min16f as def32" modifier in FXC bytecode not honored when converting to SPIR-V/ESSL (<a href="https://issuetracker.unity3d.com/issues/min16f-as-def32-modifier-in-fxc-bytecode-not-honored-when-converting-to-spir-v-slash-essl">1228687</a>)</p></li>
<li><p>Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked (<a href="https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene">1250293</a>)</p></li>
<li><p>Shuriken: Crash after an Overflow in memory allocator when changing Particle System's Duration in Play Mode (<a href="https://issuetracker.unity3d.com/issues/crash-after-an-overflow-in-memory-allocator-when-changing-particle-systems-duration-in-play-mode">1273529</a>)</p></li>
<li><p>WebGL:  Using XElement.Load(string uri) causes an uncaught abort exception when using dlopen() dynamic linking in Emscripten (<a href="https://issuetracker.unity3d.com/issues/webgl-built-project-causes-an-uncaught-abort-exception-when-using-dlopen-dynamic-linking-in-emscripten">1192963</a>)</p></li>
</ul>