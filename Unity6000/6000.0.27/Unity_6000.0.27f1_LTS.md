# Unity 6000.0.27f1 LTS
Published at Thu, 14 Nov 2024 07:07:52 GMT  
https://unity.com/releases/editor/whats-new/6000.0.27

# Known Issues in 6000.0.27f1

- Asset - Database: Crash on GetAssetCachedInfoV2 when opening a project
    ([UUM-14959](https://issuetracker.unity3d.com/issues/crash-on-getassetcachedinfov2-when-opening-a-project))

- Asset - Database: Crash on MonoBehaviour::Transfer<GenerateTypeTreeTransfer> when the XR Interaction Toolkit Sample Assets are updated
    ([UUM-76934](https://issuetracker.unity3d.com/issues/crash-on-monobehaviour-transfer-when-the-xr-interaction-toolkit-sample-assets-are-updated))

- DirectX12: Allocated graphics memory does not get released when the Editor is out of focus while using D3D12 graphics API
    ([UUM-86354](https://issuetracker.unity3d.com/issues/allocated-graphics-memory-does-not-get-released-when-the-editor-is-out-of-focus-while-using-d3d12-graphics-api))

- DirectX12: The Camera does not render correctly when the Camera.Rect() is changed and HDR is enabled and DX12 graphics API is selected
    ([UUM-86917](https://issuetracker.unity3d.com/issues/the-camera-does-not-render-correctly-when-the-camera-dot-rect-is-changed-and-hdr-is-enabled-and-dx12-graphics-api-is-selected))

- Graphics Device Features: [Quest] Editor crashes on toggleFoveation when activating SRP Foveated Rendering in DX12
    ([UUM-85208](https://issuetracker.unity3d.com/issues/quest-editor-crashes-on-togglefoveation-when-activating-srp-foveated-rendering-in-dx12))

- HDRP: Graphics Compositor breaks Unity rendering when the "Output Camera" is changed to a scene Camera and one Camera SubLayer is active.<br>
    https://issuetracker.unity3d.com/product/unity/issues/guid/UUM-84610

- Input: Crash on InputDeviceIOCTL when closing Unity editor
    ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))

- Scripting Runtime: Crash on tlsf_free when exiting Play Mode in a specific project
    ([UUM-86106](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-exiting-play-mode-in-a-specific-project))

- Shader System: Shaders are always recompiled when the Editor is opened
    ([UUM-75262](https://issuetracker.unity3d.com/issues/shaders-are-always-recompiled-when-the-editor-is-opened))

- SpeedTree: This release of SpeedTree includes a change to the interface of the SpeedTree8Wind shadergraph node. If you have an animated SpeedTree in the shadergraph, be sure to connect an ObjectSpacePosition node to the input of the SpeedTree8Wind.  If the wind node does not have an input on the ObjectSpacePosition port, the mesh will be shrunk down to a point at origin \(making it seem to vanish\).<br>
    https://issuetracker.unity3d.com/product/unity/issues/guid/UUM-84616

- Terrain: Trees do not render in 'Unity Terrain - URP Demo Scene'
    ([UUM-84616](https://issuetracker.unity3d.com/issues/trees-do-not-render-in-unity-terrain-urp-demo-scene))

- Text: Editor hangs when rendering TMP Text Component with Left and Right Margins set in the Extra Settings
    ([UUM-84379](https://issuetracker.unity3d.com/issues/editor-hangs-when-rendering-tmp-text-component-with-left-and-right-margins-set-in-the-extra-settings))

- Vulkan: [Android] Particles not rendered in the Player on some Android devices with Android 14
    ([UUM-68080](https://issuetracker.unity3d.com/issues/android-particles-not-rendered-in-the-player-on-some-android-devices-with-android-14))



# 6000.0.27f1 Release Notes

## Fixes

- 2D: Fixed light blending issues with shadows.
    ([UUM-82787](https://issuetracker.unity3d.com/issues/2d-light-overlap-order-is-not-evaluated-when-shadows-are-being-produced-with-render-graph-compatibility-mode-disabled))

- Documentation: Improved EventInterestAttribute documentation by specifying what happens with event types that are not part of an EventInterestAttribute argument.
    ([UUM-79521](https://issuetracker.unity3d.com/issues/eventinterestattribute-does-not-filter-all-other-events-when-clickevent-is-specified))

- Editor: Fixed a crash that would occur due to memory corruption in the Burst domain after logging a warning to the Editor console.
    ([UUM-78956](https://issuetracker.unity3d.com/issues/crash-on-unload-thread-main-when-reloading-scripts-after-switching-to-debug-mode))

- Editor: Fixed a warning about probe volume.
    ([UUM-75179](https://issuetracker.unity3d.com/issues/hdrp-water-multiple-shader-warnings-are-thown-in-the-console-after-building-water-samples-scenes))

- Editor: Fixed an issue for 'Recursive serialization is not allowed for threaded serialization' when the build profile context instance is created in a serialization callback.
    (UUM-84096)

- Editor: Fixed an issue there the export window maintains initial selection after selecting different items in the Project Browser.
    (UUM-82656)

- Editor: Fixed an issue when moving the registration of the SceneViewMotion and RectSelection shortcut contexts to the OnEnable method of the Scene view.
    ([UUM-86183](https://issuetracker.unity3d.com/issues/scene-view-freezes-when-nullreferenceexception-is-thrown-in-a-delaycall))

- Editor: Fixed an issue where Android build profiles with player settings overrides weren't behaving based on the value of the scripting backed setting of the build profile, but instead were behaving based on the global/project settings player setting value.
    (UUM-85834)

- Editor: Fixed an issue where Screen Space Shadows did not work on Decals.
    ([UUM-81517](https://issuetracker.unity3d.com/issues/screen-space-decals-stop-receiving-shadows-when-screen-space-shadows-is-enabled-and-rendering-path-is-set-to-forward-or-forwads-plus))

- Editor: Fixed an issue where sometimes the Editor Tools system would not refresh when the selection changes while the Inspector window is locked.
    (UUM-54858)

- Editor: Fixed an issue where the default humanoid in the animation preview window would be pink when the auto option was selected.
    (UUM-84489)

- Editor: Fixed an issue with emojis in TextField on mobile.
    ([UUM-72689](https://issuetracker.unity3d.com/issues/android-writing-text-or-adding-more-emojis-after-an-emoji-in-the-inputfield-causes-the-first-emoji-to-disappear-and-be-changed-to-two-question-marks-when-hide-mobile-input-is-enabled-on-some-android-devices))

- Editor: Fixed an issue with missing legacy deformers shapes for new water decal.
    (UUM-85483)

- Editor: Fixed corrupted Font crashing the editor when opened in FontAssetCreator.
    ([UUM-78705](https://issuetracker.unity3d.com/issues/crash-on-textcore-fontengine-getfontfaces-slash-errors-are-thrown-when-reopening-the-font-asset-creator-when-a-specific-font-is-selected-as-the-source-font))

- Editor: Fixed crash that occurred during Multiplayer Role Stripping when using scenes that contained Do Not Destroy On Load components.
    (MTTB-533)

- Editor: Fixed sprite asset fallbacks not working on a job.
    ([UUM-85568](https://issuetracker.unity3d.com/issues/sprites-are-not-generated-when-using-fallback-sprite-assets))

- Editor: Mouse jumping is disabled on Linux when using Wayland.
    ([UUM-82831](https://issuetracker.unity3d.com/issues/linux-wayland-slider-values-or-scene-view-moves-exponentially-faster-when-moving-the-mouse-to-a-side-of-the-monitor))

- Entities: Fixed an issue where an exception would be thrown when exiting play mode after closing and opening a sub scene.
    ([UUM-86554](https://issuetracker.unity3d.com/issues/missing-prefab-error-appears-in-the-console-window-when-re-importing-the-sub-scene-containing-a-prefab-during-repeated-entry-into-play-mode))

- Graphics: Fixed an issue where RayTracingAccelerationStructure.AddInstances assigning the same instance ID to all ray tracing instances added to the acceleration structure, making it impossible to identify individual instances added using this function.
    ([UUM-85733](https://issuetracker.unity3d.com/issues/raytracing-impossible-to-identify-individual-instances-added-using-rtas-dot-addinstances-in-a-compute-shader-when-using-ray-queries))

- Graphics: Fixed an Issue where resizing the SceneView would throw errors.
    ([UUM-83527](https://issuetracker.unity3d.com/issues/rendertexture-create-failed-errors-are-shown-in-the-console-when-the-scene-window-is-shrunk-with-bloom-intensity-set-to-1))

- Graphics: Fixed crash when using native graphics jobs on Metal.
    ([UUM-44469](https://issuetracker.unity3d.com/issues/player-crashes-without-stack-frames-in-metal-submission-thread-on-macos-when-graphics-jobs-are-enabled))

- Graphics: \[Metal\] Fixed an issue where the blend state and color mask specified in Shader Passes were not applied to the correct render targets.
    ([UUM-83382](https://issuetracker.unity3d.com/issues/ios-silicon-colormask-render-target-3-and-above-does-not-work-correctly-when-using-multiple-render-target))

- HDRP: Fixed an issue that caused HDAdditionalLightData with preserveCachedShadow to be evicted from the cachedShadowManager.
    ([UUM-83766](https://issuetracker.unity3d.com/issues/unable-to-add-renderer-to-the-scene-after-culling-dot-and-nullreferenceexception-object-reference-not-set-to-an-instance-of-an-object-errors-spawned-when-changing-the-light-shadow-settings-in-the-player))

- Physics: Fixed an issue where the CharacterController component would not properly have it's transform synced to the data set to the Transform component.
    ([UUM-83065](https://issuetracker.unity3d.com/issues/ontriggerenter-is-triggered-when-editing-character-controller-slope-limit))

- Physics: Fixed Repeated OnTriggerEnter Events with CharacterController Slope Limit Updates.
    ([UUM-83065](https://issuetracker.unity3d.com/issues/ontriggerenter-is-triggered-when-editing-character-controller-slope-limit))

- Physics: Renamed serialized property names within Rigidbody component: Drag and AngularDrag are now LinearDamping and AngularDamping. The change was done in order to no longer be inconsistent with respect to the Rigidbody API which already adheres to this naming convention.
    (PHYS-396)

- Scene/Game View: Fixed an issue with EditorTools icon not showing when importing a new package.
    (UUM-86481)

- Shadergraph: Fixed an issue where the shader graph was not marked dirty when toggling checkboxes in its Graph Settings.
    (UUM-83383)

- Shaders: Fixed a rare crash when saving the tracked shader variants into a variant collection.
    ([UUM-86510](https://issuetracker.unity3d.com/issues/editor-crash-when-saving-currently-tracked-variants-to-asset))

- Shaders: Fixed an issue with the shader compiler crashing when encountering a kernel directive without a provided name.
    ([UUM-85898](https://issuetracker.unity3d.com/issues/internal-shader-error-is-shown-when-a-corrupted-shader-is-imported))

- SRP Core: Fixed an issue where Lens Flare was not rendering properly in OpenGLES3.
    (UUM-84431)

- Terrain: Fixed an issue in which calling terrainData.SyncTexture\(TerrainData.HolesTextureName\) causes a crash when no holes have been created before due to a null variable.
    (UUM-76880)

- uGUI: Fixed exception thrown when pasting text into TMP inputfield with custom validator.
    ([UUM-76312](https://issuetracker.unity3d.com/issues/argumentoutofrangeexception-is-thrown-when-using-textmeshpro-input-field-with-custom-validator))

- Undo System: Fixed an issue by marking array size changes to keep duplicates within a single undo action.
    (UUM-84565)

- Universal RP: Fixed an issue where Game View would flip upside down when using HDR Debug Mode.
    ([UUM-83764](https://issuetracker.unity3d.com/issues/game-view-is-flipped-upside-down-when-hdr-debug-mode-is-set-to-gamut-view-in-the-lighting-rendering-debugger))

- Universal RP: Fixed an issue with warning \(Missing types referenced from component UniversalRenderPipelineGlobalSettings...\) caused by URP Template project on platforms where ENABLE_VR is not defined.
    ([UUM-82247](https://issuetracker.unity3d.com/issues/missing-types-referenced-from-component-universalrenderpipelineglobalsettings-on-game-object-universalrenderpipelineglobalsettings-dot-dot-dot-warning-is-thrown-after-switching-the-platform-to-tvos))

- VFX Graph: Fixed an issue when creating a Custom HLSL operator with two outputs could prevent the generated shader from compiling.
    ([UUM-83676](https://issuetracker.unity3d.com/issues/vfx-custom-hlsl-operator-with-two-output-parameters-function-duplicates-its-code))

- VFX Graph: Fixed an issue when using the same name as a built-in attribute in a custom HLSL function's parameter would lead to a compilation error.
    ([UUM-83782](https://issuetracker.unity3d.com/issues/vfx-graph-hsls-redefinition-error-when-input-have-the-same-name-as-attributes))

- Web: Improved error message in abort handler.
    ([UUM-83890](https://issuetracker.unity3d.com/issues/webgl-unclear-error-when-gzip-compressed-data-or-webassembly-dont-have-correct-http-headers))

- WebGL: \[WebGPU\] Fixed an error with write_buffer for memory addresses greater than 2GB.
    (UUM-85703)

- WebGL: \[WebGPU\] Fixed AsyncGPUReadback for textures when request format is specified.
    (UUM-85988)

- Windows: Fixed an issue where changing the default icon is not refreshed by Windows Explorer when re-building a project into the same build folder used previously.
    ([UUM-71022](https://issuetracker.unity3d.com/issues/changing-the-default-icon-does-not-change-the-executables-icon-when-re-building-the-project))

- XR: Fixed crash with foveated rendering in D3D12.
    ([UUM-85208](https://issuetracker.unity3d.com/issues/quest-editor-crashes-on-togglefoveation-when-activating-srp-foveated-rendering-in-dx12))




## Package changes in 6000.0.27f1

## Packages updated

- com.unity.xr.oculus: [4.3.0](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.3//changelog/CHANGELOG.html) to [4.4.0](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.4//changelog/CHANGELOG.html)

- com.unity.transport: [2.3.0](https://docs.unity3d.com/Packages/com.unity.transport@2.3//changelog/CHANGELOG.html) to [2.4.0](https://docs.unity3d.com/Packages/com.unity.transport@2.4//changelog/CHANGELOG.html)