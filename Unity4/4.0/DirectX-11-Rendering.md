# Unity 4.0

https://unity3d.com/unity/whats-new/unity-4.0

## DirectX 11 Rendering



*   On Windows Vista and later, and with DX10 or better level GPU, you can use DirectX 11 now.
*   New features:
    *   Geometry shaders (require DX10 GPU) and hull/domain shaders (require DX11 GPU). #pragma geometry, hull, domain in shader files.
    *   Compute shaders (\*.compute files, ComputeShader in scripts).
    *   ComputeBuffer scripting API ("structured buffers" in DX11 lingo). Can use them in compute shaders and regular shader model 5.0 shaders (Material.SetBuffer, Shader.SetGlobalBuffer).
    *   Render textures with "random write" access ("UAVs" in DX11 lingo). Graphics.SetRandomWriteTarget, RenderTexture.enableRandomWrite.
    *   Graphics.DrawProcedural & DrawProceduralIndirect.
    *   DX11-specific RenderTexture formats: RenderTextureFormat.R8, ARGBInt, RGInt, RInt.
    *   3D RenderTextures (RenderTexture.isVolume, volumeDepth). Fill them as "random write" textures from a compute or pixel shader.
    *   In shaders, can optionally use CBUFFER\_START(name) .. CBUFFER\_END macros to markup separate constant buffers.
*   Usage and documentation:
    *   Player Settings has "Use DX11" option; when it it set the editor and player will try using DX11. Editor will have “” in the title bar when it is in DX11 mode.
    *   See “Using DirectX 11” page in the documentation.
    *   New image effects take advantage of DX11: Depth of Field, Camera Motion Blur, Noise.
    *   “Tessellation Shaders” standard package has several shaders that use DX11 tessellation.