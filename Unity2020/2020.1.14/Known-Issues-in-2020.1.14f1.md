# Unity 2020.1.14
https://unity3d.com/unity/whats-new/2020.1.14

## Known Issues in 2020.1.14f1

<ul>
<li><p>Asset Import Pipeline: Texture Assets are reimported when the launched Editor is recovering from an unexpected close if there were compilation errors (<a href="https://issuetracker.unity3d.com/issues/texture-assets-are-reimported-when-the-launched-editor-is-recovering-from-an-unexpected-close-if-there-were-compilation-errors">1264055</a>)</p></li>
<li><p>Asset Importers: [Performance Regression] Importing an fbx model is noticeably slower when the model contains Animations (<a href="https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations">1265275</a>)</p></li>
<li><p>Global Illumination: [OSX] Crash on 'Preparing Bake' stage when rebaking GI after changing lighting settings and clearing baked data (<a href="https://issuetracker.unity3d.com/issues/osx-crash-on-preparing-bake-stage-when-rebaking-gi-after-changing-lighting-settings-and-clearing-baked-data">1271626</a>)</p></li>
<li><p>Global Illumination: [macOS] BugReporter doesn't get invoked when the project crashes (<a href="https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes">1219458</a>)</p></li>
<li><p>Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup (<a href="https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup">1162775</a>)</p></li>
<li><p>IL2CPP: UnityLinker strips classes used with the SerializeReference attribute (<a href="https://issuetracker.unity3d.com/issues/unitylinker-strips-classes-used-with-the-serializereference-attribute">1232785</a>)</p></li>
<li><p>IMGUI: Editor performance loss when selecting an object in the Select Object window (<a href="https://issuetracker.unity3d.com/issues/editor-performance-loss-when-selecting-an-object-in-the-select-object-window">1285342</a>)</p></li>
<li><p>Linux:  InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked (<a href="https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked">1248389</a>)</p></li>
<li><p>MacOS: [Metal][Editor] Memory grows continuously until Editor crashes when importing 100k materials (<a href="https://issuetracker.unity3d.com/issues/metal-editor-memory-grows-continuously-until-editor-crashes-when-importing-100k-materials">1214197</a>)</p></li>
<li><p>Mesh Renderer: Crash on SkinnedMeshRendererManager::RemoveRenderer(SkinnedMeshRenderer&amp;) when exiting Play Mode (<a href="https://issuetracker.unity3d.com/issues/crash-on-skinnedmeshrenderermanager-removerenderer-when">1292526</a>)</p></li>
<li><p>Package: [Reflect] Standalone build fails with package errors if Unity Reflect is installed (<a href="https://issuetracker.unity3d.com/issues/reflect-standalone-build-fails-with-package-errors-if-unity-reflect-is-installed">1266377</a>)</p></li>
<li><p>Scripting: Crashes on mono_class_init when entering Play Mode after recompiling scripts (<a href="https://issuetracker.unity3d.com/issues/crashes-on-mono-class-init-when-entering-play-mode-after-recompiling-scripts">1262671</a>)</p></li>
<li><p>Serialization: [SerializeReference] Polymorphic instances are always recreated when applying <em>any</em> inspector value change (<a href="https://issuetracker.unity3d.com/issues/serializereference-non-serialized-initialized-fields-lose-their-values-when-entering-play-mode">1193322</a>)</p></li>
<li><p>Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked (<a href="https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene">1250293</a>)</p></li>
<li><p>WebGL: [Linux] WebGL build always fails and throws a FileNotFoundException (<a href="https://issuetracker.unity3d.com/issues/linux-webgl-build-always-fails-and-throws-a-filenotfoundexception">1268262</a>)</p></li>
<li><p>XR: [XR SDK][Oculus] EarlyUpdate.XRUpdate spikes inconsistently (<a href="https://issuetracker.unity3d.com/issues/xr-sdk-oculus-earlyupdate-dot-xrupdate-spikes-inconsistently">1262597</a>)</p></li>
<li><p>iOS:  Crash on il2cpp::vm::LivenessState::AddProcessObject when using Social.LoadUsers and then changing scenes (<a href="https://issuetracker.unity3d.com/issues/ios-il2cpp-crash-on-il2cpp-vm-livenessstate-addprocessobject-when-using-social-dot-loadusers-and-then-changing-scenes">1270230</a>)</p></li>
<li><p>iOS: [UaaL] UnityFramework with 3rd party plugins triggers watchdog termination after launch (<a href="https://issuetracker.unity3d.com/issues/ios-unityframework-with-3rd-party-plugins-triggers-watchdog-termination-after-launch">1262272</a>)</p></li>
<li><p>iOS: [iOS 14] VideoPlayer crashes on EXC_BAD_ACCESS or signal SIGABRT when audioOutputMode is set to APIOnly or Audio Source (<a href="https://issuetracker.unity3d.com/issues/ios-videoplayer-crashes-when-audiooutputmode-is-set-to-apionly-or-audiosource">1274837</a>)</p></li>
</ul>
