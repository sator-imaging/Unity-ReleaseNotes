# Unity 2020.3.0

https://unity3d.com/unity/whats-new/2020.3.0

## Known Issues in 2020.3.0f1



*   Cloth: Cloth is broken when parent GameObject scale is lower than 1 and Surface Penetration constraints are set 0 ([1319488](https://issuetracker.unity3d.com/issues/cloth-is-broken-when-parent-gameobject-scale-is-lower-than-1-and-surface-penetration-constraints-are-set-0))
    
*   Mobile: FixedUpdate gets called multiple times before the first Update when Build is run on a Device ([1318647](https://issuetracker.unity3d.com/issues/mobile-fixedupdate-gets-called-multiple-times-before-the-first-update-when-build-is-run-on-a-device))
    
*   2D: "NullReferenceException: SerializedObject of SerializedProperty" is thrown when building Sprite Atlas ([1318332](https://issuetracker.unity3d.com/issues/nullreferenceexception-serializedobject-of-serializedproperty-is-thrown-when-building-sprite-atlas))
    
*   Shuriken: Crash on ParticleSystem\_ShapeModule\_CUSTOM\_set\_sprite\_Injected when changing the shape.sprite of a null ParticleSystem ([1319658](https://issuetracker.unity3d.com/issues/crash-on-particlesystem-shapemodule-custom-set-sprite-injected-when-changing-the-shape-dot-sprite-of-a-null-particlesystem))
    
*   Profiling: \[Profiler\] Timeline sample names from surrounding frames disappear when zooming or panning ([1317697](https://issuetracker.unity3d.com/issues/profiler-timeline-sample-names-from-surrounding-frames-disappear-when-zooming-or-panning))
    
*   Linux: Linux Editor throws "X Server took longer than x miliseconds to respond to SetGtkWindowSizeAndPosition" error after opening ([1309607](https://issuetracker.unity3d.com/issues/linux-editor-throws-x-server-took-longer-than-x-miliseconds-to-respond-to-setgtkwindowsizeandposition-error-after-opening))
    
*   Shuriken: Crash on ParticleSystem::EndUpdateAll ([1311212](https://issuetracker.unity3d.com/issues/shuriken-crash-on-particlesystem-endupdateall))
    
*   Shader System: Crash on PAL\_LocalIPC\_IsConnected when IPC fails on launch ([1319336](https://issuetracker.unity3d.com/issues/crash-on-pal-localipc-isconnected-when-ipc-fails-on-launch))
    
*   Universal RP: \[URP\] Unable to add "Overrides" in "Volume Profile" ([1318535](https://issuetracker.unity3d.com/issues/urp-unable-to-add-overrides-in-volume-profile))
    
*   Templates: Editor Crashes when performing Undo and Redo after duplicating Game Object with LEGO Model Asset component ([1298503](https://issuetracker.unity3d.com/issues/crash-when-redoing-and-undoing-pasting-prefabs-in-scene-in-lego-microgame))
    
*   Linux: InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked ([1248389](https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked))
    
*   Asset Importers: \[Performance Regression\] Importing an fbx model is noticeably slower when the model contains Animations ([1265275](https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations))
    
*   Physics: Crash in physx::NpArticulationReducedCoordinate::createCache() when calling JointState.SaveJointState for unparented bodies ([1264800](https://issuetracker.unity3d.com/issues/crash-in-physx-nparticulationreducedcoordinate-createcache-when-calling-jointstate-dot-savejointstate-for-unparented-bodies))
    
*   Shader System: \[URP Template\] Major performance drop in the Editor during Play Mode ([1277222](https://issuetracker.unity3d.com/issues/urp-template-major-performance-drop-in-the-editor-during-play-mode))
    
*   Mobile: Screen.dpi returns 0 on iPad Pro for projects built from 2019.4.16f1 ([1300359](https://issuetracker.unity3d.com/issues/screen-dot-dpi-returns-0-on-ipad-pro-for-projects-built-from-2019-dot-4-16f1))
    
*   Cloth: Skinned Mesh Renderer's Bounds Extent is set to half of the Transform's Scale when using a Cloth Component ([1209765](https://issuetracker.unity3d.com/issues/skinned-mesh-renderers-bounds-extent-is-set-to-half-of-the-transforms-scale-when-using-a-cloth-component))
    
*   Shader System: Shader error db grows on each build ([1317744](https://issuetracker.unity3d.com/issues/shader-error-db-grows-on-each-build))
    
*   Serialization: Editor crashes on RaiseException when allocating huge amount of memory ([1313492](https://issuetracker.unity3d.com/issues/editor-crashes-on-raiseexception-when-allocating-huge-amount-of-memory))
    
*   Polybrush: \[PolyBrush\] Something went wrong saving brush settings Warning is thrown when Saving a Brush after opening the PolyBrush Window ([1315475](https://issuetracker.unity3d.com/issues/polybrush-something-went-wrong-saving-brush-settings-warning-is-thrown-when-saving-a-brush-after-opening-the-polybrush-window))
    
*   Templates: \[Linux\] Missing libdl.so library causes crash when entering Playmode for the second time or closing the Editor ([1237642](https://issuetracker.unity3d.com/issues/missing-libdl-dot-so-library-causes-crash-when-entering-playmode-for-the-second-time-or-closing-the-editor))