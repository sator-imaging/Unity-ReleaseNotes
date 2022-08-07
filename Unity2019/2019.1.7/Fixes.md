# Unity 2019.1.7
https://unity3d.com/unity/whats-new/2019.1.7

## Fixes

<ul>
<li><p>Android: Fixed ASTC HDR textures in Mac Editor. (<a href="https://issuetracker.unity3d.com/issues/astc-hdr-textures-are-broken-in-maceditor-slash-metal">1142953</a>, 1145498)</p></li>
<li><p>Android: Fixed problem with Android manifest containing incorrect values for platformBuildVersionCode and platformBuildVersionName. (<a href="https://issuetracker.unity3d.com/issues/android-android-manifest-contains-incorrect-values-for-platformbuildversioncode-and-platformbuildversionname">1118325</a>, 1160630)</p></li>
<li><p>Animation: Fixed a crash when animating optimized hierarchies with constant animated properties (<a href="https://issuetracker.unity3d.com/issues/animator-controller-causes-the-editor-to-crash-on-mecanim-animation-transformvaluesfromclip-when-entering-play-mode">1142636</a>, 1151041)</p></li>
<li><p>Asset Import: Fixes an issue where if a mesh asset has no vertex data, the import crashes in some cases. (<a href="https://issuetracker.unity3d.com/issues/unity-freeze-and-mono-arch-find-jit-info-ext-crash-when-importing-corrupted-mesh-asset-files">1144169</a>, 1150808)</p></li>
<li><p>Asset Pipeline: Fixed sprite mask sorting layer resetting to default when asset is loaded from asset bundle. (<a href="https://issuetracker.unity3d.com/issues/asset-bundles-sprite-mask-sorting-layer-resets-to-default-when-asset-is-loaded-from-asset-bundle">1119829</a>, 1153004)</p></li>
<li><p>Editor: Fixed a case where a Version Controlled Project would not update ProjectSettings/ProjectVersion.txt on editor start. (<a href="https://issuetracker.unity3d.com/issues/perforce-reverting-the-projectversion-file-marks-it-as-read-only-preventing-any-further-updates">1131599</a>, 1146736)</p></li>
<li><p>Editor: Fixed a crash while using TextRenderingPrivate::GetFormatString with specific string. (<a href="https://issuetracker.unity3d.com/issues/crash-on-textrenderingprivate-getformatstring-when-using-specific-string">1150645</a>, 1156737)</p></li>
<li><p>Editor: Fixed host local address not validated on GET HTTP request. (1146895, 1152795)</p></li>
<li><p>Editor: Fixed issue where SceneVis was not preventing picking of objects with gizmos and no renderers. (<a href="https://issuetracker.unity3d.com/issues/canvas-objects-are-selectable-when-they-are-hidden">1141999</a>, 1146284, 1157414, 1157416)</p></li>
<li><p>Editor: Fixed the scale error by updating the scale once the platform is switched. (<a href="https://issuetracker.unity3d.com/issues/switching-between-platforms-results-into-game-views-resolution-slash-aspect-ratio-scale-settings-not-changing">918311</a>, 1153435)</p></li>
<li><p>GI: Fixed a potential baking crash when objects HideFlags are configured. (<a href="https://issuetracker.unity3d.com/issues/console-is-continuously-spammed-with-assertion-failed-on-expression-kvalidsceneobjectidentifier-equals-equals-res-after-project-update">1064691</a>, 1156004)</p></li>
<li><p>Graphics: Fixed excessive stripping of shaders without users keywords resulting in missing usage of vertex components and discarding them. (<a href="https://issuetracker.unity3d.com/issues/meshes-lose-vertex-color-in-builds-with-static-batching-enabled-when-certain-shaders-are-present-in-the-scene">914736</a>, 1149323)</p></li>
<li><p>Graphics: Fixed Vulkan Editor on AMD GPUs. (<a href="https://issuetracker.unity3d.com/issues/vulkan-amd-objects-do-not-get-rendered-when-the-camera-has-clear-flags-set-to-skybox">1145367</a>, 1149412)</p></li>
<li><p>iOS: Fixed error/crash on startup when using DisplayP3 color gamut. (<a href="https://issuetracker.unity3d.com/issues/ios-metal-displayp3-color-gamut-results-in-metal-errors-on-startup-in-generatebuiltintextures">1136841</a>, 1152114)</p></li>
<li><p>Particles: Fixed an issue where the Particle System Inspector can become slow after editing its material but not saving the changes. (<a href="https://issuetracker.unity3d.com/issues/system-becomes-slow-when-using-a-particle-system-with-a-material-that-has-a-shader-that-uses-a-custom-shader-gui">1154688</a>, 1159216)</p></li>
<li><p>Physics: Fixed crash that happened when destroying Colliders that had OnCollisionStay scripts attached. (<a href="https://issuetracker.unity3d.com/issues/crash-on-simulationcallbackreceiver-oncontact-when-objects-are-destructing">1113545</a>, 1161860)</p></li>
<li><p>Physics: Fixed Rigidbodies not following their parent sometimes. (<a href="https://issuetracker.unity3d.com/issues/ontriggerenter-is-called-inconsistently-when-moving-a-trigger-via-input-key-press-with-addforce">1140632</a>, 1161857)</p></li>
<li><p>Timeline: Fixed "Add Signal Emitter" commands should be listed first in a track's context menu. (1131166, 1133970)</p></li>
<li><p>Universal Windows Platform: Fixed files in StreamingAssets directory not treated as generic data files so they won't get consumed by various VS tools like the XAML compiler. (<a href="https://issuetracker.unity3d.com/issues/uwp-il2cpp-visual-studios-builds-fails-with-xamlcompiler-error">1110262</a>, 1152577)</p></li>
<li><p>Version Control: Fixed prompting when attempting to check out ProjectSettings/XRSettings.asset. (<a href="https://issuetracker.unity3d.com/issues/vcs-xrsettings-file-shows-checkout-pop-up-which-is-inconsistent-with-other-settings-files">1144407</a>, 1151473)</p></li>
<li><p>Windows: Fixed locked cursor getting placed slightly off center in the editor and the standalone player. (<a href="https://issuetracker.unity3d.com/issues/input-dot-mouseposition-returns-incorrect-value-when-using-locked-cursor">824304</a>, 1152574)</p></li>
<li><p>Windows: Fixed Standalone Player remains paused/inactive after using WIN+D shortcut to restore the app window (case 1117930). (<a href="https://issuetracker.unity3d.com/issues/canvas-elements-are-disabled-in-the-build-project-when-navigating-in-and-out-of-desktop-by-using-win-plus-d">1117930</a>, 1147086)</p></li>
<li><p>XR: Fixed a crash in the Lumin video player when open fails. (1150947, 1151175)</p></li>
<li><p>XR: Fixed issue in HoloLens where we weren't using the correct anchor view for switching away from on screen keyboard in XAML. (1156224, 1156227)</p></li>
<li><p>XR: Fixed SwitchAsync call to use correct anchor view id. (1156224, 1156227)</p></li>
</ul>
