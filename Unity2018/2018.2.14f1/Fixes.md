# Unity 2018.2.14f1
https://unity3d.com/unity/whatsnew/unity-2018.2.14

## Fixes

<ul>
<li><p>Asset Pipeline: Fixed crash when importing FBX containing a CameraSwitcher node. (<a href="https://issuetracker.unity3d.com/issues/unity-freezes-when-importing-a-specific-fbx-file">1083284</a>, 1086520)</p></li>
<li><p>Build Pipeline: Clarified size values presented by the Build Report. (<a href="https://issuetracker.unity3d.com/issues/when-building-editor-dot-log-build-report-complete-size-is-massive-slash-too-big">1006704</a>)</p></li>
<li><p>Editor: Fixed shift+delete project asset deletion not working. (<a href="https://issuetracker.unity3d.com/issues/assets-can-no-longer-be-instantly-deleted-using-shift-plus-delete">1057094</a>, 1062584)</p></li>
<li><p>GI: Fixed an issue where, in forward rendering, no shadow casting light using LPPVs would use baked occlusion even if they should not.</p></li>
<li><p>Graphics: Fixed dynamic batching with tangents and unused normals. (<a href="https://issuetracker.unity3d.com/issues/dynamic-batching-dynamic-batching-corrupts-tangents-on-a-fbx-that-has-calculate-tangents-enabled">1069184</a>)</p></li>
<li><p>iOS: Fixed TLS error using WebSockets when certificate chain includes root certificate. (<a href="https://issuetracker.unity3d.com/issues/unable-to-establish-wss-connection-in-ios-and-android">1082184</a>, 1091206)</p></li>
<li><p>Mobile: Fixed a crash when creating Texture2DArray in ETC format on Adreno 3xx on devices with Android 4.4. (<a href="https://issuetracker.unity3d.com/issues/android-apk-crashes-when-uploading-texture2darray-to-the-gpu-on-an-android-device-with-an-adreno-300-series-gpus-and-os-4-dot-4-star">1077349</a>)</p></li>
<li><p>Particles: Fixed some confusing behaviour and messages regarding non-read/write meshes on the shape module and renderer. (<a href="https://issuetracker.unity3d.com/issues/particle-system-renderer-mesh-becomes-missing-when-loading-it-from-a-prefab-in-editor">1084398</a>, 1084858)</p></li>
<li><p>Scripting: Fixed error in CSharpNameParser when parsing conditional directives. (<a href="https://issuetracker.unity3d.com/issues/error-in-csharpnameparser">1077417</a>)</p></li>
<li><p>Video: Fixed Video build error on headless server. (<a href="https://issuetracker.unity3d.com/issues/video-build-error-on-headless-server-microsoft-media-foundation-initialization-failed">1053877</a>)</p></li>
<li><p>VR: Fixed issue of error spam when depth buffer sharing was enabled during Holographic Remoting or Simulation. (<a href="https://issuetracker.unity3d.com/issues/windowsmr-failure-to-get-rendering-parameters-for-main-camera-when-depth-buffer-sharing-is-enabled">1047269</a>)</p></li>
<li><p>Vulkan: Fixed [iOS] Crash in Animator Controller destructor with DeallocateResources. (1046701)</p></li>
</ul>

#### Revision: 3262fb3b0716
