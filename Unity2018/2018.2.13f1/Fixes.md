# Unity 2018.2.13f1
https://unity3d.com/unity/whatsnew/unity-2018.2.13

## Fixes

<ul>
<li><p>Android: Fixed crash when closing scene with active webcamTexture. (<a href="https://issuetracker.unity3d.com/issues/android-crash-when-closing-scene-with-active-webcamtexture">1059444</a>)</p></li>
<li><p>Asset Import: Fixed the Rig setup workflow in the Model Importer to enable setting up the avatar using scripts and presets. (<a href="https://issuetracker.unity3d.com/issues/model-importer-doesnt-allow-creation-of-a-new-humanoid-avatar-from-a-model-file-automatically-through-a-script">1060952</a>, 1066786)</p></li>
<li><p>Editor: Fixed GradientEditor closing when selecting the color picker tool on OSX. Color picker tool is now cancelled when changing keyboard focus. (<a href="https://issuetracker.unity3d.com/issues/gradient-editor-window-closes-automatically-when-clicking-on-color-picker">1059666</a>)</p></li>
<li><p>Editor: Fixed issue with .asmdef assemblies referencing player-only .asmdefs not getting properly compiled on startup in projects without a Library folder/clean import. Potentially leading to missing MonoBehaviour references in scenes until the next recompile of scripts. (<a href="https://issuetracker.unity3d.com/issues/regenerating-the-library-folder-looses-script-references">1082746</a>)</p></li>
<li><p>Editor: Fixed issue with script compilation not triggering correctly when moving a script from one .asmdef folder to another .asmdef folder. (<a href="https://issuetracker.unity3d.com/issues/unity-doesnt-recognize-missing-assembly-references-when-moving-a-script-thats-referred-by-others-from-one-assembly-to-another">1082699</a>)</p></li>
<li><p>Editor: Fixed keypad period and delete for input fields (linux).</p></li>
<li><p>Editor: Fixed Null reference exceptions while typing in project window search bar. (<a href="https://issuetracker.unity3d.com/issues/editor-typing-in-project-window-search-bar-during-play-mode-causes-nullreference-exceptions">1077389</a>)</p></li>
<li><p>Editor: Fixed persistence of user-added items in Component menu. (<a href="https://issuetracker.unity3d.com/issues/selecting-custom-menuitem-from-component-tab-results-in-cant-be-checked-because-doesnt-exist-error-message">1038153</a>)</p></li>
<li><p>Graphics: Fixed multi-threading crash where default property values have to be pulled from the Material when Graphics.DrawMeshInstanced is called. (<a href="https://issuetracker.unity3d.com/issues/ecs-finddatasource-crash-when-playing-a-scene">1046126</a>)</p></li>
<li><p>Graphics: Metal: Fixed unity applications not correctly reported as "Requires High Perf GPU" in Activity Monitor. Vulkan/Metal/OpenGL: Compute shader compilation optimizations.</p></li>
<li><p>IMGUI: Fixed Exception when calling EditorGUIUtility ObjectPicker methods from Custom Editor. (<a href="https://issuetracker.unity3d.com/issues/unityexception-is-thrown-when-calling-editorguiutility-objectpicker-methods-from-custom-editor">1061966</a>, 1077369)</p></li>
<li><p>Mobile: Updated iOS and Android editor game view resolutions and aspect ratios.</p></li>
<li><p>Physics: Fixed issue where physics internal data wasn't being updated if the scene only contained static colliders, causing issues with shape casts. (<a href="https://issuetracker.unity3d.com/issues/windows-physics-dot-spherecast-does-not-properly-detect-collisions-when-clicking-on-certain-objects-spots">1064897</a>)</p></li>
<li><p>Scripting Upgrade: Fixed crash callstacks on OSX. (1074280)</p></li>
<li><p>Shuriken: Fixed transform not recached immediately whena  particle system play state is changed. (<a href="https://issuetracker.unity3d.com/issues/moving-particle-emitters-instantiated-by-an-object-pool-leave-short-flickers-when-reactivated">1027576</a>)</p></li>
<li><p>XR: Updated Google VR for iOS to v1.170. Should resolve issue with orientation changes in Cardboard on iOS. (1087865)</p></li>
</ul>

#### Revision: 83fbdcd35118
