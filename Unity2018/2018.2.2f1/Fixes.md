# Unity 2018.2.2f1
https://unity3d.com/unity/whatsnew/unity-2018.2.2

## Fixes

<ul>
<li>Android: Fixed rendering on Tegra 3 devices.</li>
<li>Android: Fixed Vulkan rendering errors on Adreno devices</li>
<li>Android: A friendly user message is now shown when using a JDK other than 8. (<a href="https://issuetracker.unity3d.com/issues/android-builds-fail-with-java-9-jdk-and-unable-to-list-target-platforms-error">956425</a>, 1060076)</li>
<li>Animation: Fixed wrong CurveModifiedType sent in function callback onCurveWasModified when changing animation events in clip. (<a href="https://issuetracker.unity3d.com/issues/animationutility-dot-oncurvewasmodified-invokes-curvemodified-with-an-unknown-binding">1047683</a>)</li>
<li>Editor: Fixed editor crashes when calling EditorUtility.SetDirty(null). (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-in-object-setdirty-when-passing-a-null-into-the-editorutility-dot-setdirty">1060898</a>, 1061076)</li>
<li>GI: Correctly sample area lights from probes in Progressive Lightmapper. (<a href="https://issuetracker.unity3d.com/issues/plm-sh-values-of-some-light-probes-are-unexpectedly-dark-when-using-area-light">1033074</a>)</li>
<li>GI: Fix low CPU utilization when baking with the progressive lightmapper (<a href="https://issuetracker.unity3d.com/issues/plm-cpu-is-underutilized-when-baking-multi-lightmaps">1013830</a>)</li>
<li>Graphics: Fixed a crash (out of bound array access) when some empty RenderPass is used in SRP context. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-in-gfxdevice-beginrenderpass-if-renderpass-dot-subpass-does-nothing">1002440</a>)</li>
<li>Graphics: Fixed possible crash during shader warmup when using Vulkan.</li>
<li>Graphics: Fixed Vulkan validation errors during texture uploads.</li>
<li>Graphics: Fixed a resource leak issue with SRP BlendState and Graphics Jobs</li>
<li>OSX: Fixed framerate being limited in batch mode when Application.targetFrameRate == -1. (1022906)</li>
<li>Package Manager: Fixed not being able to create assets from drop down menu if any projectSettings are opened in inspector. (<a href="https://issuetracker.unity3d.com/issues/assets-are-not-created-from-drop-down-menu-if-any-projectsettings-are-opened-in-inspector">975732</a>)</li>
<li>Particles: Particles are now allowed to use dynamic batching and GPU instancing at the same time for mesh particle systems. Batching allows for a single material setup between systems, and instancing allows for efficient rendering of mesh particles.</li>
<li>Scripting: Fixed "using static" directive causing Unity to not find the class in the script (<a href="https://issuetracker.unity3d.com/issues/default-argument-value-makes-the-editor-recognize-a-script-as-not-valid">962043</a>, <a href="https://issuetracker.unity3d.com/issues/using-static-directive-causes-unity-to-not-find-the-class-in-the-script">962275</a>)</li>
<li>Scripting: Fixed crash when dragging a script with a UI or RectTransform component requirement to a GameObject. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-adding-a-script-with-requirecomponent-typeof-text-to-a-parent-gameobject-with-no-text-component">1036699</a>, 1057076)</li>
<li>Scripting: Fixed random memory corruption and crash usually surfaced during liveness.</li>
<li>Timeline: Fixed parent constraint does not work in timeline preview. (1057525)</li>
<li>XR: Fixed crash that causes the VR device to stop rendering when render texture size is too large and not a power of 2. (1027366)</li>
<li>XR: Fixed issue where HMD's would only render a single frame and black everywhere else when Game tab isn't visible during play mode. (<a href="https://issuetracker.unity3d.com/issues/vr-during-play-mode-headset-rendering-breaks-if-scene-window-is-focused">878454</a>)</li>
</ul>
