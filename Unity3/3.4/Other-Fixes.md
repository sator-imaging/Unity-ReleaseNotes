# Unity 3.4
https://unity3d.com/unity/whats-new/unity-3.4

## Other Fixes

<ul>
<li>Web player: 
<ul>
<li>Fix several cases that caused crash in rare occasions and improve error handling in general.</li>
<li>Fix issue that prevented Web Player from working in closed networks.</li>
<li>Fix issue that prevented auto update from working for non-administartor users on Mac OS X.</li>
<li>Prevent cursor from vanishing in fullscreen mode when cursor trail is enabled.</li>
<li>Prevent cursor from vanishing when another game is running on a different browser tab.</li>
<li>Stabilized web player framerates.</li>
<li>Web player now behaves correctly when resizing window in Firefox4.</li>
<li>Removed 16 kilobyte limit for Application.ExternalCall() and ExternalEval().</li>
<li>Chrome, Safari and FF4 on Mac OS X now registers keypresses on input string.</li>
<li>Input.GetAxis() returns correct value when focus is restored.</li>
<li>Fixed an occasional crash when switching to fullscreen on Mac OS X.</li>
<li>Fixed audio pausing in the background in Dashboard on Mac OS X.</li>
</ul></li>
<li>Networking: 
<ul>
<li>Fixed error when reading 32bit Network View IDs, huge amounts of views can properly be instantiated.</li>
</ul></li>
<li>MonoDevelop: 
<ul>
<li>Fixed bug where seemingly random parts of the Unity API would fail to show up in autocomplete lists.</li>
<li>Fixed update expandability of items in the Locals pad when debugging over a slow network.</li>
</ul></li>
<li>Asset pipeline: 
<ul>
<li>Made clearer error message when importing .dds file with missing mipmap levels in texture importer.</li>
<li>3DStudio Max importer no longer crashes when trying to parse a broken .3ds file.</li>
<li>Changing "Pack Margin" and other settings in the advanced Model import setting is now recognized as a change.</li>
</ul></li>
<li>Input: 
<ul>
<li>Shift keys now recognized in fullsceen on Mac OS X web players.</li>
<li>Mouse position now reported correctly for Windows 7 touchscreens (only works in full screen for now – see known issues).</li>
</ul></li>
<li>Physics: 
<ul>
<li>ConfigurableJoint.configuredInWorldSpace will no longer result in a wrong coordinate space. Projects using this setting need to be readjusted!</li>
<li>Better Skinned Cloth behaviour when the mesh does not have normals, or is rendered with a shader that does not use normals.</li>
</ul></li>
<li>Other fixes: 
<ul>
<li>Fixed a bunch of minor mistakes in the documentation.</li>
<li>Cleaned up the use of non-public APIs that caused Mac OS X standalone builds to be rejected for the Mac App Store.</li>
<li>Fixed crash when doing raycasts on 64 bit standalone players.</li>
<li>AssetBundle.Load() now preloads all dependent assets like AssetBundle.LoadAsync() does.</li>
<li>Fixed regression introduced in Unity 3.3 where preload data was not written correctly leading to some hiccups during gameplay when first accessing a referenced asset.</li>
<li>Fixed crash when loading Asset Bundles to big to fit in memory.</li>
<li>Fix bug preventing standalone player &amp; web player from using more than 2GB of ram on Windows.</li>
<li>Fixed crash when deleting the last slot of a builtin array.</li>
<li>Fix bug where enums were sometimes not displayed correctly for embedded classes in arrays.</li>
<li>Fixed creation of empty cache folders for each new project.</li>
<li>Workaround for crash in Apple's Font unloading code in Mac OS X 10.7.</li>
</ul></li>
</ul>
