# Unity 2019.1.4
https://unity3d.com/unity/whats-new/2019.1.4

## Fixes

<ul>
<li><p>2D: Foxed sprite atlases being packed when entering Play Mode when Sprite Packer Mode is set to "Enabled for builds". (<a href="https://issuetracker.unity3d.com/issues/sprite-atlases-are-packed-by-entering-play-mode-when-sprite-packer-mode-is-set-to-enabled-for-builds">1136349</a>, 1148006)</p></li>
<li><p>Android: Fixed a crash when SRP batcher is enabled on Vulkan on Mali GPUs. (1141817, 1149380)</p></li>
<li><p>Android: Fixed wrong rendering in LWRP on GPUs that have EGL_GL_COLORSPACE_SRGB_KHR extension. (1145351, 1149381)</p></li>
<li><p>Asset Import: Fixed an issue where blendshapes normals are always recalculated although the blend shape normals import setting is set to 'none'. (<a href="https://issuetracker.unity3d.com/issues/blend-shape-normals-are-always-calculating-even-when-its-set-to-none-in-import-settings">1123265</a>, 1140796)</p></li>
<li><p>Asset Import: Fixed an issue where blendShapes normals are broken when upgrading the project. (<a href="https://issuetracker.unity3d.com/issues/blendshapes-normals-are-broken-when-upgrading-the-project">1117764</a>, 1150188)</p></li>
<li><p>Asset Import: Fixed an issue where normal import settings get applied to the whole selection when selecting multiple model assets. (1150179)</p></li>
<li><p>Asset Import: Fixed an issue where some kinds of assets might not refresh after an Editor restart using ADB v1. (<a href="https://issuetracker.unity3d.com/issues/assetdatabase-does-not-refresh-asset-after-editor-restart">1140289</a>, 1149023)</p></li>
<li><p>Asset Import: Fixed the root node of a model importer preset to be visible and editable. (<a href="https://issuetracker.unity3d.com/issues/editor-root-node-value-comes-as-null-when-creating-fbx-preset">1144441</a>, 1150227)</p></li>
<li><p>Core: Fixed executing an IJobParallelFor accessing deallocated memory and cause Unity to crash. (1153961, 1157296)</p></li>
<li><p>Editor: Ensured duplicated prefabs retains transform values and other overrides. (<a href="https://issuetracker.unity3d.com/issues/game-objects-are-moved-to-random-places-when-duplicating-prefabs">1132860</a>, 1152739)</p></li>
<li><p>Editor: Fixed an Editor crash when clicking Shader dropdown in Material inspector. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-in-shader-issupported-when-trying-to-change-materials-shader-hdrp-slash-lit-to-any-other-shader-via-a-dropdown-menu">1150686</a>, 1154053)</p></li>
<li><p>Editor: Fixed crash when duplicating prefabs with ConfigurableJoints. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-with-transform-getposition-when-duplicating-prefabs-with-configurable-joints">1137347</a>, 1152740)</p></li>
<li><p>Editor: Fixed importing badly broken prefab variants where components could be assigned to multiple GameObjects. (<a href="https://issuetracker.unity3d.com/issues/editor-crashing-when-selecting-a-prefab-variant">1113802</a>, 1152733)</p></li>
<li><p>Editor: Fixed interacting with custom property drawer array resets the scroll bar position. (<a href="https://issuetracker.unity3d.com/issues/selected-array-element-in-the-inspector-carries-value-over-to-other-elements-when-scrolling">1109673</a>, 1117759, <a href="https://issuetracker.unity3d.com/issues/mouse-click-does-not-select-the-correct-array-element-in-the-inspector-window-while-scrolling">1132074</a>, 1151035)</p></li>
<li><p>Editor: Fixed reverting files in Collab occasionally displaying a blank message. (1151178, 1151182)</p></li>
<li><p>Editor: Removed Extra FileIDs property that appears for some assets in the inspector. (1103218, 1155362)</p></li>
<li><p>Graphics: Fixed issue with large scaled meshes with texture mip map streaming. (<a href="https://issuetracker.unity3d.com/issues/fbx-model-exported-with-specific-measuring-units-loses-texture-quality-upon-scene-switching">1058192</a>, 1149319)</p></li>
<li><p>Graphics: Fixed Unsupported textures such as reflection probes now load highest mip. (<a href="https://issuetracker.unity3d.com/issues/texture-streaming-loads-wrong-mipmap-levels-when-the-associated-transforms-scale-is-not-equal-to-one">1139189</a>, 1148714)</p></li>
<li><p>IAP: Fixed editor crashing when updating/installing/importing IAP plugin. (<a href="https://issuetracker.unity3d.com/issues/iap-editor-crashes-when-updating-slash-installing-slash-importing-iap-plugin">1138783</a>, 1149292)</p></li>
<li><p>iOS: Fixed larger than 2k payloads not sent by UnityWebRequest when HTTP/2. (<a href="https://issuetracker.unity3d.com/issues/mobile-unitywebrequest-fails-sending-post-request-if-the-server-supports-http-slash-2-with-no-fallback-to-http-slash-1">1146305</a>, 1152777)</p></li>
<li><p>OSX: [Metal] Fixed excessive fencing causing all GPU workload to be serialized. (1154010)</p></li>
<li><p>Package Manager: Fixed import of Complete Project category Asset Store Packages from 2018.1-2018.3, which could break Package Manager configuration in the importing project. (1139199, 1139263)</p></li>
<li><p>Particles: Fixed particle rendering inconsistencies between Windows and macOS when a particle is generated by specifying RandomSeed. (<a href="https://issuetracker.unity3d.com/issues/particle-rendering-inconsistencies-between-windows-and-macos-when-a-particle-is-generated-by-specifying-randomseed">1138802</a>, 1142738)</p></li>
<li><p>Profiler: Fixed an issue where the compilation guards for the memory profiler API would not reset after doing a player build. (<a href="https://issuetracker.unity3d.com/issues/memory-profiler-cancels-spanshot-due-to-compilation-in-progress-after-build-and-run">1152043</a>)</p></li>
<li><p>Profiler: Reduced profiler overhead when flushing data from Job threads. (1147129, 1151146)</p></li>
<li><p>SceneManager: Fixed default shortcuts missing from SceneVis, Isolation and multi-hide are inaccessible. (1124247, 1144482)</p></li>
<li><p>Services: Fixed crash from background thread on UWP when Crash Reporting is enabled. (1130184, 1150581)</p></li>
<li><p>Terrain: Fixed terrain's Texture2D texture appearing white when copied using Instantiate Method via Script. (<a href="https://issuetracker.unity3d.com/issues/terrains-texture2d-texture-appears-white-when-copied-using-instantiate-method-via-script">1126400</a>, 1148331)</p></li>
<li><p>Timeline: Fixe the PlayableGraph from being created twice when playing a timeline in play mode with the Timeline window opened.F (1147247, 1148481)</p></li>
<li><p>Web: Fixed encoding support in url escaping. (<a href="https://issuetracker.unity3d.com/issues/unitywebrequest-unitywebrequest-dot-escapeurl-ignores-specified-encoding-when-creating-the-url">1151016</a>, 1152779)</p></li>
<li><p>Windows: Fixed documentation summary in Visual Studio not being shown. (<a href="https://issuetracker.unity3d.com/issues/documentation-summary-in-visual-studio-is-not-being-shown">1148065</a>, 1148634)</p></li>
<li><p>XR: Fixed crash when transitioning to VR Mode from non-VR. (1150910, 1152534)</p></li>
<li><p>XR: Fixed shell script permission denied error with Google VR when building iOS using the generated xcode project. (<a href="https://issuetracker.unity3d.com/issues/google-vr-xcode-permission-denied-on-shell-scripts">1129546</a>, 1155363)</p></li>
</ul>
