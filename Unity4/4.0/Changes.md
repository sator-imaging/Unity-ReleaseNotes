# Unity 4.0
https://unity3d.com/unity/whats-new/unity-4.0

## Changes

<ul>
<li>Android: New Unity3d splash screen.</li>
<li>Android: The video player activity has been removed. Fullscreen video is still supported but not as a separate activity.</li>
<li>Android: "Google Play OBB Downloader" is now available in the asset store. The plugin can be used on devices that does not support automatic downloading of APK Expansion Files".</li>
<li>Android: "Google Play Application License Verification" is now available on the asset store and thus no longer embedded in the standard distribution.</li>
<li>Android: Removed X&lt;-&gt;Y axis mismatch for Android input. Now out of the box it should match iOS input. Requires code refactoring!</li>
<li>Editor: Requires a DX9-capable GPU now (pretty much anything since 2004).</li>
<li>Editor: PreferenceItem attribute now works on private static methods.</li>
<li>Editor: Added new default window layout.</li>
<li>Editor: When in OpenGL ES 1.1 graphics emulation, maximum texture size increased from 1024 to 2048 now.</li>
<li>Editor: Temporary meshes created by GUI texts are excluded from vertex buffer count/size statistics in game view.</li>
<li>Editor: If necessary, build dialog now automatically performs a "Switch Platform" when pressing "Build" or "Build &amp; Run" (fixes class layout build errors some have encountered).</li>
<li>Editor: Positive values are enforced in Terrain Detail Wizard.</li>
<li>Editor: Prevent multiple editors from opening the same project on OSX.</li>
<li>Flash: Removed support for Flash Player 11.0 and Flash Player 11.1; players both had serious bugs in memory opcodes. Unity now defaults to Flash 11.2 as target player.</li>
<li>Flash: Disabled GrabPass shaders; they now behave like in Unity non-Pro instead of rendering nothing. Flash can't support GrabPass due to Stage3D limitations.</li>
<li>GameObjects: Active state is now recursive. If a GameObject is inactive, all children will inherit that state.</li>
<li>GameObject.active is now deprecated to make users aware of the new behavior. GameObject.SetActive() or GameObject.activeInHieararchy should be used instead.</li>
<li>Graphics: Low-level rendering API (Graphics and GL classes) do not require Pro license anymore.</li>
<li>Graphics: Marked Get/SetTriangleStrip on Mesh as obsolete</li>
<li>Input: Removed support for assigning an input axis of window movement (only ever worked on Mac).</li>
<li>iOS: removed Unity-iPhone-simulator build target from Xcode trampoline. Now simulator specific changes are backed directly into Unity-iPhone build target. It still requires to rebuild Xcode project after switching between device and simulator SDK.</li>
<li>iOS: PVRTC compressor updated.</li>
<li>iOS: added iOS 6.0 OS target.</li>
<li>iOS: SystemInfo.deviceModel now returns full device name, including revision number.</li>
<li>iOS: Exposed AOT.MonoPInvokeCallbackAttribute custom attribute. Passing managed delegates to native functions is now possible, though limited to static methods only.</li>
<li>iOS: PVRTC compressor upgraded to imgtec 3.0@2144429.</li>
<li>iOS: Gyro and other sensors implementation moved to the trampoline. Provides more possibilities for customizations.</li>
<li>iOS: Now iOS sensors follow screen orientation. No more complicated code for axis remapping! This can be switched off via Input.compensateSensors. Requires code refactoring!</li>
<li>iOS: Removed unneeded one frame of latency (presentRenderBufer moved to the end of Repaint).</li>
<li>iOS: Added iPad Mini and iPad 4gen to iPhoneGeneration.</li>
<li>Prefabs can now have an active state which is copied to instances on instantiation.</li>
<li>Mobile: ARMv6 is not supported anymore.</li>
<li>Model Importing: Model importer no longer triangle strips but does vertex cache optimization if mesh GPU optimization is turned on. GPU optimization is turned on by default.</li>
<li>Model Importing: When using the new animation import mode, Unity will no longer attempt to move the SkinnedMeshRenderer to the root bone.</li>
<li>Native Client: NaCl is now it's own BuildTarget instead of a checkbox in the WebPlayer build target.</li>
<li>NavMeshAgent: Avoidance priority made consistent with e.g. audio priority: Most important = 0. Least important = 99. Default = 50. Loading older scenes will reset agent avoidance priority to new default value (50).</li>
<li>Scripting: Removed SceneView.RenderMode from Editor API(was not documented, but public). Use the documented DrawCameraMode instead.</li>
<li>Scripting: Development player emits warnings when accessing the script API from the wrong thread (or using explicit object initializers).</li>
<li>Scripting: OnEnable no longer changes the execution order of Awake. Execution order for scripts is now much more consistent. The call to OnEnable always comes immediately after Awake.</li>
<li>Substance: Added "Bake and keep" and "Bake and discard" load behaviours, to allow the baking of bitmaps on supported platforms.</li>
<li>UnityObject: Deprecated, and will no longer be used when building a WebPlayer.</li>
<li>UnityOject2: New install script when building the WebPlayer, replaces UnityObject giving more flexibility to developers.</li>
</ul>
