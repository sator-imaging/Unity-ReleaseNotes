# Unity 4.5
https://unity3d.com/unity/whats-new/unity-4.5

## Upgrade guide

<ul>
<li>iOS: Bumped minimum version of Xcode to 5.0.</li>
<li>Rendering: The internal value of TextureFormat.BGRA32 enum has changed. Any code using that enum in a .NET assembly must be rebuilt. </li>
<li>Mac OS X: Standalone and Webplayer games require OS X 10.6 or later now (i.e. dropped support for 10.5).</li>
<li>NaCl: The Google Native Client build target has been removed and is no longer supported. You need to use Unity 4.2 if you wish to target Google Native client. </li>
<li>Webplayer: Games built in Unity 2.x will no longer run in the Unity Web Player on Mac OSX 10.9 Mavericks.</li>
<li>Webplayer: Use of the Chain of Trust system now requires a Unity-supplied authorization token. If you are using this system, please contact support.</li>
<li>Editor: To have the New Hierarchy Window alphabetically sorted please check out docs at <a href="http://docs.unity3d.com/Documentation/ScriptReference/BaseHierarchySort.html">http://docs.unity3d.com/Documentation/ScriptReference/BaseHierarchySort.html</a>. Once a Editor script is created and derived from BaseHierarchySort a button will appear in the hierarchy window where you can select the sorting method.</li>
</ul>
