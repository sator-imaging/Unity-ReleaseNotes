# Unity 2019.1
https://unity3d.com/unity/whats-new/2019.1.0

## API Changes

<ul>
<li><p>2D: Added a new property TextureGenerationSettings.secondarySpriteTextures, which lets you assign secondary textures to the Sprite texture asset that is being generated.</p></li>
<li><p>2D: Added a new property TextureImporter.secondarySpriteTextures, which lets you assgin secondary textures to a texture asset imported as Sprite.</p></li>
<li><p>2D: Added a new struct UnityEngine.SecondarySpriteTexture, which encapsulates a Texture2D and its shader property name to give Sprite-based renderers access to a secondary texture, in addition to the main Sprite texture.</p></li>
<li><p>Android: Added Android API 28 (Pie)</p></li>
<li><p>Android: Added AndroidJNI methods which use sbyte parameters or return sbyte values (1069247)</p></li>
<li><p>Android: Deprecated AndroidJNI methods which use byte parameters or return byte values (1069247)</p></li>
<li><p>Android: Removed public API for setting the JVM Max heap size</p></li>
<li><p>Animation: Added <code>AnimationStream.GetInputWeight(int index)</code>.</p></li>
<li><p>Animation: Added <code>Animator.BindCustomStreamProperty(string propertyName, PropertyType type)</code> to UnityEngine.Experimental.Animations.</p></li>
<li><p>Animation: Made Playable delay features obsolete (Playable.Set/GetDelay).</p></li>
<li><p>Animation: Made writing to a scene handle obsolete (experimental API).</p></li>
<li><p>Asset Import: Added <code>AssetImporter.SupportsRemappedAssetType</code> to inform the user if the importer supports remapping certain Asset types (such as Materials).</p></li>
<li><p>Asset Import: Added <code>MaterialEditorExtensions.PerformBumpMapCheck</code>. This iterates over all Material properties with the Normal flag and checks that Unity imports the Textures they reference as normal maps.</p></li>
<li><p>Editor: Added more API points for <code>TransformHandle</code> to provide granular control over which handles appear.</p></li>
<li><p>Editor: Added new API to detect &amp; control async shader compilation better in the Editor.</p></li>
<li><p>Editor: Added <code>AssemblyBuilder.referencesOptions</code> to allow building assemblies using <code>UnityEngine</code> module .dlls instead of the default monolithic UnityEngine.dll.</p></li>
<li><p>Editor: Added <code>CompilationPipeline.compilationStarted</code> and <code>CompilationPipeline.compilationFinished</code> events for when compilation starts and finishes in the Editor.</p></li>
<li><p>Editor: Added <code>CompilationPipeline.GetAssemblyDefinitionFilePathFromAssemblyReference</code>, <code>CompilationPipeline.GetAssemblyDefinitionReferenceType</code>, <code>CompilationPipeline.GUIDToAssemblyDefinitionReferenceGUID</code>, and  <code>CompilationPipeline.AssemblyDefinitionReferenceGUIDToGUID</code> APIs for dealing with Assembly Definition File references that can be either a GUID or assembly name.</p></li>
<li><p>Editor: Added <code>EditorApplication.EnterPlayMode()</code> and <code>EditorApplication.ExitPlayMode()</code>.</p></li>
<li><p>Editor: Added <code>EditorUtility.GetDirtyCount()</code>, which returns how many times <code>SetDirty</code> is invoked on the specified Asset. The counter is reset to zero when the Asset is saved.</p></li>
<li><p>Editor: Added <code>EditorUtility.IsDirty()</code>, which returns <code>true</code> if <code>SetDirty</code> is invoked on the specified Asset.</p></li>
<li><p>Editor: Added <code>GameObjectUtility.GetMonoBehavioursWithMissingScriptCount</code> and <code>GameObjectUtility.RemoveMonoBehavioursWithMissingScript</code> to be able to remove MonoBehaviours with a missing script from a GameObject.</p></li>
<li><p>Editor: Added <code>Handles.TransformHandle()</code>.</p></li>
<li><p>Editor: Added <code>UnityEditor.ShortcutManagement</code> API for managing keyboard shortcuts in the editor.</p></li>
<li><p>Editor: Blocked illegal commands for Editor and PlayMode tests when in Play mode. (1093572)</p></li>
<li><p>Editor: Exposed <code>IShortcutManager.IsProfileIdValid</code> method for checking if a Shortcuts Manager profile ID is valid.</p></li>
<li><p>Editor: Exposed <code>ProjectWindowUtil.CreateScriptAssetFromTemplateFile</code>, which allows Editor scripts to create new text-based assets from template files. This is similar to how the built-in C# script template is used.</p></li>
<li><p>Editor: Fixed input fields for sliders that have a width lower than 150 with no label. (<a href="https://issuetracker.unity3d.com/issues/impossible-to-enter-sliders-value-in-the-input-field-when-imgui-slider-is-of-a-width-of-less-than-150">1078003</a>)</p></li>
<li><p>Editor: Renamed <code>SceneView.SceneViewCameraSettings</code>  API to <code>SceneView.CameraSettings</code>.</p></li>
<li><p>GI: Added <code>Gizmos.exposure</code> texture which, when set, is read back to determine exposure correction for LightProbe gizmos. This is the alternative to correcting them via Post-processing.</p></li>
<li><p>Graphics: Added a simulatation function to fast-forward a VisualEffect.</p></li>
<li><p>Graphics: Added a variant static function for ShaderUtil.UpdateShaderAsset &amp; ShaderUtil.CreateShaderAsset to skip compilation of the initial variant. This can save compilation time for ShaderGraph and Visual Effect Graph but it doesn't log any early compilation errors.</p></li>
<li><p>Graphics: Added Graphics and CommandBuffer method overloads to allow blitting to and from a texture array in the corresponding blit methods.</p></li>
<li><p>Graphics: Added Texture2DArray property "allSlices".  The "allSlices" property can be used instead of "-1" to indicate that all texture array slices should be bound for methods that support texture arrays.</p></li>
<li><p>Graphics: Added the <code>Texture2D.normalTexture</code> property, which returns a small, neutral Normal Texture.</p></li>
<li><p>Graphics: Added UnityEngine.Rendering.GraphicsFence class to replace GPUFence.</p></li>
<li><p>Graphics: Added <code>Camera.HorizontalToVerticalFieldOfView(float horizontalFieldOfView, float aspectRatio)</code> and <code>Camera.VerticalToHorizontalFieldOfView(float verticalFieldOfView, float aspectRatio)</code> methods.</p></li>
<li><p>Graphics: Added <code>Material.ComputeCRC()</code>, which returns a CRC hash value of the Material Asset’s content.</p></li>
<li><p>Graphics: Added <code>Shader.GetDependency()</code> for querying a dependent shader by name.</p></li>
<li><p>Graphics: Added <code>SortingLayerRange</code> to <code>FilterRenderSettings</code> to allow for the filtering of sorting layers by <code>ScriptableRenderContext</code>.</p></li>
<li><p>Graphics: Changed the SRP signature of <code>BeginCameraRendering</code> and <code>BeginFrameRendering</code> to give access to the <code>ScriptableRenderContext</code>. Added callbacks for end camera and end frame rendering.</p></li>
<li><p>Graphics: Exposed setting for a number of jobs used when using occlusion culling.</p></li>
<li><p>Graphics: UnityEngine.Rendering.GPUFence class has been deprecated and replaced with UnityEngine.Rendering.GraphicsFence.</p></li>
<li><p>GraphView: Added a new constructor with <code>OnResized</code> callback parameter to <code>Resizer</code> manipulator.</p></li>
<li><p>GraphView: Added <code>canAcceptDrop</code> callback to <code>BlackBoardSection</code>.</p></li>
<li><p>GraphView: Added <code>OnResized</code> callback to <code>MiniMap</code>.</p></li>
<li><p>GraphView: Added <code>Renamable</code> capability to <code>GraphElement</code>.</p></li>
<li><p>GraphView: <code>GraphView.GetElementByGuid()</code> now returns the first element with the given GUID, within all of GraphView, not just elements contained in layers.</p></li>
<li><p>Kernel: Added a central cache for <code>TypeTrees</code>.</p></li>
<li><p>Memory Profiler: Added <code>Dispose</code> functionality to the <code>PackedMemorySnapshot</code> class to prevent instances from locking the snapshot file for longer than necessary.</p></li>
<li><p>Memory Profiler: Added <code>UnityEditor.Profiling.Memory.Experimental.PackedMemorySnapshot.Convert</code> to handle conversion from a <code>MemoryProfiler.PackedMemorysnapshot</code> object to a <code>UnityEditor.Profiling.Memory.Experimental.PackedMemorySnapshot</code> file.</p></li>
<li><p>Multiplayer: Added <code>NetworkTransport.SetMulticastLock</code> API to acquire/release multicast locks, which is required to receive broadcast packets on Android. (<a href="https://issuetracker.unity3d.com/issues/onreceivedbroadcast-not-called-on-android-slash-ios-devices-when-acting-as-a-client">988573</a>)</p></li>
<li><p>Package Manager: Exposed the <code>type</code> property of <code>PackageInfo</code>.</p></li>
<li><p>Physics: Added "Rigidbody2D.SetRotation(angle)" to allow you to set the Rigidbody2D z-axis rotation in degrees.</p></li>
<li><p>Physics: Added "Rigidbody2D.SetRotation(quaternion)" to allow you to set the Rigidbody2D rotation in quaternions.</p></li>
<li><p>Physics: Added Collider2D method overloads to provide List&lt;&gt; support for Raycast(), Cast(), GetContacts() and OverlapCollider().</p></li>
<li><p>Physics: Added CompositeCollider2D method overloads to provide List&lt;&gt; support for GetPath().</p></li>
<li><p>Physics: Added Physics2D method overloads to provide List&lt;&gt; support for LineCast(), RayCast(), BoxCast(), CapsuleCast(), CircleCast(), OverlapPoint, OverlapArea(), OverlapBox(), OverlapCapsule(), OverlapCircle(), OverlapCollider() and GetContacts().</p></li>
<li><p>Physics: Added PhysicsScene2D method overloads to provide List&lt;&gt; support for LineCast(), RayCast(), BoxCast(), CapsuleCast(), CircleCast(), OverlapPoint, OverlapArea(), OverlapBox(), OverlapCapsule(), OverlapCircle() and OverlapCollider().</p></li>
<li><p>Physics: Added PolygonCollider2D method overloads to provide List&lt;&gt; support for GetPath() and SetPath().</p></li>
<li><p>Physics: Added Rigidbody2D method overloads to provide List&lt;&gt; support for Cast(), GetContacts(), OverlapCollider() and GetAttachedColliders().</p></li>
<li><p>Physics: Added <code>Collision.GetContact(List)</code> and <code>Collision2D.GetContact(List)</code> methods.</p></li>
<li><p>Physics: Exposed additional query types in the PhysicsScene class. Note that only the non-allocating types are available.</p></li>
<li><p>Physics: Exposed <code>Physics.GetIgnoreCollision</code> class for checking whether the collision detection system ignores all collisions/triggers between two colliders.</p></li>
<li><p>Playables: Added an editor only method, <code>PlayableOutput.GetEditorName</code>, to get the PlayableOutput name.</p></li>
<li><p>Playables: Added <code>FrameData.effectivePlayState</code> to pass the accumulated PlayState of a Playable. (1077846)</p></li>
<li><p>Player: Deprecated ResolutionDialogSetting, PlayerSettings.displayResolutionDialog, and PlayerSettings.resolutionDialogBanner.</p></li>
<li><p>Profiler: Added <code>Profiler.EmitFrameMetaData</code> API for saving arbitrary data to the Profiler stream and reading it in the Editor.</p></li>
<li><p>Profiler: Exposed the Editor UI used to connect to a player from the Profiler or Console Window. In <code>UnityEditor.Experimental.Networking.PlayerConnection</code>, <code>EditorGUIUtility.GetAttachToPlayerState(EditorWindow parentWindow)</code> gets the connection state, and <code>EditorGUILayout/EditorGUI.AttachToPlayerDropdown</code> draws it.</p></li>
<li><p>Profiler: Exposed <code>UnityEditor.Profiling.HierarchyFrameDataView</code> API for accessing CPU Profiler data in a hierarchical way.</p></li>
<li><p>Profiler: Extended <code>HierarchyFrameDataView</code> profiling API with <code>ResolveItemCallstack</code> (returns a sample callstack in the Editor) and <code>GetItemMergedSamplesColumnDataAsFloats</code> (returns sample values for a merged sample).</p></li>
<li><p>Scripting: Added <code>GarbageCollector.isIncremental</code>, <code>GarbageCollector.incrementalTimeSliceNanoseconds</code>,  and <code>GarbageCollector.CollectIncremental</code>.</p></li>
<li><p>Shaders: Added functions to the <strong>ShaderUtil</strong> class to retrieve and clear errors/warnings from Shader compilation. Also added the <strong>ShaderMessage</strong> class to provide error/warning details.</p></li>
<li><p>Shaders: Added the <code>Shader.FindPassTagValue</code> method for querying pass tag values.</p></li>
<li><p>Shaders: Added the <code>Shader.passCount</code> property for retrieving the number of shader passes of the active SubShader.</p></li>
<li><p>Shaders: Made the [ShaderIncludePath] attribute obsolete. All shader header files must be under the Assets folder or in a package. To include shader headers directly from a package, use <code>#include "Packages//</code>.</p></li>
<li><p>Terrain: Added a hotkey Terrain tool selection API, which lets you bind custom Terrain tools to hotkeys.</p></li>
<li><p>Terrain: Added a new version of the TerrainTools <code>ShowBrushGUI()</code> callback with flags for choosing which controls to display.</p></li>
<li><p>Terrain: Added a non-allocating version overload to the new <code>TerrainData.GetInterpolatedHeights</code> API.</p></li>
<li><p>Terrain: Added new callback APIs to monitor changes to Terrain Textures.</p> 
<ul>
<li><code>TerrainAPI.TerrainCallbacks.heightmapChanged</code></li>
<li><code>TerrainAPI.TerrainCallbacks.textureChanged</code>
These callbacks return both the rect region being changed, and whether the change is synchronized to the CPU or is GPU only.</li>
</ul></li>
<li><p>Terrain: Added new TerrainData APIs to modify Terrain Textures more easily.</p> 
<ul>
<li><code>TerrainData.CopyActiveRenderTextureToHeightmap</code></li>
<li><p><code>TerrainData.CopyActiveRenderTextureToTexture</code>
Use the two above functions to copy content of the active RT into Terrain Textures, and optionally delay CPU synchronization, for instance, when a mousemove event occurs in the middle of painting.</p></li>
<li><p><code>TerrainData.DirtyHeightmapRegion</code></p></li>
<li><p><code>TerrainData.DirtyTextureRegion</code>
Use these two functions instead of ones initially listed if the user directly changes the GPU resources through other means.</p></li>
<li><p><code>TerrainData.SyncHeightmap</code></p></li>
<li><code>TerrainData.SyncTexture</code>
Use these two functions to perform a full synchronization from GPU to CPU, for instance, when a mouseup event occurs.</li>
</ul></li>
<li><p>Terrain: Added the <code>TerrainData.GetInterpolatedHeights</code> method for querying interpolated Terrain height values over a grid of samples.</p></li>
<li><p>Terrain: Deprecated <code>Terrain.ApplyDelayedHeightmapModification</code>. Use <code>TerrainData.SyncHeightmap</code> instead.</p></li>
<li><p>Terrain: Improved the Terrain Stamp tool controls, and improved the tool’s behavior across Terrain of different height.</p></li>
<li><p>Terrain: Made the TerrainTools <code>IOnPaint.RepaintAllInspectors()</code> function obsolete. Replaced it with <code>Repaint(RepaintFlags)</code>, which is available in all Terrain Tool callback interfaces.</p></li>
<li><p>Timeline: Changed <code>TrackAsset.CreatePlayable(PlayableGraph, GameObject, TimelineClip)</code> to virtual to match its behavior in 2018.1. (<a href="https://issuetracker.unity3d.com/issues/method-trackasset-dot-createplayable-cannot-be-overridden">1096350</a>)</p></li>
<li><p>Timeline: Exposed methods for creating and manipulating animation curves on tracks.</p></li>
<li><p>Timeline: Exposed methods for working with infinite clips on Animation tracks.</p></li>
<li><p>Timeline: Exposed the FootIK property on Animation clips in Timeline. (<a href="https://issuetracker.unity3d.com/issues/the-object-animation-is-clipping-when-adding-animation-in-the-timeline">1115652</a>, 1121781)</p></li>
<li><p>XR: Added a command to set single-pass stereo mode with a command buffer. (1096603)</p></li>
</ul>
