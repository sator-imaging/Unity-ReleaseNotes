# Unity 2021.1.18

https://unity3d.com/unity/whats-new/2021.1.18

## Known Issues in 2021.1.18f1



*   Ads: \[Android\] Unity Ad return app to Lock screen ([1281041](https://issuetracker.unity3d.com/issues/android-unity-ad-return-app-to-lock-screen))
    
*   Asset Import Pipeline: Editor crashes with out of memory while importing a lot of assets (mostly textures) at once, on Windows/DX11 ([1324536](https://issuetracker.unity3d.com/issues/editor-crashes-with-system-out-of-memory-error-when-importing-size-heavy-textures))
    
*   Asset Importers: Editor crashes on UnityEditor.Unsupported:IsDestroyScriptableObject when applying changes to a custom asset ([1353925](https://issuetracker.unity3d.com/issues/editor-crashes-on-unityeditor-dot-unsupported-isdestroyscriptableobject-when-applying-changes-to-a-custom-asset))
    
*   Asset Importers: \[MacOS\] Second Unity instance in Activity Monitor is "not responding” after importing ([1331736](https://issuetracker.unity3d.com/issues/macos-second-unity-instance-in-activity-monitor-is-not-responding-after-importing))
    
*   Audio: Crash on AudioCustomFilter::GetOrCreateDSP when recompiling scripts while in Play Mode ([1354002](https://issuetracker.unity3d.com/issues/crash-on-audiocustomfilter-getorcreatedsp-when-recompiling-scripts-while-in-play-mode))
    
*   Audio: Crash on AudioMixer\_CUSTOM\_FindSnapshot when passing null as an argument to FindSnapshot() ([1341752](https://issuetracker.unity3d.com/issues/crash-on-audiomixer-custom-findsnapshot-when-passing-null-as-an-argument-to-findsnapshot))
    
*   Global Illumination: Crash while sculpting Terrain and Baking Lightmaps ([1266511](https://issuetracker.unity3d.com/issues/crash-while-sculpting-terrain))
    
*   Global Illumination: \[Enlighten\] Fatal Error when closing the Editor while Generating Lighting ([1354238](https://issuetracker.unity3d.com/issues/fatal-error-when-closing-the-editor-while-generating-lighting))
    
*   Global Illumination: \[LightProbes\] Probes lose their lighting data after entering Play mode when Baked and Realtime GI are enabled ([1052045](https://issuetracker.unity3d.com/issues/light-probes-lose-their-lighting-data-after-entering-play-mode-when-baked-and-realtime-gi-are-enabled))
    
*   Input: Input.GetKey does not trigger when the mouse cursor is outside the Game window ([1358134](https://issuetracker.unity3d.com/issues/input-dot-getkey-does-not-trigger-when-the-mouse-cursor-is-outside-the-game-window))
    
*   Linux: Crash on DisableSubMenu when double clicking to close a context menu ([1347655](https://issuetracker.unity3d.com/issues/linux-crash-on-disablesubmenu-when-double-clicking-to-close-a-context-menu))
    
*   Linux: Linux Editor crashes at "\_XFreeX11XCBStructure" when loading tutorials ([1323204](https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-xfreex11xcbstructure-when-loading-tutorials))
    
*   Metal: Performance in Game View is significantly impacted by Gfx.WaitForPresentOnGfxThread when a second monitor is connected ([1327408](https://issuetracker.unity3d.com/issues/performance-in-game-view-is-significantly-impacted-by-gfx-dot-waitforpresentongfxthread-when-a-second-monitor-is-connected))
    
*   Mobile: \[Android\] App stops due to OnPixelCopyFinishedListener not being supported on devices with lower than 24 SDK ([1331290](https://issuetracker.unity3d.com/issues/app-stops-due-to-onpixelcopyfinishedlistener-not-being-supported-on-devices-with-lower-than-24-sdk))
    
*   Mobile: \[Android\] Using TouchScreenKeyboard.Open with a non-empty placeholder multiple times causes the app to crash ([1347370](https://issuetracker.unity3d.com/issues/android-using-touchscreenkeyboard-dot-open-with-a-non-empty-placeholder-multiple-times-causes-the-app-to-crash))
    
*   Mono: \[Mono Upgrade\] CommandBuffer native plugin events hang in the Editor ([1308216](https://issuetracker.unity3d.com/issues/commandbuffer-native-plugin-events-hang-in-the-editor))
    
*   Packman: User can't easily configure location of both UPM and Asset Store package local cache ([1317232](https://issuetracker.unity3d.com/issues/user-cant-easily-configure-location-of-both-upm-and-asset-store-package-local-cache))
    
*   Scene Management: Crash on BuildPrefabInstanceCorrespondingObjectMap when overriding nested prefab inside AssetDatabase.StartAssetEditing() block ([1324978](https://issuetracker.unity3d.com/issues/crash-on-buildprefabinstancecorrespondingobjectmap-when-overriding-nested-prefab-inside-assetdatabase-dot-startassetediting-block))
    
*   Scripting: Crashes on mono\_class\_init when entering Play Mode after recompiling scripts ([1262671](https://issuetracker.unity3d.com/issues/crashes-on-mono-class-init-when-entering-play-mode-after-recompiling-scripts))
    
*   Scripting: DomainReloadTests performance tests have regressed due to removal of built-in support for Visual Studio as a code editor ([1336648](https://issuetracker.unity3d.com/issues/domainreloadtests-performance-tests-have-regressed-due-to-removal-of-built-in-support-for-visual-studio-as-a-code-editor))
    
*   Scripting: Error CS8035 is thrown on opening a project when using rulesets ([1349517](https://issuetracker.unity3d.com/issues/error-cs8035))
    
*   Scripting: Increased Script Assembly reload time ([1323490](https://issuetracker.unity3d.com/issues/increased-reload-time))
    
*   Scripting: Only some assemblies fail to be loaded when assembly name does not match the file name ([1345099](https://issuetracker.unity3d.com/issues/only-some-assemblies-fail-to-be-loaded-when-assembly-name-does-not-match-the-file-name))
    
*   Scripting: Performance degradation when activating or deactivating uGUI GameObject ([1348763](https://issuetracker.unity3d.com/issues/performance-degradation-when-activating-or-deactivating-ugui-gameobject))
    
*   Scripting: Unity does not execute code weavers when the project is opened for the first time ([1350116](https://issuetracker.unity3d.com/issues/unity-does-not-execute-code-weavers-when-its-opened-for-the-first-time))
    
*   Terrain: Terrain Lit Opacity as Density option causes alpha'd areas on the 5th layer or greater to appear with artifacts ([1283124](https://issuetracker.unity3d.com/issues/terrain-lit-opacity-as-density-option-causes-alphad-areas-on-the-5th-layer-or-greater-to-appear-with-artifacts))
    
*   Vulkan: \[Editor\] The Scene's GameObjects textures are seemingly random and change colours depending on the Scene's Camera pos. ([1337772](https://issuetracker.unity3d.com/issues/vulkan-editor-the-scenes-gameobjects-textures-are-seemingly-random-and-change-colours-depending-on-the-scenes-camera-pos))