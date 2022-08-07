# Unity 5.3.3
https://unity3d.com/unity/whats-new/unity-5.3.3

## Improvements

<ul>
<li>GI: Optimized GISceneManager.Update in order to take less processor time on scene start (769044).</li>
<li>Graphics: D3D11 native plugin API now supports obtaining native texture type underpinning a RenderBuffer. (752855)</li>
<li>IL2CPP: Removed warnings from generated C++ code when compiling with clang.</li>
<li>Smart TV: Correspond 2016 TV's fonts and remote controller.</li>
<li>Substance: A FreezeAndReleaseSourceData() method was added to the ProceduralMaterial class. This renders the ProceduralMaterial immutable and releases some of the underlying data to decrease the memory footprint. To release even more of the underlying data, it is necessary to call Resources.UnloadUnusedAssets() afterwards. Once frozen, the ProceduralMaterial cannot be cloned, its ProceduralTextures cannot be rebuilt, nor its inputs be set.</li>
<li>VR: Mask invisible pixels so GPU time is not wasted near screen edges (Oculus SDK 1.0+).</li>
</ul>
