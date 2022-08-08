# Unity 2019.3.0

https://unity3d.com/unity/whats-new/2019.3.0

## API Changes



*   Android: Added: Added `UnityEditor.Android.AndroidExternalToolsSettings` to control External Tools Settings.
    
*   Animation: Added: Added `Animator.AddJobDependency(JobHandle)` to allow user to run jobs prior to animator jobs.
    
*   Animation: Changed: Moved Animation C# jobs out of experimental namespace `UnityEngine.Experimental.Animations` to `UnityEngine.Animations`
    
*   Asset Import: Added: Added the `CollectImportedDependenciesAttribute` to allow users to set up dependencies on imported Assets (to be used from AssetPostprocessors).
    
*   Asset Import: Added: While importing a Model, you can now use `ModelImporter.avatarSetup` to change the way avatars are created, based on the AnimationType.
    
*   Asset Import: Changed: Renamed the `ModelImporterMaterialImportMode.Import` enum to `ModelImporterMaterialImportMode.ImportViaMaterialDescription`.
    
*   Asset Pipeline: Added: Added the experimental `AssetDatabaseExperimental.GetAvailableImporterTypes` API for listing the importer types which can handle an Asset type.
    
*   Audio: Added: New `AudioSettings.Mobile.interface` to detect mute state on Android/iOS and to stop/start AudioOutput thread to reduce energy consumption
    
*   Build Pipeline: Added: Expose `PackedAssets` class as part of the BuildReport, used for AssetBundle and sharedassets analysis
    
*   Build Pipeline: Obsoleted: Renamed `ContentBuildInterface.PrepareScene` to `ContentBuildInterface.CalculatePlayerDependenciesForScene`
    
*   Build Pipeline: Obsoleted: Replaced `ContentBuildInterface.WriteSerializedFile` & `WriteSceneSerializedFile` individual parameters with a struct of parameters
    
*   Editor: Added: Added `InitializeOnEnterPlayModeAttribute` to execute reset code for the configurable Enter Play Mode feature.
    
*   Editor: Added: Added `EditorTool.OnDrawHandles` method for drawing handles on inactive custom Editor tools.
    
*   Editor: Added: Added `EditorUtility.ClearDirty`, which tells Unity that an object is not dirty, and does not need to be saved to disk.
    
*   Editor: Added: Added `EditorUtility.DisplayDialog` overload that takes a `DialogOptOutDecision` Type and an identifying string. Using this overload gives users the the ability to opt-out of seeing modal system dialogs.
    
*   Editor: Added: Added `UnityEditor.Compilation.CompilationPipeline.RequestScriptCompilation` public API that allows user code to trigger script compilation.
    
*   Editor: Added: Added `UnityEditor.EditorUtility.RequestScriptReload` public API that allows Script reloading.
    
*   Editor: Changed: Added a new default API for Presets that works with a list instead of a single Preset, and supports default filtering.
    
*   Editor: Obsoleted: Marked the `UnityEditorInternal.InternalEditorUtility.RequestScriptReload` public API as obsolete.
    
*   Editor: Removed: Removed `EditorSnapSettings.active`, `EditorSnapSettings.enabled`, and `EditorSnapSettings.preferGrid`. Use `EditorSnapSettings.gridSnapEnabled` instead.
    
*   GI: Added: Added `Lightmapping.lightingDataUpdated` event. This event is called when the LightingDataAsset is updated.
    
*   GI: Added: Added API to set environment sample count for Progressive Lightmapper. `LightmapEditorSettings.environmentSampleCount`.
    
*   Graphics: Added: Added a binding on the `useColorTemperature` property of the light.
    
*   Graphics: Added: Added command buffer API to control single-pass instancing multiplier
    
*   Graphics: Added: Added index support to `Color32` struct.
    
*   Graphics: Added: Added initial event support for `VisualEffect`.
    
*   Graphics: Added: Added `InvokeOnRenderObjectCallback` to ScriptableRenderContext.
    
*   Graphics: Added: Added `SystemInfo.supportsRayTracing` to check whether you can create a D3D12 Raytracing Device on the current platform.
    
*   Graphics: Added: Exposed the default red, gray, and linear gray Texture objects via the `Texture2D.red`, `Texture2D.gray`, and `Texture2D.linearGray` properties.
    
