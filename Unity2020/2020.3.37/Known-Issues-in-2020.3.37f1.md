# Unity 2020.3.37

https://unity3d.com/unity/whats-new/2020.3.37

## Known Issues in 2020.3.37f1



*   AI Core: NavMesh::Raycast freezes the whole editor in an infinite loop on Application.UpdateScene ([UUM-2496](https://issuetracker.unity3d.com/issues/navmesh-raycast-freezes-the-whole-editor-in-an-infinite-loop-on-application-dot-updatescene))
    
*   GI: If a user is experience lighting coruption they be may required to reimport due to a fix to which correctly fixes a Uv unwrapping issue (1330830).
    
*   Inspector Framework: List element overlaps everything when using Serializable struct/class ([UUM-7683](https://issuetracker.unity3d.com/issues/list-element-overlaps-everything-when-using-serializable-struct-slash-class))
    
*   Metal: Consistent EditorLoop 5-10ms spikes when using Metal API ([1378985](https://issuetracker.unity3d.com/issues/consistent-gfx-dot-waitforpresentongfxthread-5-10ms-spikes-when-using-metal-api))
    
*   Scene Management: Scene causes Editor crash when specific Lighting Data Asset is used ([UUM-9319](https://issuetracker.unity3d.com/issues/scene-causes-editor-crash-when-specific-lighting-data-asset-is-used))
    
*   Shadows/Lights: Scene is brighter in Standalone player if it was open in the Editor at build time ([UUM-2743](https://issuetracker.unity3d.com/issues/scene-is-brighter-in-standalone-player-if-it-was-open-in-the-editor-at-build-time-1))
    
*   Text: \[Mac\] ShortcutManager ignores Shift modifier ([UUM-4083](https://issuetracker.unity3d.com/issues/mac-shortcutmanager-ignores-shift-modifier-1))
    
*   Texture: \[Backport\] \[MacOS\] Crash on \_\_pthread\_kill when Render Texture has no Depth buffer and Dimension is 3D ([UUM-5459](https://issuetracker.unity3d.com/issues/backport-macos-crash-on-pthread-kill-when-render-texture-has-no-depth-buffer-and-dimension-is-3d))