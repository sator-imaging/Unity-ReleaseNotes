# Unity 2019.1.7

https://unity3d.com/unity/whats-new/2019.1.7

## Fixes



*   Android: Fixed ASTC HDR textures in Mac Editor. ([1142953](https://issuetracker.unity3d.com/issues/astc-hdr-textures-are-broken-in-maceditor-slash-metal), 1145498)
    
*   Android: Fixed problem with Android manifest containing incorrect values for platformBuildVersionCode and platformBuildVersionName. ([1118325](https://issuetracker.unity3d.com/issues/android-android-manifest-contains-incorrect-values-for-platformbuildversioncode-and-platformbuildversionname), 1160630)
    
*   Animation: Fixed a crash when animating optimized hierarchies with constant animated properties ([1142636](https://issuetracker.unity3d.com/issues/animator-controller-causes-the-editor-to-crash-on-mecanim-animation-transformvaluesfromclip-when-entering-play-mode), 1151041)
    
*   Asset Import: Fixes an issue where if a mesh asset has no vertex data, the import crashes in some cases. ([1144169](https://issuetracker.unity3d.com/issues/unity-freeze-and-mono-arch-find-jit-info-ext-crash-when-importing-corrupted-mesh-asset-files), 1150808)
    
*   Asset Pipeline: Fixed sprite mask sorting layer resetting to default when asset is loaded from asset bundle. ([1119829](https://issuetracker.unity3d.com/issues/asset-bundles-sprite-mask-sorting-layer-resets-to-default-when-asset-is-loaded-from-asset-bundle), 1153004)
    
*   Editor: Fixed a case where a Version Controlled Project would not update ProjectSettings/ProjectVersion.txt on editor start. ([1131599](https://issuetracker.unity3d.com/issues/perforce-reverting-the-projectversion-file-marks-it-as-read-only-preventing-any-further-updates), 1146736)
    
*   Editor: Fixed a crash while using TextRenderingPrivate::GetFormatString with specific string. ([1150645](https://issuetracker.unity3d.com/issues/crash-on-textrenderingprivate-getformatstring-when-using-specific-string), 1156737)
    
*   Editor: Fixed host local address not validated on GET HTTP request. (1146895, 1152795)
    
*   Editor: Fixed issue where SceneVis was not preventing picking of objects with gizmos and no renderers. ([1141999](https://issuetracker.unity3d.com/issues/canvas-objects-are-selectable-when-they-are-hidden), 1146284, 1157414, 1157416)
    
*   Editor: Fixed the scale error by updating the scale once the platform is switched. ([918311](https://issuetracker.unity3d.com/issues/switching-between-platforms-results-into-game-views-resolution-slash-aspect-ratio-scale-settings-not-changing), 1153435)
    
*   GI: Fixed a potential baking crash when objects HideFlags are configured. ([1064691](https://issuetracker.unity3d.com/issues/console-is-continuously-spammed-with-assertion-failed-on-expression-kvalidsceneobjectidentifier-equals-equals-res-after-project-update), 1156004)
    
*   Graphics: Fixed excessive stripping of shaders without users keywords resulting in missing usage of vertex components and discarding them. ([914736](https://issuetracker.unity3d.com/issues/meshes-lose-vertex-color-in-builds-with-static-batching-enabled-when-certain-shaders-are-present-in-the-scene), 1149323)
    
*   Graphics: Fixed Vulkan Editor on AMD GPUs. ([1145367](https://issuetracker.unity3d.com/issues/vulkan-amd-objects-do-not-get-rendered-when-the-camera-has-clear-flags-set-to-skybox), 1149412)
    
*   iOS: Fixed error/crash on startup when using DisplayP3 color gamut. ([1136841](https://issuetracker.unity3d.com/issues/ios-metal-displayp3-color-gamut-results-in-metal-errors-on-startup-in-generatebuiltintextures), 1152114)
    
*   Particles: Fixed an issue where the Particle System Inspector can become slow after editing its material but not saving the changes. ([1154688](https://issuetracker.unity3d.com/issues/system-becomes-slow-when-using-a-particle-system-with-a-material-that-has-a-shader-that-uses-a-custom-shader-gui), 1159216)
    
*   Physics: Fixed crash that happened when destroying Colliders that had OnCollisionStay scripts attached. ([1113545](https://issuetracker.unity3d.com/issues/crash-on-simulationcallbackreceiver-oncontact-when-objects-are-destructing), 1161860)
    
*   Physics: Fixed Rigidbodies not following their parent sometimes. ([1140632](https://issuetracker.unity3d.com/issues/ontriggerenter-is-called-inconsistently-when-moving-a-trigger-via-input-key-press-with-addforce), 1161857)
    
*   Timeline: Fixed "Add Signal Emitter" commands should be listed first in a track's context menu. (1131166, 1133970)
    
*   Universal Windows Platform: Fixed files in StreamingAssets directory not treated as generic data files so they won't get consumed by various VS tools like the XAML compiler. ([1110262](https://issuetracker.unity3d.com/issues/uwp-il2cpp-visual-studios-builds-fails-with-xamlcompiler-error), 1152577)
    
*   Version Control: Fixed prompting when attempting to check out ProjectSettings/XRSettings.asset. ([1144407](https://issuetracker.unity3d.com/issues/vcs-xrsettings-file-shows-checkout-pop-up-which-is-inconsistent-with-other-settings-files), 1151473)
    
*   Windows: Fixed locked cursor getting placed slightly off center in the editor and the standalone player. ([824304](https://issuetracker.unity3d.com/issues/input-dot-mouseposition-returns-incorrect-value-when-using-locked-cursor), 1152574)
    
*   Windows: Fixed Standalone Player remains paused/inactive after using WIN+D shortcut to restore the app window (case 1117930). ([1117930](https://issuetracker.unity3d.com/issues/canvas-elements-are-disabled-in-the-build-project-when-navigating-in-and-out-of-desktop-by-using-win-plus-d), 1147086)
    
*   XR: Fixed a crash in the Lumin video player when open fails. (1150947, 1151175)
    
*   XR: Fixed issue in HoloLens where we weren't using the correct anchor view for switching away from on screen keyboard in XAML. (1156224, 1156227)
    
*   XR: Fixed SwitchAsync call to use correct anchor view id. (1156224, 1156227)