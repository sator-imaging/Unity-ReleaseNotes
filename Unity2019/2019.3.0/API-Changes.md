# Unity 2019.3.0
https://unity3d.com/unity/whats-new/2019.3.0

## API Changes

<ul>
<li><p>Android: Added: Added <code>UnityEditor.Android.AndroidExternalToolsSettings</code> to control External Tools Settings.</p></li>
<li><p>Animation: Added: Added <code>Animator.AddJobDependency(JobHandle)</code> to allow user to run jobs prior to animator jobs.</p></li>
<li><p>Animation: Changed: Moved Animation C# jobs out of experimental namespace <code>UnityEngine.Experimental.Animations</code> to <code>UnityEngine.Animations</code></p></li>
<li><p>Asset Import: Added: Added the <code>CollectImportedDependenciesAttribute</code> to allow users to set up dependencies on imported Assets (to be used from AssetPostprocessors).</p></li>
<li><p>Asset Import: Added: While importing a Model, you can now use <code>ModelImporter.avatarSetup</code> to change the way avatars are created, based on the AnimationType.</p></li>
<li><p>Asset Import: Changed: Renamed the <code>ModelImporterMaterialImportMode.Import</code> enum to <code>ModelImporterMaterialImportMode.ImportViaMaterialDescription</code>.</p></li>
<li><p>Asset Pipeline: Added: Added the experimental <code>AssetDatabaseExperimental.GetAvailableImporterTypes</code> API for listing the importer types which can handle an Asset type.</p></li>
<li><p>Audio: Added: New <code>AudioSettings.Mobile.interface</code> to detect mute state on Android/iOS and to stop/start AudioOutput thread to reduce energy consumption</p></li>
<li><p>Build Pipeline: Added: Expose <code>PackedAssets</code> class as part of the BuildReport, used for AssetBundle and sharedassets analysis</p></li>
<li><p>Build Pipeline: Obsoleted: Renamed <code>ContentBuildInterface.PrepareScene</code> to <code>ContentBuildInterface.CalculatePlayerDependenciesForScene</code></p></li>
<li><p>Build Pipeline: Obsoleted: Replaced <code>ContentBuildInterface.WriteSerializedFile</code> &amp; <code>WriteSceneSerializedFile</code> individual parameters with a struct of parameters</p></li>
<li><p>Editor: Added: Added <code>InitializeOnEnterPlayModeAttribute</code> to execute reset code for the configurable Enter Play Mode feature.</p></li>
<li><p>Editor: Added: Added <code>EditorTool.OnDrawHandles</code> method for drawing handles on inactive custom Editor tools.</p></li>
<li><p>Editor: Added: Added <code>EditorUtility.ClearDirty</code>, which tells Unity that an object is not dirty, and does not need to be saved to disk.</p></li>
<li><p>Editor: Added: Added <code>EditorUtility.DisplayDialog</code> overload that takes a <code>DialogOptOutDecision</code> Type and an identifying string. Using this overload gives users the the ability to opt-out of seeing modal system dialogs.</p></li>
<li><p>Editor: Added: Added <code>UnityEditor.Compilation.CompilationPipeline.RequestScriptCompilation</code> public API that allows user code to trigger script compilation.</p></li>
<li><p>Editor: Added: Added <code>UnityEditor.EditorUtility.RequestScriptReload</code> public API that allows Script reloading.</p></li>
<li><p>Editor: Changed: Added a new default API for Presets that works with a list instead of a single Preset, and supports default filtering.</p></li>
<li><p>Editor: Obsoleted: Marked the <code>UnityEditorInternal.InternalEditorUtility.RequestScriptReload</code> public API as obsolete.</p></li>
<li><p>Editor: Removed: Removed <code>EditorSnapSettings.active</code>, <code>EditorSnapSettings.enabled</code>, and <code>EditorSnapSettings.preferGrid</code>. Use <code>EditorSnapSettings.gridSnapEnabled</code> instead.</p></li>
<li><p>GI: Added: Added <code>Lightmapping.lightingDataUpdated</code> event. This event is called when the LightingDataAsset is updated.</p></li>
<li><p>GI: Added: Added API to set environment sample count for Progressive Lightmapper. <code>LightmapEditorSettings.environmentSampleCount</code>.</p></li>
<li><p>Graphics: Added: Added a binding on the <code>useColorTemperature</code> property of the light.</p></li>
<li><p>Graphics: Added: Added command buffer API to control single-pass instancing multiplier</p></li>
<li><p>Graphics: Added: Added index support to <code>Color32</code> struct.</p></li>
<li><p>Graphics: Added: Added initial event support for <code>VisualEffect</code>.</p></li>
<li><p>Graphics: Added: Added <code>InvokeOnRenderObjectCallback</code> to ScriptableRenderContext.</p></li>
<li><p>Graphics: Added: Added <code>SystemInfo.supportsRayTracing</code> to check whether you can create a D3D12 Raytracing Device on the current platform.</p></li>
<li><p>Graphics: Added: Exposed the default red, gray, and linear gray Texture objects via the <code>Texture2D.red</code>, <code>Texture2D.gray</code>, and <code>Texture2D.linearGray</code> properties.</p></li>
<li><p>Graphics: Added: Moved shader property APIs from <code>UnityEditor.ShaderUtils</code> to <code>UnityEngine.Shader</code> to make them available in players.<br> The APIs are:<br></p>

