# Unity 2019.1
https://unity3d.com/unity/whats-new/2019.1.0

## Fixes

<ul>
<li><p>2D: "sprite.textureRect" returns values for master SpriteAtlas instead of SpriteAtlas Variant (<a href="https://issuetracker.unity3d.com/issues/sprite-dot-texturerect-returns-values-for-master-spriteatlas-instead-of-spriteatlas-variant">1115285</a>, 1125298)</p></li>
<li><p>2D: Added missing docs for <code>TextureImportSettings.SpriteMeshType</code>. (1080294)</p></li>
<li><p>2D: Crash in FitBlockMaskInBlockMaskUsingPadding when packing a Sprite Atlas with blockOffset value set to 0 (<a href="https://issuetracker.unity3d.com/issues/crash-in-fitblockmaskinblockmaskusingpadding-when-packing-a-sprite-atlas-with-blockoffset-value-set-to-0">1121583</a>, 1125296)</p></li>
<li><p>2D: Fix exception when trimming Sprite alpha on a texture that is downsized (<a href="https://issuetracker.unity3d.com/issues/indexoutofrangeexception-error-is-thrown-when-trimming-a-sprite-that-has-a-greater-resolution-than-its-import-settings">1104094</a>, 1113929)</p></li>
<li><p>2D: Fix Grid.GetCellCenterWorld returning an offset position when using an Isometric Grid layout (<a href="https://issuetracker.unity3d.com/issues/grid-dot-getcellcenterworld-returns-a-value-offset-from-the-center-when-using-an-isometric-grid-layout">1116814</a>, 1136013)</p></li>
<li><p>2D: Fix Sprite Editor Window module breakage when window is maximized and restore (1114929, 1114930)</p></li>
<li><p>2D: Fix Sprite Frame Inspector window overlaps the header and options when the window is shrunk diagonally (<a href="https://issuetracker.unity3d.com/issues/sprite-editor-sprite-setting-window-overlaps-the-header-and-options-when-the-window-is-shrunk-diagonally">1113250</a>, 1114470)</p></li>
<li><p>2D: Fix when entering negative values in width/height of Sprite Editor Window causes irregular sprite movement (1100307)</p></li>
<li><p>2D: Fixed an assertion message when <code>SpriteRenderer</code> was selected with no Sprite with the <strong>Sprite Editor</strong> window open. (1122260, 1122262)</p></li>
<li><p>2D: Fixed an issue where a Sprite was not generated from a texture when user selected the <strong>Apply</strong> action at the <strong>Unapplied import</strong> settings popup. (1117274, 1122263)</p></li>
<li><p>2D: Fixed an issue where the Editor crashed on clicking <strong>Pack Preview</strong> when same atlas was added in <strong>Packables</strong> in Debug View. (<a href="https://issuetracker.unity3d.com/issues/2d-editor-crashes-on-clicking-pack-preview-when-same-atlas-is-added-in-packables-in-debug-view">1107235</a>)</p></li>
<li><p>2D: Fixed an issue where the side of a Sprite was cut off when its <strong>Max Size</strong> property was changed. (<a href="https://issuetracker.unity3d.com/issues/the-side-of-a-sprite-is-chopped-off-when-its-max-size-property-is-changed">1101500</a>)</p></li>
<li><p>2D: Fixed issue where Sorting Groups did not update in Play Mode when Play Mode was paused in the Editor.</p></li>
<li><p>2D: Fixed issue where Sprites referenced both the original Sprite assets and Sprite Atlas, which resulted in increased memory usage. (<a href="https://issuetracker.unity3d.com/issues/sprites-reference-both-the-original-sprite-assets-and-sprite-atlas-resulting-in-increased-memory-usage">1071494</a>)</p></li>
<li><p>2D: Fixed issue where Sprites rendered through Command Buffers were not displayed until they were rendered once with a default Renderer. (<a href="https://issuetracker.unity3d.com/issues/sprites-rendered-through-command-buffers-not-displayed-until-rendered-once-with-a-default-renderer">1097465</a>)</p></li>
<li><p>2D: Fixed issue where SpriteShapeRenderer passed an invalid <code>_texelSize.zw</code>. (<a href="https://issuetracker.unity3d.com/issues/spriteshaperenderer-passes-invalid-texelsize-dot-zw">1099636</a>)</p></li>
<li><p>2D: Fixed the offset of the TilemapCollider2D collider for Isometric Tilemaps.</p></li>
<li><p>2D: Made a Sprite that is not packed into a Sprite Atlas remain invisible. (1083304)</p></li>
<li><p>2D: Made changes so that when you click and drag on an unselected Sprite, the Sprite Editor Window shows a normal cursor to indicate dragging a Sprite, instead of the resize cursor used for resizing a border. (<a href="https://issuetracker.unity3d.com/issues/trying-to-move-the-green-outline-on-a-sprite-in-the-sprite-editor-moves-the-entire-rect-when-clicking-on-an-unselected-sprite">1077700</a>)</p></li>
<li><p>2D: Made changes to allow users to reset the Sorting Layer and Sorting Order settings of Renderer components from the Inspector Settings (cog button). (<a href="https://issuetracker.unity3d.com/issues/tilemap-renderer-properties-does-not-reset-when-resetting-the-component-using-cogwheel">1096375</a>)</p></li>
<li><p>2D: PSB files do not get packed when added to Sprite Atlas (1114959, 1121775)</p></li>
<li><p>AI: Unity crashes when repathing agent destination (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-when-repathing-agent-destination">1104500</a>)</p></li>
<li><p>Analytics: Fixed a bug that resulted in performance data still being sent from mobile devices when a developer disabled Analytics at runtime. (<a href="https://issuetracker.unity3d.com/issues/performance-data-is-being-sent-when-analytics-are-disabled-in-runtime-on-mobile-devices">1105108</a>)</p></li>
<li><p>Android: Added a fix in the new input system so Deadzoning is not performed in the native backend for game controller axes.</p></li>
<li><p>Android: Added a fix in the new input system so mouse delta is correctly calculated.</p></li>
<li><p>Android: Added detection for when the Editor does not manage to install the application to the device (<a href="https://issuetracker.unity3d.com/issues/android-editor-doesnt-show-that-pushing-built-apps-to-android-4-dot-1-is-failing">1086410</a>)</p></li>
<li><p>Android: Added the ability to opt-out from stopping Gradle daemons upon Editor exit. (1098578, 1138085)</p></li>
<li><p>Android: Added <code>StreamingAssets</code> folders starting with an underscore in Gradle builds</p></li>
<li><p>Android: Enabled EGL sRGB backbuffer in Android 9.0</p></li>
<li><p>Android: Fix black screen when PlayerSetting "Use 32-bit Display Buffer" is disabled (<a href="https://issuetracker.unity3d.com/issues/android-app-shows-black-screen-when-built-without-use-32-bit-display-buffer-option">1103404</a>)</p></li>
<li><p>Android: Fixed a crash on startup in Development Builds on older Android devices</p></li>
<li><p>Android: Fixed a problem with exceptions when exporting an Android Gradle project (<a href="https://issuetracker.unity3d.com/issues/android-gradle-export-throws-trying-to-add-unity-classes-dot-jar-slash-androidmanifest-dot-xml-to-the-list-of-output-files">1089510</a>)</p></li>
<li><p>Android: Fixed a Vulkan shader compile error when using <code>SV_RenderTargetArrayIndex</code> in the vertex shader output (<a href="https://issuetracker.unity3d.com/issues/android-lwrp-pp-building-project-for-the-first-time-there-are-shader-errors-in-the-console-if-using-vulkan-graphics-api">1098973</a>)</p></li>
<li><p>Android: Fixed an issue where a black screen appears when trying to use linear rendering with 16bit backbuffer</p></li>
<li><p>Android: Fixed an issue where Android quickly changing screen orientation twice stretches the view (<a href="https://issuetracker.unity3d.com/issues/android-quickly-changing-screen-orientation-twice-stretches-view">1098327</a>)</p></li>
<li><p>Android: Fixed an issue where Gradle builds fail when using quotes and backslashes in keystore passwords and aliases (<a href="https://issuetracker.unity3d.com/issues/android-gradle-build-fails-if-keystore-slash-key-password-contains-a-single-slash-double-quote">996504</a>, <a href="https://issuetracker.unity3d.com/issues/android-gradle-build-system-does-not-escape-backslash-character-on-keystore-alias-password">1071288</a>)</p></li>
<li><p>Android: Fixed an issue where redundant render pass was created for clear when using Vulkan</p></li>
<li><p>Android: Fixed an issue where the application froze when displaying the Android ProgressBar (<a href="https://issuetracker.unity3d.com/issues/android-application-freezes-when-progressbar-appears-on-the-screen">1053736</a>)</p></li>
<li><p>Android: Fixed an issue where the il2cpp library was relinked when building to Android (1089122)</p></li>
<li><p>Android: Fixed an issue where the <code>CrashReportint</code> module was not stripped on il2cpp when not used.</p></li>
<li><p>Android: Fixed an issue where <code>s_MainWindowRenderingOffscreen == false</code> and <code>CurrentThread::IsMainThread()</code> was firing on Android when using SRP. (1120743, 1133156)</p></li>
<li><p>Android: Fixed an OpenGL ES 3.0 shader compile error when generated code requires <code>bitfieldInsert</code></p></li>
<li><p>Android: Fixed Android touch input scale when changing screen orientation with a custom resolution (<a href="https://issuetracker.unity3d.com/issues/android-button-cannot-be-pressed-on-the-right-slash-bottom-half-of-the-screen-after-changing-resolution-and-screen-orientation-mode">1085580</a>)</p></li>
<li><p>Android: Fixed automatic resolution scaling when using Vulkan (1108491, 1118293)</p></li>
<li><p>Android: Fixed dynamic resolution on some older Mali GPUs on Vulkan (<a href="https://issuetracker.unity3d.com/issues/android-dynamic-resolution-doesnt-work-on-samsung-galaxy-s6-edge-plus">1065227</a>)</p></li>
<li><p>Android: Fixed HDR rendering when using Vulkan on older Mali drivers (<a href="https://issuetracker.unity3d.com/issues/lights-not-rendered-correctly-on-samsung-s6-edge-device-on-vulkan">1105065</a>, 1115919)</p></li>
<li><p>Android: Fixed missing draws when using Vulkan on Adreno (<a href="https://issuetracker.unity3d.com/issues/android-vulkan-meshes-with-standard-shader-and-gpu-instancing-enabled-are-not-rendered-correctly-on-adreno-gpus">1094348</a>)</p></li>
<li><p>Android: Fixed shader compiler errors with Mali 450 drivers</p></li>
<li><p>Android: Fixed Terrain rendering when Vulkan on Adreno is used (<a href="https://issuetracker.unity3d.com/issues/android-vulkan-terrain-with-draw-instanced-enabled-is-not-rendered-on-android-devices-with-adreno-gpu">1102440</a>)</p></li>
<li><p>Android: Fixed the Bluetooth related crash on Android 5 devices when no headset is connected (<a href="https://issuetracker.unity3d.com/issues/android-project-crashes-on-xiaomi-mi-4i">1089471</a>)</p></li>
<li><p>Android: Fixed the load failure of il2cpp player using OBB files (<a href="https://issuetracker.unity3d.com/issues/android-error-of-failed-to-extract-resources-needed-by-il2cpp-when-building-with-split-application-binary-set-to-true">1124777</a>, 1130918)</p></li>
<li><p>Android: Fixed the wrong <code>\</code> director separator in <code>DIR_UNITYPROJECT&amp;amp;DIR_GRADLEPROJECT</code> on Windows (<a href="https://issuetracker.unity3d.com/issues/android-windows-template-variable-dir-unityproject-on-windows-does-not-escape-slash-characters">1088160</a>)</p></li>
<li><p>Android: Fixed <code>Activity  has leaked ServiceConnection</code> errors when calling <code>Application.Unload</code> (<a href="https://issuetracker.unity3d.com/issues/activity-has-leaked-serviceconnection-errors-when-calling-application-dot-unload">1091255</a>)</p></li>
<li><p>Android: Fixed <code>Android Screen.safeArea</code> coordinate system to be in screen space.</p></li>
<li><p>Android: Fixed <code>Application.Unload</code> sometimes crashing on Android (<a href="https://issuetracker.unity3d.com/issues/android-application-dot-unload-causes-a-crash-after-multiple-openings-within-native-android-app">1093574</a>)</p></li>
<li><p>Android: Fixed <code>GrabPass</code> when using linear rendering on Android (<a href="https://issuetracker.unity3d.com/issues/android-object-becomes-brighter-when-grabpass-is-used-and-color-space-is-set-to-linear">1088699</a>)</p></li>
<li><p>Android: Fixed <code>RenderTextureFormat ARGB2101010</code> when using Vulkan on Adreno</p></li>
<li><p>Android: GPU Instanced mesh renders with artifacts on Adreno 630 devices (<a href="https://issuetracker.unity3d.com/issues/android-cube-using-displacement-pixel-map-is-not-rendered-or-rendered-with-artifacts-on-adreno-630-devices">1079627</a>)</p></li>
<li><p>Android: Improved performance of <strong>Cubemap</strong> convolution on Mali GPUs (<a href="https://issuetracker.unity3d.com/issues/vr-android-very-poor-performance-on-galaxy-s8">989820</a>)</p></li>
<li><p>Android: Linker errors print to console when using il2cpp.</p></li>
<li><p>Android: Refactored and improved Android device detection and selection during builds (<a href="https://issuetracker.unity3d.com/issues/android-retrying-build-on-authorized-android-device-which-was-unauthorized-when-starting-the-build-still-doesnt-build">1102133</a>)</p></li>
<li><p>Android: Touch and mouse position's y-value is inverted in the native backend instead of managed code in the new input system</p></li>
<li><p>Android: <code>Keyboard.onTextInput</code> and <code>Keyboard.onIMECompositionChange</code> correctly calls for physical and virtual keyboard events</p></li>
<li><p>Animation: Fixed a crash in the avatar configurator when a faulty bone was selected after AutoMap. (1075651)</p></li>
<li><p>Animation: Fixed a crash when a cycle occurs in an animation graph. (<a href="https://issuetracker.unity3d.com/issues/playables-crash-on-cyclic-graphs">792020</a>)</p></li>
<li><p>Animation: Fixed a crash when opening the Animator window from a bad Animator Controller setup. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-if-using-a-specific-animator-controller-on-play-mode-when-opening-animator-window">1080436</a>)</p></li>
<li><p>Animation: Fixed a crash when the Animation window previewed a disabled GameObject. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-with-mecanim-setvaluemask-when-enabling-animation-keyframe-recording-mode">1125266</a>, 1127071)</p></li>
<li><p>Animation: Fixed a crash when the animator changed the bindings of the next animator. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-with-unityengine-animation-setgenericfloatpropertyvalues-when-switching-timeline-with-constrains">1099988</a>)</p></li>
<li><p>Animation: Fixed an issue where additive animations would build up values when other layers were not writing (<a href="https://issuetracker.unity3d.com/issues/empty-animatorcontroller-on-animator-used-by-playables-breaks-layer-blending">1094706</a>, 1127817)</p></li>
<li><p>Animation: Fixed an issue where AnimationClip.empty always returns true when Animation Type is set to Legacy. (<a href="https://issuetracker.unity3d.com/issues/when-animation-type-is-set-to-legacy-animation-clip-could-not-be-loaded-from-assetbundle-in-build">1061700</a>)</p></li>
<li><p>Animation: Fixed an issue where querying clips in partially-loaded Override Controllers would crash (<a href="https://issuetracker.unity3d.com/issues/crash-in-animatoroverridecontroller-getoriginalclip-when-using-an-indexer-operator-to-access-an-animation-clip">1118196</a>, 1127823)</p></li>
<li><p>Animation: Fixed an issue where the Animation window opened when an AnimationClip was double-clicked. (<a href="https://issuetracker.unity3d.com/issues/double-clicking-animation-clip-does-not-open-animation-editor-window">1058422</a>)</p></li>
<li><p>Animation: Fixed an issue with AnimationStreamSource.PreviousInputs when used with humanoid characters. (1102231)</p></li>
<li><p>Animation: Fixed an issue with frame rounding in the Animation window. (1101186)</p></li>
<li><p>Animation: Fixed an issue with the animator that occurred after instantiation. (<a href="https://issuetracker.unity3d.com/issues/animator-first-frame-of-animator-isnt-updated-by-playablegraph-after-being-instantiated">995978</a>)</p></li>
<li><p>Animation: Fixed an issue with [burstcompile] not working on animation jobs.</p></li>
<li><p>Animation: Fixed erroneous range when changing orders of sprite keyframes in AnimationClip (1076068)</p></li>
<li><p>Asset Import: Added a fix to properly assign the Diffuse Color when a HDRP/Lit materical is generated froma FBX standard material in HDRP projects. (<a href="https://issuetracker.unity3d.com/issues/hdrp-material-imported-with-model-doesnt-preserve-original-base-color-and-set-texture">1087977</a>, 1114076)</p></li>
<li><p>Asset Import: Changed the icon of the Assets generated using ScriptedImporters to match the icon of other model files.</p></li>
<li><p>Asset Import: Clamped the global scale in ModelImporter to at most 10 digits. (<a href="https://issuetracker.unity3d.com/issues/editor-unity-crashes-when-the-fbx-adam-scale-factor-set-to-value-having-20-digits-or-above">1082327</a>)</p></li>
<li><p>Asset Import: Fix Missing Avatar assignement in older projects (<a href="https://issuetracker.unity3d.com/issues/missing-avatar-assignement-in-a$-mecanim-gdc2013-sample-project">1107242</a>)</p></li>
<li><p>Asset Import: Fixed an issue where importing FBX files with skinned meshes and with Index Format set to 16-bit produced corrupt data and/or errors. (<a href="https://issuetracker.unity3d.com/issues/bone-related-errors-and-animation-issues-when-importing-fbx-with-index-format-set-to-16bit">1126943</a>, 1139690)</p></li>
<li><p>Asset Import: Fixed an issue with <code>ModelImporter</code> where imported materials had no textures assigned in HDRP projects.</p></li>
<li><p>Asset Import: Fixed error when selecting multiple fbx with different Material settings. Multi-selection is not supported on this panel. (<a href="https://issuetracker.unity3d.com/issues/buildexternalobjectscache-throws-nullreferenceexception-when-inspecting-multiple-fbx-assets-at-once">1118475</a>, 1121738)</p></li>
<li><p>Asset Import: Fixed import of Blender files with Blender 2.80. (<a href="https://issuetracker.unity3d.com/issues/blender-2-dot-8-files-not-compatible-with-unity">1115353</a>, 1140789)</p></li>
<li><p>Asset Import: Fixed issue where the Model Importer <strong>Use File Scale</strong> property did not display the multiple different values checkbox in multiple selection.</p></li>
<li><p>Asset Import: Fixed Sprite asset references are missing after upgrading (<a href="https://issuetracker.unity3d.com/issues/sprite-asset-references-are-missing-after-upgrading">1102809</a>)</p></li>
<li><p>Asset Import: Made changes so that ProjectBrowser icons refresh correctly when the Model Importer is applied.</p></li>
<li><p>Asset Import: Made changes to prevent the use of a previously created avatar in the AvatarCopy field of the ModelImporter Rig panel.</p></li>
<li><p>Audio: Added a slider for Cutoff Frequency in the Audio High Pass Filter component. (<a href="https://issuetracker.unity3d.com/issues/audio-high-pass-filter-component-has-no-slider">818332</a>, 1131466)</p></li>
<li><p>Audio: Fixed an issue in the profiler where the time spent collecting audio data depended on the number of audio clips with loaded audio data. (<a href="https://issuetracker.unity3d.com/issues/profiler-dot-collectaudiostats-time-ms-is-very-high-when-preload-audio-data-is-enabled-on-many-audio-files">1086988</a>)</p></li>
<li><p>Audio: Fixed an issue where the Edit key option displayed incorrect parameters in the Curve editor. (713681)</p></li>
<li><p>Audio: Fixed an issue with calling AudioSource.GetSpatializerFloat or AudioSource.SetSpatializerFloat before an AudioSource was played.</p></li>
<li><p>Audio: Fixed an issue with importing short audio files that caused importer errors. (882227)</p></li>
<li><p>Audio: Fixed the tree view for Audio Mixer groups in the Output object selector. (<a href="https://issuetracker.unity3d.com/issues/audio-output-groups-are-not-shown-with-a-tree-structure-but-as-a-flat-list-in-output-group-object-selector">1010156</a>, 1131468)</p></li>
<li><p>Build Pipeline: Added a fix so failed builds are not treated as "successful".</p></li>
<li><p>Build Pipeline: Added a fix to unload asset bundles before building a player or other asset bundles. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-with-cachedwriter-write-when-building-project-with-missing-project-id">1081760</a>)</p></li>
<li><p>Build Pipeline: Added a fixed to allow the <strong>Scripting Define Symbols</strong> line in <strong>Player Settings</strong> to be reverted with the Undo command. (<a href="https://issuetracker.unity3d.com/issues/scripting-define-symbols-line-does-not-change-when-using-undo-command">1083481</a>)</p></li>
<li><p>Build Pipeline: Fix rare data corruption when building asset bundles with LZMA compression.</p></li>
<li><p>Build Pipeline: Fixed an issue where <code>PlayerSettings.applicationIdentifier</code> would not return the identifier for the active build target when editing settings for a different build target. (<a href="https://issuetracker.unity3d.com/issues/playersettings-dot-applicationidentifier-reports-incorrect-value">1041443</a>)</p></li>
<li><p>Build Pipeline: Fixed an object ordering indeterminism issue in the results returned by ContentBuildInterface.PrepareScene</p></li>
<li><p>Build Pipeline: Removed duplicate mono folder in Mac standalone builds. Also removed around 500 kb of unnecessary data from builds.</p></li>
<li><p>Compute: Vulkan/Metal/OpenGL: compute shader compilation optimizations (1022026)</p></li>
<li><p>DX12: Fixed crash related to memory allocation issues when using a camera with the <strong>Depth</strong> or <strong>Don't Clear</strong> flags. (<a href="https://issuetracker.unity3d.com/issues/dx12-crash-with-memory-allocation-issues-when-using-a-camera-with-the-depth-or-dont-clear-flags">969582</a>)</p></li>
<li><p>DX12: Fixed exclusive fullscreen always reverting to windowed fullscreen.</p></li>
<li><p>DX12: Fixed issue where test runner crashed while running tests containing RenderTexture instantiation from the command prompt. (1015725)</p></li>
<li><p>Editor: Added <strong>Main Menu/</strong> prefix to main menu commands displayed in the Shortcuts Manager Command list with <strong>Category</strong> set to <strong>All Unity Commands</strong>.</p></li>
<li><p>Editor: Added a fix for consistent logfile option handling for all desktop platforms, the Editor, and the Player. This improves the handling of edge cases and scenarios with logfile parameter. (<a href="https://issuetracker.unity3d.com/issues/command-line-logfile-with-no-parameters-outputs-to-screen-on-os-x-but-not-on-windows">900754</a>, <a href="https://issuetracker.unity3d.com/issues/after-opening-and-building-project-in-the-appdata-slash-locallow-folder-appear-two-new-folders-with-and-and-dot-escaped-characters">960012</a>, 1068907)</p></li>
<li><p>Editor: Added a fix so that items can be activated with space bar input in the Linux Editor inspector. (<a href="https://issuetracker.unity3d.com/issues/linux-editor-the-inspector-does-not-take-space-bar-input">1061975</a>)</p></li>
<li><p>Editor: Added a fix so that selecting <strong>Open</strong> on the <strong>Context Menu</strong> performs actions on folders. (1079852)</p></li>
<li><p>Editor: Added a fix to disallow naming Assembly definitions as predefined assembly names. (<a href="https://issuetracker.unity3d.com/issues/typeloadexception-is-thrown-when-highlighting-a-script-and-reflectiontypeloadexception-is-thrown-when-entering-play-mode">1081704</a>)</p></li>
<li><p>Editor: Added a fix to improve performance when deserializing uint64 values from text serialized assets.</p></li>
<li><p>Editor: Added a fix to stop Android release builds from forwarding network traffic to device. (<a href="https://issuetracker.unity3d.com/issues/android-slash-linux-unable-to-forward-network-traffic-to-device">1090170</a>)</p></li>
<li><p>Editor: Added a horizontal scrollbar to Preset Manager settings. (<a href="https://issuetracker.unity3d.com/issues/assigned-presets-are-not-visible-in-preset-manager-when-settings-window-is-shrinks-horizontally">1087969</a>)</p></li>
<li><p>Editor: Added button to clear binding in Keys preferences.</p></li>
<li><p>Editor: Added diagnostic warning icon under text. (1093938)</p></li>
<li><p>Editor: Added missing size and style to <code>CacheFontForText</code>. (1087730)</p></li>
<li><p>Editor: Added null protection when iterating using <code>ExtendVisibleAsChild</code>. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-on-extendvisibleaschild-when-onsceneguidelegate-references-a-method-which-calls-handleutility-dot-pickgameobject">1083254</a>)</p></li>
<li><p>Editor: Bring back Imported Header for AssetImporter component (<a href="https://issuetracker.unity3d.com/issues/imported-object-header-is-missing">1104131</a>)</p></li>
<li><p>Editor: Corrected a typo in the tooltip for the 2D/3D switch in the Scene view control bar. (<a href="https://issuetracker.unity3d.com/issues/2d-slash-3d-toggle-button-in-scene-view-has-toggled-mispelled-as-togggled">1048139</a>)</p></li>
<li><p>Editor: Creating a new material while an item is selected in scene could yield "IndexOutOfRange" errors (1128724, 1131937)</p></li>
<li><p>Editor: Debug Internal inspector no displays all properties (1109531, 1118915)</p></li>
<li><p>Editor: EditorWindow notification is rendered behind UI elements when the elements are instantiated from UXML (<a href="https://issuetracker.unity3d.com/issues/editorwindow-notifaction-is-rendered-behind-ui-elements-when-the-elements-are-instantiated-from-uxml">1116944</a>, 1131498)</p></li>
<li><p>Editor: Enabled editing a script field when the script is missing. (<a href="https://issuetracker.unity3d.com/issues/object-picker-cannot-be-used-to-assign-missing-script-when-having-missing-script-component-in-inspector-window">1117624</a>, 1126282)</p></li>
<li><p>Editor: Fix a crash when using hyperlink tag without the closing tag. (<a href="https://issuetracker.unity3d.com/issues/crash-on-textrenderingprivate-nativetextgenerator-getrectinstring-when-opening-a-project-with-textmeshpro-plugin">1113075</a>, 1135091)</p></li>
<li><p>Editor: Fix an issue where asset store window could turn blank when redocking (<a href="https://issuetracker.unity3d.com/issues/linux-editor-asset-store-window-turns-blank-after-docking-and-undocking">1100443</a>)</p></li>
<li><p>Editor: Fix an issue where custom editors with scrollviews would be squashed in the inspector window (1103342)</p></li>
<li><p>Editor: Fix Crash on dragging Script to component in inspector (1124734, 1131934)</p></li>
<li><p>Editor: Fix crash on editor window destruction</p></li>
<li><p>Editor: Fix crash while setting version control mode to visible meta files (<a href="https://issuetracker.unity3d.com/issues/unity-editor-crashes-on-gameobject-setsupportedmessagesdirty-when-changing-version-control-mode-to-visible-meta-files">1128867</a>, 1132704)</p></li>
<li><p>Editor: Fix editor crash while saving a scene with missing script. (1111432, 1115552)</p></li>
<li><p>Editor: Fix Exceptions raised and Inspector is broken after user removes a component from multiselected GameObjects (1126938, 1131936)</p></li>
<li><p>Editor: Fix extra shift being present in some contextual menu shortcuts in Timeline.</p></li>
<li><p>Editor: Fix Inspector Window's uxml contains strings that are no longer localized (1122433, 1131929)</p></li>
<li><p>Editor: Fix issue where EditorApplication.quitting callbacks were not being called in batchmode</p></li>
<li><p>Editor: Fix keypad period and delete for input fields (Linux)</p></li>
<li><p>Editor: Fix menu shortcuts before first menu show on Linux</p></li>
<li><p>Editor: Fix selecting items with duplicate names in test hierarchy of Test Runner window (<a href="https://issuetracker.unity3d.com/issues/test-runner-hierarchy-doesnt-correctly-select-an-item">987587</a>, 1140566)</p></li>
<li><p>Editor: Fix SettingsWindow layout breaks from 18.3 (<a href="https://issuetracker.unity3d.com/issues/project-settings-window-breaks-a-custom-layout-after-upgrading-to-2019-dot-1-and-2019-dot-2-when-the-layout-was-made-in-2018-dot-3">1124696</a>, 1129237)</p></li>
<li><p>Editor: Fix: Copying and pasting selected text copies an additional letter that is not selected (<a href="https://issuetracker.unity3d.com/issues/copying-and-pasting-selected-text-that-has-a-parenthesis-at-the-end-still-includes-the-even-if-its-not-selected">1107289</a>, 1114040)</p></li>
<li><p>Editor: Fixed a Null Reference Exception thrown when multiple Assembly Definition Assets are added to the same folder. (1120826, 1120982)</p></li>
<li><p>Editor: Fixed an incorrect <code>Input.keyCode</code> value when keyboard layout changes on macOS.</p></li>
<li><p>Editor: Fixed an incorrect <code>Input.keyCode</code> value when using  the Dvorak - QWERTY Command keyboard layout on macOS. (<a href="https://issuetracker.unity3d.com/issues/macos-hotkeys-are-mapped-as-standard-dvorak-shortcuts-and-ignore-system-preferences-when-using-dvorak-qwerty-keyboard-layout">1103558</a>, 1131774)</p></li>
<li><p>Editor: Fixed an issue in the Shortcuts Manager Commmand list where right-clicking an entry did not select that entry, and displayed the context menu from the previously selected entry. (<a href="https://issuetracker.unity3d.com/issues/shortcut-manager-right-clicking-a-command-does-not-select-it">1110804</a>, 1120069)</p></li>
<li><p>Editor: Fixed an issue in the Shortcuts Manager where changes were not saved to the profile when users unassigned shortcuts or reset shortcuts to their default settings.</p></li>
<li><p>Editor: Fixed an issue in the Shortcuts Manager where selecting a new category from the Category list did not reset the selected entry in the Command list. (1104559, 1120070)</p></li>
<li><p>Editor: Fixed an issue in the Shortcuts Manager where users could assign reserved modifier keys (<strong>Shift</strong>, <strong>Ctrl/Cmd</strong>, and so on) to commands. (<a href="https://issuetracker.unity3d.com/issues/shortcut-manager-you-can-assign-commands-to-the-modifier-keys-by-dragging-and-dropping-via-the-keyboard-layout-panel">1110790</a>, 1120071)</p></li>
<li><p>Editor: Fixed an issue on Linux where the progress bar window changed size repeatedly while creating or opening a project. (1100653)</p></li>
<li><p>Editor: Fixed an issue on macOS where entering Unity keyboard shortcuts while a project was loading crashed Unity. (<a href="https://issuetracker.unity3d.com/issues/osx-holding-cmd-plus-while-creating-slash-opening-project-opens-preferences-window-before-editor-is-opened">1004336</a>)</p></li>
<li><p>Editor: Fixed an issue on macOS where launching the Editor with <code>-batchmode</code> as the first argument caused a crash. (<a href="https://issuetracker.unity3d.com/issues/macos-unity-crashes-with-segmentation-fault-11-or-bus-error-10-when-launching-with-batchmode-followed-by-projectpath">1059028</a>)</p></li>
<li><p>Editor: Fixed an issue on macOS where opening and closing utility windows caused a crash. (<a href="https://issuetracker.unity3d.com/issues/editor-crash-on-clicking-animation-curve-created-using-uielement-for-mac-osx">1046287</a>)</p></li>
<li><p>Editor: Fixed an issue where artifacts appeared in Sprite sheets when users clicked drop-down menus in the Inspector. (<a href="https://issuetracker.unity3d.com/issues/sprite-sheet-grid-artifact-appears-when-clicking-drop-down-menus">1055868</a>)</p></li>
<li><p>Editor: Fixed an issue where assets from Unity's built-in resources could not be loaded by <code>AssetDatabase.LoadAllAssetsAtPath</code>. (<a href="https://issuetracker.unity3d.com/issues/using-loadallassetsatpath-to-load-the-paths-does-not-load-objects-stored-at-paths-and-leaves-the-the-expecting-object-empty">1104874</a>)</p></li>
<li><p>Editor: Fixed an issue where calling <code>RenderTexture.ReleaseTemporary</code> twice for same texture caused a crash. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-with-renderbuffermanager-textures-garbagecollect-when-calling-rendertexture-dot-releasetemporary-twice">1091561</a>)</p></li>
<li><p>Editor: Fixed an issue where changing the shortcut for a main-menu item using the Shortcuts Manager would not update the menu with the new shortcut.</p></li>
<li><p>Editor: Fixed an issue where closing the Editor while the Asset Store or Services window was loading caused a crash. (<a href="https://issuetracker.unity3d.com/issues/closing-unity-while-a$-or-services-tab-is-loading-crashes-editor">1024048</a>)</p></li>
<li><p>Editor: Fixed an issue where creating a parameter for an Animation condition after creating the condition sometimes threw a NullReferenceException. (<a href="https://issuetracker.unity3d.com/issues/previously-empty-conditions-for-an-animation-transition-cannot-be-updated-after-creating-the-first-parameter">1127789</a>, 1131535)</p></li>
<li><p>Editor: Fixed an issue where drag and dropping a texture onto a <strong>GameObject</strong> in the Scene created a material with no texture in HDRP projects.</p></li>
<li><p>Editor: Fixed an issue where dragging a GameObject to the position directly after a child object in the Hierarchy window inserted the dragged object in the wrong position. (<a href="https://issuetracker.unity3d.com/issues/game-object-is-not-inserted-correctly-in-hierarchy-window-when-placed-after-child-object">1069565</a>)</p></li>
<li><p>Editor: Fixed an issue where empty <strong>Editor Settings</strong> password fields were returning asterisks for empty fields. (<a href="https://issuetracker.unity3d.com/issues/vcs-password-field-still-shows-up-as-not-empty-after-deleting-password">958884</a>)</p></li>
<li><p>Editor: Fixed an issue where empty strings caused <code>TextField</code> to crash. (<a href="https://issuetracker.unity3d.com/issues/shortcut-manager-an-assertion-failure-occurs-when-entering-a-user-profile-name-with-multiple-spaces-at-the-beginning">1107172</a>)</p></li>
<li><p>Editor: Fixed an issue where having multiple GameObjects selected and using the Component context menu to call <code>GameObject.DestroyImmediate</code> on Components crashed Unity. (<a href="https://issuetracker.unity3d.com/issues/crash-on-scripting-scriptingwrapperfor-when-destroying-component-with-gameobject-dot-destroyimmediate-after-re-adding-it">1056115</a>)</p></li>
<li><p>Editor: Fixed an issue where keyboard shortcuts for main menu commands would not work if the key combination included the <strong>Space</strong> key. (<a href="https://issuetracker.unity3d.com/issues/menuitem-functions-with-assigned-shortcuts-involving-the-space-key-are-not-called-when-the-corresponding-shortcut-is-pressed">1106151</a>, 1120068)</p></li>
<li><p>Editor: Fixed an issue where layouts were saved and loaded incorrectly. (1078964)</p></li>
<li><p>Editor: Fixed an issue where lines were not drawn when using <code>Handles.DrawDottedLine</code> in a custom inspector. (<a href="https://issuetracker.unity3d.com/issues/handles-dot-drawdottedline-does-nothing-when-used-in-the-editor">954149</a>)</p></li>
<li><p>Editor: Fixed an issue where modifying an Avatar's  <strong>Per-Muscle Settings</strong> caused a NullReferenceException. (<a href="https://issuetracker.unity3d.com/issues/null-reference-exception-on-tweaking-the-pre-muscle-settings-of-a-avatar-when-scene-view-is-in-focus">1068870</a>)</p></li>
<li><p>Editor: Fixed an issue where searching for an asset in the Project window, and then renaming it via the context menu would not work if the Project widow was using the one-column layout. (<a href="https://issuetracker.unity3d.com/issues/renaming-asset-while-searching-in-the-project-view-does-not-work-in-one-column-layout">1073306</a>)</p></li>
<li><p>Editor: Fixed an issue where selecting assets in the last row of the Project window made the scroll bar blink. (<a href="https://issuetracker.unity3d.com/issues/project-window-scrollbar-disappears-after-selecting-assets-from-the-bottom-row">1076266</a>)</p></li>
<li><p>Editor: Fixed an issue where SerializedProperty children were not visible when put in a horizontal group. (<a href="https://issuetracker.unity3d.com/issues/serializedproperty-children-not-visible-when-put-in-horizontal-group">1068811</a>)</p></li>
<li><p>Editor: Fixed an issue where switching platforms and recompiling scripts did not clear compile errors from the Console. (1078935)</p></li>
<li><p>Editor: Fixed an issue where Test Runner console messages could overlap the test menu. (<a href="https://issuetracker.unity3d.com/issues/test-runner-result-console-tab-is-transparent">1094277</a>)</p></li>
<li><p>Editor: Fixed an issue where the <strong>Add Component</strong> menu is not displayed in some cases. (<a href="https://issuetracker.unity3d.com/issues/add-component-shortcut-ctrl-plus-shift-plus-a-no-longer-works">1104169</a>)</p></li>
<li><p>Editor: Fixed an issue where the <strong>Undo</strong> command did not work after setting/resetting the layout to <strong>Default</strong>. (<a href="https://issuetracker.unity3d.com/issues/windows-unable-to-use-undo-if-editor-layout-is-set-to-default">1068662</a>)</p></li>
<li><p>Editor: Fixed an issue where the color picker ignored copied hex codes when they included the number sign (#) prefix. (<a href="https://issuetracker.unity3d.com/issues/color-picker-ignores-the-color-hex-code-when-copied-with">804231</a>)</p></li>
<li><p>Editor: Fixed an issue where the Editor recommended updating to an earlier version.</p></li>
<li><p>Editor: Fixed an issue where the Editor used the OS locale. (<a href="https://issuetracker.unity3d.com/issues/windows-editor-uses-os-locale-settings-i-dot-e-commas-instead-of-dots-in-float-values-with-net-4-dot-6">1089361</a>)</p></li>
<li><p>Editor: Fixed an issue where the Game view layout was not changing when the application was paused. (<a href="https://issuetracker.unity3d.com/issues/editor-maximized-game-view-doesnt-get-minimized-after-disabling-the-maximize-on-play-and-toggling-pause-button">1104417</a>)</p></li>
<li><p>Editor: Fixed an issue where the IME input was causing text duplication in the Editor. (1117859, 1117878)</p></li>
<li><p>Editor: Fixed an issue where the Inspector did not display GUI label tooltips. (1057359)</p></li>
<li><p>Editor: Fixed an issue where the Layers drop-down menu in the Inspector did not list grouped Layers properly. (<a href="https://issuetracker.unity3d.com/issues/creating-layer-groups-with-the-slash-symbol-creates-multiple-groups-with-the-same-name-containing-only-a-single-layer">1068422</a>)</p></li>
<li><p>Editor: Fixed an issue where the mouse position was offset in the Game view when using IMGUI. (1097051)</p></li>
<li><p>Editor: Fixed an issue where the preview icon for the Material Preset flickered. (<a href="https://issuetracker.unity3d.com/issues/presets-material-preset-preview-icon-flickers-when-viewing-a-material-preset-in-the-inspector">1099296</a>)</p></li>
<li><p>Editor: Fixed an issue where the RuntimeInitializeOnLoadMethodAttribute was ignored inside player-only code blocks (such as when using #if !UNITY_EDITOR) and inside player-only  assemblies created with an Assembly Definition. (<a href="https://issuetracker.unity3d.com/issues/conditional-compilation-problem-with-runtimeinitializeonloadmethod">922692</a>, 1071599)</p></li>
<li><p>Editor: Fixed an issue where the Scene icon was not updated after the png file was changed. (1084630)</p></li>
<li><p>Editor: Fixed an issue where <code>LoadSceneAsync</code> would not trigger subscribed callbacks on load. (<a href="https://issuetracker.unity3d.com/issues/after-loading-editorapplication-dot-loadlevelasyncinplaymode-the-subscribed-completed-event-doesnt-triggers">1049526</a>)</p></li>
<li><p>Editor: Fixed an issue with overriden main menu shortcuts.</p></li>
<li><p>Editor: Fixed an issue with project update from 2017.4 to 2019.1. (<a href="https://issuetracker.unity3d.com/issues/2019-dot-1-a-fatal-error-is-thrown-after-updating-a-project-from-2017-dot-4-to-2019-dot-1">1099240</a>)</p></li>
<li><p>Editor: Fixed arrow keys logging errors in editor log slowing down editor.</p></li>
<li><p>Editor: Fixed button style is not correct in texture inspector.</p></li>
<li><p>Editor: Fixed clutch shortcut stuck if key is released while editor is not in focus.</p></li>
<li><p>Editor: Fixed crash when building player with Services enabled, and using .NET 3.5. (<a href="https://issuetracker.unity3d.com/issues/deployment-management-editor-crashes-when-building-a-project-for-any-platform-with-services-enabled">1103349</a>)</p></li>
<li><p>Editor: Fixed custom layout menu items getting out of sync with Shortcut Manager. (<a href="https://issuetracker.unity3d.com/issues/assigning-shortcuts-to-editor-layout-not-working">1097041</a>)</p></li>
<li><p>Editor: Fixed CustomEditorAttributes scanning order (1108536)</p></li>
<li><p>Editor: Fixed default shortcuts for Cut/Copy/Paste/Select All/Undo/Redo menu items not usable for other commands in Shortcuts window.</p></li>
<li><p>Editor: Fixed Editor crashes on <code>HomeWindowHandler::LearnTabOpenedCallback</code> while opening Project or entering Play Mode. (<a href="https://issuetracker.unity3d.com/issues/wild-crash-editor-crashes-on-homewindowhandler-learntabopenedcallback-while-opening-project-or-entering-play-mode">1090455</a>)</p></li>
<li><p>Editor: Fixed game view dimensions to address issue where <code>Camera.ScreenPointToRay</code> returned slightly offset coordinates when drawing the Ray from the main camera to the mouse position. (<a href="https://issuetracker.unity3d.com/issues/box-colliders-position-has-a-slight-offset-when-using-a-raycast-to-hit-it">1083316</a>)</p></li>
<li><p>Editor: Fixed generic menu issue related to incorrect grouping of child menu item's when parent menu item contains space(" ") as its last character. (<a href="https://issuetracker.unity3d.com/issues/guicontent-items-in-genericmenu-containing-spaces-before-the-slash-symbol-are-not-grouped-correctly">1116792</a>, 1129941)</p></li>
<li><p>Editor: Fixed Hiding objects in the scene view does not work with SRP (<a href="https://issuetracker.unity3d.com/issues/hiding-objects-in-the-scene-view-does-not-work-with-srp">1105161</a>)</p></li>
<li><p>Editor: Fixed Hierarchy view hover issues (1131017, 1131031)</p></li>
<li><p>Editor: Fixed invalid screen parameters when multiple game views instances are active. (<a href="https://issuetracker.unity3d.com/issues/game-view-does-not-scale-correctly-on-resizing-it-when-multiple-game-views-are-open-in-the-editor">1110671</a>, 1131010)</p></li>
<li><p>Editor: Fixed issue where holding arrow keys sometimes caused editor to stop redrawing.</p></li>
<li><p>Editor: Fixed issue where Unity would crash when the Save Assets dialog box displayed before exiting the Editor. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-when-saving-animation-clip-with-verify-saving-assets-setting-checked">1062146</a>)</p></li>
<li><p>Editor: Fixed key down events dispatched twice if not used.</p></li>
<li><p>Editor: Fixed menu items forgetting their default shortcut bindings.</p></li>
<li><p>Editor: Fixed performance issues when using the Test Runner for Projects with many assemblies.</p></li>
<li><p>Editor: Fixed performance regressions related to UIElements moving out of experimental (1103391)</p></li>
<li><p>Editor: Fixed scene visibility column hiding the search path of the hierarchy (<a href="https://issuetracker.unity3d.com/issues/hierarchy-search-path-display-is-obscured-by-the-visibility-icons-area-when-searching">1114645</a>, 1122512)</p></li>
<li><p>Editor: Fixed serialization issue in which MonoBehaviours with no script would cause a crash while saving the Scene. (<a href="https://issuetracker.unity3d.com/issues/crash-in-output-l-when-saving-the-scene">925313</a>)</p></li>
<li><p>Editor: Fixed standard macOS text editing key bindings inside web views.</p></li>
<li><p>Editor: Fixed state propagation when a VisualElement is added to a hierarchy. (1093728)</p></li>
<li><p>Editor: Fixed strip debug info from release editor. (1070559, 1126323)</p></li>
<li><p>Editor: Fixed text fields in Save Scenes dialog window not being navigable using arrow keys.</p></li>
<li><p>Editor: Fixed the <strong>Verify Save Assets</strong> option to work in the Linux Editor. (<a href="https://issuetracker.unity3d.com/issues/linux-editor-files-are-not-saved-if-verify-saving-assets-is-enabled">957853</a>)</p></li>
<li><p>Editor: Fixed unhideable material's render queue for Scriptable Render Pipelines using Shader Graph. (1108637)</p></li>
<li><p>Editor: Generated  for <code>mcs.rsp</code> references. (1053714)</p></li>
<li><p>Editor: Made changes so that Unity Test Runner won't execute the PrebuildSetup code for ignored playmode tests or tests disabled on the selected platform.</p></li>
<li><p>Editor: Made the <code>VisualElementAsset</code> id field deterministic. (1100451)</p></li>
<li><p>Editor: Made <code>MinMaxslider</code> <code>dragElement</code> position absolute. Previously it was relative, which broke layouts. (1090242)</p></li>
<li><p>Editor: Make sure that modules depeding on disabled modules are also disabled</p></li>
<li><p>Editor: Make sure that we bail out immediately when dragging a preset on a UnityObject that already has the dragged component (<a href="https://issuetracker.unity3d.com/issues/endlayoutgroup-error-is-thrown-when-adding-preset-of-an-already-added-component">1074291</a>)</p></li>
<li><p>Editor: Minimize button("-") does not work for Scene, Game, Hierarchy etc. windows on Mac. (<a href="https://issuetracker.unity3d.com/issues/editor-minimize-button-doesnt-work-for-scene-game-hierarchy-etc-windows-on-mac">1117896</a>, 1118033)</p></li>
<li><p>Editor: Null reference fix for semversion (<a href="https://issuetracker.unity3d.com/issues/scripting-console-spammed-with-errors-when-version-defines-saved">1129026</a>, 1141029)</p></li>
<li><p>Editor: Prefab Component overrides now remain visible in the Inspector after a domain reload. (1102487)</p></li>
<li><p>Editor: Recover from modal window being closed using the X button (windows)</p></li>
<li><p>Editor: Removed an extra separator from the context menu in the Hierarchy window. (1080882)</p></li>
<li><p>Editor: Removed cursor warning when calling <code>Cursor.SetCursor</code> on a texture loaded from an asset bundle. (<a href="https://issuetracker.unity3d.com/issues/cursor-dot-setcursor-prints-invalid-texture-used-warning-when-the-texture-is-loaded-with-assetbundles">1028350</a>)</p></li>
<li><p>Editor: Removed duplicate for Rider path discovery on Linux.</p></li>
<li><p>Editor: Renamed the <strong>Child Controls Size</strong> property to <strong>Control Child Size</strong> in the <strong>Horizontal Layout Group</strong> and <strong>Vertical Layout Group</strong> components. (<a href="https://issuetracker.unity3d.com/issues/horizontal-layout-group-and-vertical-layout-group-child-controls-size-fields-are-mislabelled">1090329</a>)</p></li>
<li><p>Editor: Renamed the UI <strong>Transparency Priority</strong> to <strong>Renderer Priority</strong> in the <strong>MeshRenderer</strong> component.</p></li>
<li><p>Editor: Show imported components on Model asset prefabs again (was hidden because we don't want to show components for normal prefab assets)</p></li>
<li><p>Editor: The <strong>Strip Engine Code</strong> setting is now available only in Player pettings for platforms that support stripping unused code.</p></li>
<li><p>Editor: The number of available glyphs is now a criterion in fallback font selection. The falback font system selects the matching font with the most available glyphs. (<a href="https://issuetracker.unity3d.com/issues/linux-editor-symbol-characters-not-shown-slash-entered-in-text-fields">1090134</a>)</p></li>
<li><p>Editor: Unity now displays an error message when recent projects contain an invalid or missing <code>ProjectSettings.txt</code> file. (<a href="https://issuetracker.unity3d.com/issues/merge-conflict-in-projectversion-dot-txt-causes-unable-to-parse-file-error-on-any-project-opened">1002683</a>)</p></li>
<li><p>Editor: Update OSX container window floating window icons (1102525)</p></li>
<li><p>Editor: Update toolbox handling for rider path detection</p></li>
<li><p>Editor: Updated Windows splash screen.</p></li>
<li><p>GI: Fix crash on application exit when GPU lightmapper openCL context is lost.</p></li>
<li><p>GI: Fixed a bug where a probeset with completely overlapping positions would cause the deringing settings array to become shifted.</p></li>
<li><p>GI: Fixed an issue in the GPU Lightmapper that stabilizes noise when iterating on lighting.</p></li>
<li><p>GI: Fixed an issue where GICache errors were thrown when baking Terrain with trees having deringing enabled on the light probes. (<a href="https://issuetracker.unity3d.com/issues/gicache-errors-are-thrown-when-baking-terrain-with-trees-having-deringing-enabled-on-the-light-probes">1100362</a>)</p></li>
<li><p>GI: Fixed an issue where running <code>UpdateMaterials</code> was causing performance issues.</p></li>
<li><p>GI: Fixed an issue where supersampling was introducing interdeterministic results with direct samples. It now uses round-robin sampling between supersamples. (<a href="https://issuetracker.unity3d.com/issues/plm-supersampling-renders-indeterministic-results-with-direct-samples">936693</a>)</p></li>
<li><p>GI: Fixed an issue where the bake could split out "Assertion failed on expression: 'm_NumInstanceTransforms == m_NumInstanceLODGroups'" and produce incorrect results for Scenes with LODs in them. It could occur when entering avatar configuration when baking or making sweeping changes to instances contained in the Scene. (1102752)</p></li>
<li><p>GI: Fixed an issue where the lightmap preview window didn't get cleared when lightmaps were removed. (<a href="https://issuetracker.unity3d.com/issues/ui-per-renderer-lightmap-preview-is-not-cleared-after-disabling-gi-and-rebaking">1082621</a>)</p></li>
<li><p>GI: Fixed an issue where the Reflection Probes progress bar didn't get cleared when cancelling.</p></li>
<li><p>GI: Fixed an issue where Unity would try to load incompatible serialized lighting data from cache and print out "Failed to load '***' because it was serialized with a newer version of Unity. (Has a higher SerializedFile version).". (1112513, 1129760)</p></li>
<li><p>GI: Fixed file reading errors with hashID.ghd while baking lighting. (<a href="https://issuetracker.unity3d.com/issues/plm-failed-reading-errors-with-hashid-dot-ghd-while-baking">1047087</a>)</p></li>
<li><p>GI: Fixed hashing issue when writing out AO textures for PLM.</p></li>
<li><p>GI: Fixed issue where the UV Overlap preview didn't display after a manual bake. (<a href="https://issuetracker.unity3d.com/issues/ui-baked-uv-overlap-mode-isnt-loaded-after-selecting-it-in-the-lightmap-preview-window">1087688</a>)</p></li>
<li><p>GI: Fixed the API documentation for <code>Lightmapping.Clear</code> and <code>Lightmapping.ClearLightingDataAsset</code>.</p></li>
<li><p>GI: Fixed the Baked UV Charts debug lightmap. (1078533)</p></li>
<li><p>GI: Fixed the Editor log outputs ''d3d11: failed to lock buffer [HASH].'' while baking using CPU PLM. (<a href="https://issuetracker.unity3d.com/issues/editor-log-outputs-d3d11-failed-to-lock-buffer-0000021b7f5b94e0-of-size-85222-0x8007000e-dot-while-baking-using-cpu-plm">1095976</a>)</p></li>
<li><p>GI: Fixed the indirect intensity slider in the Progressive Lightmapper so that it now also affects indirect probe lighting. (<a href="https://issuetracker.unity3d.com/issues/indirect-intensity-slider-has-no-effect-on-lightprobes-in-progressive-backends">1060939</a>)</p></li>
<li><p>GI: GPU Lightmapper, fix number of bounces (was doing two extra).</p></li>
<li><p>GI: GPU Lightmapper, use interpolated vertex normal when shading bounce light, rather than plane normal.</p></li>
<li><p>GI: GPU Lightmapper: Ensure OpenCL kernel are recompiled on Nvidia even when only the include files changes.</p></li>
<li><p>GI: GPU Lightmapper: For baking default is to select the same graphic hardware as the editor.</p></li>
<li><p>GI: Improved sampling when baking lightmaps in scenes with translucent objects. (<a href="https://issuetracker.unity3d.com/issues/cpu-plm-correlation-artifacts-when-using-semi-transparent-surfaces">1132640</a>, 1133463)</p></li>
<li><p>GI: Renamed "Auto Bake On/Off" to "Auto Generate Lighting On/Off" in the app bar.</p></li>
<li><p>Graphics: Added a fix so HDR Mode in Graphics Settings is respected in LWRP. (<a href="https://issuetracker.unity3d.com/issues/lwrp-graphics-settings-hdr-mode-is-being-ignored">1104140</a>)</p></li>
<li><p>Graphics: Added extra validation for RT volumeDepth. (1096019)</p></li>
<li><p>Graphics: Assert '0 == m_CurrentBuiltInBindMask' in HDRP test when Async Shader Compilation is ON (1117989, 1122369)</p></li>
<li><p>Graphics: Choose the correct occlusion camera when occlusion visualization is turned on</p></li>
<li><p>Graphics: Do not render the skybox in the scene view if using an SRP as the SRP will handle the skybox render.</p></li>
<li><p>Graphics: DX11: Fix for not being able to bind a a 2D Render Texture with a slice index of -1.</p></li>
<li><p>Graphics: Fix crash when stripping Umbra module on platforms supporting native code stripping. (1116487, 1118313)</p></li>
<li><p>Graphics: Fix crash when usign DrawMeshInsted with SRP batcher enabled (1122017, 1122357)</p></li>
<li><p>Graphics: Fix for postprocessing and instanced stereo rendering only a white screen in LWRP (<a href="https://issuetracker.unity3d.com/issues/xr-graphics-lwrp-postprocess-when-using-post-process-effects-with-lwrp-and-instancing-stereo-rendering-only-a-white-screen">1100898</a>)</p></li>
<li><p>Graphics: Fix issue with argument buffer not being bound properly (only a subset of the view was bound)</p></li>
<li><p>Graphics: Fix memory leak in Mac threaded texture creation (1126615, 1127347)</p></li>
<li><p>Graphics: Fixed a crash that happened when creating a <code>Texture2DArray</code> with a YUY2 <code>TextureFormat</code>. (<a href="https://issuetracker.unity3d.com/issues/macos-creating-a-texture2darray-with-a-yuy2-textureformat-crashes-the-editor">1094777</a>)</p></li>
<li><p>Graphics: Fixed a Frame Debugger texture tooltip, so it shows correct dimension info for 3D textures.</p></li>
<li><p>Graphics: Fixed a performance issue that prevented GPU drivers from utilizing internal texture compression. (Not applicable to RenderTexture.)</p></li>
<li><p>Graphics: Fixed a warning message in the Editor for Mac OS with an Android build target, where a warning would show up for decompressing ETC textures. (1115543, 1120074)</p></li>
<li><p>Graphics: Fixed an issue that would deplete memory when trying to compile Shaders that uses a self-referencing macro. (<a href="https://issuetracker.unity3d.com/issues/mobile-os-restarts-because-of-high-memory-usage-when-compiling-shaders-for-opengles2">1104217</a>)</p></li>
<li><p>Graphics: Fixed an issue where activated second display is not rendering when running the project in Standalone (<a href="https://issuetracker.unity3d.com/issues/activated-second-display-is-not-rendering-when-running-the-project-in-standalone">1099190</a>)</p></li>
<li><p>Graphics: Fixed an issue where copying raw depth buffers caused a crash. (<a href="https://issuetracker.unity3d.com/issues/copying-directional-light-depthmap-in-rawdepth-mode-crashes-unity-editor">1040591</a>)</p></li>
<li><p>Graphics: Fixed an issue where Frame Debugger was showing bad keywords when connected to a standalone Player. (<a href="https://issuetracker.unity3d.com/issues/frame-debugger-does-not-display-all-additional-shader-keywords-when-debugging-a-built-player">1070614</a>)</p></li>
<li><p>Graphics: Fixed an issue where Inspector Previews were using black cubemaps for environment reflection. (<a href="https://issuetracker.unity3d.com/issues/metallic-objects-are-very-dark-in-the-preview-window">1039018</a>)</p></li>
<li><p>Graphics: Fixed an issue where MeshTopology.Quads generated a draw call that uses 3 point patches instead of 4. (<a href="https://issuetracker.unity3d.com/issues/meshtopology-dot-quads-generates-a-draw-call-that-uses-3-point-patches-instead-of-4-point">1078885</a>)</p></li>
<li><p>Graphics: Fixed an issue where Reflection Probes weren't rebaking in the Editor after changes were made to the Shader code of the renderers used in the baked Reflection Probes. (<a href="https://issuetracker.unity3d.com/issues/srp-template-template-geometry-is-hot-pink">1020358</a>)</p></li>
<li><p>Graphics: Fixed an issue where the <strong>Package Manager</strong> UI was not rendering correctly on GLES2. (<a href="https://issuetracker.unity3d.com/issues/package-manager-window-is-rendering-blobs-instead-of-letters-for-lwrp-in-glsl2">1108286</a>, 1117897)</p></li>
<li><p>Graphics: Fixed an issue with Animator preview not rendering grids in Sciptable Render Pipelines. (1044281)</p></li>
<li><p>Graphics: Fixed async readback when using Vulkan.</p></li>
<li><p>Graphics: Fixed blicking when rendering at native resolution in fullscreen with OpenGL on Windows (<a href="https://issuetracker.unity3d.com/issues/graphic-errors-slash-glitches-when-running-player-fullscreen">1039035</a>)</p></li>
<li><p>Graphics: Fixed crash that infrequently occurred when instancing properties were absent from the MaterialPropertyBlock object sent to DrawMeshInstanced calls. (1115627, 1124733)</p></li>
<li><p>Graphics: Fixed Crash when calling Graphics.ExecuteCommandBuffer() if CommandBuffer.SetShadowSamplingMode() is used before it (<a href="https://issuetracker.unity3d.com/issues/crash-when-calling-graphics-dot-executecommandbuffer-if-commandbuffer-dot-setshadowsamplingmode-is-used-before-it">1102773</a>, 1124728)</p></li>
<li><p>Graphics: Fixed crash when user-created RT has an unsupported sample count. (1095433)</p></li>
<li><p>Graphics: Fixed Fog settings not being preserved for the additively loaded Scenes. (<a href="https://issuetracker.unity3d.com/issues/lighting-settings-mix-settings-from-two-different-scenes-in-multi-scene-editing">1024864</a>)</p></li>
<li><p>Graphics: Fixed graphics format that should support random writes. (<a href="https://issuetracker.unity3d.com/issues/opengl-rendertexture-dot-create-failed-format-unsupported-for-random-writes-rgba4-unorm-7">1096000</a>)</p></li>
<li><p>Graphics: Fixed loading of compressed textures with incomplete mipmap chains. (<a href="https://issuetracker.unity3d.com/issues/opengl-unity-can-only-read-1-mipmap-from-dot-ktx-textures-when-the-texture-was-compressed-using-etc">1045189</a>, 1115580)</p></li>
<li><p>Graphics: Fixed memory leak in metal threaded texture creation (1126615, 1127347)</p></li>
<li><p>Graphics: Fixed memory overwrites in the DX11 render target setting code.</p></li>
<li><p>Graphics: Fixed problem so that the correct SubShader is selected when rendering with the Editor Camera.</p></li>
<li><p>Graphics: Fixed RenderTexture asset UI preventing to select the color format (<a href="https://issuetracker.unity3d.com/issues/render-texture-inspector-enum-broken">1115203</a>, 1115204)</p></li>
<li><p>Graphics: Fixed RenderTexture asset UI to lose selected format data when the selected format is not supported. (<a href="https://issuetracker.unity3d.com/issues/render-texture-enum-can-lose-users-data">1116500</a>, 1116501)</p></li>
<li><p>Graphics: Fixed scene view rendering default skybox when SRP is enabled (<a href="https://issuetracker.unity3d.com/issues/sceneview-renders-legacy-skybox-when-custom-rp-is-active">1076246</a>)</p></li>
<li><p>Graphics: Fixed scissor/viewport handling when used with Dynamic Resolution feature.</p></li>
<li><p>Graphics: Fixed sRGB RenderTexture failing to be created when enableRandomWrite is on (1115223, 1115226)</p></li>
<li><p>Graphics: Fixed support for 32 bit vertex index buffer sub-mesh on dx11 during SRP batching. (<a href="https://issuetracker.unity3d.com/issues/srp-batcher-doesnt-support-32-bit-vertex-index-buffer-mesh-on-dx11">1117383</a>, 1120326)</p></li>
<li><p>Graphics: Fixed Texture.allowThreadedTextureCreation to correctly allow control of which thread textures are created on. (1131041, 1132127)</p></li>
<li><p>Graphics: Fixed Vulkan-Enabled GPU skinning for blend shapes. (<a href="https://issuetracker.unity3d.com/issues/2019-dot-1-vulkan-directx-11-using-models-with-blend-shapes-causes-the-skinning-to-happen-on-the-cpu-instead-of-the-gpu">1134323</a>, 1138973)</p></li>
<li><p>Graphics: Improved RenderTexture asset UI to store the user requested format (<a href="https://issuetracker.unity3d.com/issues/render-texture-inspector-enum-broken">1115203</a>, 1115204)</p></li>
<li><p>Graphics: Made changes to explicitly disallow the destroying of temporary render textures. (<a href="https://issuetracker.unity3d.com/issues/calling-destroyimmediate-after-rendertexture-dot-releasetemporary-causes-the-crash-in-renderbuffermanager-textures-gettempbuffer">1070564</a>)</p></li>
<li><p>Graphics: Made changes to skip shadow lights and shadow casters culling when shadows are disabled. (<a href="https://issuetracker.unity3d.com/issues/osx-shadows-disabling-shadows-in-quality-settings-doesnt-stop-shadow-caster-culling">1072624</a>)</p></li>
<li><p>Graphics: Optimizes single-colored ambient probe updates. (<a href="https://issuetracker.unity3d.com/issues/the-rendersettings-dot-ambientlight-color-is-changing-inconsistenly-when-using-color-dot-lerp">1115645</a>, 1136076)</p></li>
<li><p>Graphics: Reinstated support for reading Terrain Brush Textures. (1102243)</p></li>
<li><p>Graphics: Renamed <strong>Renderer Priority</strong> to <strong>Priority</strong> in the <strong>Mesh Renderer</strong> component.</p></li>
<li><p>Graphics: Vulkan: Disabled error messages when attempting to draw with missing bindings</p></li>
<li><p>Graphics: Vulkan: Fixed a race condition between updating ComputeBuffers from script and rendering from them within Graphics jobs.</p></li>
<li><p>Graphics: Vulkan: Fixed crash when rendering reflection probes on Android</p></li>
<li><p>Graphics: Vulkan: Fixed crash with certain shaders</p></li>
<li><p>Graphics: Vulkan: Fixed debug marker locations in RenderDoc trace</p></li>
<li><p>Graphics: Vulkan: Fixed various issues with FPS Samplegame</p></li>
<li><p>Graphics: (1086957)</p></li>
<li><p>IL2CPP: Add support for building with Xcode 10 and the macOS 10.14 SDK.</p></li>
<li><p>IL2CPP: Avoid using managed exceptions during time zone initialization. This cause cause crashes on some platforms. (1100856, 1117453)</p></li>
<li><p>IL2CPP: Correct a build error when script debugging is enabled for a project with no user scripts. (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1082185">1082185</a>)</p></li>
<li><p>IL2CPP: Fixed IL2CPP build failing if Visual Studio 2019 is installed on the machine.</p></li>
<li><p>IL2CPP: Fixed invoking IEnumerable.GetEnumerator method on COM objects that implemenet Windows.Foundation.Collections.IIterable interface. (<a href="https://issuetracker.unity3d.com/issues/invoking-system-dot-collections-dot-ienumerable-dot-getenumerator-fails-on-native-objects-that-dont-implement-ibindablevector-interface">878766</a>, 1127105)</p></li>
<li><p>IL2CPP: Fixes a compilation error that can occur when the debugger is enabled but there are no source files specified in the symbol data. (1078027)</p></li>
<li><p>IL2CPP: Fixes an issue with UnsafeUtility.SizeOf() crashing IL2CPP when called with an enum type.</p></li>
<li><p>IL2CPP: Fixing an unhandled exception in IL2CPP. Adding support for pointer types when executing an initobj instruction.</p></li>
<li><p>IL2CPP: Prevent a compilation error in generated C++ code when the ldtoken opcode is used in some cases.</p></li>
<li><p>IL2CPP: Prevent a possible crash when a list of generic or nullable types with a field that is a struct with explicit layout is reallocated. (1121969, 1122739)</p></li>
<li><p>IL2CPP: Prevent finalizer from being incorrect injected for COM types.</p></li>
<li><p>IL2CPP: Support the AttributeType property of of the TypeInfo object.</p></li>
<li><p>Input: Added a fix in the new input system to correctly set and get sampling frequencies for sensors on iOS and Android platforms.</p></li>
<li><p>iOS: Added a fix so <code>DISABLE_TOUCH_DELAYS</code> does not create a warning on iOS 12 devices. (<a href="https://issuetracker.unity3d.com/issues/ios-disable-touch-delays-define-causes-a-warning-on-ios-12-devices">1087337</a>)</p></li>
<li><p>iOS: Added a fixed so <code>Screen.allowedOrientations</code> is not updated every frame. (1103167)</p></li>
<li><p>iOS: Fix warnings related to launch image when building for iOS in Xcode 10 (<a href="https://issuetracker.unity3d.com/issues/ios-game-crashes-when-forcing-portrait-upside-down-orientation-on-iphone-xs-slash-xs-max">1085602</a>)</p></li>
<li><p>iOS: Fixed a Lighweight Render Pipeline crash on several SoCs (<a href="https://issuetracker.unity3d.com/issues/ios-lwrp-execution-of-the-command-buffer-was-aborted-error-is-being-thrown-when-launching-template-project">1098913</a>)</p></li>
<li><p>iOS: Fixed an issue where a full screen movie reset after the app was minimized (<a href="https://issuetracker.unity3d.com/issues/handheld-dot-playfullscreenmovie-movie-resets-when-minimizing-and-maximizing-the-application">840951</a>)</p></li>
<li><p>iOS: Fixed an issue where changing <code>Screen.Orientation</code> on some iOS devices would not update the variable that holds the current orientation state (<a href="https://issuetracker.unity3d.com/issues/ios-screen-dot-orientation-returns-wrong-value-on-some-devices-when-specific-orientation-was-forced-after-few-states">1088729</a>)</p></li>
<li><p>iOS: Fixed an issue where particles were being rendered over non-transparent objects in a Low Poly Strategy Prototyper project (<a href="https://issuetracker.unity3d.com/issues/metal-ios-some-particles-are-being-rendered-over-non-transparent-objects-in-low-poly-strategy-prototyper-project">1107546</a>, 1122520)</p></li>
<li><p>iOS: Fixed crash on startup on 32bit devices using oldish iOS (<a href="https://issuetracker.unity3d.com/issues/ios-bad-access-exception-thrown-on-deploying-build-on-devices-with-ios-version-10-or-lower">1109610</a>, 1117891)</p></li>
<li><p>iOS: Fixed DiscardContents and GrabIntoRenderTexture interop on Metal (<a href="https://issuetracker.unity3d.com/issues/ios-depth-texture-in-commandbuffer-and-customized-depth-of-field-shader-will-damage-the-rendertexture">1082159</a>)</p></li>
<li><p>iOS: Fixed incorrect <code>Screen.safeArea</code> on plus sized iPhones (<a href="https://issuetracker.unity3d.com/issues/ios-a-bunch-of-launch-image-warnings-are-thrown-when-building-for-ios-in-xcode-10">1087954</a>)</p></li>
<li><p>iOS: Fixed issues with reporting orientation when autorotating and tweaked enabled orientations (<a href="https://issuetracker.unity3d.com/issues/ios-screen-dot-orientation-returns-upsidedown-value-after-using-screen-dot-autorotatetoportrait-when-device-is-in-portrait-mode">1075839</a>, <a href="https://issuetracker.unity3d.com/issues/ios-unity-rendering-in-wrong-screen-orientation-after-auto-rotation-on-ios-using-screen-dot-orientation">1075855</a>)</p></li>
<li><p>iOS: Fixed UnauthorizedAccessException when building for iOS (1108549)</p></li>
<li><p>iOS: Uncoupled the accelerometer from the gyroscope (<a href="https://issuetracker.unity3d.com/issues/ios-the-accelerometer-stops-working-when-disabling-the-gyroscope-in-build">1085244</a>)</p></li>
<li><p>iOS: <code>Gamepad.startButton</code> works correctly. The iOS <code>startButton</code> (or Menu button) only reports a down event and an up event is simulated immediately after to simulate a click. (<a href="https://issuetracker.unity3d.com/issues/ios-gamepad-gamepad-dot-current-dot-startbutton-doesnt-return-expected-value">1093829</a>, 1132630)</p></li>
<li><p>iOS: <code>Keyboard.onTextInput</code> and <code>Keyboard.onIMECompositionChange</code> correctly calls for physical and virtual keyboard events.</p></li>
<li><p>iOS: <code>Pen.tilt</code> values are correctly returned in the new input system (<a href="https://issuetracker.unity3d.com/issues/ios-pen-tilt-dot-x-is-centered-on-1-dot-5-and-goes-to-0-when-tilting-both-left-and-right">1093816</a>, 1132629)</p></li>
<li><p>Kernel: Fixed a temp job warning in C# jobs when the job was executing for longer than one frame.</p></li>
<li><p>Linux: Added a fix for touchpad sced an issue where touchpad scrolling was too sensitive in the Linux Editor. (<a href="https://issuetracker.unity3d.com/issues/linux-scroll-sensitivity-of-touchpad-is-too-high">1073152</a>)</p></li>
<li><p>Linux: Added a fix to allow Linux and Mac launch the BugReport crash handler when a SIGABRT is sent. (<a href="https://issuetracker.unity3d.com/issues/linux-editor-forcecrash-forcedcrashcategory-dot-abort-not-being-caught-by-crash-reporter">1074324</a>)</p></li>
<li><p>Linux: Fix crash on Editor startup when using -force-vulkan (<a href="https://issuetracker.unity3d.com/issues/unity-cannot-start-if-force-vulkan-is-used-in-linux">1109529</a>, 1123925)</p></li>
<li><p>Linux: Fix using multiple identical webcams on Linux (<a href="https://issuetracker.unity3d.com/issues/linux-when-using-2-identical-webcams-with-same-name-second-webcam-does-not-return-frames">1115884</a>, 1123759)</p></li>
<li><p>Linux: Fixed an Editor windows repaint bug in Ubuntu 16.04. (1107716)</p></li>
<li><p>Linux: Fixed an issue where tabs were incorrectly processed twice. (<a href="https://issuetracker.unity3d.com/issues/linux-editor-android-key-creation-dialog-tabbing-skips-every-other-field">1080441</a>)</p></li>
<li><p>Linux: Fixed annoying "'Unity' is not responding" message on Linux. (<a href="https://issuetracker.unity3d.com/issues/gnome-pops-application-is-not-responding-dialog-behind-fullscreen-player-preventing-further-interaction-with-the-player">1072712</a>, 1122090)</p></li>
<li><p>Linux: Fixed issue with keyboard input not being captured by the Game view when in Play mode (<a href="https://issuetracker.unity3d.com/issues/linux-focus-cannot-be-properly-gained-on-play-mode-making-keyboard-input-switch-screens">1109908</a>, 1118063)</p></li>
<li><p>Linux: Fixed Linux Editor executable being much larger than it used to be (1.2GB instead of ~350MB)</p></li>
<li><p>Linux: Fixed progress bar freeze when sprite assets have invalid names (<a href="https://issuetracker.unity3d.com/issues/editor-freeze-when-creating-tile-assets-with-special-characters-star-in-the-name">1106232</a>, 1115875)</p></li>
<li><p>Linux: Strong Input lag when locking cursor and using mouse with 1000hz polling rate (<a href="https://issuetracker.unity3d.com/issues/linux-strong-input-lag-when-using-standart-asset-pack-and-mouse-with-1000hz-pooling-rate">1023587</a>, 1118295)</p></li>
<li><p>Linux: Unity Editor and Build dips in Frame count when scrolling with the Mouse Wheel (1066760, 1117507)</p></li>
<li><p>Linux: [Linux][Editor]Fixed Shift+tab selects previous window instead of previous tabbed element. (1107323, 1117698)</p></li>
<li><p>Lumin: Fixed an issue where the minimum platform API level in a custom manifest was not being respected.</p></li>
<li><p>LWRP: Fixed RenderTexture sRGB flag set incorrectly. (<a href="https://issuetracker.unity3d.com/issues/lwrp-scene-darkens-when-using-antialiasing-in-gamma-lighting-if-hdr-is-not-on">1133874</a>, 1136097)</p></li>
<li><p>Mobile: Added support for Bluetooth headphones' microphone for both Android and iOS (<a href="https://issuetracker.unity3d.com/issues/mobile-support-for-bluetooth-headphones-microphone">946201</a>)</p></li>
<li><p>Mobile: Fixed Ambient Occlusion in PostProcessing v2 (<a href="https://issuetracker.unity3d.com/issues/ios-post-processing-ambient-occlusion-does-not-work">1059893</a>)</p></li>
<li><p>Mobile: Fixed an issue where reflection was distorted when using baked reflection probes (<a href="https://issuetracker.unity3d.com/issues/mobile-reflection-is-distorted-when-using-baked-reflection-probes">1114605</a>, 1117116)</p></li>
<li><p>Mobile: Fixed an issue where the <code>TargetFPS</code> and <code>vSyncCount</code> has no effect on the FPS (<a href="https://issuetracker.unity3d.com/issues/razer-phone-targetfps-and-vsynccount-has-no-effect-on-the-actual-fps">1078663</a>, 1136554)</p></li>
<li><p>Mobile: Fixed Standard shader artifacts on mobiles</p></li>
<li><p>Mobile: Fixed the Crunch decoder to avoid access out of vector boundaries (<a href="https://issuetracker.unity3d.com/issues/ios-player-crashes-at-decode-alpha-selectors-etc-when-decoding-crunched-etc-texture">983436</a>, 1140135)</p></li>
<li><p>Multiplayer: Fixed issue where the unet hlapi package was not being automatically added to old projects opened in 2019.1, bumped version in editor manifest to 1.0.1 as well</p></li>
<li><p>OSX: Fix Empty Project builds for Mac/Win/Linux Standalone contain extra ~4MB of doc .xml files (1112215, 1125589)</p></li>
<li><p>OSX: Fixed an issue building the Mac Editor using customer source code distributions</p></li>
<li><p>OSX: Fixed an issue where Unity would crash if the resolution was set to invalid values via script. (<a href="https://issuetracker.unity3d.com/issues/mac-standalone-after-set-the-width-and-height-to-be-0-player-quits-then-crashes">1070915</a>)</p></li>
<li><p>OSX: Fixed GPU selector always being disabled. (<a href="https://issuetracker.unity3d.com/issues/mac-cant-change-graphics-device-to-use-in-standalone-built-project">1055634</a>)</p></li>
<li><p>OSX: Fixed issue where the option "Use Metal Editor" did not display on some versions of Unity. (1094058)</p></li>
<li><p>OSX: Fixed occasional crash when using Camera (be it FaceTime or coming from UnityRemote) (<a href="https://issuetracker.unity3d.com/issues/ios-unity-remote-5-getting-assertion-failed-on-expression-uploaddstformat-equals-equals-format-errors-on-ios-device">1101944</a>, <a href="https://issuetracker.unity3d.com/issues/graphics-crash-when-running-a-particular-scene">1110670</a>, 1115830, 1116526)</p></li>
<li><p>OSX: Fixed the icon at 128x128 being corrupt in macOS build (<a href="https://issuetracker.unity3d.com/issues/macos-deployment-the-icon-at-128x128-is-corrupt-in-macos-build">1038984</a>, 1132657)</p></li>
<li><p>OSX: Metal: Unity applications now correctly reported as "Requires High Perf GPU" in Activity Monitor (1055912)</p></li>
<li><p>Package Manager: A "Failed to fetch versions information" error would be displayed in Package Manager window for all unknown packages.</p></li>
<li><p>Package Manager: Add a warning message if you disable a package and that causes dependencies to also be disabled.</p></li>
<li><p>Package Manager: Add information to compiler errors explaining if a package has been disabled as a dependency of another package</p></li>
<li><p>Package Manager: Add information to info messages for disabled components in the inspector explaining if a package has been disabled as a dependency of another package</p></li>
<li><p>Package Manager: Added opening offline documentation when the online documentation is not accessible.</p></li>
<li><p>Package Manager: Fix an issue that prevented specific native plugins to be correctly identified the second time a project was loaded.</p></li>
<li><p>Package Manager: Fix an issue where packages would not be found because the project configured registry URL ended with an extraneous slash.</p></li>
<li><p>Package Manager: Fix Closing the 'Reset Packages to Defaults' confirmation window still resets the Packages. (<a href="https://issuetracker.unity3d.com/issues/closing-the-reset-packages-to-defaults-confirmation-window-still-resets-the-packages">1134754</a>, 1137060)</p></li>
<li><p>Package Manager: Fix for upgraded projects that use XR or Timeline and have disabled modules (<a href="https://issuetracker.unity3d.com/issues/package-manager-ui-does-not-show-up-and-there-are-compilation-errors-when-upgrading-projects-to-2019-dot-1">1111566</a>, 1115043)</p></li>
<li><p>Package Manager: Fix imcompatible packages showing up in the list of packages to install (<a href="https://issuetracker.unity3d.com/issues/package-manager-window-is-empty-when-package-manager-ui-package-is-updated">1066979</a>)</p></li>
<li><p>Package Manager: Fix incorrect text with the update button when a package is being installed (1124632, 1139328)</p></li>
<li><p>Package Manager: Fix Package Manager timeouts when opening a project inside a closed network.</p></li>
<li><p>Package Manager: Fix Package Manager UI refreshes the package list when entering play mode (<a href="https://issuetracker.unity3d.com/issues/package-manager-ui-refreshes-the-package-list-when-entering-play-mode">1135815</a>, 1135840)</p></li>
<li><p>Package Manager: Fixed a <strong>Package Manager</strong> error displaying "Input string was not in a correct format" when using Locales with the <code>,</code> number separator (<a href="https://issuetracker.unity3d.com/issues/package-manager-throws-system-dot-formatexception-input-string-was-not-in-a-correct-format-errors-when-using-pl-pl-locale">1131566</a>, 1139270)</p></li>
<li><p>Package Manager: Fixed an issue where an error message appeared when dragging the Packages folder in to the Favorites section. (<a href="https://issuetracker.unity3d.com/issues/move-of-a-savedfilter-has-invalid-input-errors-appear-when-dragging-packages-folder-on-to-favorite-section-in-project-window">1084176</a>)</p></li>
<li><p>Package Manager: Fixed an issue where native plugins inside a package would not get resolved on OSX</p></li>
<li><p>Package Manager: Made changes so packages that aren't installed are shown in package manager window. (<a href="https://issuetracker.unity3d.com/issues/not-installed-packages-are-shown-in-package-manager-window">1098870</a>)</p></li>
<li><p>Package Manager: Made changes so that packages, which are imported as dependencies for other packages, are not shown in Package Manager UI. (<a href="https://issuetracker.unity3d.com/issues/packages-that-are-imported-as-dependencies-for-other-packages-are-not-shown-in-package-manager-ui">1057210</a>)</p></li>
<li><p>Package Manager: The Asset Database refresh could hang when removing or updating the version of an installed package.</p></li>
<li><p>Package Manager: Use SemVer in core packages instead of 0.0.0-builtin</p></li>
<li><p>Particles: Apply collisions during the initial simulation step of newly spawned particles. (<a href="https://issuetracker.unity3d.com/issues/some-particles-fail-to-collide-with-the-object-when-spawning-a-lot-of-particles-at-once">1082981</a>, 1120773)</p></li>
<li><p>Particles: Apply the Simulation Speed modifier to the initial simulation step when spawning new particles (<a href="https://issuetracker.unity3d.com/issues/particle-systems-height-slash-distribution-in-play-mode-is-affected-when-changing-the-simulation-speed">1111729</a>, 1122166)</p></li>
<li><p>Particles: Fixed Prefabs with Sub emitters that have emit probability of 0 by default.</p></li>
<li><p>Particles: Opening a legacy Prefab with a ParticleSystem in Prefab Mode: ParticleSystemRenderer component is now correctly hidden in the Inspector.</p></li>
<li><p>Particles: Recompute particle bounds after executing a C# Job. (<a href="https://issuetracker.unity3d.com/issues/iparticlesystemjob-bounding-box-is-not-recalculated-after-the-job">1116569</a>, 1120793)</p></li>
<li><p>Physics: CharacterController will now ignore Rigidbodies that have their collision detection turned off. (<a href="https://issuetracker.unity3d.com/issues/charactercontroller-doesnt-respect-rigidbody-dot-detectcollisions-set-to-false">984035</a>)</p></li>
<li><p>Physics: Ensured that 2D trigger/collision exit callbacks occur when destroying a GameObject inside a 2D trigger/collision callback. (<a href="https://issuetracker.unity3d.com/issues/ontriggerexit2d-not-triggered-when-collider-gameobject-is-destroyed-from-another-colliders-ontriggerenter2d">1057320</a>)</p></li>
<li><p>Physics: Ensured that 2D trigger/collision exit callbacks occur when disabling a GameObject or 2D collider component. (<a href="https://issuetracker.unity3d.com/issues/ontriggerexit2d-is-not-being-triggered-when-disabling-other-gameobject-with-a-trigger">1071700</a>)</p></li>
<li><p>Physics: Fixed a crash in the 2D physics manager on iOS upon start-up when Physics2D package is disabled. (<a href="https://issuetracker.unity3d.com/issues/ios-crash-in-initialize-at-physicsmanager2d-before-the-splash-screen">1080899</a>)</p></li>
<li><p>Physics: Fixed a crash that occurred when adding a MeshCollider without CookingOptions.CookForFasterSimulation. Fixed by PhysX 3.4 Upgrade. (<a href="https://issuetracker.unity3d.com/issues/adding-meshcollider-meshes-without-cookingoptions-dot-cookforfastersimulation-causes-crash-in-physx-subsortquick-sort4">1041838</a>)</p></li>
<li><p>Physics: Fixed a spelling issue in the Physics settings (renamed Default Max Angular Speed). (<a href="https://issuetracker.unity3d.com/issues/default-max-angular-speed-spelling-mistake-in-physics-settings">1104527</a>, 1127096)</p></li>
<li><p>Physics: Fixed an issue that occurred when copying and pasting cloth component values. (<a href="https://issuetracker.unity3d.com/issues/pasting-cloth-component-values-causes-scene-view-to-break">975495</a>)</p></li>
<li><p>Physics: Fixed PhysicsScene.SphereCast having a set of default parameters that's inconsistent with the other queries. (<a href="https://issuetracker.unity3d.com/issues/all-arguments-are-mandatory-for-int-physicsscene-dot-spherecast-even-though-they-shouldnt-be">1096382</a>)</p></li>
<li><p>Physics: Fixed poor performance of self and inter collision gizmos for cloth. (<a href="https://issuetracker.unity3d.com/issues/having-the-self-and-inter-collision-gizmos-visible-lowers-performance-significantly">963985</a>)</p></li>
<li><p>Physics: Fixed <code>Rigidbody.AddExplosionForce</code> docs that were out of sync with code. (<a href="https://issuetracker.unity3d.com/issues/addexplosionforce-s-added-force-to-rigidbodys-velocity-is-not-proportional-to-explosion-position">1108989</a>, 1140551)</p></li>
<li><p>Physics: Made the bodies connected by <code>ConfigurableJoint</code> wake up when changing parameters, to match what happens when doing this in the Editor. (<a href="https://issuetracker.unity3d.com/issues/changing-the-linear-limit-of-a-configurable-joint-does-nothing-when-its-being-changed-by-the-script">1075514</a>, 1140550)</p></li>
<li><p>Physics: Physics Fix "Selected Object Info" in Physics Debug View being expanded incorrectly (<a href="https://issuetracker.unity3d.com/issues/selected-object-info-foldout-is-misbehaving-in-the-physics-debugger">1122474</a>, 1134269)</p></li>
<li><p>Physics: RelativeJoint2D now correctly handles rotation. (<a href="https://issuetracker.unity3d.com/issues/physics2d-relativejoint2d-should-support-driven-rotations-as-per-box2d">1103365</a>)</p></li>
<li><p>Physics: Stopped NullReferenceException due to sprite-snapping when dragging a Joint2D anchor when the same GameObject contains a SpriteRenderer without an assigned Sprite. (<a href="https://issuetracker.unity3d.com/issues/nullreferenceexception-when-moving-around-a-springjoint2d-with-a-rigidbody-reference-to-an-empty-sprite">1077680</a>)</p></li>
<li><p>Prefabs: Added localization to Overrides window and PrefabUtility dialogs.</p></li>
<li><p>Prefabs: Do not block saving a Prefab in Prefab Mode to a new Prefab when in Animation Mode</p></li>
<li><p>Prefabs: Don't include Importer Error Log in source prefab file when saving from PrefabMode</p></li>
<li><p>Prefabs: Fix handling of Transform replacement in Prefab instances and assets</p></li>
<li><p>Prefabs: Fix loosing selection of Prefab root in Prefab Mode after draggging script to Inspector.</p></li>
<li><p>Prefabs: Fix memory leak when calculating prefab dependencies during import.</p></li>
<li><p>Prefabs: More robust throwing of exceptions for invalid input to PrefabUtility apply and revert methods. (1090918)</p></li>
<li><p>Prefabs: Prefab Mode: Fix automatic UI reparenting to leave out the prefab itself when looking for a Canvas to render with</p></li>
<li><p>Prefabs: PrefabMode: For broken prefabs use the root that the PrefabImporter has chosen when opening the prefab file in Prefab Mode, other dangling roots are deleted.</p></li>
<li><p>Prefabs: Support reparenting prefab root in Awake and OnEnable when opening Prefab Mode.</p></li>
<li><p>Profiler: Fix ArgumentNullException thrown by "Show Related Object" pane of Profiler Window. (<a href="https://issuetracker.unity3d.com/issues/profiler-argumentnullexception-thrown-in-the-console-when-show-related-object-option-is-selected-for-a-sample">1090876</a>)</p></li>
<li><p>Profiler: Fixed an issue where Profiler stats was recording when profiling the Editor with runtime profiler API.</p></li>
<li><p>Profiler: Fixed issue with increased memory usage by the profiler for long-lasting background operations. (1094748)</p></li>
<li><p>SceneManager: Add 'Collapse All' functionality to the Hierarchy Window to easily collapse all rows in the Hierarchy. Added to the Hierarchy window context menu. (1137167, 1138476)</p></li>
<li><p>SceneManager: Fix SceneHierarchy throwing null ref exception in rare cases on LostFocus events. (1136536, 1138475)</p></li>
<li><p>SceneManager: Fix Unity hangs after dropping a parent transform into a SubScene below it. (1136535, 1138474)</p></li>
<li><p>Scripting: Added <code>System.Data.dll</code> in the references. (<a href="https://issuetracker.unity3d.com/issues/the-project-cant-be-compiled-because-library-targeting-net-standard-2-dot-0-doesnt-work">1075265</a>)</p></li>
<li><p>Scripting: Assigning a custom <code>Debug.logger.logHandler</code> now intercepts thrown exceptions. (<a href="https://issuetracker.unity3d.com/issues/assigning-a-custom-debug-dot-logger-dot-loghandler-doesnt-intercept-thrown-exceptions">753944</a>)</p></li>
<li><p>Scripting: Enabled empty assembly definition references and relaxed the need for a reference on an assembly. (<a href="https://issuetracker.unity3d.com/issues/compilation-errors-after-reimporting-the-project-that-has-an-assembly-definition-that-references-another-assembly-definitions">1130125</a>, 1136092)</p></li>
<li><p>Scripting: Fix compiler error reporting in Editor.log (1115012, 1115994)</p></li>
<li><p>Scripting: Fix potential crash when calling Editor.CreateEditor with a type that does not derive from UnityEditor.Editor. (1119535, 1126301)</p></li>
<li><p>Scripting: Fixed a bug where building players with "using alias" directives pointing to types in other assemblies would fail, if those types were not actually used.</p></li>
<li><p>Scripting: Fixed a crash where a whole hierarchy was destroyed when <code>GameObject</code> instantiated a new <code>GameObject</code> on the parent during an <code>OnDestroy</code> callback. (<a href="https://issuetracker.unity3d.com/issues/crash-when-instantiating-new-gameobject-with-the-parent-of-the-gameobject-that-is-being-destroyed-and-exiting-play-mode">1121506</a>, 1125293)</p></li>
<li><p>Scripting: Fixed an issue where the <code>originalProjection</code> variable in the <code>Camera.projectionMatrix</code> Scripting API example was not initialized. (<a href="https://issuetracker.unity3d.com/issues/errors-are-throw-when-using-documentation-example-of-camera-dot-projectionmatrix">1097500</a>)</p></li>
<li><p>Scripting: Fixed crash when adding multiple components of a disallowed type. (<a href="https://issuetracker.unity3d.com/issues/trying-to-add-two-same-script-components-with-disallowmultiplecomponent-via-test-causes-unity-to-crash">959136</a>)</p></li>
<li><p>Scripting: Fixed invalid UTF8 characters from imported assets. (<a href="https://issuetracker.unity3d.com/issues/copyright-symbol-c-causes-invalid-utf8-string-error-when-observing-scripts-inspector-window">1086920</a>, 1114945)</p></li>
<li><p>Scripting: Fixed issue where Unity couldn't stop <code>Coroutine</code> via <code>StopCoroutine()</code> if it had three or more nested yield return coroutines. (<a href="https://issuetracker.unity3d.com/issues/coroutine-cant-be-stopped-via-stopcoroutine-if-it-has-3-or-more-nested-yield-return-coroutines">1089467</a>)</p></li>
<li><p>Scripting: Fixes potential crash when an exception is thrown during domain unload (<a href="https://issuetracker.unity3d.com/issues/potential-crash-when-exception-is-raised-in-mono-domain-unload">879906</a>, 1115911)</p></li>
<li><p>Scripting: Made changes to disallow modifications of serialized data in <code>m_Component</code> on a GameObject. (<a href="https://issuetracker.unity3d.com/issues/the-editor-crashes-when-exiting-the-play-mode-in-the-specific-project">1022204</a>, <a href="https://issuetracker.unity3d.com/issues/crash-on-gameobject-isactive-when-calling-prefabutility-dot-instantiateprefab">1082089</a>)</p></li>
<li><p>Scripting: Make exception errors appear in Editor console when they're received from player. (<a href="https://issuetracker.unity3d.com/issues/debug-dot-logexception-messages-arent-shown-in-the-editors-console-when-the-player-is-connected-using-an-ip-address">1103744</a>, 1121783)</p></li>
<li><p>Scripting: NET_LEGACY is now only set when NET 2.0 or .NET 2.0 Subset profile is used.</p></li>
<li><p>Scripting: Small performance improvement to <code>Renderer.bounds</code>. We were doing an unnecessary call to GetComponent()</p></li>
<li><p>Scripting Upgrade: Fix crash when debugging with Rider (<a href="https://issuetracker.unity3d.com/issues/crash-on-clear-assembly-from-modifiers-when-entering-play-mode-from-rider-debug">1111226</a>, 1118829)</p></li>
<li><p>Scripting Upgrade: Fix GC performing unnecessary full collections when incremental GC is enabled (<a href="https://issuetracker.unity3d.com/issues/incremental-gc-doesnt-spread-collection-across-multiple-frames">1129037</a>, 1132628)</p></li>
<li><p>Scripting Upgrade: Fixed a crash from a method with too many variables. (<a href="https://issuetracker.unity3d.com/issues/allocating-too-many-variables-in-a-method-leads-to-a-crash">1103205</a>, 1128765)</p></li>
<li><p>Scripting Upgrade: Fixed a crash in <code>Marshal.PtrToStructure</code> with a generic struct. (<a href="https://issuetracker.unity3d.com/issues/if-marshal-dot-ptrtostructure-raises-an-exception-the-editor-crashes">1106422</a>, 1123902)</p></li>
<li><p>Scripting Upgrade: Fixed a crash when a delegate constructor was invoked with the NULL method. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-with-g-logv-when-entering-play-mode-with-active-flowcanvas-script">1091693</a>, 1123904)</p></li>
<li><p>Scripting Upgrade: Fixed a crash when the method has Task return type. (<a href="https://issuetracker.unity3d.com/issues/crash-on-mono-generic-class-get-class-when-function-has-task-return-type">1111048</a>, 1123903)</p></li>
<li><p>Scripting Upgrade: Fixed a hang from race condition in C# sockets on Windows. (<a href="https://issuetracker.unity3d.com/issues/streamreader-readline-stops-receiving-messages-after-the-server-hangs">1028819</a>, 1128764)</p></li>
<li><p>Scripting Upgrade: Fixed a hang when using Photon networking on Windows. (<a href="https://issuetracker.unity3d.com/issues/photon-unity-networking-messages-timeout-when-using-net-4-dot-x">1054137</a>, 1128761)</p></li>
<li><p>Scripting Upgrade: Fixed excessive garbage collection allocations when using TLS. (<a href="https://issuetracker.unity3d.com/issues/mono-net-4-dot-x-tls-1-dot-2-excessive-gc-usage-while-reading-from-tls-stream">1084800</a>, 1128767)</p></li>
<li><p>Scripting Upgrade: Fixed random crash on x86 Linux with TLS connections ("GCHandle value belongs to a different domain")</p></li>
<li><p>Scripting Upgrade: Fixed sizes for <code>System.Numerics</code> types. (<a href="https://issuetracker.unity3d.com/issues/system-dot-numerics-vector-sizes-are-all-16-bytes-instead-of-8-12-and-16-bytes">1118631</a>, 1123901)</p></li>
<li><p>Scripting Upgrade: Fixed the use of <code>DataContractJsonSerializer</code> with <code>UseSimpleDictionaryFormat</code> option enabled. (<a href="https://issuetracker.unity3d.com/issues/datacontractjsonserializer-usesimpledictionaryformat-doesnt-work-when-deserializing">1070667</a>, 1128766)</p></li>
<li><p>Scripting Upgrade: Fixed <code>GetThreadContext failed</code> assertion message on Windows. (<a href="https://issuetracker.unity3d.com/issues/gc-getthreadcontext-failed-crash-when-calling-gc-dot-collect-and-yielding-the-thread">1114668</a>, 1131234)</p></li>
<li><p>Shaders: Added more clean and useful editor logs on shader compiler crashes. (<a href="https://issuetracker.unity3d.com/issues/unity-displays-millions-of-lines-of-shader-source-in-editor-log-when-the-shader-compiler-crashes-during-builds">1097215</a>)</p></li>
<li><p>Shaders: Added zero-init appdata in the domain surface shader to avoid a compiler error about the out parameter not being fully initialized.</p></li>
<li><p>Shaders: Fixed issue where edge/inside tessellation factors were improperly handled by the metal shader compiler. (<a href="https://issuetracker.unity3d.com/issues/metal-edge-length-tessellation-throws-compilation-error-when-using-vertex-normal-on-the-vertex-function">1065883</a>)</p></li>
<li><p>Shaders: Fixed issue where the surface shader analysis step sometimes had missing inputs when keepalpha was specified. (<a href="https://issuetracker.unity3d.com/issues/two-pass-surface-shader-does-not-include-vertex-color-data-in-the-second-pass">864173</a>)</p></li>
<li><p>Shaders: Made Particles StandardSurface shader support gles2 again (<a href="https://issuetracker.unity3d.com/issues/gles2-particles-slash-standard-surface-shader-doesnt-render-on-devices">1103043</a>)</p></li>
<li><p>Shaders: The XR wireframe shader now works correctly with OpenGL and DirectX. (1022184, 1131099)</p></li>
<li><p>SpeedTree: Fixed incorrect normal directionn on v7 assets.</p></li>
<li><p>SpeedTree: Fixed normal mapping on newly imported v8 assets.</p></li>
<li><p>SpeedTree: Fixed the import of collision objects from SpeedTree v8 Assets.</p></li>
<li><p>Terrain: Changed vertex/hull shader program translation into a tessellation compute kernel when there is no vertex input. (<a href="https://issuetracker.unity3d.com/issues/terrain-crash-when-moving-terrain-in-scene-view">1087072</a>)</p></li>
<li><p>Terrain: Fixed a rare crash loading in a corrupted Terrain Data asset. (<a href="https://issuetracker.unity3d.com/issues/splatdatabase-checkconsistency-crash-when-opening-a-gaia-scene">1132798</a>, 1139361)</p></li>
<li><p>Terrain: Fixed the Terrain selection outline so that it works from the back side as well. (<a href="https://issuetracker.unity3d.com/issues/terrain-back-side-of-terrain-not-included-in-selection-pass">1098438</a>)</p></li>
<li><p>Terrain: Made changes so the Remove Light Probe Ringing setting can be serialized and undone. (<a href="https://issuetracker.unity3d.com/issues/terrain-remove-light-probe-ringing-not-serialized-and-tracked-by-undo-in-terrain-settings">1093751</a>)</p></li>
<li><p>Terrain: Streamlined the experimental terrain tool API, to follow Unity conventions and reduce code complexity.</p></li>
<li><p>Timeline: Changed behaviour of the Timeline Window to apply modifications immediately during Playmode (<a href="https://issuetracker.unity3d.com/issues/timeline-mute-state-persists-from-first-played">922846</a>, 1111908, 1120859, 1120870)</p></li>
<li><p>Timeline: Clip edit mode clutch keys will not get stuck when holding multiple keys at the same time (1097216, 1120865)</p></li>
<li><p>Timeline: Clip inspector will no longer throw exceptions when changing values when the inspector is locked (1115984, 1120863)</p></li>
<li><p>Timeline: Double separator in context menu of animation track (1102911, 1117193)</p></li>
<li><p>Timeline: Fixed a Notifications crash when creating an instance of <code>GameObjects</code>. (<a href="https://issuetracker.unity3d.com/issues/crash-on-scripting-scriptingwrapperfor-when-setting-gameobject-parent-via-timeline-signals">1129866</a>, 1139320)</p></li>
<li><p>Timeline: Fixed an issue where a circular reference warning appeared in the Control Clip inspector even if there was no circular reference (1116520, 1121828)</p></li>
<li><p>Timeline: Fixed an issue where events were being sent twice near the end of a clip. (<a href="https://issuetracker.unity3d.com/issues/timeline-sequence-doesnt-fire-animation-events-that-are-on-the-last-frames-when-several-clips-are-played">1017658</a>, <a href="https://issuetracker.unity3d.com/issues/timeline-animation-event-thats-close-to-the-last-frame-gets-called-twice-when-it-transitions-to-another-animation">1022016</a>)</p></li>
<li><p>Timeline: Fixed an issue where it was difficult to select a marker at the edge of a clip. (1102591, 1120860)</p></li>
<li><p>Timeline: Fixed an issue where non-public custom tracks did not appear in the Add Track menu. (1122803, 1129914)</p></li>
<li><p>Timeline: Fixed an issue where Notifications with the Retroactive flag are triggered when the timeline loops. (<a href="https://issuetracker.unity3d.com/issues/notifications-with-retroactive-flag-are-triggered-when-the-timeline-loops">1137266</a>, 1141569)</p></li>
<li><p>Timeline: Fixed an issue where the Signal Receiver would throw exceptions if the Inspector was locked. (<a href="https://issuetracker.unity3d.com/issues/selecting-a-signal-emitter-in-timeline-while-the-inspector-is-locked-causes-nullreferenceexceptions">1114526</a>, 1120867)</p></li>
<li><p>Timeline: Fixed an issue where the Track context menu did not appear when right-clicking on a track header after a copy operation. (1131095, 1141893)</p></li>
<li><p>Timeline: Fixed an issue where you were able to select clips and markers located under the Timeline ruler and the Marker Header track. (1102598, <a href="https://issuetracker.unity3d.com/issues/the-clip-is-selected-when-selecting-playhead-and-the-clip-is-partially-visible-in-the-timeline">1117925</a>, 1118966, 1121827)</p></li>
<li><p>Timeline: Fixed appearance of muted tracks (1018643, 1120861)</p></li>
<li><p>Timeline: Fixed issue where performing undo after moving items on multiple tracks would not undo some items. (1131071, 1133964)</p></li>
<li><p>Timeline: Fixed Timeline Inspectors leaving <em>EditorGUI.showMixedValue</em> in the wrong state. (<a href="https://issuetracker.unity3d.com/issues/timeline-editorgui-dot-showmixedvalue-is-used-internally-in-the-clip-inspector-thus-causing-some-parts-of-the-editor-to-misbehave">1123895</a>, 1133951)</p></li>
<li><p>Timeline: Fixed <em>Match Offsets</em> commands causing improper animation defaults to be applied. (911678, 1133939)</p></li>
<li><p>Timeline: Inline curves dissappear from the timeline window. (1111871, 1117197)</p></li>
<li><p>Timeline: Marker Track shows up in the context menus. (1107586, 1117195)</p></li>
<li><p>Timeline: Pasted marker has "(Clone)" in its name. (1111899, 1117198)</p></li>
<li><p>Timeline: PlayableDirector.played event is now called after entering or exiting Playmode (<a href="https://issuetracker.unity3d.com/issues/timelineeditor-dot-inspecteddirector-dot-played-event-isnt-called-after-entering-slash-exiting-play-mode">1088918</a>, 1120858)</p></li>
<li><p>Timeline: Remap default prev/next shortcuts on OSX to avoid conflict with system shortcut.</p></li>
<li><p>Timeline: Removed warning that appeared when creating a new project (<a href="https://issuetracker.unity3d.com/issues/timeline-warnings-are-produced-when-creating-a-new-project">1106556</a>, 1117194)</p></li>
<li><p>Timeline: Signal is not triggered while playing when the time is manually set. (1111595, 1117196)</p></li>
<li><p>Timeline: Undoing a paste track operation in a group will no longer corrupt the timeline (1116052, 1120888)</p></li>
<li><p>UI: Added back-removed API for <code>Selectable.allSelectables</code> and options for a non-allocating version. (<a href="https://issuetracker.unity3d.com/issues/ui-api-breaking-changes-on-upgrading-project-ffrom-2018-dot-3-to-2019-dot-1">1126186</a>, 1126525)</p></li>
<li><p>UI: Cached <code>referencePixelsPerUnit</code> when the canvas parent is disabled. (<a href="https://issuetracker.unity3d.com/issues/the-borders-of-an-image-change-when-disabling-and-re-enabling-a-canvas-after-changing-its-worldcamera">1066689</a>)</p></li>
<li><p>UI: CanvasRenderer.SetMesh will now produce an error if a non-readable mesh is passed. (<a href="https://issuetracker.unity3d.com/issues/application-crashes-when-rendering-non-read-slash-write-enabled-mesh-to-canvas-in-built-application">1101813</a>, 1131495)</p></li>
<li><p>UI: Fix 4 split layout only showing perspective in scene views. (<a href="https://issuetracker.unity3d.com/issues/ui-viewport-display-only-perspective-view-instead-of-top-front-and-right-after-switching-layout-to-4-split">1112970</a>, 1114618)</p></li>
<li><p>UI: Fixed a breaking API change in <code>layoutGroup</code> where <code>scaleFactor</code> was added and inserted in the middle of the parameter list. (<a href="https://issuetracker.unity3d.com/issues/undocumented-breaking-api-change-layoutgroup-dot-setchildalongaxis">1129157</a>, 1133937)</p></li>
<li><p>UI: Fixed a bug where changing the Constraint Count for a Grid Layout Component caused a Division by Zero error. (<a href="https://issuetracker.unity3d.com/issues/dividebyzeroexception-division-by-zero-error-when-changing-the-constraint-count-for-a-grid-layout-1">1075194</a>)</p></li>
<li><p>UI: Fixed a bug where the drop-down menu sometimes didn’t close when clicking outside it. (<a href="https://issuetracker.unity3d.com/issues/dropdown-doesnt-close-when-clicking-outside-it-under-certain-cicumstance">1064466</a>)</p></li>
<li><p>UI: Fixed an issue where the Canvas was enabled and <code>RectTransform</code> data was polled in awake, it started returning incorrect values for root <code>RectTransform</code>s.</p></li>
<li><p>UI: Fixed an issue where Undo would break in the <strong>Image</strong> component when a Sprite is replaced. (<a href="https://issuetracker.unity3d.com/issues/ui-image-component-breaks-when-the-sprite-is-replaced">1114240</a>, 1119502)</p></li>
<li><p>UI: Fixed an issue where <code>IndexedSet</code> didn't return <code>-1</code> when the element is not found in the dictionary.</p></li>
<li><p>UI: Fixed an issue with UI Scrollbar blocking Prefab mode. (1115796, 1115799)</p></li>
<li><p>UI: Fixed issue where creating a ui element under a disabled canvas would create a new canvas (<a href="https://issuetracker.unity3d.com/issues/creating-ui-on-a-disabled-ui-parent-also-adds-new-ui-element-thats-the-same-as-parent-every-time">1089472</a>)</p></li>
<li><p>UI: Fixed issue where loading a Scene with an orphaned UI component caused a crash. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-on-transform-getlocalposition-when-opening-a-specific-scene">1085469</a>)</p></li>
<li><p>UI: Fixed issue where nested canvases with canvas groups and custom alphas didn’t work properly. (<a href="https://issuetracker.unity3d.com/issues/canvas-group-children-with-canvas-component-are-faded-when-changing-alpha-parameter-in-the-canvas-group">1084745</a>)</p></li>
<li><p>UI: Fixed issue where nested canvases with canvas scalers didn’t work properly. (<a href="https://issuetracker.unity3d.com/issues/ui-removing-or-disabling-canvasscaler-corrupts-ui-which-cannot-be-undone">1033895</a>)</p></li>
<li><p>UI: Fixed issue where the input field cursor wasn’t positioned properly. (<a href="https://issuetracker.unity3d.com/issues/inputfields-image-doesnt-extend-to-fit-the-length-of-the-text-fields-value-when-editing-it-in-the-inspector">1083649</a>)</p></li>
<li><p>UI: Fixed issue where UI filtering in Scene view didn't function properly. (1064210)</p></li>
<li><p>UI: Fixed issue where <code>ListView.Refresh</code> computed an incorrect offset for the first row when an item source changed.</p></li>
<li><p>UI: Fixed memory from being allocated every frame in <code>CanvasScaler.Update()</code>. (<a href="https://issuetracker.unity3d.com/issues/2019-dot-1-canvasscaler-dot-update-allocates-memory-every-frame">1105332</a>, 1118317)</p></li>
<li><p>UI: Fixed PopupField text overflow.</p></li>
<li><p>UI Elements: Fix GraphView badges behavior on zoom in/out</p></li>
<li><p>UI Elements: Fixed : Setting a TextField's "Password" attribute via C# doesn't work. (1109699, 1115308)</p></li>
<li><p>UI Elements: Fixed : Setting a TextField's "Password" attribute via UXML doesn't work. (1109697, 1115309)</p></li>
<li><p>UI Elements: Fixed an issue where closing a window from a scheduler callback gave errors. (1098721)</p></li>
<li><p>UI Elements: Fixed an issue where pressing delete did not clear the contents of the ObjectField. (<a href="https://issuetracker.unity3d.com/issues/uielements-objectfield-pressing-delete-does-not-clear-contents-like-imgui-behaviour">1062184</a>)</p></li>
<li><p>UI Elements: Fixed an issue where the List View selection was not dimmed when unfocused. (1085251)</p></li>
<li><p>UI Elements: Fixed an issue where the position of text elements was reset during layout. (1106914)</p></li>
<li><p>UI Elements: Fixed an issue where the UIElements scheduler ran expired items. (1138634, 1140174)</p></li>
<li><p>UI Elements: Fixed an issue where UIElements did not respond to the Return key, Enter key, and the spacebar with fields such as Toggle, GradientField, CurveField, ObjectField, EnumField, and popup-related fields.</p></li>
<li><p>UI Elements: Fixed an issue with GraphView where the group title name was not visible during editing. (1106992)</p></li>
<li><p>UI Elements: Fixed an issue with measuring text elements that were not added to a hierarchy. (<a href="https://issuetracker.unity3d.com/issues/measurevisualelementtextsize-in-measurevisualelementtextsize">1108699</a>)</p></li>
<li><p>UI Elements: Fixed an issue with setting the showVertical and showHorizontal properties of a Scrollview with a callback. (1137340, 1139666)</p></li>
<li><p>UI Elements: Fixed an issue with text and numeric fields where pressing Enter did not end editing. (1096200)</p></li>
<li><p>UI Elements: Fixed an issue with text and numeric fields where pressing Escape did not end editing and restore the previous value. (1096199)</p></li>
<li><p>UI Elements: Fixed an issue with UXML template instances where they always appeared at the end of their parent. (1104566)</p></li>
<li><p>UI Elements: Fixed an issue with VectorXXFields when the window is resized. (1049285)</p></li>
<li><p>UI Elements: Fixed GraphView getting blurred when reframing the view (1114357, 1117687)</p></li>
<li><p>UI Elements: Fixed inconsistent border width at non integer scaling. (1131952, 1136268)</p></li>
<li><p>UI Elements: Fixed incorrectly displayed selection state in Graphview (1136637, 1137863)</p></li>
<li><p>UI Elements: Fixed Line and Trail Renderers throw errors in the console when Inspector window is of certain dimensions (1121685, 1131006)</p></li>
<li><p>UI Elements: Fixed missing GraphView nodes on OpenGL (macOS) (1117681, 1117689)</p></li>
<li><p>UI Elements: Fixed Null Reference exception thrown on changing scale factor of the screen from Window's display settings (<a href="https://issuetracker.unity3d.com/issues/editor-null-reference-exception-thrown-on-changing-scale-factor-of-the-screen-from-windows-display-settings">1104793</a>, 1123854)</p></li>
<li><p>UI Elements: Fixed NullReferenceExceptions in GraphView when displaying elements with empty sizes (1111567, 1117688)</p></li>
<li><p>UI Elements: Fixed the delayed behaviour when mouse dragger is used on numeric input field. (1117379, 1131767)</p></li>
<li><p>UI Elements: Fixed the foldout visual triangle that changed to checkmark. (1116011, 1118229)</p></li>
<li><p>UI Elements: Fixed the GradientField not showing the alpha checker (1118985, 1123838)</p></li>
<li><p>UI Elements: Fixed the indentation of custom scripts variables into the Inspector Window (<a href="https://issuetracker.unity3d.com/issues/2019-dot-1-variables-of-custom-script-components-are-indented-in-the-inspector">1114055</a>, 1137231)</p></li>
<li><p>UI Elements: Fixed the Inspector Window not redrawing when switching from Normal to Debug and vice-versa (1125071, 1133805)</p></li>
<li><p>UI Elements: Fixed the layout struggling when opening a prefab in the window hierarchy (1120821, 1131003)</p></li>
<li><p>UI Elements: Fixed the multiline TextField not supporting Tab character (<a href="https://issuetracker.unity3d.com/issues/uielements-multi-lines-textfield-does-not-support-tab-character">984808</a>, 1115525)</p></li>
<li><p>UI Elements: Fixed the multiselection of animation clip showing debug output in the inspector (<a href="https://issuetracker.unity3d.com/issues/animation-multi-selecting-animation-clips-in-project-window-show-debug-options">1115027</a>, 1132587)</p></li>
<li><p>UI Elements: Fixed the ObjectPicker setting none in ObjectField when cancelling. (<a href="https://issuetracker.unity3d.com/issues/cancelling-objectpicker-window-resets-objectfield-to-none-instead-of-an-already-set-value">1123688</a>, 1131001)</p></li>
<li><p>UI Elements: Fixed the preview of UXML files in the Inspector. (1111250, 1128632)</p></li>
<li><p>UI Elements: Fixed the shortcutmanager where long names are not displayed correctly in the profile selector. (<a href="https://issuetracker.unity3d.com/issues/long-names-are-not-displayed-properly">1099039</a>, 1118262)</p></li>
<li><p>UI Elements: Fixed the Toolbar search cancel button not showing correctly. (1115354, 1124647)</p></li>
<li><p>UI Elements: Fixed the value not being in synch when doing a Cut or Paste action from contextual menu in TextFields (<a href="https://issuetracker.unity3d.com/issues/ui-elements-context-menu-paste-makes-the-internal-state-of-a-textfield-come-out-of-sync-from-what-its-displaying">1120588</a>, 1124654)</p></li>
<li><p>UI Elements: Fixed the visual output of the CurveField (1118999, 1131858)</p></li>
<li><p>UI Elements: Fixed the yoga layout not rounding values correctly. (1105567, 1123832)</p></li>
<li><p>UI Elements: Properly dirty repaint on nested VisualElement view-transforms (1117229, 1117951)</p></li>
<li><p>UI Elements: Reduced recurrent memory allocations performed by UIElements. (1135055, 1136266)</p></li>
<li><p>UI Elements: UIElements Debugger splitter resets after entering Play Mode (<a href="https://issuetracker.unity3d.com/issues/uielements-debugger-splitter-resets-after-entering-play-mode">1113790</a>, 1131497)</p></li>
<li><p>UI Elements: UIR: fix broken edge expansion system and tesselation (1125408, 1125417)</p></li>
<li><p>Unity Test Runner: Fixed issue where the test runner would not reopen the original scene after running playmode tests. (<a href="https://issuetracker.unity3d.com/issues/unity-loads-new-untitled-scene-instead-of-previous-after-running-playmode-tests">1118111</a>, 1123900)</p></li>
<li><p>Universal Windows Platform: Fixed "Open Download Page" button navigating to non-existent file (<a href="https://issuetracker.unity3d.com/issues/editor-on-selecting-open-download-page-button-for-universal-windows-platform-directs-to-web-page-error">1106517</a>)</p></li>
<li><p>Universal Windows Platform: Fixed build failure in generated VS project due to duplicate Extension nodes in the appx manifest (1123172, 1124732)</p></li>
<li><p>Universal Windows Platform: Fixed Enter and Tab keys not working in multiline InputField UI (<a href="https://issuetracker.unity3d.com/issues/uwp-enter-key-is-not-working-for-inputfield-in-a-uwp-build">1108599</a>, 1131081)</p></li>
<li><p>Universal Windows Platform: Fixed IL2CPP crashing when using certain new types (like Windows.Foundation.GuidHelper.Equals) in Windows SDK 17763 or newer.</p></li>
<li><p>Universal Windows Platform: Fixed InputField text selection so that it works on Windows 10 touch-enabled devices. (<a href="https://issuetracker.unity3d.com/issues/uwp-input-fields-blinking-cursor-position-cant-be-change-on-devices-with-touch-input-enabled">1002834</a>)</p></li>
<li><p>Universal Windows Platform: Fixed issue where WebCamTexture failed to play in certain rare situations. (<a href="https://issuetracker.unity3d.com/issues/uwp-app-triggers-an-exception-when-starting-to-play-webcam-texture">1044635</a>)</p></li>
<li><p>Universal Windows Platform: Fixed the Visual Studio warning from generated UWP projects concerning a missing VS2015 toolset. (<a href="https://issuetracker.unity3d.com/issues/uwp-warning-is-printed-in-visual-studios-2017-for-a-missing-visual-studio-2015-v140-toolset">1091279</a>)</p></li>
<li><p>Universal Windows Platform: Made builds fail if the certificate is expired. (<a href="https://issuetracker.unity3d.com/issues/wsa-unity-allows-building-with-an-expired-uwp-certificate">1022794</a>)</p></li>
<li><p>Video: Added VR single-pass instancing mode to the VideoPlayer component. (950205)</p></li>
<li><p>Video: Fix for multiple GameViews, Camera Preview, and manual Camera Render. (<a href="https://issuetracker.unity3d.com/issues/video-player-video-clip-renders-only-in-single-game-window-when-multiple-game-windows-are-open">1109551</a>, 1114623)</p></li>
<li><p>Video: Fixed a crash on iOS when switching between videos with 6 audio channels. (<a href="https://issuetracker.unity3d.com/issues/ios-videoplayer-video-with-6-audio-channels-crashes-when-switching-between-videos">935497</a>)</p></li>
<li><p>Video: Fixed a crash that occurred while importing the ARCore SDK for Unity 1.7.0 package. (1133177, 1139365)</p></li>
<li><p>Video: Fixed a crash with "-[AVFoundationMediaLoader GetNumAudioChannels:]" when entering Play Mode. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-on-avfoundationmedialoader-getnumaudiochannels-when-entering-play-mode">1104510</a>, 1139367)</p></li>
<li><p>Video: Fixed an issue where the Editor crashes on skipping transcoding twice for video. (<a href="https://issuetracker.unity3d.com/issues/video-editor-crashes-on-skipping-transcoding-twice-for-video">1104507</a>, 1139450)</p></li>
<li><p>Video: Fixed an issue with the "LZ4" or "LZ4HC" compression methods when viewing a video in the Standalone Player. (<a href="https://issuetracker.unity3d.com/issues/using-lz4-or-lz4hc-compression-methods-results-in-an-error-in-standalone-player-when-viewing-a-video">1092265</a>, 1139366)</p></li>
<li><p>Video: Fixed crash on specific AVI video files on Windows. (<a href="https://issuetracker.unity3d.com/issues/crash-on-windowsvideomedia-copytorgba-when-importing-avi-file">1088203</a>)</p></li>
<li><p>Video: Fixed crash on specific MPEG2 video files on Windows. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-playing-mpeg2-video-in-inspector">1082071</a>)</p></li>
<li><p>Video: Fixed issue where the frame rate dropped drastically when using Movie Recorder to record as WebM. (<a href="https://issuetracker.unity3d.com/issues/recorder-frame-rate-drops-drastically-when-using-movie-recorder-to-record-as-webm">1052060</a>)</p></li>
<li><p>Video: Improved VideoPlayer network error handling on Windows. (<a href="https://issuetracker.unity3d.com/issues/windows-videoplayer-dot-errorreceived-callback-is-not-triggered-when-internet-connection-is-lost">1051461</a>)</p></li>
<li><p>Video: Made changes so that VideoPlayer Camera Plane targets are visible in the SRP. (<a href="https://issuetracker.unity3d.com/issues/video-player-doesnt-show-anything-on-hd-scriptable-render-pipeline">1024877</a>)</p></li>
<li><p>Video: Made changes to disregard unsupported streams on Windows. (<a href="https://issuetracker.unity3d.com/issues/an-error-is-thrown-when-playing-mov-file-which-was-made-on-iphone-ios-10">1065499</a>)</p></li>
<li><p>Video: [WINDOWS 7] Imported Video File cannot be played in 2019.1 (1133061, 1133666)</p></li>
<li><p>VR: [Lumin] Fixed an issue where including TrackedPoseDriver in a scene would produce incorrect headpose results (1105315, 1118305)</p></li>
<li><p>WebGL: Fixed an issue where the Editor prevented builds for WebGL when linear color space was enabled. (<a href="https://issuetracker.unity3d.com/issues/webgl-cant-build-with-linear-color-space-due-to-wrong-error">1103083</a>)</p></li>
<li><p>WebGL: Fixed an issue where WebGL froze when switching to full-screen. (<a href="https://issuetracker.unity3d.com/issues/webgl-switching-to-full-screen-causes-webgl-player-freeze">1106442</a>, 1144828)</p></li>
<li><p>WebGL: Fixed the Build window Linear Color Space compatibility check. (<a href="https://issuetracker.unity3d.com/issues/linear-color-space-build-can-be-started-with-webgl-1-dot-0-in-the-api-list">1105479</a>)</p></li>
<li><p>WebGL: Fixed the Performance Reporting integer overflow in WebAssembly development builds.</p></li>
<li><p>WebGL: Fixed WebGL build failure when python is already installed (<a href="https://issuetracker.unity3d.com/issues/webgl-build-fails-conflicting-with-existing-emscripten-and-python-installation">938826</a>)</p></li>
<li><p>WebGL: Fixed <code>Application.Quit()</code> and memory cleanup. (<a href="https://issuetracker.unity3d.com/issues/webgl-player-continues-to-run-after-webgl-content-is-removed-from-dom">1032870</a>)</p></li>
<li><p>WebGL: WebGL: Fix build&amp;run with wasm streaming enabled. (<a href="https://issuetracker.unity3d.com/issues/wasm-streaming-doesnt-work-using-build-and-run">1104514</a>, 1125367)</p></li>
<li><p>Windows: Fixed an issue where the Editor froze when certain devices (Steinberg UR 22 mk II, Cronus MAX) were connected to the computer. (<a href="https://issuetracker.unity3d.com/issues/unity-hangs-when-opening-project-with-steinberg-ur-22-mk-ii-connected">917526</a>)</p></li>
<li><p>Windows: Fixed cursor confinement to window not matching window bounds visually</p></li>
<li><p>Windows: Fixed headless build crashing if closed via the "X" button in the console</p></li>
<li><p>Windows: Fixed WinPixEventRuntime.dll deployed with non-development builds (<a href="https://issuetracker.unity3d.com/issues/building-an-application-generates-winpixeventruntime-dot-dll-when-development-build-is-unchecked-and-architecture-is-x86-64">1118833</a>, 1131483)</p></li>
<li><p>Windows: Improved error messages after failing to load native plugins on Windows Standalone and UWP if one of their dependencies is missing. (1083178, 1116537)</p></li>
<li><p>XR: Fix invalid return when using XRDevice.GetNativePointer with Oculus</p></li>
<li><p>XR: Fix white flash before splash screen on Gear VR applications (<a href="https://issuetracker.unity3d.com/issues/gearvr-when-returning-from-the-oculus-menu-to-app-there-is-a-white-flash">893599</a>)</p></li>
<li><p>XR: Fixed a regression where Android based VR was locked to 30fps. (<a href="https://issuetracker.unity3d.com/issues/oculus-go-apllications-are-capped-at-30-fps-when-building-a-project-for-oculus-go">1135328</a>, 1140824)</p></li>
<li><p>XR: Fixed head-tracking and rendering for in-editor remoting to HoloLens devices (<a href="https://issuetracker.unity3d.com/issues/hololens-remoting-hololens-device-does-not-render-anything-when-emulation-mode-is-set-to-remote-to-device">1138473</a>, 1140716)</p></li>
<li><p>XR: Fixed issue that caused the player to crash when using Google Cardboard API with both GLES3 and Vulkan included in the graphics APIs. (<a href="https://issuetracker.unity3d.com/issues/xr-android-application-crashes-and-does-not-fall-back-to-gles3-when-having-both-gles3-and-vulkan-included-in-graphics-apis">1102049</a>)</p></li>
<li><p>XR: Fixed issue where VR Billboarded trees were improperly lit on macOS if VR was enabled. (1025108)</p></li>
<li><p>XR: Fixed issue where VR tree shader used alpha to coverage multi-sampling when multi-sample anti-aliasing (MSAA) was disabled. (<a href="https://issuetracker.unity3d.com/issues/details-are-lost-too-early-for-terrain-trees-in-vr">1074421</a>)</p></li>
</ul>
