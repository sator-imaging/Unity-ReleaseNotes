# Unity 4.2
https://unity3d.com/unity/whats-new/unity-4.2

## Editor Features

<ul>
<li>Integrated version control support for Perforce. 
<ul>
<li>Do common Perforce operations right inside Unity editor.</li>
<li>We've made the integrated version control system extensible; support for more VCS will be coming later. Or you can write your own VCS plugin, see our plugin page on github.</li>
</ul></li>
<li>Platform switching, player building and asset importing can be cancelled now! How cool is that?</li>
<li>Custom GameView resolutions &amp; aspect ratios. Custom settings are saved per project for easy sharing through version control (ProjectSettings/GameViewSizes.asset).</li>
<li>Preset Libraries: You can now save the following types as presets: 
<ul>
<li>Curves in the Curve Editor and Particle System Curve Editor.</li>
<li>Gradients in the Gradient Editor.</li>
<li>Colors in the Color Picker.</li>
<li>Create new libraries either as personal libraries (saved in preferences) or shared libraries (saved in the project folder).</li>
</ul></li>
<li>Added a Quad primitive ;)</li>
<li>Memory Profiler: Now shows the objects that have references to another loaded object. This can help pinpoint why a given object is in memory.</li>
<li>Shader importer can have default textures specified. When you initially set a shader on a material or reset a material the textures will be set to these default textures.</li>
<li>Texture importer now has "Alpha is Transparency" setting, which does color dilation to fix edge artifacts on semitransparent textures. It is enabled by default for GUI textures.</li>
</ul>
