# Unity 2018.2.6f1
https://unity3d.com/unity/whatsnew/unity-2018.2.6

## Fixes

<ul>
<li>(1070250 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1064071/">1064071</a>)) - 2D: Fixed an issue where building sprite atlas via batchmode with -no-graphics on the command line would result in point sampled sprites.</li>
<li>(1064876 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1063235/">1063235</a>)) - Asset Import: Fixed FBX model import crash when importing files that contains stereo cameras.</li>
<li>(1072565 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1045074/">1045074</a>)) - Editor: Fixed drag/dropping material preset onto a material not correctly refreshing the material inspector and the material icon.</li>
<li>(1072564)- Editor: Fixed PresetManagerEditor not correctly refreshing the list of available presets whenever the list of the manager is changing.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1066405/">1066405</a>) - IL2CPP: Prevented a memory leak in delegate unsubscription with the new script runtime.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1068657/">1068657</a>) - IL2CPP: Prevented a crash in il2cpp::os::Image::Initialize when Unity is embedded in another app on iOS.</li>
<li>(1045881 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1027704/">1027704</a>)) (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1030311/">1030311</a>) - iOS: Fixed crash when using Depth Only camera and when using LWSRP.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1042973/">1042973</a>) - UI: Fixed FieldMouseDragger on labels in ShaderGraph.</li>
<li>(1047330) - XR: Windows MR now reports it's inputs properly and no longer spams the console.</li>
<li>(None) - XR: XR.InputTracking now only reports XRNodeStates for connected controllers on mobile.</li>
</ul>

#### Revision: c591d9a97a0b
