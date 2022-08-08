# Unity 2019.1

https://unity3d.com/unity/whats-new/2019.1.0

## API Changes



*   2D: Added a new property TextureGenerationSettings.secondarySpriteTextures, which lets you assign secondary textures to the Sprite texture asset that is being generated.
    
*   2D: Added a new property TextureImporter.secondarySpriteTextures, which lets you assgin secondary textures to a texture asset imported as Sprite.
    
*   2D: Added a new struct UnityEngine.SecondarySpriteTexture, which encapsulates a Texture2D and its shader property name to give Sprite-based renderers access to a secondary texture, in addition to the main Sprite texture.
    
*   Android: Added Android API 28 (Pie)
    
*   Android: Added AndroidJNI methods which use sbyte parameters or return sbyte values (1069247)
    
*   Android: Deprecated AndroidJNI methods which use byte parameters or return byte values (1069247)
    
*   Android: Removed public API for setting the JVM Max heap size
    
*   Animation: Added `AnimationStream.GetInputWeight(int index)`.
    
*   Animation: Added `Animator.BindCustomStreamProperty(string propertyName, PropertyType type)` to UnityEngine.Experimental.Animations.
    
*   Animation: Made Playable delay features obsolete (Playable.Set/GetDelay).
    
*   Animation: Made writing to a scene handle obsolete (experimental API).
    
*   Asset Import: Added `AssetImporter.SupportsRemappedAssetType` to inform the user if the importer supports remapping certain Asset types (such as Materials).
    
*   Asset Import: Added `MaterialEditorExtensions.PerformBumpMapCheck`. This iterates over all Material properties with the Normal flag and checks that Unity imports the Textures they reference as normal maps.
    
*   Editor: Added more API points for `TransformHandle` to provide granular control over which handles appear.
    
*   Editor: Added new API to detect & control async shader compilation better in the Editor.
    
*   Editor: Added `AssemblyBuilder.referencesOptions` to allow building assemblies using `UnityEngine` module .dlls instead of the default monolithic UnityEngine.dll.
    
*   Editor: Added `CompilationPipeline.compilationStarted` and `CompilationPipeline.compilationFinished` events for when compilation starts and finishes in the Editor.
    
*   Editor: Added `CompilationPipeline.GetAssemblyDefinitionFilePathFromAssemblyReference`, `CompilationPipeline.GetAssemblyDefinitionReferenceType`, `CompilationPipeline.GUIDToAssemblyDefinitionReferenceGUID`, and `CompilationPipeline.AssemblyDefinitionReferenceGUIDToGUID` APIs for dealing with Assembly Definition File references that can be either a GUID or assembly name.
    
*   Editor: Added `EditorApplication.EnterPlayMode()` and `EditorApplication.ExitPlayMode()`.
    
*   Editor: Added `EditorUtility.GetDirtyCount()`, which returns how many times `SetDirty` is invoked on the specified Asset. The counter is reset to zero when the Asset is saved.
    
*   Editor: Added `EditorUtility.IsDirty()`, which returns `true` if `SetDirty` is invoked on the specified Asset.
    
*   Editor: Added `GameObjectUtility.GetMonoBehavioursWithMissingScriptCount` and `GameObjectUtility.RemoveMonoBehavioursWithMissingScript` to be able to remove MonoBehaviours with a missing script from a GameObject.
    
*   Editor: Added `Handles.TransformHandle()`.
    
*   Editor: Added `UnityEditor.ShortcutManagement` API for managing keyboard shortcuts in the editor.
    
*   Editor: Blocked illegal commands for Editor and PlayMode tests when in Play mode. (1093572)
    
*   Editor: Exposed `IShortcutManager.IsProfileIdValid` method for checking if a Shortcuts Manager profile ID is valid.
    
*   Editor: Exposed `ProjectWindowUtil.CreateScriptAssetFromTemplateFile`, which allows Editor scripts to create new text-based assets from template files. This is similar to how the built-in C# script template is used.
    
