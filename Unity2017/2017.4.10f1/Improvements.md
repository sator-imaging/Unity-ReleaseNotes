# Unity 2017.4.10f1
https://unity3d.com/unity/whatsnew/unity-2017.4.10

## Improvements

<ul>
<li>Editor: Reduced enter play mode and recompile time by optimizing EditorCompilationInterface.GetTargetAssembly and EditorCompilationInterface.GetTargetAssembliesWithScripts. Has a high impact on projects with lots of scripts and lots of .asmdef files</li>
<li>XR: Updated Oculus to version 1.27.1.</li>
</ul>

### Fixes
<ul>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1035312/">1035312</a>) - 2D: Fixed sprite not being loaded from Sprite Atlas issue when referenced anywhere in the scene.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1058281/">1058281</a>) - Android: Fixed crash on 'crnlib::crn_comp::append_chunks' when Packing Sprite atlas.</li>
<li>(1046581) - Android: Fixed problem with graphical corruption when screen resolution is changed.</li>
<li>(1048647) - Android: Fixed instant apps not being correctly signed.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1041327/">1041327</a>) - Animation: Fixed crash on race condition when deleting Animation component and MeshRenderer under high stress.</li>
<li>(1061418) - Asset Bundles: Fixed an issue where building bundles could cause a hang in the Editor.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/943254/">943254</a>) - Collab: Fixed a bug where Collab Toolbar would sometimes get stuck after downloading changes that caused conflicts.</li>
<li>(1021955) - Editor: Fixed Editor hanging when encountering exceptions or errors in BatchMode.</li>
<li>(1048493) - Editor: Search in project and hierarchy/scene now only starts after the user has finished typing.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1030584/">1030584</a>) - Editor: Fixed crash while packing a huge sprite with sprite atlas when the graphics API is set to D3D11 or D3D12).</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/997622/">997622</a>) - Editor - Other: Fixed detached Editor windows going behind the Editor when clicked outside issue.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1033074/">1033074</a>) - Global Illumination: Fixed area lights not being correctly sampled from probes in Progressive Lightmapper.</li>
<li>(1063738) - Graphics: Fixed a crash on shutdown when using compute shaders.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/970038/">970038</a>) - Graphics: Improved CPU performance running GLES3 on some Android devices particularly for scenes with large number of draw calls.</li>
<li>(1063289) - iOS: Fixed splash screenshowing incorrectly after initially showing correctly on iPhone.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1038876/">1038876</a>) - Mobile: Fixed GLSL uniform arrays on android 4.* VideoCore and Vivante GPU.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1064232/">1064232</a>) - Particles: Fixed unnecessary sync of Light Transforms when using the Particle System Lights module.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1005502/">1005502</a>) - Scripting: Fixed crash when MonoImporter.SetExecutionOrder is called from RuntimeInitializeOnLoadMethod.</li>
<li>(None) - Scripting: Fixed random memory corruption and crash usually surfaced during liveness.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/987068/">987068</a>) - Shuriken: Fixed Timeline Control Track not applying start delay to particles.</li>
<li>(1046113) - VR: Updated copy of warning and log message when using Canvas screen space overlay render mode when VR is enabled.</li>
<li>(1051206) - Vuforia: Fixed exception being thrown when building iOS project with Vuforia's plugin.</li>
<li>(None) - XR: Fixed nullptr returns for XRDevice.GetNativeSDKPointer() when using Oculus.</li>
</ul>

#### Revision: f2cce2a5991f