<ul>
<li><code>FindPropertyIndex</code><br></li>
<li><code>GetPropertyAttributes</code><br></li>
<li><code>GetPropertyCount</code><br></li>
<li><code>GetPropertyDefaultFloatValue</code><br></li>
<li><code>GetPropertyDefaultVectorValue</code><br></li>
<li><code>GetPropertyDescription</code><br></li>
<li><code>GetPropertyFlags</code><br></li>
<li><code>GetPropertyName</code><br></li>
<li><code>GetPropertyRangeLimits</code><br></li>
<li><code>GetPropertyTextureDefaultName</code><br></li>
<li><code>GetPropertyTextureDimension</code><br></li>
<li><code>GetPropertyType</code></li>
</ul></li>
<li><p>Graphics: Changed: Moved <code>RenderingThreadingMode</code> and <code>renderingThreadingMode</code> from <code>UnityEngine.Experimental.Rendering</code> namespace to <code>UnityEngine.Rendering</code> namespace</p></li>
<li><p>Graphics: Changed: Removed the Experimental tag from the following: <code>VisualEffect</code> component, <code>VisualEffectAsset</code>, and <code>VFXManager</code>.</p></li>
<li><p>Graphics: Changed: Renamed GPU Skinning on non-DirectX platforms to Compute Skinning</p></li>
<li><p>Graphics: Removed: Removed <code>TextureCompressionQuality</code> enum from the <code>UnityEngine</code> namespace. (1108722)</p></li>
<li><p>Graphics: Removed: Removed the <code>RenderPipelineManager</code> callbacks signatures that was not taking a <code>ScriptableRenderContext</code> in parameter</p></li>
<li><p>iOS: Deprecated: Open GLES2 and GLES3 have been deprecated on iOS and tvOS</p></li>
<li><p>Kernel: Added: Added <code>Unity.Jobs.LowLevel.Unsafe.JobWorkerCount</code> and <code>Unity.Jobs.LowLevel.Unsafe.JobWorkerMaximumCount</code> to query and set the number of job worker threads in the main Unity Job System</p></li>
<li><p>Kernel: Added: Added <code>Unity.Jobs.LowLevel.Unsafe.ResetJobWorkerCount</code> to reset the job worker count back to the Unity defaults</p></li>
<li><p>Package Manager: Added: Added the new <code>UnityEditor.PackageManager.UI.Window.Open</code> function to open the Package Manager window to a selected package.</p></li>
<li><p>Package Manager: Obsoleted: Renamed the <code>recommended</code> property <code>verified</code> on the <code>UnityEditor.PackageManager.PackageInfo</code> class.</p></li>
<li><p>Physics: Added: Added the ability to create a standard Unity Mesh from any Collider2D using "Collider2D.CreateMesh()"</p></li>
<li><p>Physics: Added: Added the ability to generate a hash value for any Collider2D geometry using "Collider2D.GetShapeHash()"</p></li>
<li><p>Playables: Obsoleted: Deprecated <code>PlayableOutput.SetSourceOutputPort</code> in favor of <code>PlayableOutput.SetSourceOutput(Playable, int)</code></p></li>
<li><p>Profiler: Added: Added <code>EditorConnection.UnregisterConnection</code>, <code>EditorConnection.UnregisterDisconnection</code>, <code>PlayerConnection.UnregisterConnection</code>, <code>PlayerConnection.UnregisterDisconnection</code></p></li>
<li><p>Profiler: Added: Added gcHandleIndex as a property to NativeObjectEntries within a PackedMemorySnapshot for simplified access to the index of it's managed counterpart</p></li>
<li><p>Profiler: Added: Added <code>HierarchyFrameDataView.columnStartTime</code> which gets the start time of Profiler samples.</p></li>
<li><p>Profiler: Added: Added TakeSnapshot overload with screenshot handling to the MemoryProfiler API</p></li>
<li><p>Scripting: Added: Add <code>EditorUserBuildSettings.waitForManagedDebugger</code>, instructs player to wait for managed debugger to attach before executing any scripts</p></li>
<li><p>Scripting: Added: Add the <code>TryGetComponent</code> API to GameObject and Component classes that do not allocate in the editor when the component does not exist</p></li>
<li><p>Scripting: Added: Added <code>PlatformSpecificOpenFileAtLine</code> to allow platform specific ways of executing applications.</p></li>
<li><p>Serialization: Added: Exposed API documentation for [SerializeReference]</p></li>
<li><p>Shaders: Obsoleted: Marked <code>ShaderUtil.ClearShaderErrors()</code> obsolete and replaced it with <code>ShaderUtil.ClearShaderMessages()</code>.</p></li>
<li><p>Terrain: Added: Added support for custom gather and scatter operations to the Terrain API.</p></li>
<li><p>Timeline: Added: Added <code>UnityEngine.Timeline.ILayerable</code> interface. Implement this interface to have custom tracks support multiple layers.</p></li>
<li><p>UI Elements: Obsoleted: <code>Button.onClick</code> is now obsolete. Use <code>Button.clicked</code> instead</p></li>
<li><p>Video: Removed: Removed <code>MovieTexture</code> class and API.</p></li>
<li><p>XR: Added: Added mirror view blit support to the display subsystem C# API.</p></li>
<li><p>XR: Added: Added more cross-platform/common stats to the display subsystem C# API.</p></li>
</ul>
