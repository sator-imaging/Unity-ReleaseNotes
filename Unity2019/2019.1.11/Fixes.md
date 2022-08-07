# Unity 2019.1.11
https://unity3d.com/unity/whats-new/2019.1.11

## Fixes

<ul>
<li><p>2D: Fixed compositing of Collider2Ds with CompositeCollider2D when CompositeCollider2D is added after. (<a href="https://issuetracker.unity3d.com/issues/colliders-are-not-merged-when-using-compositecollider2d">1156794</a>, 1163336)</p></li>
<li><p>2D: Fixed the offset of a Tile's Collider shape when a Grid Collider type is used with an Isometric Grid. (<a href="https://issuetracker.unity3d.com/issues/tilemaps-collider-is-offset-on-the-x-axis-when-using-isometric-tilemap">1148573</a>, 1163380)</p></li>
<li><p>Android: Fixed subsystems not being found when using Android app bundles. (<a href="https://issuetracker.unity3d.com/issues/xr-subsystems-are-not-found-when-using-android-app-bundles">1162654</a>, 1162657)</p></li>
<li><p>Animation: Fixed issue where TextMesh with just a empty quad would crash. (<a href="https://issuetracker.unity3d.com/issues/mesh-recalculatesubmeshboundsinternal-crashes-when-writing-material-equals-1-in-the-text-field-of-text-mesh-component">1158732</a>, 1166853)</p></li>
<li><p>Asset Import: Fixed compression quality issue found with some textures using DXT1/BC1 and DXT5/BC3 compressed texture formats. (<a href="https://issuetracker.unity3d.com/issues/normal-quality-texture-compression-in-unity-2019-causes-significantly-more-color-banding-than-in-unity-2018-dot-3">1132906</a>, 1148708)</p></li>
<li><p>Asset Import: Fxed not use FILE_SHARE_READ | FILE_SHARE_WRITE | FILE_SHARE_DELETE share mode when opening file for read on Windows. (<a href="https://issuetracker.unity3d.com/issues/temp-files-generated-by-excel-or-similair-applications-fail-to-be-read-and-imported">1037669</a>, 1158653)</p></li>
<li><p>Editor: Fixed clickable stacktrace not handling parentheses in path. (<a href="https://issuetracker.unity3d.com/issues/console-window-breaks-when-console-log-that-has-path-containing-parentheses-is-clicked">1139181</a>, 1150437)</p></li>
<li><p>HDRP: Fixed editor crash while importing a model with bad mesh data which has 0 triangle. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-gfxdeviced3d11base-drawbuffersbatchmode-when-selecting-imported-fbx-while-hdrp-is-set-as-srp">1153037</a>, 1160014)</p></li>
<li><p>OSX: Fixed focus issues between multiple visible game views. (<a href="https://issuetracker.unity3d.com/issues/macos-osx-native-plugin-works-only-after-refocusing-unity">1145433</a>, 1153164)</p></li>
<li><p>WebRequest: Fixed handshake renegotiation requests by the server are now supported (UnityWebRequest &amp; .Net Apis). (<a href="https://issuetracker.unity3d.com/issues/rest-request-to-ssl-server-failed-to-receive-data">1141642</a>, 1146142)</p></li>
</ul>
