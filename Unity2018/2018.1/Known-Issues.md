# Unity 2018.1

https://unity3d.com/unity/whats-new/unity-2018.1.0

## Known Issues



*   Editor: Editor Skin becomes grey when player settings are changed from outside the Editor - for example, when fetching a project from Collab for the first time or when modifying the project by hand. Restarting the Editor clears the issue. ([994405](https://issuetracker.unity3d.com/issues/editor-skin-becomes-grey-when-a-collab-project-is-opened-for-the-first-time))
    
*   GI: When working with instances generated through level geometry tools (i.e. Terrain/ProBuilder), Progressive Lightmapper restarts baking for every change by the user. In doing so it distrupts level authoring workflow. This can be seen on newly created 3D projects since Progressive Lightmapper is on by default for new 3D projects. Will be addressed post 2018.1.0 release. ([1028364](https://issuetracker.unity3d.com/issues/user-experienc-eissues-with-generating-geometry-and-progressive-lightmapper-on-autogenerate))
    
*   Graphics: Render Pipeline HD - Errors are spewed after package is installed. Will be addressed in a patch release. ([1004692](https://issuetracker.unity3d.com/issues/render-pipeline-hd-errors-are-spewed-after-package-is-installed))
    
*   Graphics: Lightweight (Preview) and Lightweight VR (Preview) templates don't build on UWP with the bundled LW pipeline. Update to the latest version of the LW pipeline package (com.unity.render-pipelines.lightweight) to overcome this issue. (1025523)
    
*   OSX: \[OSX 10.13\]\[2018.1\] Rapidly switching between 2 Game view tabs multiple times may freeze or crash the Editor when rendering with Metal. Note: it's much harder to reproduce on the latest 10.13.4 Beta (17E160e). ([991828](https://issuetracker.unity3d.com/issues/osx-10-dot-13-2018-dot-1-switching-between-2-game-view-tabs-multiple-times-freezes-editor))
    
*   Particles: Line Renderer is rendered in the Scene and Game windows when you select a GameObject in the Project window. Will be addressed post 2018.1 release. ([972298](https://issuetracker.unity3d.com/issues/line-renderer-is-render-in-scene-slash-game-window-when-selecting-object-in-the-project-window))
    
*   Scripting: Editor crashes when opening external folder through MenuItem ([1018162](https://issuetracker.unity3d.com/issues/editor-crashes-when-opening-external-folder-through-menuitem))
    
*   XR: VRModule may be stripped when using IL2CPP with 'Strip Engine Code' enabled, resulting in build not entering VR mode. See https://forum.unity.com/threads/2018-1-il2cpp-vrmodule-stripping-issue.528799/ for details on how to work around this issue. Will be addressed post 2018.1 release.