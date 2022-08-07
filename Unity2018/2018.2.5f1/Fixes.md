# Unity 2018.2.5f1
https://unity3d.com/unity/whatsnew/unity-2018.2.5

## Fixes

<ul>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1052530/">1052530</a>) - Android: Fixed an issue on Android with the Auto and Never blit types causing a blank scene to be displayed.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1054584/">1054584</a>) - Build Pipeline: Fixed stripping objects from disabled modules resulting in crashes in generated builds.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1052180/">1052180</a>) - Build Pipeline: Fixed AssetBundleManifestPath not working when building scenes asset bundles.</li>
<li>(1056461) - Editor: Fixed case of "Callback registration failed kMaxCallback" error.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1067552/">1071436</a>) (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1071188/">1071189</a>) - Editor: Fixed CSharpNamespaceParser backport classname parsing.</li>
<li>(None) - Editor: Fixed gui view refresh after resizing views on linux.</li>
<li>(None) - Editor: Fixed keyboard inputs on popups and dropdowns within the Editor on Linux.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1030337/">1030337</a>) - Global Illumination: Fixed Assertion '(srcInfo.GetChannelMask() &amp; copyChannels).</li>
<li>(None) - Graphics: Fixed rare deadlock when using Graphics Jobs and uploading textures which require processing i.e. crunch decompression, scaling, padding.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1066405/">1066405</a>) - IL2CPP: Prevented a memory leak in delegate unsubscription with the new script runtime.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1068657/">1068657</a>) - IL2CPP: Prevented a crash in il2cpp::os::Image::Initialize when Unity is embedded in another app on iOS.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1047005/">1047005</a>) - Input: Fixed cursor resuming locked state after ALT+TAB (Command + Alt).</li>
<li>(None) - Kernel: Added in-range detection for pens on Windows.</li>
<li>(None) - Kernel: Made ProjectWindowUtil.CreateAssetWithContent public again (was accidentally reverted to internal).</li>
<li>(None) - Kernel: Removed automatic device reset on focus loss and add support for explicit device reset IOCTL.</li>
<li>(None) - Kernel: Fixed HIDs sometimes getting picked up twice on OSX.</li>
<li>(None) - Kernel: Fixed various incorrect orientations of scroll and delta Y values.</li>
<li>(None) - Kernel: Fixed mouse coordinates in OSX and Windows player.</li>
<li>(None) - Kernel: Fixed mouse coordinates not respecting HighDPI in Windows editor.</li>
<li>(None) - Kernel: Improved ArchiveStorageHeader::ReadString() performance.</li>
<li>(1030576) - Linux: Fixed a race condition in thread creation in Linux.</li>
<li>(1049050) - OSX: Fixed not being able to reliably set screen resolution from script on first Update.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1033341/">1033341</a>) - Particles: Fixed particle jobs running when baking meshes.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1054584/">1054584</a>) - Particles: Fixed legacy particles module being disabled by default.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1041509/">1041509</a>) - Physics: Fixed experimental multithreaded 2D physics not solving joints the same as non-threaded 2D physics.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1059296/">1062155</a>) - Physics: Fixed an issue where trigger events may not be fired if collider/triggers change local scale only.</li>
<li>(1064472(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1054444/">1054444</a>)) - Physics: Fixed a crash triggered by changing cook option on a deactivated mesh collider.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1051325/">1051325</a>) - Timeline: Fixed keyframing in Timeline when OS is set to non-US cultures.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1061507/">1061507</a>) - XR: OpenVR trackpad axes are reported as 0 on the frame they are pressed.</li>
<li>(1066060 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1036422/">1036422</a>)) - XR: Fixed unneeded.dll created for Audio Spatializer when built for Standalone.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1042946/">1042946</a>) - XR: Fixed UnityEngine.XR.InputTracking.GetNodeNames returning null when a valid uniqueId is given.</li>
</ul>

#### Revision: 3071d1717b71
