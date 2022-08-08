# Unity 2019.4.7

https://unity3d.com/unity/whats-new/2019.4.7

## Known Issues in 2019.4.7f1



*   AI: Editor crashes on MemoryManager::GetAllocator when selecting NavMeshAgent Component in the Inspector window ([1257220](https://issuetracker.unity3d.com/issues/editor-crashes-on-memorymanager-getallocator-when-selecting-navmeshagent-component-in-the-inspector-window))
    
*   Asset Bundles: \[Performance Regression\] AssetBundleLoadAllAssets - Load\_Prefabs\_AllAssets is significantly slower than 18.4 ([1203512](https://issuetracker.unity3d.com/issues/performance-regression-assetbundleloadallassets-load-prefabs-allassets-is-significantly-slower-than-18-dot-4))
    
*   Asset Bundles: \[Performance Regression\] AssetBundleLoadSingleAssets : LoadAsync\_Prefabs\_SingleAssets is significantly slower than 18.4 ([1203511](https://issuetracker.unity3d.com/issues/assetbundleloadsingleassets-loadasync-prefabs-singleassets-is-significantly-slower-than-18-dot-4))
    
*   Asset Import Pipeline: \[AssetDatabase2\] Editor encounters an endless recursion when importing a Prefab from a Unity Package file ([1260657](https://issuetracker.unity3d.com/issues/assetdatabase2-editor-encounters-an-endless-recursion-when-importing-a-prefab-from-a-unity-package-file))
    
*   Global Illumination: \[URP\] Transparencies are ignored because URP uses \_BaseMap as main texture identifier ([1246262](https://issuetracker.unity3d.com/issues/urp-shadows-from-alpha-materials-are-not-baked-into-a-lightmap-when-using-baked-lit-shader))
    
*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup ([1162775](https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup))
    
*   Graphics - LowLevel: AsyncGPUReadback can leak memory under certain circumstances. ([1260624](https://issuetracker.unity3d.com/issues/asyncgpureadback-can-leak-memory-under-certain-circumstances))
    
*   Graphics - LowLevel: Gfx.WaitForPresent / Gfx.WaitForPresentOnGfxThread huge spikes in Profiler when in Play Mode with vSync set to "Don't Sync" ([1108469](https://issuetracker.unity3d.com/issues/gfx-dot-waitforpresent-huge-spikes-in-profiler-when-vsync-is-off))
    
*   IAP: Disabling and re-enabling IAP in services window throws multiple errors about failing to find assemblies ([1193774](https://issuetracker.unity3d.com/issues/disabling-and-re-enabling-iap-in-services-window-throws-multiple-errors-about-failing-to-find-assemblies))
    
*   IAP: Unity purchasing gives error on project upgrade due to failing to find UnityEngine.UI assembly ([1193773](https://issuetracker.unity3d.com/issues/unity-purchasing-fails-to-load-due-to-failing-to-find-unityengine-dot-ui-assembly))
    
*   Inspector Framework: Crash on mono\_method\_signature\_checked when selecting a Context Menu option that has been removed from code ([1263906](https://issuetracker.unity3d.com/issues/crash-on-mono-method-signature-checked-when-selecting-a-context-menu-option-that-has-been-removed-from-code))
    
*   Linux: Linux Editor returns the "O" key's KeyCode when the Space key is being pressed ([1263921](https://issuetracker.unity3d.com/issues/linux-editor-returns-the-o-keys-keycode-when-the-space-key-is-being-pressed))
    
*   MacOS: \[Mac\] Many artifacts can be seen in Scene View when Scene Light is enabled and HDR is on with Metal API and Mac OS X 10.15.4 ([1240265](https://issuetracker.unity3d.com/issues/mac-many-artifacts-can-be-seen-in-scene-view-when-scene-light-is-enabled-on-with-metal-api-and-mac-os-x-10-dot-15-dot-4))
    
*   MacOS: \[macOS\] Unity kernel crashes Mac with OpenGL when only Intel Graphics are present ([1232673](https://issuetracker.unity3d.com/issues/macos-mac-crashes-when-opening-the-project-with-m-apis-under-windowsstandalonesupport-with-only-integrated-iris-gpu))
    
*   Metal: Metal Editor view repaint causes geometry explosion randomly ([1267126](https://issuetracker.unity3d.com/issues/metal-editor-view-repaint-causes-geometry-explosion-randomly))
    
*   Mono: Crash with various stack traces when exiting Play Mode after recompiling scripts ([1238859](https://issuetracker.unity3d.com/issues/crash-with-various-stack-traces-when-exiting-play-mode-after-recompiling-scripts))
    
*   Packman: Asset Store 'Complete Projects' overwriting Project Settings with no warning ([1255256](https://issuetracker.unity3d.com/issues/asset-store-complete-projects-overwriting-project-settings-with-no-warning))
    
*   Profiling: Performance issue in "Profiler" UI with increasing number of events ([967289](https://issuetracker.unity3d.com/issues/performance-issue-in-profiler-ui-with-increasing-number-of-events))
    
*   Scene Management: Unity crashes when opening a project with two identical scenes, one of them being unloaded ([1069650](https://issuetracker.unity3d.com/issues/unity-crashes-when-opening-a-project-with-two-identical-scenes-one-of-them-being-unloaded))
    
*   Scripting: \[SerializeReference\] Polymorphic instances are always recreated when applying _any_ inspector value change ([1193322](https://issuetracker.unity3d.com/issues/serializereference-non-serialized-initialized-fields-lose-their-values-when-entering-play-mode))
    
*   Scripting: \[SerializedField\] fields produce "Field is never assigned to..." warning ([1080427](https://issuetracker.unity3d.com/issues/serializedfield-fields-produce-field-is-never-assigned-to-dot-dot-dot-warning))
    
*   Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked ([1250293](https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene))
    
*   Window Management: Crash on block\_remove when initiating a drag and closing the window from which the drag originated ([1221016](https://issuetracker.unity3d.com/issues/crash-on-block-remove-when-initiating-a-drag-and-closing-the-window-from-which-the-drag-originated))
    
*   Window Management: ReloadAssembly -> EndReloadAssembly processing freezes Editor for minutes ([1253165](https://issuetracker.unity3d.com/issues/reloadassembly-endreloadassebly-processing-freezes-editor-for-minutes))