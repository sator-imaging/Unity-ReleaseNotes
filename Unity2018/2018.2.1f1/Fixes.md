# Unity 2018.2.1f1
https://unity3d.com/unity/whatsnew/unity-2018.2.1

## Fixes

<ul>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1027063/">1027063</a>) - 2D: Fixed tab button not switching to other input fields in the sprite editor window.</li>
<li>(1054125(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1045785/">1045785</a>)) - Android: Fixed android crash on startup related to having 18 thousand or more assets.</li>
<li>(1045436) - Android: Fixed crash when "Use 32-bit Display buffer" is unchecked in PlayerSettings.</li>
<li>(1056241) - Animation: Fixed parent-child constraint source weight influencing even if set to Zero.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/947055/">947055</a>) - Asset Import: ScriptedImporter - Fixed display of properties that should be read-only in the inspector.</li>
<li>(1059266(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1035312/">1035312</a>)) - Editor: Fixed issue where sprite was not loaded correctly from Sprite Atlas into scene after late binding.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/947055/">947055</a>) - Editor: Fixed ScriptedImporter fields not read-only in Inspector.</li>
<li>(1058290(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1037161/">1037161</a>)) - Editor: Fixes VSCode opens multiple files with spaces in project name.</li>
<li>(1028797) - Editor: Fix issue with script compilation triggering at random times during synchronous import of scripts. Could cause erroneous compilation errors to be emitted to the Editor.log.</li>
<li>(1041276(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/948616/">948616</a>)) - Editor: Fixed an issue where Menu.SetChecked would not update items in the Context menu popup.</li>
<li>(1040404(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1018539/">1018539</a>)) - Editor: Fixed a transform error caused by particle collision events when it's object was being destroyed.</li>
<li>(1058347(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1046782/">1046782</a>)) - Facebook: Fixed for Facebook platform support is not detected by the editor.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1046782/">1046782</a>) - Facebook: Fixed for Facebook platform support is not detected by the editor.</li>
<li>(None) - GI: Fixed up so that area lights have a toggle instead of a dropdown.</li>
<li>(1057921) - Graphics: Fixed Metal/Vulkan/OpenGL shader codegen issue with translating a special case with MOVC instruction.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1020262/">1020262</a>) - IL2CPP: Fixed an issue with call-by-reference method arguments not being properly preserved in certain circumstances.</li>
<li>(1037601) - IL2CPP: Improved performance of thread synchronization for reflection calls.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1045847/">1045847</a>) - IL2CPP: Fixed IL2CPP build failing when project contains a .winmd file that is compiled from C# code.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1044485/">1044485</a>) - IL2CPP: Fixed calls to native functions from delegates using stdcall calling convention, even if explicitly marked as cdecl. Caused problems on windows x86 (and UWP x86), leading to rare crashes in code using SSLStream.</li>
<li>(1042026) - Scripting: Fixed crash when calling DestroyImmediate(gameObject) in OnApplicationQuit after script recompile in the editor. Fixes ZenInject crash that would happen sometimes after exiting play mode.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1053937/">1053937</a>) - Timeline: Fixed issue where the PlayableDirector would not report the correct state when going into play mode after the editor was previously paused.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1043171/">1043171</a>) - Universal Windows Platform: IL2CPP will now successfully be able to P/Invoke into kernel32.dll!GetNativeSystemInfo and Event tracing APIs in advapi32.dll.</li>
<li>(1049132(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1041274/">1041274</a>)) - Web: Fixed crash when sending the same UnityWebRequest twice.</li>
</ul>

#### Revision: 1a9968d9f99c
