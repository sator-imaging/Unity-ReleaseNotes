# Unity 2018.1
https://unity3d.com/unity/whats-new/unity-2018.1.0

## API Changes

<ul>
<li><p>2D: Added <code>DetectChunkCullingBounds</code> to <code>TilemapRenderer</code> to allow for correct culling of large tiles. (<a href="https://issuetracker.unity3d.com/issues/tilemap-frustum-culling-is-culling-large-tiles-incorrectly">971087</a>)</p></li>
<li><p>2D: Experimental API <code>TextureGenerator.GenerateTexture</code> now takes in a NativeArrray for image buffer instead of setting an <code>IntPtr</code> in <code>TextureGenerationSettings</code>.</p></li>
<li><p>AI: Changed struct name in the Experimental API for Navmesh Queries from <code>PolygonID</code> to <code>PolygonId</code>.</p></li>
<li><p>AI: New experimental API for NavMesh queries, usable within C# jobs: <code>namespace UnityEngine.Experimental.AI</code>; <code>struct PolygonID</code>; <code>struct NavMeshLocation</code>; <code>enum PathQueryStatus</code>; <code>enum NavMeshPolyTypes</code>; <code>struct NavMeshWorld</code>; <strong><code>struct NavMeshQuery</code></strong> with these methods: <code>BeginFindPath()</code>, <code>UpdateFindPath()</code>, <code>EndFindPath()</code>, <code>GetPathResult()</code>, <code>IsValid()</code>, <code>GetAgentTypeIdForPolygon()</code>, <code>MapLocation()</code>, <code>GetPortalPoints()</code>, <code>MoveLocations()</code>, <code>MoveLocation()</code>, <code>PolygonLocalToWorldMatrix()</code>, <code>PolygonWorldToLocalMatrix()</code>, <code>GetPolygonType()</code>, <code>Dispose()</code>.</p></li>
<li><p>Animation: Added <code>AnimationClipPlayable.GetApplyPlayableIK</code> and <code>AnimationClipPlayable.SetApplyPlayableIK</code>.</p></li>
<li><p>Animation: Moved <code>AnimationUtility.SetGenerateMotionCurves</code> and <code>AnimationUtility.GetGenerateMotionCurves</code> from internal to public.</p></li>
<li><p>Animation: <code>AnimatorTransitionBase</code> and <code>Motion</code> are now abstract.</p></li>
<li><p>Animation: <code>AvatarBuilder.BuildHumanAvatar</code> is no longer supported on the .NET scripting backend.</p></li>
<li><p>Asset Import: Added <code>OnPreprocessAsset</code> callback in <code>AssetPostprocessor</code>. (Also see Features)</p></li>
<li><p>Asset Pipeline: API manual previously stated that <code>AssetDatabase.GetSubFolders()</code> takes absolute paths, which was incorrect.  This has now been updated to relative paths, consistent with other AssetDatabase methods.</p></li>
<li><p>Build Pipeline: Added <code>EditorBuildSettings</code> API methods: <code>AddConfigObject</code>, <code>TryGetConfigObject</code>, <code>GetConfigObjectNames</code>, <code>RemoveConfigObejct</code>.</p></li>
<li><p>Build Pipeline: Added <code>IPreprocessBuildWithReport</code>, <code>IPostprocessBuildWithReport</code>, and <code>IProcessSceneWithReport</code> interfaces to provide the BuildReport object during the build process.</p></li>
<li><p>Build Pipeline: Renamed <code>BuildSummary.errors</code> and <code>BuildSummary.warnings</code> to <code>BuildSummary.totalErrors</code> and <code>BuildSummary.totalWarnings</code> respectively.</p></li>
<li><p>Build Pipeline: Reverted <code>IPreprocessBuild</code>, <code>IPostprocessBuild</code> and <code>IProcessScene</code> interfaces to their 2017.3 signatures.</p></li>
<li><p>Build Pipeline: The <code>IPreprocessBuild</code>, <code>IPostprocessBuild</code> and <code>IProcessScene</code> interfaces have been changed to pass the <code>BuildReport</code> object instead of just the path to the build and target platform.</p></li>
<li><p>Build Pipeline: <code>BuildReport</code> API has been moved to the <code>UnityEditor.Build.Reporting</code> namespace.</p></li>
<li><p>Editor: Added <code>Application.wantsToQuit</code> and <code>Application.quitting</code> events.</p></li>
<li><p>Editor: Added <code>EditorApplication.hierarchyChanged</code> event and clarified API documentation.</p></li>
<li><p>Editor: Added <code>EditorApplication.projectChanged</code> event and clarified API documentation.</p></li>
<li><p>Editor: Added <code>UnityEngine.TestTools.Utils</code> to the Playmode test framework. This namespace contains utility classes to compare 'Vector2', 'Vector3', 'Vector4', <code>Quaternion</code>, Color and <code>float</code> types using <code>NUnit</code> constraints. (Also mentioned under Improvements)</p></li>
<li><p>Editor: Explicitly setting the following delegates to null will no longer draw a control handle, instead of drawing using a default implementation: <code>PrimitiveBoundsHandle.midpointHandleDrawFunction</code>, <code>ArcHandle.angleHandleDrawFunction</code>, <code>ArcHandle.radiusHandleDrawFunction</code>, <code>JointAngularLimitHandle.angleHandleDrawFunction</code>.</p></li>
<li><p>Editor: Explicitly setting the following delegates to null will now result in a handle size of 0 instead of using a default value: <code>PrimitiveBoundsHandle.midpointHandleSizeFunction</code>, <code>ArcHandle.angleHandleSizeFunction</code>, <code>ArcHandle.radiusHandleSizeFunction</code>, <code>JointAngularLimitHandle.angleHandleSizeFunction</code>.</p></li>
<li><p>Editor: <code>ColorPickerHDRConfig</code> is now obsolete and is no longer used.</p></li>
<li><p>Editor: <code>EditorApplication.hierarchyWindowChanged</code> is now obsolete, superceded by <code>EditorApplication.hierarchyChanged</code>.</p></li>
<li><p>Editor: <code>EditorApplication.projectWindowChanged</code> is now obsolete, superceded by <code>EditorApplication.projectChanged</code>.</p></li>
<li><p>Editor: <code>EditorGUI.ColorField()</code> and <code>EditorGUILayout.ColorField()</code> signatures taking a <code>ColorPickerHDRConfig</code> are now obsolete.</p></li>
<li><p>Editor: <code>UnityEditor.AndroidTargetDevice</code> is now obsolete, superceded by <code>UnityEditor.AndroidArchitecture</code>. <code>UnityEditor.PlayerSettings.targetDevice</code> is now obsolete, superceded by <code>UnityEditor.PlayerSettings.targetArchitectures</code>.</p></li>
<li><p>GI: Experimental Lightmapping scripting API now uses <code>NativeArray</code> instead of Lists.</p></li>
<li><p>Graphics: Added a new API to extract shader information (ShaderData).</p></li>
<li><p>Graphics: Exposed <code>RenderPipelineAsset.OnValidate</code> and <code>OnDisable</code> methods.</p></li>
<li><p>Graphics: <code>Graphics.ConvertTexture</code> now supports <code>RenderTexture</code> as source.</p></li>
<li><p>Graphics: <code>Texture</code> is now abstract.</p></li>
<li><p>Input: <code>TouchScreenKeybord.done</code> and <code>TouchScreenKeyboard.wasCanceled</code> are now obsolete, superceded by <code>UseTocuhScreenKeyboard.status</code>.</p></li>
<li><p>Multiplayer: Added <code>GetHostPort</code> function, reporting the port number assigned to the host.</p></li>
<li><p>Multiplayer: Deprecated unused function <code>NetworkTransport.GetAssetId()</code>. (<a href="https://issuetracker.unity3d.com/issues/unet-unetasset-getassetid-crashes-when-entering-to-play-mode">950325</a>)</p></li>
<li><p>Playables: New functions in <code>UnityEditor.Playables.Utility</code> to retrieve all the PlayableGraphs and events for when a PlayableGraph is created or destroyed.</p></li>
<li><p>Playables: New LeadTime feature allowing you to "pre-warm" the data inside the playable node.</p></li>
<li><p>Playables: PlayableGraphs can now have names.</p></li>
<li><p>Playables: <code>Playable.ConnectInput</code> can now optionally take a weight for the connected input.</p></li>
<li><p>Player: Added an experimental API which allows you to change the order in which engine systems are invoked, remove engine systems from the update order, or insert new C# entrypoints at any point in the update cycle: <code>UnityEngine.Experimental.LowLevel.PlayerLoop</code>. (Also mentioned under Features)</p></li>
<li><p>Player: Added <code>Application.wantsToQuit</code> and <code>Application.quitting</code> events.</p></li>
<li><p>Player: Deprecated <code>Application.CancelQuit</code> method.</p></li>
<li><p>Scripting: Added constructor for <code>TextAsset</code> that allows you to specify a string for its text contents.</p></li>
<li><p>Scripting: Added <code>ShaderUtil.GetAllShaderInfo</code> for listing all available shaders.</p></li>
<li><p>Scripting: Added <code>Vector2.Perpendicular</code> to calculate a perpendicular vector in 2D space.</p></li>
<li><p>Scripting: Extended <code>Vector2</code> to support component-wise multiplication and division between two <code>Vector2</code> values.</p></li>
<li><p>Scripting: Made unimplemented parameterless constructors for the following classes private: <code>AudioManager</code>, <code>EditorSettings</code>, <code>GraphicsSettings</code>, <code>InputManager</code>, <code>LightmapSettings</code>, <code>MonoManager</code>,<code>Physics2DSettings</code>, <code>PhysicsManager</code>, <code>PlayerSettings</code>, <code>QualitySettings</code>, <code>RenderSettings</code>, <code>Shader</code>, <code>Sprite</code>, <code>TagManager</code>, <code>TimeManager</code>, <code>AssetBundle</code>, <code>AssetBundleManifest</code>, <code>AudioClip</code>, <code>ComputeShader</code>, <code>LightingDataAsset</code>, <code>LightProbes</code>, <code>MovieTexture</code>, <code>ProceduralTexture</code>, <code>SceneAsset</code>, <code>SubstanceArchive</code>, <code>VideoClip</code>, <code>RuntimeAnimatorController</code>.</p></li>
<li><p>UI: Added <code>characterLimit</code> property for <code>TouchScreenKeyboard</code>.</p></li>
<li><p>XR: Added PlayerSettings <code>Get</code>/<code>SetVirtualRealitySupported</code>, <code>Get</code>/<code>SetVirtualRealitySDKs</code>, and <code>GetAvailableVirtualRealitySDKs</code> for acquiring and setting the XR Settings Virtual Reality Supported toggle and Virtual Reality SDKs list.</p></li>
<li><p>XR: Added <code>XR.WSA.HolographicSettings.IsContentProtectionEnabled</code>.</p></li>
<li><p>XR: Added <code>XR.WSA.HolographicSettings.ReprojectionMode</code>.</p></li>
</ul>
