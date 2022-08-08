# Unity 2017.2

https://unity3d.com/unity/whats-new/unity-2017.2.0

## The following are changes and fixes to 2017.2.0 features and regressions...

- [Improvements](#improvements)
- [Fixes](#fixes)


### Improvements

*   Multiplayer: Improved batch sending for web sockets.

### Fixes

*   Editor: Fixed race condition that could cause Editor to freeze on entering play mode. ([954551](https://issuetracker.unity3d.com/issues/unity-sometimes-deadlocks-when-entering-play-mode-due-to-a-race-condition-in-persistentmanager), 956287)
    
*   Editor: Resolved an issue where reverting changes to a prefab would corrupt the prefab. ([696346](https://issuetracker.unity3d.com/issues/reverted-prefab-objects-cannot-be-removed-by-undo-function), [864619](https://issuetracker.unity3d.com/issues/reverting-model-back-to-a-prefab-and-then-undoing-these-changes-creates-an-additional-broken-non-prefab-object), [883861](https://issuetracker.unity3d.com/issues/roottransform-equals-null-assert-followed-by-a-crash-when-undoing-slash-redoing), [931300](https://issuetracker.unity3d.com/issues/argumentnullexception-is-shown-when-reverting-the-prefab-instance), [931877](https://issuetracker.unity3d.com/issues/unity-crashes-when-deleting-prefab-clone-after-prefab-revert))
    
*   Graphics: Fixed crash when opening Occlusion tab in a scene containing Speedtrees. ([940486](https://issuetracker.unity3d.com/issues/regression-windows-crash-in-quadtreenode-preparebuffers-when-opening-occlusion-tab-in-a-scene-with-occluded-speedtrees))
    
*   iOS: Fixed iOS11 crash when launching app in landscape mode. ([949029](https://issuetracker.unity3d.com/issues/ios-arkit-arkit-builds-crash-in-unity-2017-dot-2-when-launched-in-landscape-mode))
    
*   iOS: Fixed startup crash on iOS 7.x and OSX 10.9.x. (957572)
    
*   Package Manager: VCS plugins now track the Package Manager manifest. (949497)
    
*   Particles: Fixed issue whereby emission bursts did not upgrade correctly when updgrading a project from an earlier version of Unity. ([956329](https://issuetracker.unity3d.com/issues/emission-min-slash-max-bursts-dont-upgrade-properly-to-random-between-two-constants))
    
*   Windows: Fixed case of Windows Standalone displaying a blank icon in the corner of window. ([954635](https://issuetracker.unity3d.com/issues/windows-standalone-game-window-has-blank-icon))
    
*   XR: Fixed crashes when running Holographic Simulator in Editor. (949293)
    
*   XR: Fixed issues with using `renderViewportScale` on WindowsMR.
    

#### Revision: 46dda1414e51