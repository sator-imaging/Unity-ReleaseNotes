# Unity 2020.1.0

https://unity3d.com/unity/whats-new/2020.1.0

## Known Issues in 2020.1.0f1



*   AI: Editor crashes on MemoryManager::GetAllocator when selecting NavMeshAgent Component in the Inspector window ([1257220](https://issuetracker.unity3d.com/issues/editor-crashes-on-memorymanager-getallocator-when-selecting-navmeshagent-component-in-the-inspector-window))
    
*   Asset Bundles: \[Performance Regression\] AssetBundleLoadAllAssets - Load\_Prefabs\_AllAssets is significantly slower than 18.4 ([1203512](https://issuetracker.unity3d.com/issues/performance-regression-assetbundleloadallassets-load-prefabs-allassets-is-significantly-slower-than-18-dot-4))
    
*   Asset Bundles: \[Performance Regression\] AssetBundleLoadSingleAssets : LoadAsync\_Prefabs\_SingleAssets is significantly slower than 18.4 ([1203511](https://issuetracker.unity3d.com/issues/assetbundleloadsingleassets-loadasync-prefabs-singleassets-is-significantly-slower-than-18-dot-4))
    
*   Asset Import Pipeline: \[AssetDatabase2\] Editor encounters an endless recursion when importing a Prefab from a Unity Package file ([1260657](https://issuetracker.unity3d.com/issues/assetdatabase2-editor-encounters-an-endless-recursion-when-importing-a-prefab-from-a-unity-package-file))
    
*   Asset Importers: Models change their position in scene when upgrading project ([1261935](https://issuetracker.unity3d.com/issues/models-change-their-position-in-scene-after-reporting-them-in-2019-dot-4))
    
*   Global Illumination: Crash with empty stacktrace when starting bake in the new scene after baking previous scene with GPU PLM ([1244384](https://issuetracker.unity3d.com/issues/crash-with-empty-stacktrace-when-starting-bake-in-the-new-scene-after-baking-previous-scene-with-gpu-plm))
    
*   Global Illumination: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup ([1162775](https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup))
    
*   Graphics - General: AsyncGPUReadback.Request never releases unused allocated memory ([1234193](https://issuetracker.unity3d.com/issues/asyncgpureadback-dot-request-never-releases-unused-allocated-memory))
    
*   IAP: Unity purchasing gives error on project upgrade due to failing to find UnityEngine.UI assembly ([1193773](https://issuetracker.unity3d.com/issues/unity-purchasing-fails-to-load-due-to-failing-to-find-unityengine-dot-ui-assembly))
    
*   Inspector Framework: Crash on ActiveEditorTracker\_CUSTOM\_Internal\_GetActiveEditorsNonAlloc when reloading Material preview floating window ([1256213](https://issuetracker.unity3d.com/issues/crash-on-activeeditortracker-custom-internal-getactiveeditorsnonalloc-when-reloading-material-preview-floating-window))
    
*   Inspector Framework: Crash on mono\_method\_signature\_checked when selecting a Context Menu option that has been removed from code ([1263906](https://issuetracker.unity3d.com/issues/crash-on-mono-method-signature-checked-when-selecting-a-context-menu-option-that-has-been-removed-from-code))
    
*   Linux: Selection frame drawn in Scene view when a GameObject is selected while Alt and left mouse buttons are pressed ([1239227](https://issuetracker.unity3d.com/issues/selection-frame-drawn-in-scene-view-when-a-gameobject-is-selected-while-alt-and-left-mouse-buttons-are-pressed))
    
*   MacOS: \[Mac\] Many artifacts can be seen in Scene View when Scene Light is enabled and HDR is on with Metal API and Mac OS X 10.15.4 ([1240265](https://issuetracker.unity3d.com/issues/mac-many-artifacts-can-be-seen-in-scene-view-when-scene-light-is-enabled-on-with-metal-api-and-mac-os-x-10-dot-15-dot-4))
    
*   Packman: Asset Store 'Complete Projects' overwriting Project Settings with no warning ([1255256](https://issuetracker.unity3d.com/issues/asset-store-complete-projects-overwriting-project-settings-with-no-warning))
    
*   Physics2D: Editor crashes on PhysicsContacts2D::EndContact when exiting Play mode after Assertion failed on expression: GetShape() == NULL ([1262936](https://issuetracker.unity3d.com/issues/editor-crashes-on-physicscontacts2d-endcontact-when-exiting-play-mode-after-assertion-failed-on-expression-getshape-equals-equals-null))
    
*   Physics: No collision appears when one of the colliding GameObjects has Non-Convex Mesh Collider and Kinematic Rigidbody ([1262418](https://issuetracker.unity3d.com/issues/no-collision-appears-when-one-of-the-colliding-gameobjects-has-non-convex-mesh-collider-and-kinematic-rigidbody))
    
*   Scripting: \[SerializeReference\] Polymorphic instances are always recreated when applying _any_ inspector value change ([1193322](https://issuetracker.unity3d.com/issues/serializereference-non-serialized-initialized-fields-lose-their-values-when-entering-play-mode))
    
*   Scripting: \[SerializedField\] fields produce "Field is never assigned to..." warning ([1080427](https://issuetracker.unity3d.com/issues/serializedfield-fields-produce-field-is-never-assigned-to-dot-dot-dot-warning))
    
*   Shader System: \[Shader Preprocessor\] Errors report the file name and not the full path ([1263687](https://issuetracker.unity3d.com/issues/shader-preprocessor-errors-report-the-file-name-and-not-the-full-path))
    
*   Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked ([1250293](https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene))
    
*   Themes: Editor does not recognize the correct values in the interactive tutorial levels when non-English locale is being used ([1109625](https://issuetracker.unity3d.com/issues/editor-does-not-recognize-the-correct-values-in-the-interactive-tutorial-levels-when-non-english-locale-is-being-used))
    
*   WebGL: Using XElement.Load(string uri) causes an uncaught abort exception when using dlopen() dynamic linking in Emscripten ([1192963](https://issuetracker.unity3d.com/issues/webgl-built-project-causes-an-uncaught-abort-exception-when-using-dlopen-dynamic-linking-in-emscripten))
    
*   Window Management: ReloadAssembly -> EndReloadAssembly processing freezes Editor for minutes ([1253165](https://issuetracker.unity3d.com/issues/reloadassembly-endreloadassebly-processing-freezes-editor-for-minutes))