*   Editor: Fixed input fields for sliders that have a width lower than 150 with no label. ([1078003](https://issuetracker.unity3d.com/issues/impossible-to-enter-sliders-value-in-the-input-field-when-imgui-slider-is-of-a-width-of-less-than-150))
    
*   Editor: Renamed `SceneView.SceneViewCameraSettings` API to `SceneView.CameraSettings`.
    
*   GI: Added `Gizmos.exposure` texture which, when set, is read back to determine exposure correction for LightProbe gizmos. This is the alternative to correcting them via Post-processing.
    
*   Graphics: Added a simulatation function to fast-forward a VisualEffect.
    
*   Graphics: Added a variant static function for ShaderUtil.UpdateShaderAsset & ShaderUtil.CreateShaderAsset to skip compilation of the initial variant. This can save compilation time for ShaderGraph and Visual Effect Graph but it doesn't log any early compilation errors.
    
*   Graphics: Added Graphics and CommandBuffer method overloads to allow blitting to and from a texture array in the corresponding blit methods.
    
*   Graphics: Added Texture2DArray property "allSlices". The "allSlices" property can be used instead of "-1" to indicate that all texture array slices should be bound for methods that support texture arrays.
    
*   Graphics: Added the `Texture2D.normalTexture` property, which returns a small, neutral Normal Texture.
    
*   Graphics: Added UnityEngine.Rendering.GraphicsFence class to replace GPUFence.
    
*   Graphics: Added `Camera.HorizontalToVerticalFieldOfView(float horizontalFieldOfView, float aspectRatio)` and `Camera.VerticalToHorizontalFieldOfView(float verticalFieldOfView, float aspectRatio)` methods.
    
*   Graphics: Added `Material.ComputeCRC()`, which returns a CRC hash value of the Material Asset’s content.
    
*   Graphics: Added `Shader.GetDependency()` for querying a dependent shader by name.
    
*   Graphics: Added `SortingLayerRange` to `FilterRenderSettings` to allow for the filtering of sorting layers by `ScriptableRenderContext`.
    
*   Graphics: Changed the SRP signature of `BeginCameraRendering` and `BeginFrameRendering` to give access to the `ScriptableRenderContext`. Added callbacks for end camera and end frame rendering.
    
*   Graphics: Exposed setting for a number of jobs used when using occlusion culling.
    
*   Graphics: UnityEngine.Rendering.GPUFence class has been deprecated and replaced with UnityEngine.Rendering.GraphicsFence.
    
*   GraphView: Added a new constructor with `OnResized` callback parameter to `Resizer` manipulator.
    
*   GraphView: Added `canAcceptDrop` callback to `BlackBoardSection`.
    
*   GraphView: Added `OnResized` callback to `MiniMap`.
    
*   GraphView: Added `Renamable` capability to `GraphElement`.
    
*   GraphView: `GraphView.GetElementByGuid()` now returns the first element with the given GUID, within all of GraphView, not just elements contained in layers.
    
*   Kernel: Added a central cache for `TypeTrees`.
    
*   Memory Profiler: Added `Dispose` functionality to the `PackedMemorySnapshot` class to prevent instances from locking the snapshot file for longer than necessary.
    
*   Memory Profiler: Added `UnityEditor.Profiling.Memory.Experimental.PackedMemorySnapshot.Convert` to handle conversion from a `MemoryProfiler.PackedMemorysnapshot` object to a `UnityEditor.Profiling.Memory.Experimental.PackedMemorySnapshot` file.
    
*   Multiplayer: Added `NetworkTransport.SetMulticastLock` API to acquire/release multicast locks, which is required to receive broadcast packets on Android. ([988573](https://issuetracker.unity3d.com/issues/onreceivedbroadcast-not-called-on-android-slash-ios-devices-when-acting-as-a-client))
    
*   Package Manager: Exposed the `type` property of `PackageInfo`.
    
*   Physics: Added "Rigidbody2D.SetRotation(angle)" to allow you to set the Rigidbody2D z-axis rotation in degrees.
    
*   Physics: Added "Rigidbody2D.SetRotation(quaternion)" to allow you to set the Rigidbody2D rotation in quaternions.
    
*   Physics: Added Collider2D method overloads to provide List<> support for Raycast(), Cast(), GetContacts() and OverlapCollider().
    
*   Physics: Added CompositeCollider2D method overloads to provide List<> support for GetPath().
    
*   Physics: Added Physics2D method overloads to provide List<> support for LineCast(), RayCast(), BoxCast(), CapsuleCast(), CircleCast(), OverlapPoint, OverlapArea(), OverlapBox(), OverlapCapsule(), OverlapCircle(), OverlapCollider() and GetContacts().
    
*   Physics: Added PhysicsScene2D method overloads to provide List<> support for LineCast(), RayCast(), BoxCast(), CapsuleCast(), CircleCast(), OverlapPoint, OverlapArea(), OverlapBox(), OverlapCapsule(), OverlapCircle() and OverlapCollider().
    
*   Physics: Added PolygonCollider2D method overloads to provide List<> support for GetPath() and SetPath().
    
*   Physics: Added Rigidbody2D method overloads to provide List<> support for Cast(), GetContacts(), OverlapCollider() and GetAttachedColliders().
    
*   Physics: Added `Collision.GetContact(List)` and `Collision2D.GetContact(List)` methods.
    
*   Physics: Exposed additional query types in the PhysicsScene class. Note that only the non-allocating types are available.
    
*   Physics: Exposed `Physics.GetIgnoreCollision` class for checking whether the collision detection system ignores all collisions/triggers between two colliders.
    
*   Playables: Added an editor only method, `PlayableOutput.GetEditorName`, to get the PlayableOutput name.
    
*   Playables: Added `FrameData.effectivePlayState` to pass the accumulated PlayState of a Playable. (1077846)
    
*   Player: Deprecated ResolutionDialogSetting, PlayerSettings.displayResolutionDialog, and PlayerSettings.resolutionDialogBanner.
    
*   Profiler: Added `Profiler.EmitFrameMetaData` API for saving arbitrary data to the Profiler stream and reading it in the Editor.
    
*   Profiler: Exposed the Editor UI used to connect to a player from the Profiler or Console Window. In `UnityEditor.Experimental.Networking.PlayerConnection`, `EditorGUIUtility.GetAttachToPlayerState(EditorWindow parentWindow)` gets the connection state, and `EditorGUILayout/EditorGUI.AttachToPlayerDropdown` draws it.
    
*   Profiler: Exposed `UnityEditor.Profiling.HierarchyFrameDataView` API for accessing CPU Profiler data in a hierarchical way.
    
*   Profiler: Extended `HierarchyFrameDataView` profiling API with `ResolveItemCallstack` (returns a sample callstack in the Editor) and `GetItemMergedSamplesColumnDataAsFloats` (returns sample values for a merged sample).
    
*   Scripting: Added `GarbageCollector.isIncremental`, `GarbageCollector.incrementalTimeSliceNanoseconds`, and `GarbageCollector.CollectIncremental`.
    
*   Shaders: Added functions to the **ShaderUtil** class to retrieve and clear errors/warnings from Shader compilation. Also added the **ShaderMessage** class to provide error/warning details.
    
*   Shaders: Added the `Shader.FindPassTagValue` method for querying pass tag values.
    
*   Shaders: Added the `Shader.passCount` property for retrieving the number of shader passes of the active SubShader.
    
*   Shaders: Made the \[ShaderIncludePath\] attribute obsolete. All shader header files must be under the Assets folder or in a package. To include shader headers directly from a package, use `#include "Packages//`.
    
*   Terrain: Added a hotkey Terrain tool selection API, which lets you bind custom Terrain tools to hotkeys.
    
*   Terrain: Added a new version of the TerrainTools `ShowBrushGUI()` callback with flags for choosing which controls to display.
    
*   Terrain: Added a non-allocating version overload to the new `TerrainData.GetInterpolatedHeights` API.
    
*   Terrain: Added new callback APIs to monitor changes to Terrain Textures.
    
    *   `TerrainAPI.TerrainCallbacks.heightmapChanged`
    *   `TerrainAPI.TerrainCallbacks.textureChanged` These callbacks return both the rect region being changed, and whether the change is synchronized to the CPU or is GPU only.
*   Terrain: Added new TerrainData APIs to modify Terrain Textures more easily.
    
    *   `TerrainData.CopyActiveRenderTextureToHeightmap`
    *   `TerrainData.CopyActiveRenderTextureToTexture` Use the two above functions to copy content of the active RT into Terrain Textures, and optionally delay CPU synchronization, for instance, when a mousemove event occurs in the middle of painting.
        
    *   `TerrainData.DirtyHeightmapRegion`
        
    *   `TerrainData.DirtyTextureRegion` Use these two functions instead of ones initially listed if the user directly changes the GPU resources through other means.
        
    *   `TerrainData.SyncHeightmap`
        
    *   `TerrainData.SyncTexture` Use these two functions to perform a full synchronization from GPU to CPU, for instance, when a mouseup event occurs.
*   Terrain: Added the `TerrainData.GetInterpolatedHeights` method for querying interpolated Terrain height values over a grid of samples.
    
*   Terrain: Deprecated `Terrain.ApplyDelayedHeightmapModification`. Use `TerrainData.SyncHeightmap` instead.
    
*   Terrain: Improved the Terrain Stamp tool controls, and improved the tool’s behavior across Terrain of different height.
    
*   Terrain: Made the TerrainTools `IOnPaint.RepaintAllInspectors()` function obsolete. Replaced it with `Repaint(RepaintFlags)`, which is available in all Terrain Tool callback interfaces.
    
*   Timeline: Changed `TrackAsset.CreatePlayable(PlayableGraph, GameObject, TimelineClip)` to virtual to match its behavior in 2018.1. ([1096350](https://issuetracker.unity3d.com/issues/method-trackasset-dot-createplayable-cannot-be-overridden))
    
*   Timeline: Exposed methods for creating and manipulating animation curves on tracks.
    
*   Timeline: Exposed methods for working with infinite clips on Animation tracks.
    
*   Timeline: Exposed the FootIK property on Animation clips in Timeline. ([1115652](https://issuetracker.unity3d.com/issues/the-object-animation-is-clipping-when-adding-animation-in-the-timeline), 1121781)
    
*   XR: Added a command to set single-pass stereo mode with a command buffer. (1096603)