# Unity 2019.4.18
https://unity3d.com/unity/whats-new/2019.4.18

## Known Issues in 2019.4.18f1

<ul>
<li><p>Asset Import Pipeline: Prefabs are reimporting every time a code change is made (<a href="https://issuetracker.unity3d.com/issues/prefabs-are-reimporting-every-time-a-code-change-is-made">1294785</a>)</p></li>
<li><p>Serialization: Crash on WalkTypeTreeComplete&lt;<code>SerializedProperty::ContainsManagedReferences'::</code>2'::IsManagedReferenceVisitor&gt; (<a href="https://issuetracker.unity3d.com/issues/crash-on-walktypetreecomplete-serializedproperty-containsmanagedreferences-2-ismanagedreferencevisitor">1302360</a>)</p></li>
<li><p>Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked (<a href="https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene">1250293</a>)</p></li>
<li><p>Audio: [editor][fmod][macOS] Editor is preventing Mac OS from entering sleep mode automatically (<a href="https://issuetracker.unity3d.com/issues/editor-is-preventing-mac-os-from-entering-sleep-mode-automatically">995866</a>)</p></li>
<li><p>Global Illumination: [URP] Transparencies are ignored because URP uses _BaseMap as main texture identifier (<a href="https://issuetracker.unity3d.com/issues/urp-shadows-from-alpha-materials-are-not-baked-into-a-lightmap-when-using-baked-lit-shader">1246262</a>)</p></li>
<li><p>Graphics Device Backends: [Mac] Editor crashes on MTLGetEnvCase on startup when metalEditorSupport is set to 0 in the ProjectSettings (<a href="https://issuetracker.unity3d.com/issues/mac-editor-crashes-on-mtlgetenvcase-on-startup-when-metaleditorsupport-is-set-to-0-in-the-projectsettings">1298617</a>)</p></li>
<li><p>Profiling: Once paused, the Profiler does not resume recording when profiling WebGL player (<a href="https://issuetracker.unity3d.com/issues/once-paused-the-profiler-does-not-resume-recording-when-profiling-webgl-player">1271012</a>)</p></li>
<li><p>Shader System: Freeze or crash with various stack traces when opening a project while connected to a VPN service (<a href="https://issuetracker.unity3d.com/issues/editor-freezes-slash-crashes-when-connected-to-nordvpn">1025558</a>)</p></li>
<li><p>Linux:  InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked (<a href="https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked">1248389</a>)</p></li>
<li><p>Global Illumination: [macOS] BugReporter doesn't get invoked when the project crashes (<a href="https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes">1219458</a>)</p></li>
<li><p>Global Illumination: gi::InitializeManagers() takes 0.6s during Editor startup (<a href="https://issuetracker.unity3d.com/issues/gi-initializemanagers-takes-0-dot-4s-during-editor-startup">1162775</a>)</p></li>
<li><p>iOS: [iOS 14] VideoPlayer crashes on EXC_BAD_ACCESS or signal SIGABRT when audioOutputMode is set to APIOnly or Audio Source (<a href="https://issuetracker.unity3d.com/issues/ios-videoplayer-crashes-when-audiooutputmode-is-set-to-apionly-or-audiosource">1274837</a>)</p></li>
<li><p>Asset Import Pipeline: Parent and child nested Scriptable Object Assets switch places when parent Scriptable Object Asset is renamed (<a href="https://issuetracker.unity3d.com/issues/parent-and-child-nested-scriptable-object-assets-switch-places-when-parent-scriptable-object-asset-is-renamed">1189089</a>)</p></li>
<li><p>iOS:  Crash on il2cpp::vm::LivenessState::AddProcessObject when using Social.LoadUsers and then changing scenes (<a href="https://issuetracker.unity3d.com/issues/ios-il2cpp-crash-on-il2cpp-vm-livenessstate-addprocessobject-when-using-social-dot-loadusers-and-then-changing-scenes">1270230</a>)</p></li>
<li><p>XR: [XR SDK][Oculus] EarlyUpdate.XRUpdate spikes inconsistently (<a href="https://issuetracker.unity3d.com/issues/xr-sdk-oculus-earlyupdate-dot-xrupdate-spikes-inconsistently">1262597</a>)</p></li>
<li><p>Packman:  Package Manager doesn't show available updates (<a href="https://issuetracker.unity3d.com/issues/package-manager-doesnt-show-available-updates">1304459</a>)</p></li>
<li><p>WebGL: [Audio] "Cannot create FMOD" Error when importing 3D Game Kit project on webGL (<a href="https://issuetracker.unity3d.com/issues/audio-cannot-create-fmod-error-when-importing-3d-game-kit-project-on-webgl">1293595</a>)</p></li>
</ul>