*   Graphics: Added: Moved shader property APIs from `UnityEditor.ShaderUtils` to `UnityEngine.Shader` to make them available in players.  
    The APIs are:  
    
    *   `FindPropertyIndex`  
        
    *   `GetPropertyAttributes`  
        
    *   `GetPropertyCount`  
        
    *   `GetPropertyDefaultFloatValue`  
        
    *   `GetPropertyDefaultVectorValue`  
        
    *   `GetPropertyDescription`  
        
    *   `GetPropertyFlags`  
        
    *   `GetPropertyName`  
        
    *   `GetPropertyRangeLimits`  
        
    *   `GetPropertyTextureDefaultName`  
        
    *   `GetPropertyTextureDimension`  
        
    *   `GetPropertyType`
*   Graphics: Changed: Moved `RenderingThreadingMode` and `renderingThreadingMode` from `UnityEngine.Experimental.Rendering` namespace to `UnityEngine.Rendering` namespace
    
*   Graphics: Changed: Removed the Experimental tag from the following: `VisualEffect` component, `VisualEffectAsset`, and `VFXManager`.
    
*   Graphics: Changed: Renamed GPU Skinning on non-DirectX platforms to Compute Skinning
    
*   Graphics: Removed: Removed `TextureCompressionQuality` enum from the `UnityEngine` namespace. (1108722)
    
*   Graphics: Removed: Removed the `RenderPipelineManager` callbacks signatures that was not taking a `ScriptableRenderContext` in parameter
    
*   iOS: Deprecated: Open GLES2 and GLES3 have been deprecated on iOS and tvOS
    
*   Kernel: Added: Added `Unity.Jobs.LowLevel.Unsafe.JobWorkerCount` and `Unity.Jobs.LowLevel.Unsafe.JobWorkerMaximumCount` to query and set the number of job worker threads in the main Unity Job System
    
*   Kernel: Added: Added `Unity.Jobs.LowLevel.Unsafe.ResetJobWorkerCount` to reset the job worker count back to the Unity defaults
    
*   Package Manager: Added: Added the new `UnityEditor.PackageManager.UI.Window.Open` function to open the Package Manager window to a selected package.
    
*   Package Manager: Obsoleted: Renamed the `recommended` property `verified` on the `UnityEditor.PackageManager.PackageInfo` class.
    
*   Physics: Added: Added the ability to create a standard Unity Mesh from any Collider2D using "Collider2D.CreateMesh()"
    
*   Physics: Added: Added the ability to generate a hash value for any Collider2D geometry using "Collider2D.GetShapeHash()"
    
*   Playables: Obsoleted: Deprecated `PlayableOutput.SetSourceOutputPort` in favor of `PlayableOutput.SetSourceOutput(Playable, int)`
    
*   Profiler: Added: Added `EditorConnection.UnregisterConnection`, `EditorConnection.UnregisterDisconnection`, `PlayerConnection.UnregisterConnection`, `PlayerConnection.UnregisterDisconnection`
    
*   Profiler: Added: Added gcHandleIndex as a property to NativeObjectEntries within a PackedMemorySnapshot for simplified access to the index of it's managed counterpart
    
*   Profiler: Added: Added `HierarchyFrameDataView.columnStartTime` which gets the start time of Profiler samples.
    
*   Profiler: Added: Added TakeSnapshot overload with screenshot handling to the MemoryProfiler API
    
*   Scripting: Added: Add `EditorUserBuildSettings.waitForManagedDebugger`, instructs player to wait for managed debugger to attach before executing any scripts
    
*   Scripting: Added: Add the `TryGetComponent` API to GameObject and Component classes that do not allocate in the editor when the component does not exist
    
*   Scripting: Added: Added `PlatformSpecificOpenFileAtLine` to allow platform specific ways of executing applications.
    
*   Serialization: Added: Exposed API documentation for \[SerializeReference\]
    
*   Shaders: Obsoleted: Marked `ShaderUtil.ClearShaderErrors()` obsolete and replaced it with `ShaderUtil.ClearShaderMessages()`.
    
*   Terrain: Added: Added support for custom gather and scatter operations to the Terrain API.
    
*   Timeline: Added: Added `UnityEngine.Timeline.ILayerable` interface. Implement this interface to have custom tracks support multiple layers.
    
*   UI Elements: Obsoleted: `Button.onClick` is now obsolete. Use `Button.clicked` instead
    
*   Video: Removed: Removed `MovieTexture` class and API.
    
*   XR: Added: Added mirror view blit support to the display subsystem C# API.
    
*   XR: Added: Added more cross-platform/common stats to the display subsystem C# API.