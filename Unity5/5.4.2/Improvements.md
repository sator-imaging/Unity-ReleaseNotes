# Unity 5.4.2
https://unity3d.com/unity/whats-new/unity-5.4.2

## Improvements

<ul>
<li>Android: Buildpipe - Added pre-build step that verifies the environment. Check Android device, SDK and JDK before compiling the project and the scripts.</li>
<li>Asset Database: Added a new API for getting asset information without loading asset into memory.</li>
<li>D3D12: Added an error message if trying to ReadPixels from outside the RenderTarget's bounds and return false to ignore the request.</li>
<li>Editor: Improved the tooltip message for Light Probes option in Renderer components.</li>
<li>GI: Added a tooltip in the editor for Light Probes option in Renderer inspectors.</li>
<li>GI: Light Probe Volume - fixed performance issue with LPPV when no Renderers are found in the same game object. Light Probe blending job is much faster now.</li>
<li>GI: Reflection Probes component: Added and updated tooltips.</li>
<li>Graphics: Improved CPU performance when calling lots of Graphics.DrawMesh API with null MaterialPropertyBlock (829800).</li>
<li>Graphics: Slight optimisation of CommandBuffer.DrawMesh and CommandBuffer.DrawRenderer.</li>
<li>Graphics: Updated tooltip test for "Box Projection", "Box Offset" &amp; "Box Size".</li>
<li>IL2CPP: Added an option to link.xml files to ignore missing assemblies.</li>
<li>iOS: Added iPhone 7 and 7+ entries to the device enum.</li>
<li>iOS: Added PlayerSettings to specify microphone and camera usage description. Needed for iOS 10 / Xcode 8 compatibility.</li>
<li>iOS: Update Build and Run to work with Xcode 8.</li>
<li>Lighting: Renamed popup menu item from "Default scene parameter" to "Scene Default Parameters".</li>
<li>Substance: Improved substance assets processing when switching platforms, upgrading a project and building.</li>
<li>tvOS: Added "Require Extended Game Controller" option to player settings.</li>
<li>VR - Updated Oculus plugin to version 1.8</li>
</ul>
