# Unity 2018.1

https://unity3d.com/unity/whats-new/unity-2018.1.0

## API Changes



*   2D: Added `DetectChunkCullingBounds` to `TilemapRenderer` to allow for correct culling of large tiles. ([971087](https://issuetracker.unity3d.com/issues/tilemap-frustum-culling-is-culling-large-tiles-incorrectly))
    
*   2D: Experimental API `TextureGenerator.GenerateTexture` now takes in a NativeArrray for image buffer instead of setting an `IntPtr` in `TextureGenerationSettings`.
    
*   AI: Changed struct name in the Experimental API for Navmesh Queries from `PolygonID` to `PolygonId`.
    
*   AI: New experimental API for NavMesh queries, usable within C# jobs: `namespace UnityEngine.Experimental.AI`; `struct PolygonID`; `struct NavMeshLocation`; `enum PathQueryStatus`; `enum NavMeshPolyTypes`; `struct NavMeshWorld`; **`struct NavMeshQuery`** with these methods: `BeginFindPath()`, `UpdateFindPath()`, `EndFindPath()`, `GetPathResult()`, `IsValid()`, `GetAgentTypeIdForPolygon()`, `MapLocation()`, `GetPortalPoints()`, `MoveLocations()`, `MoveLocation()`, `PolygonLocalToWorldMatrix()`, `PolygonWorldToLocalMatrix()`, `GetPolygonType()`, `Dispose()`.
    
*   Animation: Added `AnimationClipPlayable.GetApplyPlayableIK` and `AnimationClipPlayable.SetApplyPlayableIK`.
    
*   Animation: Moved `AnimationUtility.SetGenerateMotionCurves` and `AnimationUtility.GetGenerateMotionCurves` from internal to public.
    
*   Animation: `AnimatorTransitionBase` and `Motion` are now abstract.
    
*   Animation: `AvatarBuilder.BuildHumanAvatar` is no longer supported on the .NET scripting backend.
    
*   Asset Import: Added `OnPreprocessAsset` callback in `AssetPostprocessor`. (Also see Features)
    
*   Asset Pipeline: API manual previously stated that `AssetDatabase.GetSubFolders()` takes absolute paths, which was incorrect. This has now been updated to relative paths, consistent with other AssetDatabase methods.
    
*   Build Pipeline: Added `EditorBuildSettings` API methods: `AddConfigObject`, `TryGetConfigObject`, `GetConfigObjectNames`, `RemoveConfigObejct`.
    
*   Build Pipeline: Added `IPreprocessBuildWithReport`, `IPostprocessBuildWithReport`, and `IProcessSceneWithReport` interfaces to provide the BuildReport object during the build process.
    
*   Build Pipeline: Renamed `BuildSummary.errors` and `BuildSummary.warnings` to `BuildSummary.totalErrors` and `BuildSummary.totalWarnings` respectively.
    
*   Build Pipeline: Reverted `IPreprocessBuild`, `IPostprocessBuild` and `IProcessScene` interfaces to their 2017.3 signatures.
    
*   Build Pipeline: The `IPreprocessBuild`, `IPostprocessBuild` and `IProcessScene` interfaces have been changed to pass the `BuildReport` object instead of just the path to the build and target platform.
    
*   Build Pipeline: `BuildReport` API has been moved to the `UnityEditor.Build.Reporting` namespace.
    
*   Editor: Added `Application.wantsToQuit` and `Application.quitting` events.
    
*   Editor: Added `EditorApplication.hierarchyChanged` event and clarified API documentation.
    
*   Editor: Added `EditorApplication.projectChanged` event and clarified API documentation.
    
*   Editor: Added `UnityEngine.TestTools.Utils` to the Playmode test framework. This namespace contains utility classes to compare 'Vector2', 'Vector3', 'Vector4', `Quaternion`, Color and `float` types using `NUnit` constraints. (Also mentioned under Improvements)
    
*   Editor: Explicitly setting the following delegates to null will no longer draw a control handle, instead of drawing using a default implementation: `PrimitiveBoundsHandle.midpointHandleDrawFunction`, `ArcHandle.angleHandleDrawFunction`, `ArcHandle.radiusHandleDrawFunction`, `JointAngularLimitHandle.angleHandleDrawFunction`.
    
*   Editor: Explicitly setting the following delegates to null will now result in a handle size of 0 instead of using a default value: `PrimitiveBoundsHandle.midpointHandleSizeFunction`, `ArcHandle.angleHandleSizeFunction`, `ArcHandle.radiusHandleSizeFunction`, `JointAngularLimitHandle.angleHandleSizeFunction`.
    
*   Editor: `ColorPickerHDRConfig` is now obsolete and is no longer used.
    
*   Editor: `EditorApplication.hierarchyWindowChanged` is now obsolete, superceded by `EditorApplication.hierarchyChanged`.
    
*   Editor: `EditorApplication.projectWindowChanged` is now obsolete, superceded by `EditorApplication.projectChanged`.
    
*   Editor: `EditorGUI.ColorField()` and `EditorGUILayout.ColorField()` signatures taking a `ColorPickerHDRConfig` are now obsolete.
    
*   Editor: `UnityEditor.AndroidTargetDevice` is now obsolete, superceded by `UnityEditor.AndroidArchitecture`. `UnityEditor.PlayerSettings.targetDevice` is now obsolete, superceded by `UnityEditor.PlayerSettings.targetArchitectures`.
    
*   GI: Experimental Lightmapping scripting API now uses `NativeArray` instead of Lists.
    
*   Graphics: Added a new API to extract shader information (ShaderData).
    
*   Graphics: Exposed `RenderPipelineAsset.OnValidate` and `OnDisable` methods.
    
*   Graphics: `Graphics.ConvertTexture` now supports `RenderTexture` as source.
    
*   Graphics: `Texture` is now abstract.
    
*   Input: `TouchScreenKeybord.done` and `TouchScreenKeyboard.wasCanceled` are now obsolete, superceded by `UseTocuhScreenKeyboard.status`.
    
*   Multiplayer: Added `GetHostPort` function, reporting the port number assigned to the host.
    
*   Multiplayer: Deprecated unused function `NetworkTransport.GetAssetId()`. ([950325](https://issuetracker.unity3d.com/issues/unet-unetasset-getassetid-crashes-when-entering-to-play-mode))
    
*   Playables: New functions in `UnityEditor.Playables.Utility` to retrieve all the PlayableGraphs and events for when a PlayableGraph is created or destroyed.
    
*   Playables: New LeadTime feature allowing you to "pre-warm" the data inside the playable node.
    
*   Playables: PlayableGraphs can now have names.
    
*   Playables: `Playable.ConnectInput` can now optionally take a weight for the connected input.
    
*   Player: Added an experimental API which allows you to change the order in which engine systems are invoked, remove engine systems from the update order, or insert new C# entrypoints at any point in the update cycle: `UnityEngine.Experimental.LowLevel.PlayerLoop`. (Also mentioned under Features)
    
*   Player: Added `Application.wantsToQuit` and `Application.quitting` events.
    
*   Player: Deprecated `Application.CancelQuit` method.
    
*   Scripting: Added constructor for `TextAsset` that allows you to specify a string for its text contents.
    
*   Scripting: Added `ShaderUtil.GetAllShaderInfo` for listing all available shaders.
    
*   Scripting: Added `Vector2.Perpendicular` to calculate a perpendicular vector in 2D space.
    
*   Scripting: Extended `Vector2` to support component-wise multiplication and division between two `Vector2` values.
    
*   Scripting: Made unimplemented parameterless constructors for the following classes private: `AudioManager`, `EditorSettings`, `GraphicsSettings`, `InputManager`, `LightmapSettings`, `MonoManager`,`Physics2DSettings`, `PhysicsManager`, `PlayerSettings`, `QualitySettings`, `RenderSettings`, `Shader`, `Sprite`, `TagManager`, `TimeManager`, `AssetBundle`, `AssetBundleManifest`, `AudioClip`, `ComputeShader`, `LightingDataAsset`, `LightProbes`, `MovieTexture`, `ProceduralTexture`, `SceneAsset`, `SubstanceArchive`, `VideoClip`, `RuntimeAnimatorController`.
    
*   UI: Added `characterLimit` property for `TouchScreenKeyboard`.
    
*   XR: Added PlayerSettings `Get`/`SetVirtualRealitySupported`, `Get`/`SetVirtualRealitySDKs`, and `GetAvailableVirtualRealitySDKs` for acquiring and setting the XR Settings Virtual Reality Supported toggle and Virtual Reality SDKs list.
    
*   XR: Added `XR.WSA.HolographicSettings.IsContentProtectionEnabled`.
    
*   XR: Added `XR.WSA.HolographicSettings.ReprojectionMode`.