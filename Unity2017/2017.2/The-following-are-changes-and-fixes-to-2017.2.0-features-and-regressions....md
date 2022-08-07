# Unity 2017.2
https://unity3d.com/unity/whats-new/unity-2017.2.0

## The following are changes and fixes to 2017.2.0 features and regressions...


### Improvements
<ul>
<li>Multiplayer: Improved batch sending for web sockets.</li>
</ul>

### Fixes
<ul>
<li><p>Editor: Fixed race condition that could cause Editor to freeze on entering play mode. (<a href="https://issuetracker.unity3d.com/issues/unity-sometimes-deadlocks-when-entering-play-mode-due-to-a-race-condition-in-persistentmanager">954551</a>, 956287)</p></li>
<li><p>Editor: Resolved an issue where reverting changes to a prefab would corrupt the prefab. (<a href="https://issuetracker.unity3d.com/issues/reverted-prefab-objects-cannot-be-removed-by-undo-function">696346</a>, <a href="https://issuetracker.unity3d.com/issues/reverting-model-back-to-a-prefab-and-then-undoing-these-changes-creates-an-additional-broken-non-prefab-object">864619</a>, <a href="https://issuetracker.unity3d.com/issues/roottransform-equals-null-assert-followed-by-a-crash-when-undoing-slash-redoing">883861</a>, <a href="https://issuetracker.unity3d.com/issues/argumentnullexception-is-shown-when-reverting-the-prefab-instance">931300</a>, <a href="https://issuetracker.unity3d.com/issues/unity-crashes-when-deleting-prefab-clone-after-prefab-revert">931877</a>)</p></li>
<li><p>Graphics: Fixed crash when opening Occlusion tab in a scene containing Speedtrees. (<a href="https://issuetracker.unity3d.com/issues/regression-windows-crash-in-quadtreenode-preparebuffers-when-opening-occlusion-tab-in-a-scene-with-occluded-speedtrees">940486</a>)</p></li>
<li><p>iOS: Fixed iOS11 crash when launching app in landscape mode. (<a href="https://issuetracker.unity3d.com/issues/ios-arkit-arkit-builds-crash-in-unity-2017-dot-2-when-launched-in-landscape-mode">949029</a>)</p></li>
<li><p>iOS: Fixed startup crash on iOS 7.x and OSX 10.9.x. (957572)</p></li>
<li><p>Package Manager: VCS plugins now track the Package Manager manifest. (949497)</p></li>
<li><p>Particles: Fixed issue whereby emission bursts did not upgrade correctly when updgrading a project from an earlier version of Unity. (<a href="https://issuetracker.unity3d.com/issues/emission-min-slash-max-bursts-dont-upgrade-properly-to-random-between-two-constants">956329</a>)</p></li>
<li><p>Windows: Fixed case of Windows Standalone displaying a blank icon in the corner of window. (<a href="https://issuetracker.unity3d.com/issues/windows-standalone-game-window-has-blank-icon">954635</a>)</p></li>
<li><p>XR: Fixed crashes when running Holographic Simulator in Editor. (949293)</p></li>
<li><p>XR: Fixed issues with using <code>renderViewportScale</code> on WindowsMR.</p></li>
</ul>

#### Revision: 46dda1414e51
