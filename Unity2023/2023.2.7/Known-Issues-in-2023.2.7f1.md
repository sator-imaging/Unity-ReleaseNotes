# Unity 2023.2.7

https://unity.com/releases/editor/whats-new/2023.2.7

## Known Issues in 2023.2.7f1



*   3D Physics: inertiaTensor does not reset to the original value when setting Rigidbody constraints from FreezeAll to None ([UUM-59748](https://issuetracker.unity3d.com/issues/inertiatensor-does-not-reset-to-the-original-value-when-setting-rigidbody-constraints-from-freezeall-to-none))
    
*   Asset Bundles: UV1 data is lost during AssetBundle build when Optimize Mesh Data is on ([UUM-57201](https://issuetracker.unity3d.com/issues/uv1-data-is-lost-during-assetbundle-build-when-optimize-mesh-data-is-on))
    
*   Audio Authoring: Wrong tooltip when hovering over the "Load In Background" property of an audio clip ([UUM-27581](https://issuetracker.unity3d.com/issues/wrong-tooltip-when-hovering-over-the-load-in-background-property-of-an-audio-clip))
    
*   Audio Random Container: Memory leak when creating ARC prefab ([UUM-61023](https://issuetracker.unity3d.com/issues/memory-leak-when-creating-arc-prefab))
    
*   Culling: Crash on PrepareDrawShadowsCommandStep1 when selecting a camera while the Occlusion Culling window is open ([UUM-506](https://issuetracker.unity3d.com/issues/crash-on-preparedrawshadowscommandstep1-when-selecting-a-camera-while-the-occlusion-culling-window-is-open))
    
*   DirectX12: Crash on D3D12Fence::Wait when using Forward+ Rendering Path with Better Shaders asset ([UUM-57113](https://issuetracker.unity3d.com/issues/crash-on-d3d12fence-wait-when-using-forward-plus-rendering-path-with-better-shaders-asset))
    
*   HD RP: Prefab preview thumbnails are not being rendered when a Project uses HDRP ([UUM-60000](https://issuetracker.unity3d.com/issues/prefab-preview-thumbnails-are-not-being-rendered-when-a-project-uses-hdrp))
    
*   HD RP: \[AMD\] Crash on GfxDeviceD3D12Base::DrawBuffersCommon when Baking Light with Virtual Offset on Probe Volumes ([UUM-59522](https://issuetracker.unity3d.com/issues/amd-crash-on-gfxdeviced3d12base-drawbufferscommon-when-baking-light-with-virtual-offset-on-probe-volumes))
    
*   IAP: \[Android\] The Player crashes with a "JNI ERROR (app bug)" error when the global reference table gets overflowed by BillingClientStateListener ([UUM-55105](https://issuetracker.unity3d.com/issues/android-the-player-crashes-with-a-jni-error-app-bug-error-when-the-global-reference-table-gets-overflowed-by-billingclientstatelistener))
    
*   IL2CPP: \[Android\] Crash on Android when AndroidJavaProxy is calling from multiple threads ([UUM-49357](https://issuetracker.unity3d.com/issues/android-crash-on-android-when-androidjavaproxy-is-calling-from-multiple-threads))
    
*   Input: Crash on InputDeviceIOCTL when closing Unity editor ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))
    
*   MacOS: Mouse and keyboard button inputs are delayed when in the Player on macOS ([UUM-59176](https://issuetracker.unity3d.com/issues/mouse-and-keyboard-button-inputs-are-delayed-when-in-the-player-on-macos))
    
*   Mono: Crash in CollectManagedImportDependencyGetters inside OpenScene in batch mode ([UUM-57742](https://issuetracker.unity3d.com/issues/crash-in-collectmanagedimportdependencygetters-inside-openscene-in-batch-mode))
    
*   PhysX Integration: ConfigurableJoint's drives behave differently after the PhysX 4.1.2 update ([UUM-55081](https://issuetracker.unity3d.com/issues/rigidbody-components-values-do-not-translate-to-the-physx-calculations-when-they-are-being-overridden-via-a-script))
    
*   Platform Audio: \[WebGL\] A looping audio sounds different on WebGL than in the editor/native desktop player ([UUM-12530](https://issuetracker.unity3d.com/issues/webgl-a-looping-audio-sounds-different-on-webgl-than-in-the-editor-slash-native-desktop-player))
    
*   Progressive Lightmapper: The Editor becomes unresponsive and memory allocation errors are spammed in the Console when Generating Lightning ([UUM-58017](https://issuetracker.unity3d.com/issues/the-editor-becomes-unresponsive-and-memory-allocation-errors-are-spammed-in-the-console-when-generating-lightning))
    
*   RP Foundation: \[Android\] Player crashes when Allow Dynamic Resolution is enabled ([UUM-42922](https://issuetracker.unity3d.com/issues/android-player-crashes-when-allow-dynamic-resolution-is-enabled))
    
*   Scene Management: Crash on GameObject::QueryComponentByType when opening a project ([UUM-58461](https://issuetracker.unity3d.com/issues/crash-on-gameobject-querycomponentbytype-when-opening-a-project))
    
*   Scripting Buildtime: Unclearable nunit error when installing/uninstalling the Entities package on a new project ([UUM-58284](https://issuetracker.unity3d.com/issues/unclearable-nunit-error-when-installing-slash-uninstalling-the-entities-package-on-a-new-project))
    
*   Shortcut Management: Scene view Camera cannot be moved with WASD/QE keys when the Right Mouse Button is held down and the Mouse is not moved ([UUM-57993](https://issuetracker.unity3d.com/issues/scene-view-camera-cannot-be-moved-with-wasd-slash-qe-keys-when-the-right-mouse-button-is-held-down-and-the-mouse-is-not-moved))
    
*   UI Toolkit Controls: Editor crashes when multi-selecting GameObjects with more than one serialized \[Flags\] enum ([UUM-60654](https://issuetracker.unity3d.com/issues/editor-crashes-when-multi-selecting-gameoobjects-with-more-than-one-serialized-flags-enum))
    
*   XR SRP: \[Quest\] Stutter/Frame Pacing with OculusRuntime.WaitToBeginFrame when the Player is built ([UUM-27247](https://issuetracker.unity3d.com/issues/quest-stutter-slash-frame-pacing-with-oculusruntime-dot-waittobeginframe-when-the-player-is-built))