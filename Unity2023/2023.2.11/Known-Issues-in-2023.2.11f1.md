# Unity 2023.2.11

https://unity.com/releases/editor/whats-new/2023.2.11

## Known Issues in 2023.2.11f1



*   3D Physics: inertiaTensor does not reset to the original value when setting Rigidbody constraints from FreezeAll to None ([UUM-59748](https://issuetracker.unity3d.com/issues/inertiatensor-does-not-reset-to-the-original-value-when-setting-rigidbody-constraints-from-freezeall-to-none))
    
*   Asset - Database: Crash in CollectManagedImportDependencyGetters inside OpenScene in batch mode ([UUM-57742](https://issuetracker.unity3d.com/issues/crash-in-collectmanagedimportdependencygetters-inside-openscene-in-batch-mode))
    
*   Asset - Database: Memory leak when creating ARC prefab ([UUM-61023](https://issuetracker.unity3d.com/issues/memory-leak-when-creating-arc-prefab))
    
*   Asset Bundles: UV1 data is lost during AssetBundle build when Optimize Mesh Data is on ([UUM-57201](https://issuetracker.unity3d.com/issues/uv1-data-is-lost-during-assetbundle-build-when-optimize-mesh-data-is-on))
    
*   Asset Importers: Crash on ConvertBlenderToFBX while importing a specific .blend file ([UUM-63758](https://issuetracker.unity3d.com/issues/crash-on-convertblendertofbx-while-importing-a-specific-blend-file))
    
*   Audio Authoring: Crash on AudioUtil\_CUSTOM\_HasAudioCallback when exiting Play Mode while the Inspector is displaying a GameObject with a script attached ([UUM-58481](https://issuetracker.unity3d.com/issues/crash-on-audioutil-custom-hasaudiocallback-when-exiting-play-mode-while-the-inspector-is-displaying-a-gameobject-with-an-empty-script-attached))
    
*   DirectX12: Crash on D3D12Fence::Wait when using Forward+ Rendering Path with Better Shaders asset ([UUM-57113](https://issuetracker.unity3d.com/issues/crash-on-d3d12fence-wait-when-using-forward-plus-rendering-path-with-better-shaders-asset))
    
*   HD RP: Prefab preview thumbnails are not being rendered when a Project uses HDRP ([UUM-60000](https://issuetracker.unity3d.com/issues/prefab-preview-thumbnails-are-not-being-rendered-when-a-project-uses-hdrp))
    
*   HD RP: \[AMD\] Crash on GfxDeviceD3D12Base::DrawBuffersCommon when Baking Light with Virtual Offset on Probe Volumes ([UUM-59522](https://issuetracker.unity3d.com/issues/amd-crash-on-gfxdeviced3d12base-drawbufferscommon-when-baking-light-with-virtual-offset-on-probe-volumes))
    
*   IAP: \[Android\] The Player crashes with a "JNI ERROR (app bug)" error when the global reference table gets overflowed by BillingClientStateListener ([UUM-55105](https://issuetracker.unity3d.com/issues/android-the-player-crashes-with-a-jni-error-app-bug-error-when-the-global-reference-table-gets-overflowed-by-billingclientstatelistener))
    
*   IL2CPP: \[Android\] Crash on Android when AndroidJavaProxy is calling from multiple threads ([UUM-49357](https://issuetracker.unity3d.com/issues/android-crash-on-android-when-androidjavaproxy-is-calling-from-multiple-threads))
    
*   Input: Crash on InputDeviceIOCTL when closing Unity editor ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))
    
*   Metal: \[iOS\] App crashes with out of memory exception in UnityGfxDeviceWorker when starting the app ([UUM-55488](https://issuetracker.unity3d.com/issues/ios-app-crashes-with-out-of-memory-exception-in-unitygfxdeviceworker-when-starting-the-app))
    
*   Platform Audio: \[Linux\] No audio output when playing audio ([UUM-53143](https://issuetracker.unity3d.com/issues/linux-no-audio-output-when-playing-audio))
    
*   Progressive Lightmapper: The Editor becomes unresponsive and memory allocation errors are spammed in the Console when Generating Lightning ([UUM-58017](https://issuetracker.unity3d.com/issues/the-editor-becomes-unresponsive-and-memory-allocation-errors-are-spammed-in-the-console-when-generating-lightning))
    
*   RP Foundation: Stacked camera is not rendering when using custom post effects is done in PreRender PostRender and Camera is not in HDR ([UUM-22444](https://issuetracker.unity3d.com/issues/ios-stacked-camera-is-not-rendering-when-using-custom-post-effects-and-build-target-is-set-to-ios))
    
*   Scene Management: Crash on GameObject::QueryComponentByType when opening a project ([UUM-58461](https://issuetracker.unity3d.com/issues/crash-on-gameobject-querycomponentbytype-when-opening-a-project))