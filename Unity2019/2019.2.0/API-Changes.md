# Unity 2019.2.0

https://unity3d.com/unity/whats-new/2019.2.0

## API Changes



*   AI: Added the `GetEdgesAndNeighbors()` method in the `NavMeshQuery` class for retrieving the shape of a given node and all the navigation nodes which it connects to. The method can be called in jobs.
    
*   Android: Added support for JNI Weak References (`AndroidJNI` class).
    
*   Asset Import: Added an API in the Model Importer to prevent GameObjects from being sorted by name in imported GameObject hierarchies.
    
*   Editor: Added API for Scene Visibility.
    
*   Editor: Added more API endpoints for `TransformHandle` to allow granular control over which handles appear.
    
*   Editor: Added new API to better detect and control async shader compilation in the Editor.
    
*   Editor: Added `AssemblyBuilder.referencesOptions` to allow building assemblies using UnityEngine module .dlls instead of the default monolithic UnityEngine.dll.
    
*   Editor: Added `AssetDatabase.OpenAsset()` overloads that take both a line number and column number.
    
*   Editor: Added `Editor.DrawFoldoutInspector` to draw a nested Inspector with a foldout title bar.
    
*   Editor: Added `EditorWindow.CreateWindow`, which works like `EditorWindow.GetWindow`, but always creates a new window.
    
*   Editor: Added `GameObjectUtility.GetMonoBehavioursWithMissingScriptCount` and `GameObjectUtility.RemoveMonoBehavioursWithMissingScript`for removing MonoBehaviours with missing scripts from GameObjects.
    
*   Editor: Added `MaterialEditor.customShaderGUI` property that returns the active ShaderGUI object for the current material.
    
