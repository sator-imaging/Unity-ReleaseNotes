# Unity 3.5
https://unity3d.com/unity/whats-new/unity-3.5

## Graphics Features

<ul>
<li>SkinnedMeshRenderer bounding volume is now always relative to the most common root bone and works much better with Ragdolls. 
<ul>
<li>UpdateWhenOffscreen bounding volume option now uses bone-relative bounding volumes instead of vertices and is around 100x faster.</li>
</ul></li>
<li>WebCamTexture class now supports cameras.</li>
<li>High-resolution screenshots can now be done via Application.CaptureScreenshot’s superSize parameter.</li>
<li>Added new Soft Shadows mode for Directional Lights that uses rotated disk sampling pattern.</li>
<li>Lightmapping: Added the “Area Light” light type (baked only).</li>
<li>Lightmapping: Skinned meshes can now be lightmapped. Use this for meshes that don't change the pose much after baking.</li>
<li>Advanced rendering controls: 
<ul>
<li>Image Effects can optionally be applied before any transparent geometries are drawn. Use ImageEffectOpaque attribute on the OnRenderImage function.</li>
<li>Subtractive/Min/Max blending support, use BlendOp Min|Max|Sub|RevSub in ShaderLab.</li>
<li>Multiple Render Targets, Graphics.SetRenderTarget can take multiple color targets.</li>
<li>Enabled sharing of depth buffers between different color buffer targets, see Graphics.SetRenderTarget, RenderTexture.colorBuffer, etc.</li>
</ul></li>
<li>Various graphics optimizations: 
<ul>
<li>Optimizations for OpenGL ES 2.0 to avoid performance spikes with dynamic geometry.</li>
<li>Optimized culling and shadow caster culling.</li>
</ul></li>
<li>More low level rendering possibilities from native code Plugins: 
<ul>
<li>Ability to access Direct3D 9 device pointer.</li>
<li>Plugin callbacks on the rendering thread, so that low-level plugin rendering can co-exist with multithreaded renderer in Unity 3.5.</li>
</ul></li>
<li>Surface Shaders: added optional final color modifier function (finalcolor directive). This can be used to implement custom Fog on platforms that can't do usual fog (like Xbox 360 or PS3).</li>
<li>Added renderer.SetMaterialBlock for a lightweight way of adding per-instance material parameters without duplicating the materials. Also, the MaterialPropertyBlock does not have fixed small capacity any longer.</li>
<li>Quality settings overhaul: 
<ul>
<li>Quality settings can now be enabled / disabled per platform. Quality levels that are disabled on a target platform will be stripped on build.</li>
<li>Maximum LOD level and LOD bias can be setup in the Quality settings.</li>
<li>The smallest LOD level in the quality settings will be used to automatically strip higher LOD levels. This makes it possible to strip any high poly models and all their dependencies on low-end devices.</li>
</ul></li>
</ul>
