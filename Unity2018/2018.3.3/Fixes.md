# Unity 2018.3.3
https://unity3d.com/unity/whats-new/2018.3.3

## Fixes

<ul>
<li><p>2D: Fixed overlapping Tiles on the Tilemap Renderer when rendering a Hexagonal Tilemap or Grid. (<a href="https://issuetracker.unity3d.com/issues/2d-tilemap-hexagon-sort-order-on-tilemap-renderer-seem-to-cause-some-hexagon-tiles-to-not-overlap-properly">1066481</a>, 1102013)</p></li>
<li><p>2D: RectInt.Contains will support RectInt.size with negative size. (<a href="https://issuetracker.unity3d.com/issues/rectint-dot-contains-doesnt-consider-rectints-width-and-height-being-negative">1079566</a>, 1102012)</p></li>
<li><p>2D: Selecting a Tilemap as the Focus On target will now center and fit the Scene View to the selected Tilemap. (1102011)</p></li>
<li><p>2D: The Grid Brush preview is now highlighted in blue when previewing a Tile with a non-zero Z-Position. (1092473)</p></li>
<li><p>2D: The Grid Brush preview will now be highlighted in the correct Scene View when multiple Scene Views are open. (1102014)</p></li>
<li><p>Android: Fix build when project contains read-only Java source plugins. (<a href="https://issuetracker.unity3d.com/issues/android-build-fails-when-the-assets-slash-plugins-slash-android-folder-which-has-a-java-file-is-set-to-non-writeable">1110471</a>, 1113451)</p></li>
<li><p>Android: Fixed gradle warmup errors when project root includes gradle files. (1109183)</p></li>
<li><p>Editor: Fix crash when calling Prepare() on a VideoPlayer component held by a delay destroyed GameObject (<a href="https://issuetracker.unity3d.com/issues/videoplayer-callbacks-renderforcamera-crashes-when-loading-a-scene-in-play-mode">1096915</a>)</p></li>
<li><p>Editor: Fix issue where duplicating GameObjects could slightly alter the Transform values (typically scale) due to floating point precision issues caused by temporarily reparenting as part of the duplication code. (<a href="https://issuetracker.unity3d.com/issues/duplicated-child-gameobject-inside-canvas-has-modified-recttransform-scale-and-position-values">912111</a>)</p></li>
<li><p>Editor: Fixed default shortcuts for Cut/Copy/Paste/Select All/Undo/Redo menu items not usable for other commands in the Shortcuts window. (1104929)</p></li>
<li><p>Editor: Updated mbedtls to version 2.7.8. (1106822)</p></li>
<li><p>GI: Update OpenCL.dll to better support latest AMD and Nvidia drivers. (<a href="https://issuetracker.unity3d.com/issues/gpu-plm-crash-and-no-fallback-to-cpu-lightmapper-when-baking-the-scene-on-gpu-lightmapper-with-old-opencl-drivers">1085235</a>)</p></li>
<li><p>Graphics: Fixed deletion of external texture not clearing internal texture binding caches. (<a href="https://issuetracker.unity3d.com/issues/ios-the-native-plugin-generated-texture-is-black-in-opengles-development-builds">1094803</a>)</p></li>
<li><p>Graphics: Shaders: made Particles StandardSurface shader support gles2 again. (<a href="https://issuetracker.unity3d.com/issues/gles2-particles-slash-standard-surface-shader-doesnt-render-on-devices">1103043</a>)</p></li>
<li><p>Graphics: Stabilized FrameDebugger behavior on game view repaint events. (<a href="https://issuetracker.unity3d.com/issues/the-draw-call-count-changes-after-moving-the-mouse-into-game-view-when-a-camera-is-rendering-to-a-rendertexture">1093178</a>, 1113210)</p></li>
<li><p>iOS: Fixed Screen.safeArea does not change when Screen.width and Screen.height are changed using Screen.SetResolution. (<a href="https://issuetracker.unity3d.com/issues/ios-screen-dot-safearea-does-not-change-when-screen-dot-width-and-screen-dot-height-are-changed-using-screen-dot-setresolution">1102732</a>)</p></li>
<li><p>Linux: Fixed undocked panels can't be resized in some Desktop Environments. (<a href="https://issuetracker.unity3d.com/issues/linux-editor-undocked-panels-cant-be-resized-in-some-desktop-environments">942780</a>)</p></li>
<li><p>Linux: Linux now has access to the scripts only build checkbox. (<a href="https://issuetracker.unity3d.com/issues/no-option-to-do-a-scripts-only-build-for-the-linux-build-target">1097195</a>, 1100809)</p></li>
<li><p>OSX: Fixed GameKit reference in the application when Game Center is not used (<a href="https://issuetracker.unity3d.com/issues/apple-platforms-gamekit-reference-in-the-application-when-game-room-is-not-used-app-store-rejects-the-build">1065311</a>, 1105054)</p></li>
<li><p>Package Manager: Fixed a permission-related issue on Windows where creating the upm.log file would fail when the process was being run with a system account. For system accounts, the log file is now created under ALLUSERSPROFILE (C:\ProgramData\Unity) instead of LOCALAPPDATA (C:\Users\AppData\Local\Unity). (1107321)</p></li>
<li><p>Package Manager: Fixed an issue where a "dest already exists" error could occur during package resolution. This is because older versions of upm using the npm Javascript library could sometimes leave empty folders inside the npm cache. When adding a package to the npm cache, if the folder already exists, it is now always overwritten. (1111212)</p></li>
<li><p>Physics: Fixes a Physics query performance regression present since 2018.2. (<a href="https://issuetracker.unity3d.com/issues/physics-query-performance-regression-in-2018-dot-2">1094014</a>)</p></li>
<li><p>Prefabs: Fixed crash during merge when Prefab instance object type does not match Prefab asset object type. (1109081)</p></li>
<li><p>Prefabs: Fixed dragging Prefab instance with missing asset to Project Browser. (1105457)</p></li>
<li><p>Scripting: Changing UnityEngine.Scripting.GarbageCollector.GCMode is no longer allowed in the editor. It has too many side effects and causes a lot of unexpected and hard to diagnose issues (1103095)</p></li>
<li><p>Scripting: Consistent target framework version across new scripting runtime. (<a href="https://issuetracker.unity3d.com/issues/vscode-needs-to-target-4-dot-7-2-instead-of-4-dot-5">1110736</a>, 1110737)</p></li>
<li><p>Scripting: Match targetframeworkversion with mono build version. (<a href="https://issuetracker.unity3d.com/issues/vscode-needs-to-target-4-dot-7-2-instead-of-4-dot-5">1110736</a>, 1110737)</p></li>
<li><p>Scripting Upgrade: Fixes a possible deadlock scenario due to SynchronizationContext holding a lock while invoking tasks (<a href="https://issuetracker.unity3d.com/issues/deadlock-due-to-unitysynchronizationcontext-invoking-event-in-lock">1084330</a>)</p></li>
<li><p>Timeline: Fixed keyframing in nested timelines not playing back the animation correctly. (<a href="https://issuetracker.unity3d.com/issues/timeline-control-track-new-recorded-animation-clip-does-not-evaluate">1111501</a>)</p></li>
<li><p>UI: Fixed performance regression with RectTransform animation (1104878)</p></li>
<li><p>VFX: Fixed values are always set to zero in timeline. (<a href="https://issuetracker.unity3d.com/issues/visual-effect-graph-values-are-always-set-to-zero-in-timeline">1111437</a>)</p></li>
<li><p>Windows: Fixed cursor confinement coordinates not readjusting when the window is moved, resized or switched to fullscreen mode using keyboard shortcuts. (<a href="https://issuetracker.unity3d.com/issues/cursor-confinement-in-windowed-mode-transitions-to-the-fullscreen-mode-with-incorrect-boundaries">1046253</a>)</p></li>
<li><p>Windows: Fixed cursor confinement to window not matching window bounds visually. (<a href="https://issuetracker.unity3d.com/issues/cursor-confinement-in-windowed-mode-transitions-to-the-fullscreen-mode-with-incorrect-boundaries">1046253</a>)</p></li>
<li><p>Windows: Fixed headless build crashing if closed via the "X" button in the console.</p></li>
<li><p>Windows: Fixed headless build not having console window when built from generation Visual Studio solution. (<a href="https://issuetracker.unity3d.com/issues/windows-standalone-the-server-build-though-vs-project-generation-does-not-have-a-command-window">1095769</a>)</p></li>
<li><p>Windows: Fixed the issue where building Windows Standalone player with "Create Visual Studio Solution" checkbox checked did not open explorer upon a successful build. (1078360)</p></li>
<li><p>Windows: When exiting fullscreen mode, the window will now be centered instead of put in the top left corner of the monitor. (<a href="https://issuetracker.unity3d.com/issues/windows-game-window-jumps-to-the-top-left-corner-when-switching-to-the-windowed-mode">1067817</a>)</p></li>
<li><p>XR: Fix game view rendering only the left eye when using Vuforia VR.</p></li>
</ul>

#### Changeset: 393bae82dbb8
