# Unity 2017.2.4f1
https://unity3d.com/unity/whats-new/unity-2017.2.4

## Fixes

<ul>
<li>Android: Fixed to only include selected abi's from an .aar plugin. (1027547(1018697)</li>
<li>Android: Fixed crash when running on Android 8 in instant app mode. (None)</li>
<li>Android: Disabled warnings in ProGuard by default; fixes build errors with 3rd party plugins. (986779)</li>
<li>Android: Fixed black screen on Adreno GPU when using postprocessing stack and GLES2 graphics API. (1013708(984292)</li>
<li>Asset Bundles: Fixed an issue where building bundles could cause a hang in the Editor. (1061418)</li>
<li>Asset Import: Fixed push pull dilation not being applied when importing lightmaps. (1014724)</li>
<li>Build: Fixed build is no longer strict. (None)</li>
<li>DCC: Updated Default Texture Format to low quality. (1039331)</li>
<li>DirectX: Fixed running player on fullscreen exclusive mode shows black screen. (805844)</li>
<li>GI: Fixed rare crash when seam stitching is enabled on object packed to the boundary of a lightmap. (1000350)</li>
<li>Graphics: Fixed crash in Mesh.ClearBlendShapes. (1049575(972060)</li>
<li>Graphics: Fixed backface culling corner cases. (1014151(1010809)</li>
<li>Graphics: Fixed rare deadlock in CreateGpuProgram when graphics jobs are enabled. (1018879(934897)</li>
<li>IL2CPP: Allow managed stack traces to work on the iOS App Store when an application is submitted with bitcode. (850163)</li>
<li>Launcher: Fixed editor crashing while loading a project if you quit Unity Hub. (1006887)</li>
<li>Mobile: Fixed screen flicker when launching Handheld.PlayFullScreenMovie. (978602)</li>
<li>Physics: Fixed cloth losing it's constraints when active on cloth component attached to a skinned mesh renderer. (962027)</li>
<li>Scene Management: Fixed modifying asset import settings from script changing 'timeCreated' in the meta-file, breaking asset representation. (856344)</li>
<li>UI: Fixed nested GameObjects without a Layout Element will effect a Layout Groups arranagement after being disabled and enabled. (1026779)</li>
<li>Video: Fixed audio from UnityEngine.Video.VideoPlayer is distorted when Audio Output Mode is Direct. (1002426)</li>
<li>VR: Updated copy of warning and log message when using Canvas screen space overlay render mode when VR is enabled. (1046113)</li>
<li>Web: Fixed crash when aborting AssetBundle download using UnityWebRequest. (976010)</li>
<li>Xbox One: Fixed rendering errors. (1058870)</li>
<li>Xbox One: Player fails to load files larger than ~2GB. (1032417)</li>
<li>Xbox One: DownloadHandlerFile constructor always fails. (1040849)</li>
</ul>

#### Revision: f1557d1f61fd
