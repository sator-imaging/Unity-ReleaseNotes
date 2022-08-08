# Unity 2019.4.8

https://unity3d.com/unity/whats-new/2019.4.8

## Known Issues in 2019.4.8f1



*   AI: Editor crashes on MemoryManager::GetAllocator when selecting NavMeshAgent Component in the Inspector window ([1257220](https://issuetracker.unity3d.com/issues/editor-crashes-on-memorymanager-getallocator-when-selecting-navmeshagent-component-in-the-inspector-window))
    
*   Asset Bundles: \[Performance Regression\] AssetBundleLoadAllAssets - Load\_Prefabs\_AllAssets is significantly slower than 18.4 ([1203512](https://issuetracker.unity3d.com/issues/performance-regression-assetbundleloadallassets-load-prefabs-allassets-is-significantly-slower-than-18-dot-4))
    
*   Asset Bundles: \[Performance Regression\] AssetBundleLoadSingleAssets : LoadAsync\_Prefabs\_SingleAssets is significantly slower than 18.4 ([1203511](https://issuetracker.unity3d.com/issues/assetbundleloadsingleassets-loadasync-prefabs-singleassets-is-significantly-slower-than-18-dot-4))
    
*   Global Illumination: \[URP\] Transparencies are ignored because URP uses \_BaseMap as main texture identifier ([1246262](https://issuetracker.unity3d.com/issues/urp-shadows-from-alpha-materials-are-not-baked-into-a-lightmap-when-using-baked-lit-shader))
    
*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup ([1162775](https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup))
    
*   Graphics - LowLevel: Gfx.WaitForPresent / Gfx.WaitForPresentOnGfxThread huge spikes in Profiler when in Play Mode with vSync set to "Don't Sync" ([1108469](https://issuetracker.unity3d.com/issues/gfx-dot-waitforpresent-huge-spikes-in-profiler-when-vsync-is-off))
    
*   IAP: Disabling and re-enabling IAP in services window throws multiple errors about failing to find assemblies ([1193774](https://issuetracker.unity3d.com/issues/disabling-and-re-enabling-iap-in-services-window-throws-multiple-errors-about-failing-to-find-assemblies))
    
*   IAP: Unity purchasing gives error on project upgrade due to failing to find UnityEngine.UI assembly ([1193773](https://issuetracker.unity3d.com/issues/unity-purchasing-fails-to-load-due-to-failing-to-find-unityengine-dot-ui-assembly))
    
*   Inspector Framework: Crash on mono\_method\_signature\_checked when selecting a Context Menu option that has been removed from code ([1263906](https://issuetracker.unity3d.com/issues/crash-on-mono-method-signature-checked-when-selecting-a-context-menu-option-that-has-been-removed-from-code))
    
*   Linux: Linux Editor returns the "O" key's KeyCode when the Space key is being pressed ([1263921](https://issuetracker.unity3d.com/issues/linux-editor-returns-the-o-keys-keycode-when-the-space-key-is-being-pressed))
    
*   MacOS: \[macOS\] Unity kernel crashes Mac with OpenGL when only Intel Graphics are present ([1232673](https://issuetracker.unity3d.com/issues/macos-mac-crashes-when-opening-the-project-with-m-apis-under-windowsstandalonesupport-with-only-integrated-iris-gpu))
    
*   Mono: Crash with various stack traces when exiting Play Mode after recompiling scripts ([1238859](https://issuetracker.unity3d.com/issues/crash-with-various-stack-traces-when-exiting-play-mode-after-recompiling-scripts))
    
*   Profiling: Performance issue in "Profiler" UI with increasing number of events ([967289](https://issuetracker.unity3d.com/issues/performance-issue-in-profiler-ui-with-increasing-number-of-events))
    
*   Scripting: \[SerializedField\] fields produce "Field is never assigned to..." warning ([1080427](https://issuetracker.unity3d.com/issues/serializedfield-fields-produce-field-is-never-assigned-to-dot-dot-dot-warning))
    
*   Serialization: \[SerializeReference\] Polymorphic instances are always recreated when applying _any_ inspector value change ([1193322](https://issuetracker.unity3d.com/issues/serializereference-non-serialized-initialized-fields-lose-their-values-when-entering-play-mode))
    
*   Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked ([1250293](https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene))
    
*   Window Management: Crash on block\_remove when initiating a drag and closing the window from which the drag originated ([1221016](https://issuetracker.unity3d.com/issues/crash-on-block-remove-when-initiating-a-drag-and-closing-the-window-from-which-the-drag-originated))
    
*   Window Management: ReloadAssembly -> EndReloadAssembly processing freezes Editor for minutes ([1253165](https://issuetracker.unity3d.com/issues/reloadassembly-endreloadassebly-processing-freezes-editor-for-minutes))