# Unity 2021.2.2

https://unity3d.com/unity/whats-new/2021.2.2

## Known Issues in 2021.2.2f1



*   Android: Sometimes text is not rendered when using OpengLES3 on a Xiaomi Redmi9A device. ([1347186](https://issuetracker.unity3d.com/issues/android-the-text-is-missing-on-a-xiaomi-redmi9a-device))
    
*   Android: \* Devices might wake up from sleep when in split screen mode.  
    
    *   Chrome OS devices that support tablet mode might not pause apps when they are no longer visible.  
        
    *   Some Android devices may experience delayed resolution updates after resizing a window.  
        
    *   Minimum window size might not be respected properly on all Android devices.
*   Asset Bundles: Building process of the AssetBundles is slow when there is a huge filecount. ([1358059](https://issuetracker.unity3d.com/issues/building-process-of-the-assetbundles-is-slow-when-the-file-count-is-huge))
    
*   Asset Import Pipeline: Crash on OnDemandScheduler::SetStandbyWorkerCount when opening a project with a symbolic link in it ([1370389](https://issuetracker.unity3d.com/issues/crash-on-ondemandscheduler-setstandbyworkercount-when-opening-a-project-with-a-symbolic-link-in-it))
    
*   CodeEditors: Crash on stopping debugging ([1355156](https://issuetracker.unity3d.com/issues/crash-on-stopping-debugging))
    
*   Global Illumination: Crash while sculpting Terrain and Baking Lightmaps ([1266511](https://issuetracker.unity3d.com/issues/crash-while-sculpting-terrain))
    
*   Global Illumination: Scene is brighter in Standalone player if it was open in the Editor at build time ([1375015](https://issuetracker.unity3d.com/issues/scene-is-brighter-in-standalone-player-if-it-was-open-in-the-editor-at-build-time))
    
*   Global Illumination: \[GPU PLM\] Crash in (nvopencl64) clGetPlatformInfo after enabling Auto Generate checkbox at the end of GI Bake ([1379762](https://issuetracker.unity3d.com/issues/gpu-plm-crash-in-nvopencl64-clgetplatforminfo-after-enabling-auto-generate-checkbox-at-the-end-of-gi-bake))
    
*   Global Illumination: \[GPU PLM\] Fallback to CPU PLM in CL\_INVALID\_MEM\_OBJECT after switching light color only and rebaking GI ([1356714](https://issuetracker.unity3d.com/issues/gpu-plm-switch-light-color-only-and-rebake-causes-fallback))
    
*   HD RP: HDRP Template fills the Console with "Shader error...couldn't open include file" messages after building the project ([1342989](https://issuetracker.unity3d.com/issues/hdrp-template-fills-the-console-with-shader-error-dot-dot-dot-couldnt-open-include-file-messages-after-building-the-project))
    
*   IL2CPP: System.Runtime.Serialization.Formatters.BinaryFormatter doesn't work when Project is build with IL2CPP Scripting Backend ([1374185](https://issuetracker.unity3d.com/issues/il2cpp-system-dot-runtime-dot-serialization-dot-formatters-dot-binaryformatter-doesnt-work-when-project-is-build-with-il2cpp-scripting-backend))
    
*   Input: Touch Input doesn't work in Play Mode when running an Editor on a Touchscreen device ([1341159](https://issuetracker.unity3d.com/issues/touch-input-doesnt-work-in-play-mode-when-running-an-editor-on-a-touchscreen-device))
    
*   Input: \[macOS\] Text input lags by one keystroke when inputting text in the Editor ([1376732](https://issuetracker.unity3d.com/issues/text-input-lags-by-one-keystroke-when-inputting-text-in-the-editor))
    
*   Linux: Linux Editor crashes at "\_\_assert\_fail\_base.cold" when opening a project ([1375312](https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-assert-fail-base-dot-cold-when-opening-a-project))
    
*   MacOS: \[Mac\] Performance regression in Editor UI ([1376273](https://issuetracker.unity3d.com/issues/mac-performance-regression-in-editor-ui))
    
*   Mono: Microsoft.Extensions.Logging Nuget Package causes errors in console when built into UWP with .NET Standard 2.1 ([1373389](https://issuetracker.unity3d.com/issues/microsoft-dot-extensions-dot-logging-nuget-package-causes-errors-in-console-when-built-into-uwp-with-net-standard-2-dot-1))
    
*   Scene Management: Instantiated FBX through code throws error after leaving Play Mode ([1363573](https://issuetracker.unity3d.com/issues/instantiated-fbx-through-code-throws-error-after-leaving-play-mode))
    
*   Scene/Game View: Tool handles are invisible in Scene View when certain objects are selected ([1374532](https://issuetracker.unity3d.com/issues/tool-handles-are-invisible-in-scene-view-when-certain-objects-are-selected))
    
*   Scripting: Crash in CombineMeshFiltersForStaticBatching after switching active additively loaded scenes and entering Play mode ([1377416](https://issuetracker.unity3d.com/issues/crash-in-combinemeshfiltersforstaticbatching-after-switching-active-scenes-and-entering-play-mode))
    
*   Scripting: Error CS8035 is thrown on opening a project when using rulesets ([1349517](https://issuetracker.unity3d.com/issues/error-cs8035))
    
*   Scripting: Only some assemblies fail to be loaded when assembly name does not match the file name ([1345099](https://issuetracker.unity3d.com/issues/only-some-assemblies-fail-to-be-loaded-when-assembly-name-does-not-match-the-file-name))
    
*   Templates: Editor crashes when exiting and keeping a tutorial project ([1338299](https://issuetracker.unity3d.com/issues/editor-crashes-when-exiting-and-keeping-a-new-micrograme-project))
    
*   uGUI: UI handles in scene view are detached from UI elements ([1376302](https://issuetracker.unity3d.com/issues/ui-handles-in-scene-view-are-detached-from-ui-elements))
    
*   Vulkan: \[Editor\] The Scene's GameObjects textures are seemingly random and change colours depending on the Scene's Camera pos. ([1337772](https://issuetracker.unity3d.com/issues/vulkan-editor-the-scenes-gameobjects-textures-are-seemingly-random-and-change-colours-depending-on-the-scenes-camera-pos))
    
*   Window Management: Broken layout stops panels located in the top left corner of the Editor from rendering in the Karting Microgame project ([1367783](https://issuetracker.unity3d.com/issues/broken-layout-stops-panels-located-in-the-top-left-corner-of-the-editor-from-rendering-in-the-karting-microgame-project))
    
*   XR SDK: Severe flickering in Unity 2020.3.21f1 with OpenXR on HL2 ([1376203](https://issuetracker.unity3d.com/issues/severe-flickering-in-unity-2020-dot-3-21f1-with-openxr-on-hl2))
    
*   XR SDK: \[XR\]\[Linux\] Scene View doesn't render when opening new AR or VR Template project or pressing "Show Tutorials" ([1362435](https://issuetracker.unity3d.com/issues/xr-linux-scene-view-doesnt-render-when-opening-new-ar-or-vr-template-project-or-pressing-show-tutorials))