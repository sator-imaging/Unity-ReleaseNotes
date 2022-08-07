# Unity 2017.4.7f1
https://unity3d.com/unity/whatsnew/unity-2017.4.7

## Fixes

<ul>
<li>(1047074(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/973427/">973427</a>)) - Android: Fixed VideoPlayer not working on Intel Baytrail.</li>
<li>(None) - Android: Fixed crash when running on Android 8 in instant app mode.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1023820/">1023820</a>) - Asset Bundles: Fix crash when existing playmode after loading a scene from an asset bundle opened using LoadFromStream API.</li>
<li>(N/A) - Audio: Audio Increase stack size for FMOD file thread to 64KB on all platforms.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/974240/">974240</a>) - GI: Fix a hash collision for identical meshes in two or more additively loaded scenes.</li>
<li>(None) - Graphics: Fix errors when using Typeless D3D11 32 bit texture formats.</li>
<li>(None) - Graphics: OpenGL: Fixed Graphics.DrawMeshInstancedIndirect not supporting 32-bit indices.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1010809/">1010809</a>) - Graphics - General: Fixed some backface culling corner cases (case 1010809).</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1047286/">1047286</a>) - IL2CPP: Fixed IL2CPP crashing if it encountered a managed .winmd file that has async method in a public type.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1047267/">1047267</a>) - IL2CPP: Fix IL2CPP build failing if any managed assembly contains a delegate type that doesn't have BeginInvoke or EndInvoke methods.</li>
<li>(850163) - IL2CPP: Allow managed stack traces to work on the iOS App Store when an application is submitted with bitcode.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/997885">997885</a>) (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1049173/">1049173</a>) - iOS: Fixed an issue where the screen was distorted on devices running iOS 8.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1015543/">1015543</a>) - Physics 2D: Particles using 2D collision mode now never collide with triggers.</li>
<li>(976639) - UWP: Platform: Fixed GI folders getting picked up as language resources by Visual Studio.</li>
<li>(978369) - UWP: Fixed TouchScreenKeyboard not working when running on Xbox One.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/995171/">995171</a>) - Version Control: Make API updater version control integration more robust to unexpected errors.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/981495/">981495</a>) - WebGL: Fix '/b' added to inputString on keyup event.</li>
<li>(1048093) - XR: PressType on HoloLens now correctly reports Select instead of None.</li>
</ul>

#### Revision: de9eb5ca33c5
