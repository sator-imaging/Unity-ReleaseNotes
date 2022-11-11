# Unity 2023.1.0 Alpha 18

https://unity3d.com/unity/alpha/2023.1.0a18

## Known Issues in 2023.1.0a18



*   2D: Fixed exception when showing PSDImporter inspector. (Case DANB-195).  
    _First seen in 2023.1.0._  
    _Fixed in 2023.1.0a19._
    
*   2D: \[Lost Crypt\] Unable to find URP 12.1.0 package error when importing Lost Crypt ([1388129](https://issuetracker.unity3d.com/issues/2d-lost-crypt-unable-to-find-urp-12-dot-1-0-package-error-when-importing-lost-crypt))
    
*   Animation: Fixed the rig builder so that it no longer prevents GameObject movement when two animations are playing in layer mixer with root motion masked on second layer ([UUM-16486](https://issuetracker.unity3d.com/issues/rig-builder-prevets-gameobject-movement-when-two-animations-are-playing-at-once))  
    _First seen in 2023.1.0a12._  
    _Fixed in 2023.1.0a19._
    
*   Asset - Database: Folder name is truncated when dot is used in the name ([UUM-7046](https://issuetracker.unity3d.com/issues/folder-name-is-truncated-when-dot-is-used-in-the-name))
    
*   Asset - Database: Infinite import on opening project (related to prefabs) ([1411189](https://issuetracker.unity3d.com/issues/infinite-import-on-opening-project-related-to-prefabs))
    
*   Asset Importers: Editor hangs when importing certain .fbx files ([UUM-15346](https://issuetracker.unity3d.com/issues/editor-hangs-when-importing-certain-fbx-files))
    
*   Audio: Audio starts playing from the beginning when Undo/Redo Audio Source changes in Play Mode ([UUM-18551](https://issuetracker.unity3d.com/issues/audio-starts-playing-from-the-beginning-when-undo-slash-redo-audio-source-changes-in-play-mode))
    
*   Editor: Fixed input issues when cursor is locked. (UUM-17514)  
    _First seen in 2023.1.0a14._  
    _Fixed in 2023.1.0a19._
    
*   HDRP: Fixed an issue with low resolution depth of field producing a cropped result in some scenarios. ([UUM-11354](https://issuetracker.unity3d.com/issues/hdrp-dof-in-half-or-quarter-resolution-results-in-cropped-frame))  
    _Fixed in 2023.1.0a19._
    
*   IL2CPP: Fixed crash in IL2CPP metadata code when loading a field RVA value (UUM-17473)  
    _Fixed in 2023.1.0a19._
    
*   IL2CPP: Linux IL2CPP builds fail with "BuildFailedException: Incremental Player build failed!" ([1427577](https://issuetracker.unity3d.com/issues/linux-il2cpp-builds-fail-with-buildfailedexception-incremental-player-build-failed))
    
*   MacOS: \[macOS\] "Visual Studio Code" is missing from the External Script Editor dropdown menu even though it is Installed and Updated ([UUM-18707](https://issuetracker.unity3d.com/issues/macos-visual-studio-code-is-missing-from-the-external-script-editor-dropdown-menu-even-though-it-is-installed-and-updated))
    
*   Metal: \[iOS\]Unable to maintain 120fps consistently in a near-empty scene on iPhone 13 Pro ([UUM-5944](https://issuetracker.unity3d.com/issues/ios-target-fps-is-ignored-on-iphone-13-pro))
    
*   Package: NullReferenceException in TMPro.MaterialReference when creating a UI Button - TextMeshPro ([UUM-13929](https://issuetracker.unity3d.com/issues/nullreferenceexception-in-tmpro-dot-materialreference-when-creating-a-ui-button-textmeshpro))
    
*   Profiling: Profiler Modules submenu and window is missing Titles of Modules and Counters ([1419236](https://issuetracker.unity3d.com/issues/profiler-modules-submenu-and-window-is-missing-titles-of-modules-and-counters))
    
*   RP Workflow: \[HDRP\] Standalone Profiler throws "HDRP Material Upgrade" pop-up and crashes after pressing "Ok" ([1422062](https://issuetracker.unity3d.com/issues/hdrp-standalone-profiler-throws-hdrp-material-upgrade-pop-up-and-crashes-after-pressing-ok))
    
*   Scene Management: Editor unselects elements when entering and then exiting the Play Mode ([UUM-16018](https://issuetracker.unity3d.com/issues/editor-unselects-elements-when-entering-and-then-exiting-the-play-mode))
    
*   Scene Management: Undo crashes Unity with segmentation violation SIGSEGV ([1385565](https://issuetracker.unity3d.com/issues/undo-crashes-unity-with-segmentation-violation-sigsegv))
    
*   ShaderGraph: \[Shader Graph\] Shader instance property gets added to CBUFFER, which causes GPU instancing with instanced properties to not work (SGB-343)
    
*   Shaders: Fixed asset bundles with shaders not loading correctly on newer versions of Unity. ([UUM-17421](https://issuetracker.unity3d.com/issues/assertion-failed-on-expression-m-bufferstobind-shadertype-bind-dot-buffer-equals-equals-null-is-thrown-when-entering-the-play-mode))  
    _Fixed in 2023.1.0a19._
    
*   Shortcut Management: Scene window stuck in orbit after context menu click from Hierarchy ([UUM-6908](https://issuetracker.unity3d.com/issues/scene-window-stuck-in-orbit-after-context-menu-click-from-hierarchy))
    
*   UI Toolkit: Enabled display of UI Toolkit warning when the serialized references are missing (as per IMGUI). (UUM-15589)  
    _First seen in 2023.1.0a11._  
    _Fixed in 2023.1.0a19._
    
*   Universal RP: Shader compilation time is higher in 2021.3 than in 2020.3 ([UUM-17405](https://issuetracker.unity3d.com/issues/shader-compilation-time-is-higher-in-2021-dot-3-than-in-2020-dot-3))