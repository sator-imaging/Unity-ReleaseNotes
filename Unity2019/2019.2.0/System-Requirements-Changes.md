# Unity 2019.2.0
https://unity3d.com/unity/whats-new/2019.2.0

## System Requirements Changes


#### Nothing changed. See below for current requirements.

### Features
<ul>
<li><p>2D: Added a Secondary Textures module to the Sprite Editor.</p></li>
<li><p>2D: The Sprite Editor window is now available as a package.</p></li>
<li><p>Android: Added AAB file size validation to Android app bundles. You can disable this in the Android Player Settings (<strong>Warn About App Bundle Size</strong>) and adjust the maximum size (<strong>App Bundle Size Threshold</strong>).</p></li>
<li><p>Android: Added Optimized Frame Pacing.</p></li>
<li><p>Animation: Added a selection filter for the Animation window to only show properties and curves of selected GameObjects.</p></li>
<li><p>Editor: Added VSCode and Rider code editor integration as Packages.</p></li>
<li><p>Editor: Updated behavior so that when you double-click on C# compile messages in the console window in Visual Studio, the corresponding C# file opens at the correct line and column.</p></li>
<li><p>Editor: Updated behavior so that when you double-click on C# compile messages in the console window, in Visual Studio in Windows, the corresponding C# file opens at the correct line and column.</p></li>
<li><p>GI: Added Static Scene Dressing, which lets the user choose whether GameObjects that contribute to Global Ilumination should receive GI from Light Probes or Lightmaps.</p></li>
<li><p>GI: Added support for multiple importance sampling the environment to the GPU lightmapper.</p></li>
<li><p>GI: Added support for the cross-platform Intel lightmap denoiser, Intel Open Image Denoise.</p></li>
<li><p>Graphics: Added SpeedTree support to the Scriptable Render Pipeline.</p></li>
<li><p>Graphics: Added support for all GPU formats for <code>RenderTexture</code> with Vulkan.</p></li>
<li><p>Graphics: Added support for partial mipmap chains in Texture classes.</p></li>
<li><p>iOS: Added client/worker multi-threaded rendering support for OpenGL ES 2 and 3.</p></li>
<li><p>Package Manager: Added the ability to show or hide Packages in the Project window and the Object Picker.</p></li>
<li><p>Physics: Upgraded the cloth library to use NVIDIA's NvCloth Library instead of the deprecated PxCloth.</p></li>
<li><p>Scripting: Added support for Assembly Definition Reference (.asmref) files.</p></li>
<li><p>UI Elements: Added UIElements Samples window. This window provides quick UIElements code snippets in the Editor.</p></li>
<li><p>VFX: Added core pieces to support MotionVectors in VFX Editor (preview Package).</p></li>
</ul>

### Backwards Compatibility Breaking Changes
<ul>
<li><p>2D: Updated the 2D Project Template manifest.json to include 'com.unity.2d.sprite' and 'com.unity.2d.tilemap' as core packages.</p></li>
<li><p>Android: Android Gradle plugin version updated up to 3.4.</p></li>
<li><p>Android: Deprecated x86 support.</p></li>
<li><p>Android: Increased the minimum Vulkan API version for Adreno drivers to 1.0.38.</p></li>
<li><p>Animation: Changed the evaluation order to evaluate constraints before the LateUpdate script. (<a href="https://issuetracker.unity3d.com/issues/sampling-the-position-of-the-gameobject-with-update-function-does-not-yield-the-correct-position">1123107</a>)</p></li>
<li><p>Asset Import: Added a warning when multiple sub-Assets are imported with the same name or type. This often happens when importing Models with multiple Meshes or Materials that have the same name in the .fbx file. Their resulting file ID (and thus references to them) may break or change if Unity re-imports them and finds a new sub-Asset with the same name before finding the existing one.</p></li>
<li><p>Asset Import: Starting with the Unity 2019.3 release, you need an external plugin to import Cinema4D files directly in Unity. The External Tools forum provides updates: https://on.unity.com/c4d.</p></li>
<li><p>Editor: Changed default shortcut for <strong>Stage</strong>/<strong>Go Back</strong> from <strong>O</strong> to <strong>H</strong> to avoid shortcut conflicts in Project templates.</p></li>
<li><p>Editor: Removed most of the legacy Module Manager. Only extension modules located inside the Unity install are loaded now. Also completely removed the <strong>Modules...</strong> menu item and window.</p></li>
<li><p>Editor: UGui Objects use ObjectFactory and default Presets when created from the GameObject menu in the Editor.</p></li>
<li><p>Facebook: Added deprecation warning for Facebook Gameroom platform.</p></li>
<li><p>Graphics: Added Rendering Layer Mask to Lights as a filtering option during shadow passes in Scriptable Render Pipelines. This is similar to Renderers Rendering Layer Masks.</p></li>
<li><p>Graphics: Added support for graphics API switching when restarting Unity.</p></li>
<li><p>Graphics: Asynchronous Shader compilation: Blit now never uses cyan dummy Shader.</p></li>
<li><p>Graphics: Asynchronous Shader compilation: DrawProcedural now skips rendering during compilation instead of trying to use the dummy Shader.</p></li>
<li><p>Graphics: Moved the Async Shader Compilation option from Preferences to Project Settings.</p></li>
<li><p>Prefabs: Prefabs created by dragging into the hierarchy are now parents to the correct parent, instead of being a root object. The correct parent will thus be set in <code>Awake</code> calls.</p></li>
<li><p>Scripting: Made the recommended Visual Studio installer upgrade version 2019</p></li>
<li><p>Scripting: Made the <code>GarbageCollector.GCMode</code> property only throw an exception on unsupported platforms when trying to change it's value, not when reading it.</p></li>
<li><p>Timeline: Clip properties can no longer be animated by recording. Clip properties are animated with the Curves view.</p></li>
<li><p>Timeline: Updated Timeline package version to 1.1.0.</p></li>
<li><p>XR: Moved Vuforia support to a package.</p></li>
<li><p>XR: Oculus (Standalone) and OpenVR (Standalone) package names have been changed to use (Desktop) instead of (Standalone).</p></li>
</ul>

### Changes
<ul>
<li><p>Android: Gradle version updated up to 5.1.1.</p></li>
<li><p>Android: Updated Bundletool to version 0.7.2.</p></li>
<li><p>VFX: Changed the awakening process of the VisualEffect component, so you can now use the Inspector even if the component is disabled. (<a href="https://issuetracker.unity3d.com/issues/vfx-graph-overrides-stored-in-prefabs-get-disabled-when-using-prefabs-in-scenes-making-new-overrides-even-when-reverting">1117103</a>)</p></li>
</ul>
