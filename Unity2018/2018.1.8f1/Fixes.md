# Unity 2018.1.8f1
https://unity3d.com/unity/whatsnew/unity-2018.1.8

## Fixes

<ul>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1002004/">1002004</a>) - 2D: Fixed specific set of sprites being packed non-optimaly in sprite packer.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1019559/">1019559</a>) - 2D: Fixed sprite indexing is rearranged in Atlas when switching platforms while having platform-dependent settings.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1048806/">1048806</a>) - Android: Fixed errors being spammed in console when android JDK/SDK is not configured.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1035960/">1035960</a>) - Asset Import: Fix for regression where the editor could crash when opened with assets missing a .meta file.</li>
<li>(1021955) - Editor: Fix Editor Hangs when encountering exceptions or errors in BatchMode.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/974240/">974240</a>) - GI: Fix a hash collision for identical meshes in two or more additively loaded scenes.</li>
<li>(1032881(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1027003/">1027003</a>)) - Graphics: Build crashes when using Shader Preloading on Metal.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1047286/">1047286</a>) - IL2CPP: Fixed IL2CPP crashing if it encountered a managed .winmd file that has async method in a public type.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1047267/">1047267</a>) - IL2CPP: Fix IL2CPP build failing if any managed assembly contains a delegate type that doesn't have BeginInvoke or EndInvoke methods.</li>
<li>(850163) - IL2CPP: Allow managed stack traces to work on the iOS App Store when an application is submitted with bitcode.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1023820/">1023820</a>) - Kernel: Fix crash when existing playmode after loading a scene from an asset bundle opened using LoadFromStream API.</li>
<li>(None) - Kernel: Fix incorrect triggering of Assert "Multiple dependency jobs should not be in ScheduleDependencies".</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/954315/">954315</a>) - Mobile Rendering: Improved mobile rendering performance.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1035015/">1035015</a>) - Scripting: Scripting: Fix SystemInfo.SupportsTextureFormat crash when called with obsolete enum value.</li>
<li>(1028089(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1025186/">1025186</a>)) - Scripting: Editor with custom theme crashes when closing with WinScreenSetup::SetWindow.</li>
<li>(978369) - Universal Windows Platform: Fixed TouchScreenKeyboard not working when running on Xbox One.</li>
<li>(1040951(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1002426/">1002426</a>)) - Video: Fix Distorted audio on OSX.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1025120/">1025120</a>) - Windows Standalone: Fixed issue #1025120 that caused setting Screen.fullScreenMode to not work properly on Windows.</li>
<li>(None) - XR: Fixes an issue with Oculus GO apps where closing from oculus Home then relaunching the app resulted in a black screen.</li>
</ul>

#### Revision: 26051d4de9e9
