# Unity 4.0
https://unity3d.com/unity/whats-new/unity-4.0

## Upgrade guide

<ul>
<li>We have changed how the active state of GameObjects is handled. GameObjects active state will now affect child GameObjects, so setting a GameObject to inactive will now turn the entire sub-hierarchy inactive. This may change the behavior of your projects. GameObject.active and GameObject.SetActiveRecursively() have been deprecated. Instead, you should now use the GameObject.activeSelf and GameObject.activeInHierarchy getters and the GameObject.SetActive() method.</li>
<li>Android: Removed X&lt;-&gt;Y axis mismatch for Android input. Now out of the box it should match iOS input. Requires code refactoring!</li>
<li>Editor: We have reset the preferences from 3.x to 4.x. This affects your saved window layouts, the project wizard list, saved filters etc.</li>
<li>Editor: While an asset is being imported it will not be persistent. E.g. if you postprocess a texture and query its asset path, it will return an empty string. Assets outside of the asset postprocessor can, of course, be accessed at any point.</li>
<li>iOS: Now iOS sensors follow screen orientation. No more complicated code for axis remapping! This can be switched off via Input.compensateSensors. Requires code refactoring!</li>
<li>iOS: Target Resolution Player Setting was redesigned to better suite development workflow on multiple iOS devices. Two new “Auto (Best performance)” and “Auto (Best Quality)” settings allow Unity Runtime to choose most optimal rendering resolution according to device GPU capabilities. Some custom editor scripts might need to be updated to comply with these changes. Rendering resolution might be also changed from game scripts using Screen.SetResolution API.</li>
<li>iOS: Device SDK Player Settings was simplified and now contains only two entries “Device SDK” and “Simulator SDK”. Corresponding editor API entries were also changed and some custom editor scripts might need to be changed.</li>
<li>iOS: Unity 4.0 discontinues support for ARMv6 devices (iPhone 1st gen, iPhone 3G, iPod Touch 1st/2nd gen). This affects existing project development in several ways: 
<ul>
<li>Target Platform Player Setting was removed from Unity Editor. Now all Unity iOS applications are ARMv7-only. Corresponding PlayerSetting.iOS Editor API entries also were removed. You might need to fix some of your editor scripts for that.</li>
<li>Graphics API level (Open GL ES 1.1 or 2.x) selection was moved to separate Graphics Level Player Setting. This setting is synced with the Android platform.</li>
<li>Applications that were already released to the App Store as supporting ARMv6+ARMv7 or ARMv6-only now can be updated only if Target iOS Version Player Setting is set to “4.3” or higher.</li>
</ul></li>
<li>Mobile: Unity 4.0 brings hard shadow support to mobiles. Shadows for mobiles are enabled at the default Quality Setting. And if the project is shared with desktop platforms then shadows might just appear on mobiles too when project gets imported into Unity 4.0. Some manual tweaking of lighting/shadow setup might be required for optimal performance on mobiles.</li>
<li>Runtime: GameObjects marked DontDestroyOnLoad are no longer temporarily deactivate when loading a level. They will also not receive an OnDisable / OnEnable call when loading a level.</li>
<li>Graphics: Unity 4.0 adds a "Read/Write Enabled" option in Mesh import settings. When this option is turned off, it saves memory since Unity can unload a copy of mesh data in the game. However, if you are scaling or instantiating meshes at runtime with a non-uniform scale, you may have to enable "Read/Write Enabled" in their import settings. The reason is that non-uniform scaling requires the mesh data to be kept in memory. Normally we detect this at build time, but when meshes are scaled or instantiated at runtime you need to set this manually. Otherwise they might not be rendered in game builds correctly.</li>
<li>Model importing: The Model Importer in Unity 4.0 has become better at mesh optimization. The "Mesh Optimization" checkbox in the Model Importer in Unity 4.0 is now enabled by default, and will reorder the vertices in your Mesh for optimal performance. You may have some post-processing code or effects in your project which depend on the vertex order of your meshes, and these might be broken by this change. In that case, turn off "Mesh Optimization" in the Mesh importer. Especially, if you are using the SkinnedCloth component, mesh optimization will cause your vertex weight mapping to change. So if you are using SkinnedCloth in a project imported from 3.5, you need to turn off "Mesh Optimization" for the affected meshes, or reconfigure your vertex weights to match the new vertex order.</li>
</ul>
