# Unity 2018.3.9
https://unity3d.com/unity/whats-new/2018.3.9

## Fixes

<ul>
<li><p>2D: Fixed SVG sprites are constanly re-imported when added into prefabs. (1125015)</p></li>
<li><p>Android: Fixed binary shaders not being cached on Android devices with Adreno GPUs. (<a href="https://issuetracker.unity3d.com/issues/android-adreno-gles-binary-shaders-are-not-cached-on-adreno">1129357</a>)</p></li>
<li><p>Animation: Fixed an issue where AnimationPlayable.iKOnFeet didn't propagate properly when multiple AnimationOutputs are connected to the same Animator. (<a href="https://issuetracker.unity3d.com/issues/footik-not-properly-applied-when-using-animator-controller-plus-timeline">1115086</a>)</p></li>
<li><p>Animation: Fixed an issue where trying to add a key to a curve would crash. (<a href="https://issuetracker.unity3d.com/issues/tried-to-add-a-keypoint-on-an-animation-curve">1101703</a>)</p></li>
<li><p>Animation: Fixed crash when changing Animator.playbackTime with a controller using synced layers. (1109439)</p></li>
<li><p>Editor: Added icon for the particle system force field in the scene view. (1107479)</p></li>
<li><p>Editor: Fixed certain shortcuts not executing when in paused play mode. (1129380)</p></li>
<li><p>Editor: Fixed editor freezing when importing/reimporting script that contains unicode characters. (<a href="https://issuetracker.unity3d.com/issues/mac-editor-freezes-when-importing-slash-reimporting-script-that-contains-unicode-characters">1111740</a>)</p></li>
<li><p>Editor: Fixed issue with compile errors not always being cleared correctly when moving the .cs file from one .asmdef folder to another .asmdef folder. (1121925)</p></li>
<li><p>Editor: Fixed issue with compile errors not being cleared correctly in some cases when moving and removing .asmdef files. (1120835)</p></li>
<li><p>Editor: Fixed issue with EditorUtility.scriptCompilationFailed being false when .asmdef assemblies failed to compile on editor startup. (<a href="https://issuetracker.unity3d.com/issues/editorutility-dot-scriptcompilationfailed-not-flagging-package-compilation-errors-during-editor-startup">1106450</a>)</p></li>
<li><p>Editor: Fixed issue with predefined assemblies (Assembly-CSharp.dll and friends) getting recompiled when modifying a Assembly Definition File assembly with "Auto Reference" disabled. (<a href="https://issuetracker.unity3d.com/issues/scripting-asmdef-with-auto-referenced-set-to-false-will-still-cause-recompilation-of-unity-assemblies-assembly-csharp-etc">1124266</a>)</p></li>
<li><p>Editor: Fixed issue with predefined assemblies (Assembly-CSharp.dll and friends) getting recompiled when modifying a Assembly Definition File assembly with "Test Assemblies" enabled. (<a href="https://issuetracker.unity3d.com/issues/scripting-assembly-csharp-dot-dll-gets-built-when-it-does-not-need-to">1082290</a>)</p></li>
<li><p>Editor: Fixed MaterialEditor inspector becoming increasingly laggy the more managed types you have. (1099071)</p></li>
<li><p>Editor: Fixed the issue with the order of items in the Edit Menu on OSX. (1110914)</p></li>
<li><p>Editor: Fixed user32.dll SetCursorPos function always moves the Cursor to the center of the screen when CursorLockMode is set to None. (<a href="https://issuetracker.unity3d.com/issues/cursorlockmode-dot-none-doesnt-work-when-user32-dot-dll-is-effecting-cursor-in-the-script">1096406</a>)</p></li>
<li><p>GI: Fixed crash on application exit when GPU lightmapper openCL context is lost.</p></li>
<li><p>Graphics: Fixed Assets with serializedVersion: 6 meshes are not rendered. (<a href="https://issuetracker.unity3d.com/issues/assets-with-serializedversion-6-meshes-are-not-rendered">1079076</a>, 1130112)</p></li>
<li><p>Graphics: Fixed crash when loading 2018.2 Compressed Mesh data in 2018.3. (1120492)</p></li>
<li><p>Graphics: Fixed particles are not rendered in XBOX One from VSE with HDRP. (1126333)</p></li>
<li><p>Graphics: Fixed Set rendertarget before setting viewport in GrabIntoRenderTexture. (1126248)</p></li>
<li><p>Graphics: Optimised cluster rendering by reducing network packet send latency. (<a href="https://issuetracker.unity3d.com/issues/cluster-rendering-performance-is-slower-on-newest-versions">965251</a>, 1131274)</p></li>
<li><p>iOS: Added 'Automatically add capabilities' checkbox to player settings. (1131078)</p></li>
<li><p>iOS: Fixed Crash when using R8 and RG16 Metal texture formats.</p></li>
<li><p>OSX: Fixed issue where on macOS in the Editor sometimes floating windows would end up in front of other apps. (1115348)</p></li>
<li><p>Package Manager: Fixed package manager for different CultureInfos. (1117469)</p></li>
<li><p>Particles: Fixed "Internal: JobTempAlloc has allocations that are more than 4 frames old" error message (1125073)</p></li>
<li><p>Particles: Fixed crash in GenerateParticleGeometry when a Particle System with Sprites Texture Sheet and FPS Mode has Infinite Start Lifetime. (1119163)</p></li>
<li><p>Particles: Fixed particle scale on GPU Instanced particles. (1117798)</p></li>
<li><p>Particles: Fixed sprite texture sheet animatio getting the wrong UV's when packed in a Sprite Atlas Variant with scale less than 1. (1115470)</p></li>
<li><p>Physics: Disallow zero bounds being passed to Physics.RebuildBroadphaseRegions. (1051407)</p></li>
<li><p>Physics: Fixed a crash that happened when re-activating Rigidbody that had a parent Rigidbody and was reparented while being inactive. (1121720)</p></li>
<li><p>Physics: Fixed a crash when Physics.OverlapSphereNonAlloc was called wiith an infinite sphere radius. (1113683)</p></li>
<li><p>Physics: Fixed a GJK issue that returned incorrect normals when a primitive's centre was so close to the surface of a convex (affected Physics.ComputePenetration). (1115449)</p></li>
<li><p>Physics: Fixed convex meshes being extra bouncy when falling on top of very thin (~contactOffset) objects. (1109477)</p></li>
<li><p>Physics: Fixed MeshCollider not following the changes to a mesh after it produced an empty geometry. (<a href="https://issuetracker.unity3d.com/issues/mesh-collider-gets-corrupted-if-no-triangles-are-specified">996035</a>)</p></li>
<li><p>Physics: Fixed the force limits of ConfigurableJoint's drives being expressed in incorrect units actually. (1116513)</p></li>
<li><p>Physics: Fixed the reset editor button actually not resetting the Collider's trigger property. (<a href="https://issuetracker.unity3d.com/issues/collider-is-trigger-value-on-box-collider-does-not-reset-when-resseting-the-component">1093243</a>)</p></li>
<li><p>Profiler: Fixed UI module chart not showing data. (<a href="https://issuetracker.unity3d.com/issues/profiling-ui-timeline-window-does-not-show-data-when-build-created-with-autoconnect-profiler">1110630</a>)</p></li>
<li><p>Scripting Upgrade: Fixed issue where an async Task throwing an exception would log errors to console repeatedly. (<a href="https://issuetracker.unity3d.com/issues/throwing-exception-in-async-method-in-start-spams-console-does-not-stop-after-leaving-the-playmode">1126231</a>)</p></li>
<li><p>Scripting Upgrade: Fixed issue where an async Task throwing an exception would stop all other Tasks. (1130295)</p></li>
<li><p>Shaders: Fixed shader compiler emitting "//null" on GLES2 as a parameter to one of the functions emulating arithmentic operations on integers using float math. (1124159)</p></li>
<li><p>Shaders: Fixed shader compiler emitting the same struct definition each time it sees it, regardless of whether it was emitted already or not. (<a href="https://issuetracker.unity3d.com/issues/opengles3-shader-compile-errors-and-duplicate-struct-defines">1099165</a>)</p></li>
<li><p>Shaders: Unity could crash if infinite dependency loop between "UsePass" and "Fallback". (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-on-resolveusepasses-when-using-named-passes-from-other-shaders">1068293</a>, 1115947)</p></li>
<li><p>Terrain: Fixed normalization issue when blending 5 or more materials on Terrain. (1129582)</p></li>
<li><p>UI: Driven properties (for example driven by UI layout) now don't get a blue margin in the Inspector and don't show up independently in the Overrides drop-down. (1115499)</p></li>
<li><p>UI: Fixed issue where canvas elements positions are set to NAN when the camera orthographic size is set to 0 and do not reset to valid positions when the orthographic size is changed again. (1125401)</p></li>
<li><p>Vulkan: Vulkan: Fixed crash if the scene does not contain any cameras. (<a href="https://issuetracker.unity3d.com/issues/vulkan-opengl-project-without-camera-crashes-when-building-a-non-development-build">1067621</a>)</p></li>
<li><p>WebGL: FIxed audio not working Safari after Apple added auto-play restrictions (requires clicking on content to enable audio). (<a href="https://issuetracker.unity3d.com/issues/sounds-do-not-play-in-webgl-builds-when-launched-in-safari-12">1089060</a>)</p></li>
<li><p>XR: Fixed performance degradation over time for Virtual Reality applications. (1130392)</p></li>
</ul>
