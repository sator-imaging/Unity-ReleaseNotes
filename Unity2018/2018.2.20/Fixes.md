# Unity 2018.2.20
https://unity3d.com/unity/whats-new/2018.2.20

## Fixes

<ul>
<li><p>Android: Fixed Texture2DArray and Texture3D not checking if the filtering mode is supported by the GPU and downgrade when necessary. (963073)</p></li>
<li><p>Animation: Fixed copy/paste and drag&amp;drop of multiple sprite selection in the animation window introducing delays in later frames. (<a href="https://issuetracker.unity3d.com/issues/importing-sprites-into-the-animation-timeline-results-in-some-sprites-being-duplicates-of-each-other">1089466</a>, 1089743)</p></li>
<li><p>GI: Fixed an issue were hashing didn't capture a change of scenes. (<a href="https://issuetracker.unity3d.com/issues/environment-lighting-is-not-applied-when-loading-a-duplicated-scene-via-scenemanager-dot-loadscene">1094637</a>)</p></li>
<li><p>Graphics: Fixed SkinnedMeshRenderer without an Animator component leaking memory. (<a href="https://issuetracker.unity3d.com/issues/rendering-a-scene-with-a-skinned-mesh-renderer-causes-a-jobtempalloc-memory-leak">1086418</a>)</p></li>
<li><p>IL2CPP: Fixed crash when using StructLayout attribute and specifying a Pack value. (1099207)</p></li>
<li><p>Scripting: Fixed passing of arguments to the script compiler not using dashes instead of slashes.</p></li>
</ul>

#### Revision: cef3e6c0c622
