# Unity 2020.3.36

https://unity3d.com/unity/whats-new/2020.3.36

## Known Issues in 2020.3.36f1



*   AI Navigation: NavMesh::Raycast freezes the whole editor in an infinite loop on Application.UpdateScene ([UUM-2496](https://issuetracker.unity3d.com/issues/navmesh-raycast-freezes-the-whole-editor-in-an-infinite-loop-on-application-dot-updatescene))
    
*   GI: If a user is experience lighting coruption they be may required to reimport due to a fix to which correctly fixes a Uv unwrapping issue (1330830).
    
*   Inspector Framework: First array element expansion is broken for arrays that use Custom Property Drawers ([1409773](https://issuetracker.unity3d.com/issues/first-array-element-expansion-is-broken-for-arrays-that-use-custom-property-drawers))
    
*   Kernel: Unity crashes on StackWalker::GetCurrentCallstack when rest-certificate.pem is corrupted ([1423569](https://issuetracker.unity3d.com/issues/unity-crashes-on-stackwalker-getcurrentcallstack-when-rest-certificate-dot-pem-is-corrupted))
    
*   Metal: Consistent EditorLoop 5-10ms spikes when using Metal API ([1378985](https://issuetracker.unity3d.com/issues/consistent-gfx-dot-waitforpresentongfxthread-5-10ms-spikes-when-using-metal-api))
    
*   Physics: Crash on internalABP::ABP\_PairManager::addPair when switching to ArticulationJointType.SphericalJoint during runtime ([1418715](https://issuetracker.unity3d.com/issues/crash-on-internalabp-abp-pairmanager-addpair-when-switching-to-articulationjointtype-dot-sphericaljoint-during-runtime))
    
*   Physics: Physics overlap queries are not consistent when used against convex Mesh Colliders with a very small scale ([1377578](https://issuetracker.unity3d.com/issues/physics-dot-computepenetration-does-not-detect-overlap-consistently-when-using-convex-mesh-colliders))
    
*   Quality of Life: \[Mac\] Shortcut manager ignores Control modifier ([1425117](https://issuetracker.unity3d.com/issues/mac-shortcut-manager-ignores-control-modifier))
    
*   Shadows/Lights: Scene is brighter in Standalone player if it was open in the Editor at build time ([UUM-2743](https://issuetracker.unity3d.com/issues/scene-is-brighter-in-standalone-player-if-it-was-open-in-the-editor-at-build-time-1))
    
*   Text: \[Mac\] ShortcutManager ignores Shift modifier ([UUM-4083](https://issuetracker.unity3d.com/issues/mac-shortcutmanager-ignores-shift-modifier-1))
    
*   Texture: \[Backport\] \[MacOS\] Crash on \_\_pthread\_kill when Render Texture has no Depth buffer and Dimension is 3D ([UUM-5459](https://issuetracker.unity3d.com/issues/backport-macos-crash-on-pthread-kill-when-render-texture-has-no-depth-buffer-and-dimension-is-3d))