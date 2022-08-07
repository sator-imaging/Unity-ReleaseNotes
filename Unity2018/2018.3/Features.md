# Unity 2018.3
https://unity3d.com/unity/whats-new/unity-2018.3.0

## Features

<ul>
<li><p>Android: Added AppBundle generation support.</p></li>
<li><p>Android: Added notch support for Android.</p></li>
<li><p>Android: Added support for requesting permissions at runtime for apps using API level 23 and above.</p></li>
<li><p>Android: Added support for using Kotlin source files as plugins.</p></li>
<li><p>Android: Added the automatic installation and configuration of OpenJDK when installing Unity Android support. Configuration to use manually installed JDKs is no longer officially supported.</p></li>
<li><p>Animation: Added SkinnedMeshRenderer.forceMatrixRecalculationPerRender. Set this property to manually render a skinned mesh multiple times within a single update. For example, for rendering out the results of an animation to a texture.</p></li>
<li><p>Asset Import: Added support for importing R16 textures.</p></li>
<li><p>Editor: Added ability to view each channel in the Texture Inspector.</p></li>
<li><p>Editor: Added improvements to the window tabs:</p> 
<ul>
<li>The selected window tab is now highlighted using a blue outline.</li>
<li>The width of the tab is now adjusted according to the length of the tab title.</li>
<li>You can now scroll through open tabs with arrows when the number of open tabs exceeds the width of the window.</li>
</ul></li>
<li><p>Editor: Introduced new searchable window to display and edit Project Settings and Preferences.</p></li>
<li><p>Editor: Rider installation path detection in Editor Preferences.</p></li>
<li><p>Facebook: The Facebook platform now uses Package Manager for Facebook SDK management. Configure this in the Facebook Build Settings (not the Package Manager UI).</p></li>
<li><p>GI: Added disc-shaped area Light type for baked lighting. Only available in the Progressive Lightmapper.</p></li>
</ul>

#### 
<ul>
<li><p>GI: Added preview version of GPU Lightmapper in Windows Editor. Select this in the Lighting window. The lightmapper is based on OpenCL and RadeonRays and works on all modern GPUs with more than 2Gb of dedicated memory.</p></li>
<li><p>Graphics: Added memory-less frame buffer depth to iOS Metal.</p></li>
<li><p>Graphics: Added shadow bias options to Particles, Lines, and Trails.</p></li>
<li><p>Graphics: Added support for render targets and the R16 texture format.</p></li>
<li><p>Graphics: Added texture 3D CopyTexture support.</p></li>
<li><p>Graphics: Added VFX editor run-time API.</p></li>
<li><p>IL2CPP: Added support for managed code debugging with IL2CPP on Xbox One.</p></li>
<li><p>Mobile: Added Dynamic Resolution Scaling support for Vulkan on Android and Metal on iOS.</p></li>
<li><p>Multiplayer: Added support for providing a custom network transport implementation to be used by Unity Multiplayer's high-level API. See documentation on <code>UnityEngine.Networking.NetworkManager.activeTransport</code> for details.</p></li>
<li><p>Package Manager: Added support for packages in the Project browser.</p></li>
<li><p>Particles: Added option to disable roll on billboard particles, which is particularly useful for VR applications.</p></li>
</ul>
