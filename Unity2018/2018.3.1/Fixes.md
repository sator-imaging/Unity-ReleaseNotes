# Unity 2018.3.1
https://unity3d.com/unity/whats-new/2018.3.1

## Fixes

<ul>
<li><p>Android: Removed extraneous log message that could be confused with a failure, when one did not occur 'Failed to load lib_burst_generated'. (<a href="https://issuetracker.unity3d.com/issues/burst-files-are-not-found-when-running-android-build">1059752</a>)</p></li>
<li><p>Animation: Fixed tangent mode not enforced when changing keyframe in recording mode. (<a href="https://issuetracker.unity3d.com/issues/clamp-auto-tangent-key-creation-is-not-accurate">1097109</a>)</p></li>
<li><p>Asset Import: Fixed crash when importing an R16 texture as a normal map. (1105211)</p></li>
<li><p>Build Pipeline: Fixed crash on AddBuildAssetInfoChecked when building project with scene that contains "Super Text Mesh" component. (<a href="https://issuetracker.unity3d.com/issues/crash-on-addbuildassetinfochecked-when-building-project-with-scene-that-contains-super-text-mesh-component">1031313</a>)</p></li>
<li><p>Editor: Allow Application.targetFramerate to be used when Time.captureFrameRate is set. (1100116)</p></li>
<li><p>Editor: Fixed issue with Menu items being enabled when modal windows are shown. (1093199)</p></li>
<li><p>Editor: Removed close X button on dock area tabs. (1105463)</p></li>
<li><p>Graphics: Fixed a legacy cubemap crash when its parameters are changed. (<a href="https://issuetracker.unity3d.com/issues/legacy-cubemap-crashes-when-parameters-are-changed">1038653</a>)</p></li>
<li><p>Graphics: Fixed against GPU driver assert for CopyTexture edge case. (<a href="https://issuetracker.unity3d.com/issues/metal-edge-length-tessellation-throws-compilation-error-when-using-vertex-normal-on-the-vertex-function">1065883</a>)</p></li>
<li><p>Graphics: Fixed an issue where unbound UAVs in shaders would cause the Editor to crash. (<a href="https://issuetracker.unity3d.com/issues/dx12-editor-switch-to-dx12-editor-crashes-if-object-in-scene-is-using-a-shader-with-uav-texture">988911</a>, 1098906)</p></li>
<li><p>Graphics: Fixed appdata not zero-initialized in domain shader causing compiler error about out parameter not being fully initialized.</p></li>
<li><p>Graphics: Fixed edge/inside tesselation factors being improperly handled. (<a href="https://issuetracker.unity3d.com/issues/metal-edge-length-tessellation-throws-compilation-error-when-using-vertex-normal-on-the-vertex-function">1065883</a>)</p></li>
<li><p>Graphics: Fixed shader translation of RWTexture2D. (1103036)</p></li>
<li><p>Graphics: Fixed vertex/hull shader program translation into a tessellation compute kernel when there is no vertex input. (1086957)</p></li>
<li><p>IL2CPP: Fixed crash when using StructLayout attribute and specifying a Pack value. (1099207)</p></li>
<li><p>IL2CPP: Fixed not checking the managed thread id at thread creation time to prevent it from being overwritten if it has already been set. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-the-unique-identifier-of-a-thread-differs-inside-and-outside-of-the-thread">1101331</a>)</p></li>
<li><p>iOS: Make "textures used in draw call" use our hash_set instead of std::set. (1061553)</p></li>
<li><p>Prefabs: Fixed exceptions when right clicking on a nested Model Prefab and choosing Open Prefab Asset. It now shows the "Open Model" menu item instead like for non-nested models. (<a href="https://issuetracker.unity3d.com/issues/improved-prefabs-argumentexception-raises-when-user-tries-to-use-open-prefab-asset-menu-item-on-models-child">1102433</a>, 1102759)</p></li>
<li><p>Prefabs: Fixed not possible to revert and apply default override properties via the property context menu again, as in previous versions of Unity. (1104791)</p></li>
<li><p>Prefabs: Fixed PrefabUtility.GetAddedGameObjects so it doesn't return added GameObjects that are themselves under added GameObjects. This is consistent with what we show in the Overrides dropdown. (1104805)</p></li>
<li><p>Prefabs: Fixed that after building a Player opening Prefab Mode fails with: 'Could not detect a Prefab root after loading'. (1107035)</p></li>
<li><p>SceneManager: Fixed editor crashing when creating a prefab of a GameObject whose parent's prefab instance is missing. (1107518)</p></li>
<li><p>Scripting: Editor: Fixed potential crash when deleting Assembly Definition Files (.asmdefs) in packages. (1101390)</p></li>
<li><p>Scripting: Fixed extreme rarely crash in Component.GetComponentsInChildren. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-getcomponentsinchildren-method">1088900</a>)</p></li>
<li><p>Scripting: Fixed plugins explicitly referencing from Assembly Definitions. (1110434)</p></li>
<li><p>Scripting Upgrade: Fixed crash when debugger invoked method with ref return. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-when-inspecting-a-ref-return-property-when-debugging-in-visual-studio">1076527</a>)</p></li>
<li><p>Shaders: Fixed ComputeShader.SetTextureFromGlobal() to work with 3d textures. (<a href="https://issuetracker.unity3d.com/issues/computeshader-dot-settexturefromglobal-errors-when-using-it-with-3d-rendertexture">1088840</a>, 1104047)</p></li>
<li><p>Shaders: Fixed Shader bundle does not rebuild when changing an included HLSL file. (<a href="https://issuetracker.unity3d.com/issues/shader-bundle-does-not-rebuild-when-changing-an-included-hlsl-file">1064917</a>)</p></li>
<li><p>Terrain: Fixed single pixel border artifact for height and collider after Undoing paint operation. (1104915)</p></li>
</ul>

#### Changeset: bb579dc42f1d
