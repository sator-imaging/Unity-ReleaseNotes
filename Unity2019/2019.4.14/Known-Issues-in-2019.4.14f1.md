# Unity 2019.4.14

https://unity3d.com/unity/whats-new/2019.4.14

## Known Issues in 2019.4.14f1



*   AI: A NavMeshAgent GameObject teleports to a near NavMeshSurface when collided with a moving NavMeshObstacle ([1072945](https://issuetracker.unity3d.com/issues/a-navmeshagent-gameobject-teleports-to-a-near-navmeshsurface-when-collided-with-a-moving-navmeshobstacle))
    
*   Animation: The Inspector is empty when selecting the Blend Tree that has been copied and pasted of other Blend Tree ([1274572](https://issuetracker.unity3d.com/issues/the-inspector-is-empty-when-selecting-the-blend-tree-that-has-been-copied-and-pasted-of-other-blend-tree))
    
*   Asset Import Pipeline: Project Startup time slow due to unmatched Custom Dependencies ([1276078](https://issuetracker.unity3d.com/issues/project-startup-time-slow-due-to-unmatched-custom-dependencies))
    
*   Asset Import Pipeline: Texture Assets are reimported when the launched Editor is recovering from an unexpected close if there were compilation errors ([1264055](https://issuetracker.unity3d.com/issues/texture-assets-are-reimported-when-the-launched-editor-is-recovering-from-an-unexpected-close-if-there-were-compilation-errors))
    
*   Audio: "Unknown platform passed to AudioImporter" error is thrown when selecting an audio file and UWP support is installed ([1279810](https://issuetracker.unity3d.com/issues/unknown-platform-passed-to-audioimporter-error-is-thrown-when-selecting-an-audio-file-and-uwp-support-is-installed))
    
*   Global Illumination: \[URP\] Transparencies are ignored because URP uses \_BaseMap as main texture identifier ([1246262](https://issuetracker.unity3d.com/issues/urp-shadows-from-alpha-materials-are-not-baked-into-a-lightmap-when-using-baked-lit-shader))
    
*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup ([1162775](https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup))
    
*   IAP: Disabling and re-enabling IAP in services window throws multiple errors about failing to find assemblies ([1193774](https://issuetracker.unity3d.com/issues/disabling-and-re-enabling-iap-in-services-window-throws-multiple-errors-about-failing-to-find-assemblies))
    
*   IL2CPP: UnityLinker strips classes used with the SerializeReference attribute ([1232785](https://issuetracker.unity3d.com/issues/unitylinker-strips-classes-used-with-the-serializereference-attribute))
    
*   IMGUI: Editor performance loss when selecting an object in the Select Object window ([1285342](https://issuetracker.unity3d.com/issues/editor-performance-loss-when-selecting-an-object-in-the-select-object-window))
    
*   Inspector Framework: Double-clicking a script in the Inspector window does not open the External Script Editor ([1287702](https://issuetracker.unity3d.com/issues/double-clicking-a-script-in-the-inspector-window-does-not-open-the-external-script-editor))
    
*   Linux: InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked ([1248389](https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked))
    
*   Mobile: \[Android\]\[IL2CPP\] App crashes during launch with "Using memoryadresses from more than 16GB of memory" messages on Android 11 ([1284525](https://issuetracker.unity3d.com/issues/android-il2cpp-empty-project-crashes-on-launch-with-using-memoryadresses-from-more-than-16gb-of-memory-messages))
    
*   Mono: Crash with various stack traces when exiting Play Mode after recompiling scripts ([1238859](https://issuetracker.unity3d.com/issues/crash-with-various-stack-traces-when-exiting-play-mode-after-recompiling-scripts))
    
*   Profiling: Profiler - RawFrameDataIterator ThreadID will always return 0 for profiler frame data loaded from .data files ([1279213](https://issuetracker.unity3d.com/issues/profiler-rawframedataiterator-threadid-will-always-return-0-for-profiler-frame-data-loaded-from-data-files))
    
*   Scripting: \[SerializedField\] fields produce "Field is never assigned to..." warning ([1080427](https://issuetracker.unity3d.com/issues/serializedfield-fields-produce-field-is-never-assigned-to-dot-dot-dot-warning))
    
*   Serialization: \[SerializeReference\] Polymorphic instances are always recreated when applying _any_ inspector value change ([1193322](https://issuetracker.unity3d.com/issues/serializereference-non-serialized-initialized-fields-lose-their-values-when-entering-play-mode))
    
*   ShaderGraph: \[Shadergraph\] Color picker in shader graph doesn't work ([1289161](https://issuetracker.unity3d.com/issues/shadergraph-color-picker-in-shader-graph-doesnt-work))
    
*   Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked ([1250293](https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene))
    
*   iOS: Crash on il2cpp::vm::LivenessState::AddProcessObject when using Social.LoadUsers and then changing scenes ([1270230](https://issuetracker.unity3d.com/issues/ios-il2cpp-crash-on-il2cpp-vm-livenessstate-addprocessobject-when-using-social-dot-loadusers-and-then-changing-scenes))
    
*   iOS: \[UaaL\] UnityFramework with 3rd party plugins triggers watchdog termination after launch ([1262272](https://issuetracker.unity3d.com/issues/ios-unityframework-with-3rd-party-plugins-triggers-watchdog-termination-after-launch))
    
*   iOS: \[iOS 14\] VideoPlayer crashes on EXC\_BAD\_ACCESS or signal SIGABRT when audioOutputMode is set to APIOnly or Audio Source ([1274837](https://issuetracker.unity3d.com/issues/ios-videoplayer-crashes-when-audiooutputmode-is-set-to-apionly-or-audiosource))