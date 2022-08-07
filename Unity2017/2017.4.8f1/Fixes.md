# Unity 2017.4.8f1
https://unity3d.com/unity/whatsnew/unity-2017.4.8

## Fixes

<ul>
<li>(1052023(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1045785/">1045785</a>)) - Android: Fixed android crash on startup related to having 18 thousand or more assets.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1005317/">1005317</a>) - Android: Fixed tessellation shader on Android Adreno GPU.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1007037/">1007037</a>) - Asset Pipeline: Assets: Fixed avatar reference set in model importer causing false dependencies if it's not being used.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/949305/">949305</a>) - Deployment Management: Fixed Lightmapping.BakeMultipleScenes executed via batch mode with -quit argument not creating lightmap textures.</li>
<li>(1040406(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1018539/">1018539</a>)) - Editor: Fix a transform error caused by particle collision events when it's object was being destroyed.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1025810/">1025810</a>) - Editor: Fix performance regression with entering PlayMode while the Test Runner window is open (performance has been improved to previous levels before the regression).</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1038721/">1038721</a>) - Editor: Allow for non-latin characters in the Unity editor install path.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1051722/">1051722</a>) - Editor: Improve the time taken to start running tests in projects with large numbers of test assemblies</li>
<li>(1061390(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/895464/">895464</a>)) - Graphics: Fixed Mesh.CombineMeshes to include only vertices of selected submeshes instead of entire mesh.</li>
<li>(1045857) - IL2CPP: Fixed IL2CPP build failing when project contains a .winmd file that is compiled from C# code.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/852470/">852470</a>) - OSX: Fixed flickering when resizing standalone game window on Mac.</li>
<li>(1005227) - Scripting: Fix crash when calling DestroyImmediate(gameObject) in OnApplicationQuit. Fixes ZenInject crash that would happen sometimes after exiting play mode.</li>
<li>(1057137(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1053937/">1059937</a>)) - Timeline: Fixed OnGraphStop and OnPlayableDestroy not being called if play mode was exited when paused previously.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1043171/">1043171</a>) - UWP: IL2CPP will now successfully be able to P/Invoke into kernel32.dll!GetNativeSystemInfo and Event tracing APIs in advapi32.dll.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1041274/">1041274</a>) - Web: Fixed crash when unused assets are unloaded during texture creation in UnityWebRequest.</li>
<li>(1045453(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1041034/">1041034</a>)) - Web: Fixed crash when sending the same UnityWebRequest twice.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/953054/">953054</a>) - XR: Fixed calling Camera.SetStereoProjectionMatrix switching rendering method to Multi-Pass.</li>
<li>(878834) - XR: Fixed splash image does not appearing in headset.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/878454/">878454</a>) - XR: Fixed headset rendering breaking during play modeif scene window is focussed.</li>
</ul>

#### Revision: 5ab7f4878ef1
