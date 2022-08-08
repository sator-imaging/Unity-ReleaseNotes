# Unity 2019.1.11

https://unity3d.com/unity/whats-new/2019.1.11

## Fixes



*   2D: Fixed compositing of Collider2Ds with CompositeCollider2D when CompositeCollider2D is added after. ([1156794](https://issuetracker.unity3d.com/issues/colliders-are-not-merged-when-using-compositecollider2d), 1163336)
    
*   2D: Fixed the offset of a Tile's Collider shape when a Grid Collider type is used with an Isometric Grid. ([1148573](https://issuetracker.unity3d.com/issues/tilemaps-collider-is-offset-on-the-x-axis-when-using-isometric-tilemap), 1163380)
    
*   Android: Fixed subsystems not being found when using Android app bundles. ([1162654](https://issuetracker.unity3d.com/issues/xr-subsystems-are-not-found-when-using-android-app-bundles), 1162657)
    
*   Animation: Fixed issue where TextMesh with just a empty quad would crash. ([1158732](https://issuetracker.unity3d.com/issues/mesh-recalculatesubmeshboundsinternal-crashes-when-writing-material-equals-1-in-the-text-field-of-text-mesh-component), 1166853)
    
*   Asset Import: Fixed compression quality issue found with some textures using DXT1/BC1 and DXT5/BC3 compressed texture formats. ([1132906](https://issuetracker.unity3d.com/issues/normal-quality-texture-compression-in-unity-2019-causes-significantly-more-color-banding-than-in-unity-2018-dot-3), 1148708)
    
*   Asset Import: Fxed not use FILE\_SHARE\_READ | FILE\_SHARE\_WRITE | FILE\_SHARE\_DELETE share mode when opening file for read on Windows. ([1037669](https://issuetracker.unity3d.com/issues/temp-files-generated-by-excel-or-similair-applications-fail-to-be-read-and-imported), 1158653)
    
*   Editor: Fixed clickable stacktrace not handling parentheses in path. ([1139181](https://issuetracker.unity3d.com/issues/console-window-breaks-when-console-log-that-has-path-containing-parentheses-is-clicked), 1150437)
    
*   HDRP: Fixed editor crash while importing a model with bad mesh data which has 0 triangle. ([1153037](https://issuetracker.unity3d.com/issues/editor-crashes-on-gfxdeviced3d11base-drawbuffersbatchmode-when-selecting-imported-fbx-while-hdrp-is-set-as-srp), 1160014)
    
*   OSX: Fixed focus issues between multiple visible game views. ([1145433](https://issuetracker.unity3d.com/issues/macos-osx-native-plugin-works-only-after-refocusing-unity), 1153164)
    
*   WebRequest: Fixed handshake renegotiation requests by the server are now supported (UnityWebRequest & .Net Apis). ([1141642](https://issuetracker.unity3d.com/issues/rest-request-to-ssl-server-failed-to-receive-data), 1146142)