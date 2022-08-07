# Unity 2018.3.2
https://unity3d.com/unity/whats-new/2018.3.2

## Fixes

<ul>
<li><p>Animation: Fixed race condition crash in Legacy animation during the domain reload. (1046821)</p></li>
<li><p>Audio: Fixed AudioCustomFilter leaks mutexes on PS4 (and probably other platforms). (1101492)</p></li>
<li><p>Build Pipeline: Fixed Missing script reference returns MonoBehavior type instead of null in ContentBuildPipeline.GetTypeForObject &amp; ContentBuildPipeline.GetTypeForObjects. (1105304)</p></li>
<li><p>Camera: Fixed case where we would crash when rendering with an invalid occlusion camera. (<a href="https://issuetracker.unity3d.com/issues/crash-on-dorenderloop-if-scene-view-is-open-when-opening-occlusion-window">1089008</a>)</p></li>
<li><p>Editor: Fixed EditorUtility.DisplayProgressBar crashing editor running example code. (<a href="https://issuetracker.unity3d.com/issues/displayprogressbar-crashes-editor-running-example-code">1095373</a>)</p></li>
<li><p>Editor: Namespace parser - optional whitespace after preprocessor directive. (1104800)</p></li>
<li><p>GI: N/A (1083081)</p></li>
<li><p>iOS: Fixed race condition that can cause a crash when aborting UnityWebRequest. (<a href="https://issuetracker.unity3d.com/issues/ios-crash-in-job-executeunitywebrequest-at-unitywebrequestproto-dot-h-226">1102938</a>)</p></li>
<li><p>iOS: Fixed Unity Remote not working on Windows. (1107874)</p></li>
<li><p>Kernel: Fixed an issue which could cause an error when reading files from disk. (1092419)</p></li>
<li><p>Linux: Fixed Linux player fails to build if there is a default icon assigned in the player settings. (1104530)</p></li>
<li><p>Package Manager: Fixed an issue where cancelling import of package assets would still result in those assets being imported after restarting Unity. The Cancel button of the asset import progress bar is now disabled. (1107329)</p></li>
<li><p>Physics: Fixed incorrect "Physics2D.CapsuleCast()" method that used "infinity" rather than the supplied distance argument. (1098251)</p></li>
<li><p>Prefabs: Fixed adding component that requires Transform to GameObject that has RectTransform. (1106473)</p></li>
<li><p>Prefabs: Fixed dragging Prefabs to embedded Package. (1096426)</p></li>
<li><p>Prefabs: Fixed null reference exception when clicking on text "No Overrides" in Overrides dropdown after applying changes via Comparison view. (<a href="https://issuetracker.unity3d.com/issues/nullreferenceexception-when-clicking-inside-the-prefab-override-popup-after-applying-overrides">1099228</a>)</p></li>
<li><p>Prefabs: Fixed referencing object in Prefab from ScriptableObject if ScriptableObject is added to Prefab asset. (1090541)</p></li>
<li><p>Profiler: Fixed profiler errors when profiling the editor in Vulkan renderer. (<a href="https://issuetracker.unity3d.com/issues/vulkan-profiler-non-matching-profiler-begin-slash-end-samples-for-gfx-dot-processcommands-being-invoked-when-profiling-editor">1087222</a>, 1089098)</p></li>
<li><p>Shaders: Fixed closing the 'Shader' dropdown menu when inspecting a Material fills the Console with !asset-&gt;IsFolderAsset() errors. (<a href="https://issuetracker.unity3d.com/issues/closing-the-shader-dropdown-menu-when-inspecting-a-material-fills-the-console-with-asset-isfolderasset-errors">1083410</a>)</p></li>
<li><p>UI: Fixed material asset file timestamp being modified when rendering with a clipping mask. (<a href="https://issuetracker.unity3d.com/issues/canvas-batching-system-dirties-project-user-created-materials-when-using-rect-mask-2d">967024</a>)</p></li>
<li><p>Universal Windows Platform: Fixed nullptr Exception thrown by WebCamTexture when stopping video playback causing memory leak. (1036939)</p></li>
<li><p>Version Control: Fixed a bug where Asset Inspectors would not be editable while working offline with VCS enabled. (<a href="https://issuetracker.unity3d.com/issues/vcs-work-offline-mode-doesnt-unlock-assets-for-edit">952780</a>)</p></li>
</ul>

#### Changeset: b3c100a4b73a
