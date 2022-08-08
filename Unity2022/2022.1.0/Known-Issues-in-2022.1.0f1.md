# Unity 2022.1.0

https://unity3d.com/unity/whats-new/2022.1.0

## Known Issues in 2022.1.0f1



*   Asset - Database: Texture size increased on first build when 'Compress Textures/Assets on Import' is enabled ([1397965](https://issuetracker.unity3d.com/issues/texture-size-increased-on-first-build-when-compress-textures-slash-assets-on-import-is-enabled))
    
*   Asset Bundles: Textures are not compressed when building bundles ([1412557](https://issuetracker.unity3d.com/issues/textures-not-compressed-when-building-bundles))
    
*   Dedicated Server: Data from mesh colliders are stripped in dedicated server builds ([1399961](https://issuetracker.unity3d.com/issues/dedicated-server-data-from-mesh-colliders-are-stripped-in-dedicated-server-builds))
    
*   DirectX11: Crash on GfxDeviceD3D11Base::ResolveDepthIntoTexture when opening the project ([1408785](https://issuetracker.unity3d.com/issues/crash-on-gfxdeviced3d11base-resolvedepthintotexture-when-opening-the-project))
    
*   DirectX12: Crash on GfxDeviceD3D12Base::DrawBuffersCommon when entering Play Mode with DX12 ([1344725](https://issuetracker.unity3d.com/issues/crash-on-gfxdeviced3d12base-drawbufferscommon-when-entering-play-mode-with-dx12))
    
*   Graphics Device Features: Random-write to UAV texture from shadowcaster shader causes GPU hang when filtering Scene Hierarchy objects ([1417589](https://issuetracker.unity3d.com/issues/random-write-to-uav-texture-from-shadowcaster-shader-causes-gpu-hang-when-filtering-scene-hierarchy-objects))
    
*   IL2CPP: \[Mobile\] \[IL2CPP\] Build fails when using custom script and target architecture ARM64 is selected ([1420369](https://issuetracker.unity3d.com/issues/mobile-il2cpp-build-fails-when-using-custom-script-and-target-architecture-arm64-is-selected))
    
*   IMGUI: Impossible to change the Gradient's location value in the Visual Effects Graph when using the keyboard ([1420954](https://issuetracker.unity3d.com/issues/impossible-to-change-the-gradients-location-value-in-the-visual-effects-graph-when-using-the-keyboard))
    
*   Inspector Framework: Tooltips are not shown when hovering over name of the value in the Inspector ([1415921](https://issuetracker.unity3d.com/issues/tooltips-are-not-shown-when-hovering-over-name-of-the-value-in-the-inspector))
    
*   Linux: PC doesn't sleep when the Editor is open ([1418023](https://issuetracker.unity3d.com/issues/linux-pc-doesnt-sleep-when-the-editor-is-open))
    
*   Linux: Editor crashes at "\_\_assert\_fail\_base.cold" when opening a project (Linux) ([1375312](https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-assert-fail-base-dot-cold-when-opening-a-project))
    
*   Linux: New Input System's Input Actions windows's Binding Path dropdown is rendered as an empty white square on Linux ([1391850](https://issuetracker.unity3d.com/issues/new-input-systems-input-actions-windowss-binding-path-dropdown-is-rendered-as-an-empty-white-square-on-linux))
    
*   Metal: Consistent EditorLoop 5-10ms spikes when using Metal API ([1378985](https://issuetracker.unity3d.com/issues/consistent-gfx-dot-waitforpresentongfxthread-5-10ms-spikes-when-using-metal-api))
    
*   Mono: \[Android\] "Found plugins with same names" error is thrown when building on Android with duplicate .dll files ([1373388](https://issuetracker.unity3d.com/issues/found-plugins-with-same-names-error-is-thrown-for-the-microsoft-extensions-logging-package-when-building-on-android-platform))
    
*   Package: Empty "StreamingAssets" folder gets created after building an empty project ([1423325](https://issuetracker.unity3d.com/issues/empty-streamingassets-folder-gets-created-after-building-an-empty-project))
    
*   Package: Unity crashes in batch mode when using -vcsMode Perforce ([1396449](https://issuetracker.unity3d.com/issues/unity-crashes-in-batch-mode-when-using-vcsmode-perforce))
    
*   Physics: Crash on internalABP::ABP\_PairManager::addPair when switching to ArticulationJointType.SphericalJoint during runtime ([1418715](https://issuetracker.unity3d.com/issues/crash-on-internalabp-abp-pairmanager-addpair-when-switching-to-articulationjointtype-dot-sphericaljoint-during-runtime))
    
*   Progressive Lightmapper: \[GPU PLM\] Fallback to CPU PLM in CL\_INVALID\_MEM\_OBJECT after switching light color only and rebaking GI ([1356714](https://issuetracker.unity3d.com/issues/gpu-plm-switch-light-color-only-and-rebake-causes-fallback))
    
*   Quality of Life: \[Mac\] ShortcutManager ignores Option modifier ([1425118](https://issuetracker.unity3d.com/issues/mac-shortcutmanager-ignores-option-modifier))
    
*   Quality of Life: \[Mac\] ShortcutManager ignores Shift modifier ([1424655](https://issuetracker.unity3d.com/issues/mac-shortcutmanager-ignores-shift-control-and-option-modifiers))
    
*   Scene Management: Reordering GameObjects in Hierarchy doesn't register Undo ([1424635](https://issuetracker.unity3d.com/issues/reordering-gameobjects-in-hierarchy-doesnt-register-undo))
    
*   Scene/Game View: Game Object Material starts flickering when dragging new material over other Game Object that touches first Object ([1423053](https://issuetracker.unity3d.com/issues/game-object-material-starts-flickering-when-dragging-new-material-over-other-game-object-that-touches-first-object))
    
*   Scene/Game View: Game View is not displayed after setting language pack in Editor ([1420291](https://issuetracker.unity3d.com/issues/gameview-is-not-displayed-after-setting-language-pack-in-unityeditor))
    
*   Search: Fail to load the search index concurrently ([1417609](https://issuetracker.unity3d.com/issues/search-fail-to-load-the-search-index-concurrently))
    
*   Serialization: Editor crash when deserializing an array of a type with a nested fixed-size buffer field ([1400774](https://issuetracker.unity3d.com/issues/editor-crash-when-deserializing-an-array-of-a-type-with-a-nested-fixed-size-buffer-field))
    
*   Settings Window: Spaces and symbols of the Project name are changed to hyphens causing "Invalid characters" warning in the Bundle Identifier ([1412412](https://issuetracker.unity3d.com/issues/spaces-and-symbols-of-the-project-name-are-changed-to-hyphens-causing-warnings-in-the-bundle-identifier))
    
*   Shader System: Editor crashes in Play mode when Groupshared memory and a constant buffer value is used in a compute shader on OpenGLES3 ([1413012](https://issuetracker.unity3d.com/issues/editor-crashes-in-play-mode-when-groupshared-memory-and-a-constant-buffer-value-is-used-in-a-compute-shader-on-opengles3))
    
*   Shadows/Lights: Scene is brighter in Standalone player if it was open in the Editor at build time ([1375015](https://issuetracker.unity3d.com/issues/scene-is-brighter-in-standalone-player-if-it-was-open-in-the-editor-at-build-time))
    
*   Texture: File could not be read error is thrown when a 16 bit .tif file is present in the project ([1404047](https://issuetracker.unity3d.com/issues/file-could-not-be-read-error-is-thrown-when-a-16-bit-tif-file-is-present-in-the-project))
    
*   uGUI: Immutable Package errors are thrown when selecting a Prefab containing Canvas Component ([1388532](https://issuetracker.unity3d.com/issues/core-render-pipeline-argumentexception-cant-save-an-immutable-prefab))
    
*   uGUI: Prefab is glitchy while editing in Prefab Mode when parent Canvas Render Mode is set to Screen Space - Camera ([1394756](https://issuetracker.unity3d.com/issues/prefab-is-glitchy-when-editing-in-prefab-mode-in-a-custom-ui-environment))
    
*   Web Platform: \[Linux\] Webgl build crashes every time when using Unity Editor on Linux ([1411380](https://issuetracker.unity3d.com/issues/linux-webgl-build-crashes-every-time-when-using-unity-editor-on-linux))
    
*   Web Platform: \[WebGL\] Profiler does not autoconnect on WebGL builds ([1387279](https://issuetracker.unity3d.com/issues/webgl-profiler-does-not-autoconnect-on-webgl-builds-1))
    
*   WebGL: WebGL Input System interactions are delayed or played preemptively when the project is built ([1405517](https://issuetracker.unity3d.com/issues/webgl-input-system-interactions-are-delayed-or-played-preemptively-when-the-project-is-built))