# Unity 5.2
https://unity3d.com/unity/whats-new/unity-5.2

## Changes

<ul>
<li>Blackberry: Discontinued Blackberry player support</li>
<li>Editor: Asset Store window is now a part of the default window layout. Docked behind the scene &amp; game views</li>
<li>Editor: Remove legacy Mac OS X corner window resize behaviour</li>
<li>GI: Set default BounceScale to 1</li>
<li>Graphics: Material.CopyPropertiesFromMaterial also copies shader keywords and render queue now</li>
<li>IL2CPP: Make engine stripping in iOS/WebGL a separate setting (PlayerSettings.stripEngineCode) from Mono stripping levels</li>
<li>Introduce EditorSettings.projectGenerationUserExtensions &amp; EditorSettings.projectGenerationBuiltinExtensions</li>
<li>Particles: Particle geometry is generated in world space now (used to be in view space before). If you have custom particle shaders that relied on view space positions coming in, you will need to change them</li>
<li>Reflection Probes: Are rendered in a separate deferred pass when using deferred shading. See Improvements section entry for details</li>
<li>Scripting: Removed hexadecimal color string support from Color and replaced with ColorUtility</li>
<li>Shaders: Can not create fixed function shaders using "new Material(string)" anymore. Shaders must come from assets or be fully precompiled in the editor</li>
<li>Shaders: Changed UnityGlobalIllumination, Unity_GlossyEnvironment, FragmentGI function signatures. If you have custom shaders that uses Unity's PBR please check UnityGlobalIllumination.cginc, UnityStandardBRDF.cginc, UnityStandardCore.cginc respectively</li>
<li>Substance: The communication between Unity's MainThread and the Substance Thread was completely rewritten to better decouple Substance processing from Unity's regular operations and to avoid stalling the MainThread. All crashes and hangs at build time, level load/change time, playmode entry/exit should be gone</li>
<li>Terrain: Changed the default hotkey bindings for terrain tools to F1-F6</li>
<li>UI: CanvasRenderer can now take multiple Materials. Like a MeshRenderer each material refers to a SubMesh of the configured Mesh</li>
<li>UI: CanvasRenderer now takes a Mesh instead of List this allows for the use of imported meshs as part of the UI</li>
<li>UI: UI.Text now accounts for trailing white spaces when performing horizontal alignment</li>
<li>WebGL: Make release builds always fully optimized</li>
<li>Windows Store Apps: AppCallbacks.LoadGfxNativePlugin has been deprecated. All plugins that are in the project and set to build for a given platform are now loaded automatically. The function still exists and does nothing, but it will be removed in a future Unity version</li>
</ul>
