# Unity 2018.2.19
https://unity3d.com/unity/whatsnew/unity-2018.2.19

## Fixes

<ul>
<li><p>Animation: Fixed Animation Window selection of nested Animation component hierarchies children of Animator component hierarchies. (<a href="https://issuetracker.unity3d.com/issues/animation-window-shows-parent-animations-for-child-elements-when-parent-has-animator-component-and-children-do-not">1089015</a>)</p></li>
<li><p>Animation: Fixed Animation Window selection of nested Animation component hierarchies children of Animator component hierarchies. (<a href="https://issuetracker.unity3d.com/issues/animation-window-shows-parent-animations-for-child-elements-when-parent-has-animator-component-and-children-do-not">1089015</a>, 1096352)</p></li>
<li><p>Build Pipeline: Fixed "Couldn't call method ShowProfilerWindow" error during Build &amp; Run with the Autoconnect Profiler option set. (<a href="https://issuetracker.unity3d.com/issues/building-with-autoconnect-profiler-enabled-throws-error-that-showprofilerwindow-could-not-be-called">1059763</a>)</p></li>
<li><p>Build Pipeline: Fixed Build &amp; Run with Autoconnect Profiler. (<a href="https://issuetracker.unity3d.com/issues/building-with-autoconnect-profiler-enabled-throws-error-that-showprofilerwindow-could-not-be-called">1059763</a>)</p></li>
<li><p>Editor: Fixed this issue by restricting the insertion of menu items into a given submenu to a prescribed limit of 1000 items and displays a warning about the same. (<a href="https://issuetracker.unity3d.com/issues/assertion-failed-failed-to-insert-item-error-is-thrown-when-scripts-count-exceed-the-limit-of-1167-scripts">1039181</a>)</p></li>
<li><p>GI: Fixed an ordering issue with textures when baking in auto mode. (<a href="https://issuetracker.unity3d.com/issues/terrain-shaders-exhibit-artifacts-when-auto-generate-is-enabled-and-the-scene-is-reloaded-via-script">1064388</a>)</p></li>
<li><p>Graphics: Fixed crash if a shader attempts to access a ComputeBuffer that is not set. (1083323)</p></li>
<li><p>IL2CPP: Fixed IL2CPP build failing if Visual Studio 2019 is installed on the machine.</p></li>
<li><p>IL2CPP: Fixed non-zero based arrays via Array.CreateInstance not being correctly created. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-indexoutofrangeexception-is-thrown-when-getting-last-array-value-with-array-dot-getvalue">1099608</a>)</p></li>
<li><p>IL2CPP: Fixed string fields of types marked with CharSet.Auto as Unicode not being properly marshalled. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-text-get-corrupted-when-creating-windows-dialog-using-charset-dot-auto-with-simplified-chinese">1087594</a>)</p></li>
<li><p>Networking: Fixed syncvar variables sequential refreshing issue. (<a href="https://issuetracker.unity3d.com/issues/syncvar-refresh-is-not-being-updated-in-sequence">1085466</a>, 1102859)</p></li>
<li><p>Physics: Fixed RaycastHit.textureCoord performance issue, was internally copying whole mesh index buffer for no good reason. (<a href="https://issuetracker.unity3d.com/issues/raycasthit-dot-texturecoord-is-very-slow">1065218</a>)</p></li>
<li><p>Scripting: Fixed an issue where SynchronizationContext.Current.CreateCopy would return a default SynchronizationContext and not a UnitySynchronizationContext. (1096869)</p></li>
<li><p>Scripting: Fixed scripting runtime version not changing when modifing it on ProjectSettings.asset from any external tool like version control / overwriting the file / etc. (<a href="https://issuetracker.unity3d.com/issues/regression-scripting-runtime-version-didnt-change-from-outside-cause-crash-on-2018-dot-1">1010811</a>)</p></li>
<li><p>Universal Windows Platform: Fixed an assert that is triggered when Xbox gamepads are disconnected in some situations. (1080114)</p></li>
<li><p>Universal Windows Platform: Fixed crash on app start when using LWRP. (<a href="https://issuetracker.unity3d.com/issues/lwrp-uwp-project-with-lightweight-rp-on-uwp-platform-trigger-an-exeption">1064175</a>)</p></li>
</ul>
