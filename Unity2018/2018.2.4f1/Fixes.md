# Unity 2018.2.4f1
https://unity3d.com/unity/whatsnew/unity-2018.2.4

## Fixes

<ul>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1059665/">1059665</a>) -  Android  :  Fixed stack overflow when decompressing ASTC textures at runtime.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1050715/">1050715</a>) -  Android  :  ETC texture compressor now preserves color channels when alpha is 0.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1051561/">1051561</a>) -  Android  :  Disabled 3D RenderTextures when using Vulkan on Adreno 4xx devices.</li>
<li>(1048803) -  Android  :  Fixed GPU memory corruption when using Vulkan on Mali devices.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1059717/">1059717</a>,  <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1062402/">1062402</a>) -  Animation  :  Fixed root motion cache so that stale data (NaN) does not propagate in the animation hierarchy.</li>
<li>(1062576, 1060971) -  Editor  :  Fixed invalid namespace in documentation for UIElements.</li>
<li>(None) -  Editor  :  Fixed launch on linux desktops running wayland.</li>
<li>(989834) -  Editor  :  Added short options for unattended mode detection in linux download assistant.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1001151/">1001151</a>) -  Editor  :  Fixed a crash when removing a toplevel menu item on linux.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1050874/">1050874</a>) -  Editor  :  Fixed crash when calling GUILayout.Window multiple times in an editor window's OnGUI.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1048553/">1048553</a>) -  Editor  :  Fixed a crash when imgui events get removed in the same frame that they're used.</li>
<li>(1048491) -  Editor  :  Fix for package scripts not showing up in script execution order inspector.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/970038/">970038</a>) -  Graphics  :  Improved CPU performance running GLES3 on some Android devices particularly for scenes with large number of draw calls.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1052529/">1052529</a>) -  IL2CPP  :  Improved managed stack traces on Android in some cases.</li>
<li>(1063886) -  IL2CPP  :  Now return the proper address list from DNS.GetHostEntry on posix platforms.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1058590/">1058590</a>) -  IL2CPP  :  Implemented the Socket.IOControl method for the new scripting runtime.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1051253/">1051253</a>) -  iOS  :  The default Adaptive icon now will only be included if no legacy or round icons are set and if the default icon field is empty.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1038876/">1038876</a>) -  Mobile - Android :  Fixed GLSL uniform arrays on android 4.* VideoCore and Vivante GPU.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1054313/">1054313</a>) -  OSX  :  Fixed a case of Mac Standalone player crashing on launch when the width / height is set to 0 in Preferences.</li>
<li>(None) -  Package Manager  :  Missing ProjectVersion.txt file would write error in console during migration</li>
<li>(1036736) -  Package Manager  :  "Failed to change file flags" spam in Unity console. </li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/943649/">943649</a>) -  Particles  :  Properly handle NaN coming from PhysX due to internal bug.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1028462/">1028462</a>) -  Particles  :  Cleanup temp memory even when simulation doesn't need advancing.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1032743/">1032743</a>) -  Particles  :  Fixed a crash when sprite atlas is not included in build.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1003997/">1003997</a>) -  Particles  :  Fixed an issue that could cause re-selecting a Particle System in the Editor to be very slow in some situations.</li>
<li>(1064472,<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1054444/">105444</a>) -  Physics  :  Fixed a crash triggered by changing cook option on a deactivated mesh collider.</li>
<li>(1049604,<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1049157/">1049157</a>) -  Profiler  :  Increased maximum allowed memory usage for profiler in the Editor to 256MB</li>
<li>(1025248) -  Scripting  :  Fixed MonoScript default constructor not working correctly.</li>
<li>(1056395) -  Scripting  :  Fixed a single quote and trailing whitespaces issues while parsing namespaces in C#.</li>
<li>(1062514) -    :  Scripting : Fixed a random crash during GC thread suspend on OSX.</li>
<li>(1062676) -    :  Scripting : Fixed a crash on exit when domains are created.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1044157/">1044157</a>) -  Scripting Upgrade  :  Fixed an issue where converting from UTC to local time may have been off by one hour for some timezones.</li>
<li>(1066020, 1059730) -  UI  :  Reduced the wobbling in the editor caused by resizing windows.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1025639/">1025639</a>) -  UI  :  Fixed EndLayout group or Stack empty error after progress dialog is displayed.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1060435/">1060435</a>) -  UnityLinker  :  Prevent an error in the linker when an unused method is stubbed and that is the only method on the type.</li>
<li>(1056212, 1056215) -  VersionControl  :  Editor Made UnityEditor.VersionContro.Asset.isInCurrentProject return true if the asset file exists and is within the current project root.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/973778/">973778</a>) -  Video  :  Fixed an issue where a specific video was not played when built via command line.</li>
<li>(1067985, <a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1025433/">1025433</a>) -  XR  :  Fixed Play mode crash when continually running Windows MR in editor.</li>
</ul>

#### Revision: cb262d9ddeaf
