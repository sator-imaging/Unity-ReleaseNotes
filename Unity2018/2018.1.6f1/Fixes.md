# Unity 2018.1.6f1
https://unity3d.com/unity/whatsnew/unity-2018.1.6

## Fixes

<ul>
<li>(None) - Android: Fixed crash when running on Android 8 in instant app mode.</li>
<li>(1046738(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/785610/">785610</a>)) - Android: Fix for graphical corruption when screen resolution is changed.</li>
<li>(1026812(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1018967/">1018967</a>)) - Android: Fix internal android build to include only required abi from aar files.</li>
<li>(1032929) - Editor: Reduced enter play mode and recompile time by optimizing EditorCompilationInterface.GetTargetAssembly and EditorCompilationInterface.GetTargetAssembliesWithScripts. Has a high impact on projects with lots of scripts and lots of .asmdef files.</li>
<li>(None) - Editor: Editor Skin becomes grey when a Collab project is opened for the first time.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1008728/">1008728</a>) - Editor: Fix commandline filtering for running Tests.</li>
<li>(1035068) - GI: Fix HDR lightmaps encoding in Gamma Color Space.</li>
<li>(None) - Graphics: Fixed Graphics.DrawMeshInstancedIndirect not supporting 32-bit indices.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1043225/">1043225</a>) - IL2CPP: Fixes an issue that occurs when constrained calls are made on pointer types in unsafe contexts.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1040777/">1040777</a>) - IL2CPP: Corrects low level IL behavior when storing values to small local integer variables. This can affect the conversion between pointers and integers in unsafe contexts.</li>
<li>(1036866) - IL2CPP: Changing stack behavior of store-indirect instructions to fix unintended side effects caused by a previous optimization to prevent too many local variables.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1017515/">1017515</a>) - IL2CPP: Fix deadlock on exit when using OnAudioFilterRead.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/984547/">984547</a>) - Physics: Fix Root Motion slowdown introduced in 2017.2.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1028321/">1028321</a>) - Package Manager: Projects created from a template would have the wrong version in ProjectVersion.txt.</li>
<li>(1039037) - Scripting Upgrade: Support Debugger.Break when using new scripting runtime.</li>
<li>(976639) - Universal Windows Platform: Fixed GI folders getting picked up as language resources by Visual Studio.</li>
<li>(1043563) - Universal Windows Platform: Fixed subscribing to Windows Runtime events on IL2CPP scripting backend with .NET Standard 2.0 profile.</li>
<li>(1017288) - Windows: Fixed an exception in RecreateDisplayList when there are no monitors attached.</li>
<li>(951118) - XR: Resolved issue with the OS minimizing the Editor when playing a Mixed Reality application on Windows RS4.</li>
<li>(954950) - XR: Resolved issues with User-Presence not working properly in the Editor for Windows Mixed Reality applications.</li>
</ul>

#### Revision: 57cc34175ccf
