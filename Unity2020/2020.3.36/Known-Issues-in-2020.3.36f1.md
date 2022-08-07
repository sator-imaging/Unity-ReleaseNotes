# Unity 2020.3.36
https://unity3d.com/unity/whats-new/2020.3.36

## Known Issues in 2020.3.36f1

<ul>
<li><p>AI Navigation: NavMesh::Raycast freezes the whole editor in an infinite loop on Application.UpdateScene (<a href="https://issuetracker.unity3d.com/issues/navmesh-raycast-freezes-the-whole-editor-in-an-infinite-loop-on-application-dot-updatescene">UUM-2496</a>)</p></li>
<li><p>GI: If a user is experience lighting coruption they be may required to reimport due to a fix to which correctly fixes a Uv unwrapping issue (1330830).</p></li>
<li><p>Inspector Framework: First array element expansion is broken for arrays that use Custom Property Drawers (<a href="https://issuetracker.unity3d.com/issues/first-array-element-expansion-is-broken-for-arrays-that-use-custom-property-drawers">1409773</a>)</p></li>
<li><p>Kernel: Unity crashes on StackWalker::GetCurrentCallstack when rest-certificate.pem is corrupted (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-on-stackwalker-getcurrentcallstack-when-rest-certificate-dot-pem-is-corrupted">1423569</a>)</p></li>
<li><p>Metal: Consistent EditorLoop 5-10ms spikes when using Metal API (<a href="https://issuetracker.unity3d.com/issues/consistent-gfx-dot-waitforpresentongfxthread-5-10ms-spikes-when-using-metal-api">1378985</a>)</p></li>
<li><p>Physics: Crash on internalABP::ABP_PairManager::addPair when switching to ArticulationJointType.SphericalJoint during runtime (<a href="https://issuetracker.unity3d.com/issues/crash-on-internalabp-abp-pairmanager-addpair-when-switching-to-articulationjointtype-dot-sphericaljoint-during-runtime">1418715</a>)</p></li>
<li><p>Physics: Physics overlap queries are not consistent when used against convex Mesh Colliders with a very small scale (<a href="https://issuetracker.unity3d.com/issues/physics-dot-computepenetration-does-not-detect-overlap-consistently-when-using-convex-mesh-colliders">1377578</a>)</p></li>
<li><p>Quality of Life: [Mac] Shortcut manager ignores Control modifier (<a href="https://issuetracker.unity3d.com/issues/mac-shortcut-manager-ignores-control-modifier">1425117</a>)</p></li>
<li><p>Shadows/Lights: Scene is brighter in Standalone player if it was open in the Editor at build time (<a href="https://issuetracker.unity3d.com/issues/scene-is-brighter-in-standalone-player-if-it-was-open-in-the-editor-at-build-time-1">UUM-2743</a>)</p></li>
<li><p>Text: [Mac] ShortcutManager ignores Shift modifier (<a href="https://issuetracker.unity3d.com/issues/mac-shortcutmanager-ignores-shift-modifier-1">UUM-4083</a>)</p></li>
<li><p>Texture: [Backport] [MacOS] Crash on __pthread_kill when Render Texture has no Depth buffer and Dimension is 3D (<a href="https://issuetracker.unity3d.com/issues/backport-macos-crash-on-pthread-kill-when-render-texture-has-no-depth-buffer-and-dimension-is-3d">UUM-5459</a>)</p></li>
</ul>
