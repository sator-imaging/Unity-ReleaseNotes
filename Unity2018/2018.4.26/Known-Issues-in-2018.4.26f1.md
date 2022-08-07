# Unity 2018.4.26
https://unity3d.com/unity/whats-new/2018.4.26

## Known Issues in 2018.4.26f1

<ul>
<li><p>Animation: Animator.Update CPU time spikes when multiple animations are playing (<a href="https://issuetracker.unity3d.com/issues/animator-dot-update-cpu-time-spikes-when-multiple-animations-are-playing">1184690</a>)</p></li>
<li><p>Asset Importers: Crash on VertexDeclarationD3D11::GetInputLayout when importing a broken FBX file (<a href="https://issuetracker.unity3d.com/issues/crash-on-vertexdeclarationd3d11-getinputlayout-when-importing-a-broken-fbx-file">1239074</a>)</p></li>
<li><p>MacOS: [Mac] Many artifacts can be seen in Scene View when Scene Light is enabled and HDR is on with Metal API and Mac OS X 10.15.4 (<a href="https://issuetracker.unity3d.com/issues/mac-many-artifacts-can-be-seen-in-scene-view-when-scene-light-is-enabled-on-with-metal-api-and-mac-os-x-10-dot-15-dot-4">1240265</a>)</p></li>
<li><p>Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.</p></li>
<li><p>macOS: If the Android Tools are not installed through the Hub, macOS 10.15 (Catalina) default security settings will prevent the Android NDK binaries being executed. These settings have to be changed or a signed Android NDK (r16b) will be needed to build Android. More information here: https://developer.android.com/ndk/downloads/older_releases.</p></li>
</ul>