*   Editor: Changing the display name of enum values in the Inspector is now done using the `InspectorNameAttribute` instead of the `DescriptionAttribute`. ([1115381](https://issuetracker.unity3d.com/issues/drawdefaultinspector-displays-enums-differently-from-editorguilayout-dot-enumpopup-when-using-cusom-inspector))
    
*   Editor: Renamed `SceneView.SceneViewCameraSettings` to `SceneView.CameraSettings`.
    
*   Editor: Replaced `EditorTool.OnActivate` and `OnDeactivate` methods with `EditorTools` events. This addresses callback order problems.
    
*   Editor: `OnOpenAsset` attribute now supports method signature `(int instanceId, int line, int column)`
    
*   GI: Added `Gizmos.exposure` texture which, when set, is readback to determine exposure correction for LightProbe gizmos.
    
*   GI: Made it so you can set Lightmap Parameters from scripts on non-prefab objects. ([966408](https://issuetracker.unity3d.com/issues/lightmap-settings-of-game-object-is-not-saved-if-game-object-is-not-prefab))
    
*   Graphics: Added the static function, Inverse3DAffine(), to Matrix4x4 to compute the inverse of an affine matrix.
    
*   Graphics: Changed the SRP signature of `BeginCameraRendering` and `BeginFrameRendering` to give access to the `ScriptableRenderContext`. Added callbacks for end camera and end frame rendering.
    
*   Kernel: The function, UnsafeUtility.MemCpyReplicate(), no longer logs a failed assertion or raises an exception when the size or Count parameters are zero. Instead, it passively exits (like the other UnsafeUtility methods).
    
*   Mobile: Added 'Screen.cutouts' which displays cutout bounding boxes
    
*   Mobile: Added `Application.absoluteURL` property and `Application.deepLinkActivated` event which handles application activation via deep link.
    
*   Package Manager: Added an Editor API for retrieving package information based on an Asset path or an assembly:
    
    *   `PackageManager.PackageInfo.FindForAssetPath(string assetPath)`
    *   `PackageManager.PackageInfo.FindForAssembly(Assembly assembly)`
*   Scripting: Added the `TryGetComponent`API to GameObject and Component classes that do not allocate in the Editor when the component does not exist.
    
*   Scripting: Added `UnityEditor.TypeCache` API which extracts derived types, methods or classes marked with an attribute quickly.
    
*   Shaders: Added the `Shader.FindPassTagValue` method for querying pass tag values.
    
*   Shaders: Added the `Shader.passCount` property for retrieving the number of shader passes of the active SubShader.
    
*   Terrain: Added a non-alloc version overload to the new `TerrainData.GetInterpolatedHeights` API.
    
*   Terrain: Added new callback APIs to monitor changes to Terrain Textures.
    
    *   `TerrainAPI.TerrainCallbacks.heightmapChanged`
    *   `TerrainAPI.TerrainCallbacks.textureChanged` These callbacks return both the changed rect region, and whether the change is synchronized to the CPU or is GPU only.
*   Terrain: Added new TerrainData APIs to modify Terrain Textures more easily.
    
    *   `TerrainData.CopyActiveRenderTextureToHeightmap`
    *   `TerrainData.CopyActiveRenderTextureToTexture` Use the two above functions to copy content of the active RT into Terrain Textures, and optionally delay CPU synchronization, for instance, when a mousemove event occurs in the middle of painting.
        
    *   `TerrainData.DirtyHeightmapRegion`
        
    *   `TerrainData.DirtyTextureRegion` Use these two functions instead of ones initially listed if the user directly changes the GPU resources through other means.
        
    *   `TerrainData.SyncHeightmap`
        
    *   `TerrainData.SyncTexture` Use these two functions to perform a full synchronization from GPU to CPU, for instance, when a mouseup event occurs.
*   Terrain: Added the `TerrainData.GetInterpolatedHeights` method for querying interpolated Terrain height values over a grid of samples.
    
*   Terrain: Added `TerrainData.SetTerrainLayersRegisterUndo` for setting the `terrainLayers` property. This function also lets undo operations in the Editor correctly handle Textures created or destroyed during the process.
    
*   Terrain: Deprecate TerrainData.UpdateDirtyRegion. Use TerrainData.DirtyHeightmapRegion instead.
    
*   Terrain: Deprecated `Terrain.ApplyDelayedHeightmapModification`. Use `TerrainData.SyncHeightmap` instead.
    
*   Terrain: Exposed the `TerrainLayerInspector` class.
    
*   Timeline: Added FootIK property to Timeline Animation clips. ([1115652](https://issuetracker.unity3d.com/issues/the-object-animation-is-clipping-when-adding-animation-in-the-timeline))
    
*   Timeline: Added the ClipEditor, TrackEditor, and MarkerEditor classes to UnityEditor.Timeline so a user can derive and modify custom clips, tracks, or markers respectively.
    
*   Timeline: Added TimelineEditor.selectedClip and TimelineEditor.selectedClips to get and set the selected clip or clips TimelineClips in the Timeline window.
    
*   Timeline: Added TrackAsset.mutedInHierarchy that indicates that a track is muted when it is in a muted group.
    
*   Video: Added overloads to MediaEncoder.AddFrame to accept timestamps for producing Variable Frame Rate movies. The timestamps are expressed with the new MediaTime struct.
    
*   Video: Added the sRGBClip property to VideoClipImporter and the sRGB property to VideoClip. These properties describe whether the content is sRGB or linear.
    
*   Video: Added Time.captureDeltaTime: a more precise floating point reciprocal of Time.captureFramerate.
    
*   XR: Added the XRSetting property `XR.XRSettings.deviceEyeTextureDimension` which allows you to determine what the XR platform's swap chain eye texture layout is.
    
*   XR: Added `UNITY_INITIALIZE_OUTPUT_STEREO_EYE_INDEX` to the built-in shader macros to allow for transfering the unity\_StereoEyeIndex from a vertex shader to a geometry shader.
    
*   XR: Added `XR.XRDevice.UpdateEyeTextureAntiAliasingSettings` to force the hmd swap chain to be reallocated when the MSAA sample count is changed.