# Unity 5.3.1
https://unity3d.com/unity/whats-new/unity-5.3.1

## Improvements

<ul>
<li>Graphics: Optimized performance of setting up shader blend/depth/raster/stencil states. This is mostly visible when using deferred rendering.</li>
<li>Graphics: Added client/worker multithreaded rendering support to OS X Metal.</li>
<li>IL2CPP: Added support for the MethodImplOptions.NoInlining option to prevent methods in the generated C++ code from being inlined.</li>
<li>iOS: Use new Game Center APIs when possible.</li>
<li>JsonUtility: Serialize Color32 fields as separate RGBA values instead of a binary blob.</li>
<li>Networking: Added a warning for NetworkIdentity on child game objects.</li>
<li>Networking: Added dontListen flag to NetworkServer. This is useful when running in single-player or offline mode, but as a Network Host. RuntimeInitializeOnLoad now fires more consistently when entering playmode in the Editor and playing at Runtime.</li>
<li>SceneManagement: Added SceneManager.UnloadScene(Scene) making it easier to unload a scene if you already have a reference to it.</li>
<li>Substance: Substance textures cached to disk/flash are now LZ4-compressed, old caches are discarded.</li>
<li>Substance: SubstanceImporter.ExportBitmaps is now public.</li>
<li>Substance: ExportPreset was added to the ProceduralMaterialInspector's context menu.</li>
<li>Substance: When importing a SBSAR file, the metallic workflow is now picked up by default if the material has the right outputs, even if it also has the right outputs for the specular workflow. Previously, if the material had the right outputs for the metallic and the specular workflows, then the specular workflow would be selected.</li>
<li>VR: Optimized Oculus to start CPU work for next frame while Rendering the current frame.</li>
</ul>
