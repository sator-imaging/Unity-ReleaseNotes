# Unity 2019.2.1
https://unity3d.com/unity/whats-new/2019.2.1

## Fixes

<ul>
<li><p>2D: Fixed specific set of sprites can be packed non-optimally. (<a href="https://issuetracker.unity3d.com/issues/sprite-packer-specific-set-of-sprites-are-packed-non-optimaly">1002004</a>, 1174641)</p></li>
<li><p>Analytics: Analytics found that the device screen size is always reported as the application render size on Android/iOS and cpu architecture is wrong for Android arm64 devices that are running 32 bit binaries. (1160171, 1160172)</p></li>
<li><p>Android: Fix Android root path initialization from enviroment variables. (1160998, 1173607)</p></li>
<li><p>Android: Fix [Android][OpenGLES] Missing UI and render texture glitches after restarting the game (<a href="https://issuetracker.unity3d.com/issues/android-opengles-missing-ui-and-render-texture-glitches-after-restarting-the-game">1145018</a>, 1157350)</p></li>
<li><p>Animation: Fixed an issue where a clip with no recorded data would cause a crash in GameObjectRecorder.SaveToClip (<a href="https://issuetracker.unity3d.com/issues/unity-runs-out-of-ram-after-calling-gameobjectrecorder-dot-savetoclip-clip">1166522</a>, 1169821)</p></li>
<li><p>Animation: Fixed Undo operation of "Add Motion" in the Blend Tree graph UI. (<a href="https://issuetracker.unity3d.com/issues/undo-removes-wrong-motion-from-blend-tree-when-add-motion-was-done-from-blend-tree-nodes-right-click-context-menu">1134780</a>, 1164506)</p></li>
<li><p>Asset Import: Added the new FileScale property to the ModelImporter class. (<a href="https://issuetracker.unity3d.com/issues/modelimporter-dot-filescale-no-longer-exists">1063711</a>, 1169693)</p></li>
<li><p>Asset Import: Fixed an issue where Unity failed to refresh the animation list after the source .fbx Asset changed. (<a href="https://issuetracker.unity3d.com/issues/new-animations-does-not-show-up-when-reinporting-fbx-file">1139051</a>, 1172117)</p></li>
<li><p>Asset Import: When importing, Unity now Ignores Constraint sources that are identical to the target. (<a href="https://issuetracker.unity3d.com/issues/maya-lt-models-and-animations-get-deformed-when-imported-to-unity">1088845</a>, 1170661)</p></li>
<li><p>Build Pipeline: Fix a crash on Standalone Player when assets with Editor only serialized properties. (<a href="https://issuetracker.unity3d.com/issues/number-if-unity-editor-serialized-properties-crash-standalone-player-when-architecture-is-x86-64">1144591</a>, 1165740)</p></li>
<li><p>Deployment Management: Worker threads for Enlighten are not set up when launching a Server Build. (<a href="https://issuetracker.unity3d.com/issues/worker-threads-for-enlighten-are-set-up-when-launching-a-server-build">1131677</a>, 1144920)</p></li>
<li><p>Editor: Added custom icons vof visual effect graph subgraphs. (1170470, 1171500)</p></li>
<li><p>Editor: Enabled Delete, Duplicate, Find, Frame Selected and Copy/Paste options for Game Objects that have "Not-Editable" flag enabled. (<a href="https://issuetracker.unity3d.com/issues/delete-duplicate-find-frame-selected-and-copy-slash-paste-are-not-working-on-gameobjects-which-have-noteditable-flag-enabled">460449</a>, 1161574)</p></li>
<li><p>Editor: Enabled Delete, Duplicate, Find, Frame Selected and Copy/Paste options for Game Objects that have "Not-Editable" flag enabled. (<a href="https://issuetracker.unity3d.com/issues/delete-duplicate-find-frame-selected-and-copy-slash-paste-are-not-working-on-gameobjects-which-have-noteditable-flag-enabled">460449</a>, 1161574)</p></li>
<li><p>Editor: Fix for an error message when calling AssetDatabase.ImportPackage on a package that contains scripts. (<a href="https://issuetracker.unity3d.com/issues/assetdatabase-dot-importpackage-throws-an-error-when-importing-a-unity-package-with-a-script-inside-of-it">1158305</a>, 1165962)</p></li>
<li><p>Editor: Fix free move handle being constricted in orthographic mode when Handles.matrix is rotated 90 degrees. (1089308, 1152134)</p></li>
<li><p>Editor: Fixed a warning when using the object selector in the avatar preview window. (1138528, 1155345)</p></li>
<li><p>Editor: Fixed an issue in the Editor where text containing special characters was not copied to the clipboard. (<a href="https://issuetracker.unity3d.com/issues/text-is-not-added-to-clipboard-when-copying-text-with-special-characters-within-textmeshpro-ugui">1152899</a>, 1171259)</p></li>
<li><p>Editor: Fixed Null Reference exceptions that occurred when trying to modify normal maps on non-instanced Terrain. (1153471, 1174638)</p></li>
<li><p>Editor: Fixed Splash Screen Background field labels being truncated in Player Settings. (<a href="https://issuetracker.unity3d.com/issues/editor-texts-are-getting-clipped-when-logo-added-to-the-list-in-splash-image">1164579</a>, 1171455)</p></li>
<li><p>Editor: Fixed text copy of special characters (<a href="https://issuetracker.unity3d.com/issues/text-is-not-added-to-clipboard-when-copying-text-with-special-characters-within-textmeshpro-ugui">1152899</a>, 1171259)</p></li>
<li><p>Editor: Fixes a crash issue with Occlusion Culling window in some scenarios (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-while-opening-the-occlusion-culling-window-if-there-is-no-camera-tagged-as-main-camera">1140940</a>, 1168988)</p></li>
<li><p>Graphics: Fixed issues uploading compressed non-power-of-two textures when using D3D11. (<a href="https://issuetracker.unity3d.com/issues/direct3d11-texture-has-yellow-tint-when-loading-it-with-loadrawtexturedata">1146074</a>, 1149021)</p></li>
<li><p>Graphics: Fixed screen space shadow errors when using dynamic resolution. (1141225, 1157021)</p></li>
<li><p>Graphics: Sped up "CullAllVisibleLights" ~5x on a scene with many baked lights (<a href="https://issuetracker.unity3d.com/issues/android-cullallvisiblelights-consume-too-much-cpu-when-only-baked-lights-are-used-in-the-scene">1087657</a>, 1170210)</p></li>
<li><p>IMGUI: Fixed a  word wrap flickering issue with IMGUI. (<a href="https://issuetracker.unity3d.com/issues/bolt-gui-text-width-is-not-calculated-correctly-when-moving-from-one-resolution-to-another-and-guistyle-uses-word-wrap">1089911</a>, 1170535)</p></li>
<li><p>macOS: Fixed a rare crash issue with the Editor build when creating or closing new windows (<a href="https://issuetracker.unity3d.com/issues/mac-os-crash-on-rendereventscontext-removecommandbuffers-when-closing-a-window">1151695</a>, 1165408)</p></li>
<li><p>Mobile: Fix android resolution changes in split-screen mode (<a href="https://issuetracker.unity3d.com/issues/android-ui-elements-get-stretched-after-changing-the-orientation-of-android-device-in-split-screen-mode">1145325</a>, 1160380)</p></li>
<li><p>Mobile: Fix [Android] UI scales incorrectly when using Constant Physical Size mode on android device (<a href="https://issuetracker.unity3d.com/issues/android-ui-scales-incorrectly-when-using-constant-physical-size-mode-on-android-device">1136224</a>, 1161877)</p></li>
<li><p>Mobile: [android] Fixed an issue where Gradle builds could fail if a settings.gradle file exists in the root of the project (<a href="https://issuetracker.unity3d.com/issues/android-gradle-build-fails-when-theres-a-settings-dot-gradle-file-in-the-project-folder">1164013</a>, 1165806)</p></li>
<li><p>Package Manager: Fixed an issue where a package could contain read-only folders if the installation process was interrupted. This made it difficult to delete parent folders without advanced file manipulations.</p></li>
<li><p>Package Manager: Fixed an issue where the execute file mode of packaged files was suppressed, which prevented executables in packages from running on macOS and Linux. (1154433, 1172896)</p></li>
<li><p>Physics: Fix crash that happened during simulation right after destroying a hierarchy of GOs that had nested Rigidbody components attached. (<a href="https://issuetracker.unity3d.com/issues/crash-in-physics-physicsmanager-simulate">1122684</a>, 1167209)</p></li>
<li><p>Profiler: Fix for lost custom samplers on some platforms, added runtime tests. (<a href="https://issuetracker.unity3d.com/issues/customsampler-dot-beginwithobject-fails-in-2019-dot-1-on-ps4-and-xboxone">1160669</a>, 1167124)</p></li>
<li><p>Profiler: Fixed errors thrown when switching between ADB and WiFi profiling. (<a href="https://issuetracker.unity3d.com/issues/profiler-errors-are-thrown-when-switching-to-adb-profiling-from-wifi-profiling">1050359</a>, 1157909)</p></li>
<li><p>Profiler: Fixed non matching Profiler.EndSample errors printed in console when closing player with connected profiler (1150065, 1153959)</p></li>
<li><p>Profiler: Fixed Profiler-Module-close-button and Chart-outline alignment issues (1164515, 1164518)</p></li>
<li><p>Shaders: Fixed an issue with GLSL where two buffers assigned to two separate shader stages could be assigned the same bind point. (<a href="https://issuetracker.unity3d.com/issues/shaders-opengl-structuredbuffer-position-buffer-binding-points-are-reset-for-each-pipeline-stage">1057118</a>, 1171393)</p></li>
<li><p>Shuriken: Particles: Fixed ParticleSystem bounds calculations when using stretched particles and a negative velocity scale (<a href="https://issuetracker.unity3d.com/issues/cone-shaped-particle-systems-bounds-are-smaller-when-renderer-mode-stretched-billboard-speed-scale-has-negative-value">1160531</a>, 1163757)</p></li>
<li><p>Terrain: Fixed issue with terrain brush slider knob disappearing on sliding to extreme left. (<a href="https://issuetracker.unity3d.com/issues/terrain-brush-size-slider-indicator-disappears-when-moving-it-to-the-left-side">1166317</a>, 1167854)</p></li>
<li><p>Terrain: Terrain brush selection shortcuts are assigned to hotkeys F1-F7 by default. (<a href="https://issuetracker.unity3d.com/issues/terrain-f1-f2-f3-f4-shortcuts-are-not-set">1155153</a>, 1167462)</p></li>
<li><p>Terrain: Trees are not generated from Code in the Built Game when Terrain Data is created via Code using the Constructor (<a href="https://issuetracker.unity3d.com/issues/trees-are-not-generated-from-code-in-the-built-game-when-terrain-data-is-created-via-code-using-the-constructor">1148469</a>, 1158548)</p></li>
<li><p>UI Elements: Crash was related to some user code modifying the hierarchy while layout was being computed.Fix is to throw an error in such cases (<a href="https://issuetracker.unity3d.com/issues/crash-on-ygnodelayoutimpl-after-calling-assetdatabase-dot-saveassets">1154561</a>, 1172315)</p></li>
<li><p>Video: VideoPlayer hangs when seeking backwards or forwards on Android (1156779, 1161629)</p></li>
<li><p>Windows: Fixed deadlock on startup on systems with a certain group policy configuration. (<a href="https://issuetracker.unity3d.com/issues/built-projects-do-not-launch-on-some-windows-7-systems">1150661</a>, 1170796)</p></li>
<li><p>Windows: Fixed OpenGL graphics API crashing on certain monitor configurations. (<a href="https://issuetracker.unity3d.com/issues/built-projects-crash-when-using-opengl-with-refresh-rate-over-60hz-and-resolution-over-1080p">1147157</a>, 1170792)</p></li>
<li><p>Windows: Fixed resolution reverting to native refresh rate after losing focus in exclusive full screen mode. (1164372, 1170787)</p></li>
<li><p>Windows: Fixed switching to exclusive full screen from full screen other modes not respecting specified refresh rate. (1164373, 1170785)</p></li>
<li><p>Windows: Fixed window being "Always on top" after switching from exclusive full screen to windowed full screen mode. (<a href="https://issuetracker.unity3d.com/issues/alt-tab-does-not-minimize-built-unity-application-after-switching-from-exclusivefullscreen-to-fullscreenwindow">1157039</a>, 1170780)</p></li>
<li><p>XR: Editor crash when using holographic emulator with hololens (<a href="https://issuetracker.unity3d.com/issues/editor-crash-when-using-holographic-emulator-with-hololens">1141385</a>, 1163557)</p></li>
<li><p>XR: Fix for Can no longer save world anchors to the store using holographic simulate in editor. (1156868, 1163554)</p></li>
<li><p>XR: Fix for Hands selection can no longer be controlled via scripts. (1152960, 1163551)</p></li>
<li><p>XR: Fix for WMR devices assert when playing in editor (1159961, 1159964)</p></li>
<li><p>XR: Fix for XR DeviceAPIs are coming back with incorrect values in Simulation (1158726, 1163548)</p></li>
<li><p>XR: Fix issue with Depth Based LSR on HoloLens V2 that caused significant jitter. (1169760, 1169761)</p></li>
<li><p>XR: Fix null deref access to vr eye texture manager instance. (<a href="https://issuetracker.unity3d.com/issues/xr-windowsmr-project-crashes-when-enabling-xrsettings-for-a-second-time">1115371</a>, 1171507)</p></li>
<li><p>XR: Fix XR Manager system still allowing Legacy XR to be enabled via the checkbox even with loader present. (1169055, 1169066)</p></li>
<li><p>XR: Fixes jiterry Time based animations on quest (<a href="https://issuetracker.unity3d.com/issues/oculus-go-oculus-quest-object-is-jittering-when-position-is-being-affected-by-time-dot-deltatime">1157271</a>, 1172495)</p></li>
<li><p>https://ono.unity3d.com/unity/unity/pull-request/90337/_/2019.2/platform/switch/sdk831</p></li>
</ul>
