# Unity 2019.3.3

https://unity3d.com/unity/whats-new/2019.3.3

## Known Issues in 2019.3.3f1



*   2D: Crash on memory allocation when double-clicking a Sprite which size is reassigned in OnDrawGizmos ([1211482](https://issuetracker.unity3d.com/issues/crash-on-memory-allocation-when-double-clicking-a-sprite-which-size-is-reassigned-in-ondrawgizmos))
    
*   Ads: Verified and default Ads package for 2019.3 should be 3.3.x instead of 2.0.8 ([1206332](https://issuetracker.unity3d.com/issues/ads-older-ads-package-is-available-in-package-manager))
    
*   Animation: "Go to previous Keyframe" button/shortcut does not work in the Animation Window ([1220385](https://issuetracker.unity3d.com/issues/go-to-previous-keyframe-button-slash-shortcut-does-not-work-in-the-animation-window))
    
*   Asset Import Pipeline: Calling AssetDatabase.ImportAsset() on a prefab, while having a reference to the prefab objects, breaks the references ([1217774](https://issuetracker.unity3d.com/issues/assets-reference-in-scriptable-object-is-lost-when-the-asset-is-reimported))
    
*   Asset Importers: NullReferenceException is thrown when inspecting a .FBX file with multiple clips and opening Animation tab ([1215431](https://issuetracker.unity3d.com/issues/nullreferenceexception-is-thrown-when-inspecting-a-fbx-file-with-multiple-clips-and-opening-animation-tab))
    
*   Global Illumination: \[CPU PLM\] Baked spotlights get their attenuation culled if the spot angle exceeds 89 degrees ([1221741](https://issuetracker.unity3d.com/issues/cpu-plm-baked-spotlights-get-their-attenuation-culled-if-the-spot-angle-exceeds-89-degrees))
    
*   Global Illumination: \[OSX\]\[GPUPLM\]OS Kernel Panic crash with 'Thread may have been prematurely finalized' after baking the scene with AMD GPU ([1160419](https://issuetracker.unity3d.com/issues/osx-gpuplm-kernel-panic-slash-editor-crash-with-thread-may-have-been-prematurely-finalized-after-baking-the-scene-with-amd-gpu))
    
*   Graphics - General: \[SRP only\] Clearing playerprefs causes assets to reimport on playmode ([1192259](https://issuetracker.unity3d.com/issues/lwrp-clearing-playerprefs-through-a-script-or-editor-causes-delay-and-console-errors-to-appear-when-entering-the-play-mode))
    
*   HD RP: \[HDRP\]\[Metal\] Crash on GfxDeviceMetalBase::CommonDrawSetup when selecting shader ([1218754](https://issuetracker.unity3d.com/issues/hdrp-metal-crash-on-gfxdevicemetalbase-commondrawsetup-when-selecting-shader))
    
*   IAP: Disabling and re-enabling IAP in services window throws multiple errors about failing to find assemblies ([1193774](https://issuetracker.unity3d.com/issues/disabling-and-re-enabling-iap-in-services-window-throws-multiple-errors-about-failing-to-find-assemblies))
    
*   IMGUI: "Render Mode" dropdown displaying items from a different component's, that was selected first, "Render Mode" dropdown ([1217278](https://issuetracker.unity3d.com/issues/render-mode-dropdown-displaying-items-from-other-componenets-render-mode-dropdown))
    
*   Inspector Framework: Canvas and Light's Render Mode's drop down values are the same when inspecting one of the Components ([1215130](https://issuetracker.unity3d.com/issues/canvas-and-lights-render-modes-drop-down-values-are-the-same-when-inspecting-one-of-the-components))
    
*   MacOS: \[Mac\] \[Metal\] \[Editor\] Switching focus to other apps and editor corrupts the text in the editor ([1156105](https://issuetracker.unity3d.com/issues/mac-editor-switching-focus-to-other-apps-and-editor-distorts-the-text-in-the-editor))
    
*   MacOS: \[macOS\] BugReporter doesn't get invoked when the project crashes ([1219458](https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes))
    
*   MacOS: \[macOS\] Clicking the 'Overrides' button for Prefabs crashes the Editor when Prefab contains a large list of overrides ([1219036](https://issuetracker.unity3d.com/issues/macos-clicking-the-overrides-button-for-prefabs-crashes-the-editor-when-prefab-contains-a-large-list-of-overrides))
    
*   Mobile: \[Android\] Loading assets from AssetBundles takes significantly more time when the project is built as an AAB ([1153358](https://issuetracker.unity3d.com/issues/android-loading-assets-from-assetbundles-takes-significantly-more-time-when-the-project-is-built-as-an-aab))
    
*   Package: Errors are Constantly thrown when Active Input Handling is set to Input System Package ([1176974](https://issuetracker.unity3d.com/issues/urp-errors-are-constantly-thrown-when-active-input-handling-is-set-to-input-system-package))
    
*   Scene Management: Prefab variant's Button component's OnClick() events are missing parameters when upgrading to Unity 2019.3.0a12 and above ([1208775](https://issuetracker.unity3d.com/issues/prefab-variants-scripts-are-missing-fields-when-upgrading-to-unity-2019-dot-3-0a12-and-above))
    
*   Scene Management: Prefabs lose their values if scripts are removed then reintroduced ([1216914](https://issuetracker.unity3d.com/issues/prefabs-lose-their-values-if-scripts-are-removed-then-reintroduced))
    
*   Shaders: Change in included hlsl file does not always trigger recompilation ([1215034](https://issuetracker.unity3d.com/issues/shaders-change-in-included-hlsl-file-does-not-always-trigger-recompilation))
    
*   Shuriken: Crash on CreateDirect3D11SurfaceFromDXGISurface when calling DrawRenderer with a Trail Renderer ([1216216](https://issuetracker.unity3d.com/issues/crash-on-createdirect3d11surfacefromdxgisurface-when-calling-drawrenderer-with-a-trail-renderer))
    
*   Shuriken: Editor crashes when Particle System is emitting shadow casting lights ([1217809](https://issuetracker.unity3d.com/issues/editor-crashes-when-particle-system-is-emitting-shadow-casting-lights))
    
*   Shuriken: Particle System that has a Stop Action gets cleared after being paused for a while ([1213288](https://issuetracker.unity3d.com/issues/particle-system-that-has-a-stop-action-gets-cleared-after-being-paused-for-a-while))
    
*   Universal RP: \[URP\] "Render Object" asset does not create in project window when added in "Render Features" field in the Inspector ([1214779](https://issuetracker.unity3d.com/issues/urp-render-object-asset-does-not-create-in-project-window-when-added-in-render-features-field-in-the-inspector))
    
*   tvOS: "Menu" button on Siri Remote returns "Joystick1Button19" instead of "Joystick1Button0" ([1214948](https://issuetracker.unity3d.com/issues/tvos-menu-button-on-siri-remote-returns-joystick1button19-instead-of-joystick1button0))