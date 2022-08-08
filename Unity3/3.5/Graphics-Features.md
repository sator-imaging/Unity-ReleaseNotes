# Unity 3.5

https://unity3d.com/unity/whats-new/unity-3.5

## Graphics Features



*   SkinnedMeshRenderer bounding volume is now always relative to the most common root bone and works much better with Ragdolls.
    *   UpdateWhenOffscreen bounding volume option now uses bone-relative bounding volumes instead of vertices and is around 100x faster.
*   WebCamTexture class now supports cameras.
*   High-resolution screenshots can now be done via Application.CaptureScreenshot’s superSize parameter.
*   Added new Soft Shadows mode for Directional Lights that uses rotated disk sampling pattern.
*   Lightmapping: Added the “Area Light” light type (baked only).
*   Lightmapping: Skinned meshes can now be lightmapped. Use this for meshes that don't change the pose much after baking.
*   Advanced rendering controls:
    *   Image Effects can optionally be applied before any transparent geometries are drawn. Use ImageEffectOpaque attribute on the OnRenderImage function.
    *   Subtractive/Min/Max blending support, use BlendOp Min|Max|Sub|RevSub in ShaderLab.
    *   Multiple Render Targets, Graphics.SetRenderTarget can take multiple color targets.
    *   Enabled sharing of depth buffers between different color buffer targets, see Graphics.SetRenderTarget, RenderTexture.colorBuffer, etc.
*   Various graphics optimizations:
    *   Optimizations for OpenGL ES 2.0 to avoid performance spikes with dynamic geometry.
    *   Optimized culling and shadow caster culling.
*   More low level rendering possibilities from native code Plugins:
    *   Ability to access Direct3D 9 device pointer.
    *   Plugin callbacks on the rendering thread, so that low-level plugin rendering can co-exist with multithreaded renderer in Unity 3.5.
*   Surface Shaders: added optional final color modifier function (finalcolor directive). This can be used to implement custom Fog on platforms that can't do usual fog (like Xbox 360 or PS3).
*   Added renderer.SetMaterialBlock for a lightweight way of adding per-instance material parameters without duplicating the materials. Also, the MaterialPropertyBlock does not have fixed small capacity any longer.
*   Quality settings overhaul:
    *   Quality settings can now be enabled / disabled per platform. Quality levels that are disabled on a target platform will be stripped on build.
    *   Maximum LOD level and LOD bias can be setup in the Quality settings.
    *   The smallest LOD level in the quality settings will be used to automatically strip higher LOD levels. This makes it possible to strip any high poly models and all their dependencies on low-end devices.