# Unity 2019.1

https://unity3d.com/unity/whats-new/2019.1.0

## Fixes



*   2D: "sprite.textureRect" returns values for master SpriteAtlas instead of SpriteAtlas Variant ([1115285](https://issuetracker.unity3d.com/issues/sprite-dot-texturerect-returns-values-for-master-spriteatlas-instead-of-spriteatlas-variant), 1125298)
    
*   2D: Added missing docs for `TextureImportSettings.SpriteMeshType`. (1080294)
    
*   2D: Crash in FitBlockMaskInBlockMaskUsingPadding when packing a Sprite Atlas with blockOffset value set to 0 ([1121583](https://issuetracker.unity3d.com/issues/crash-in-fitblockmaskinblockmaskusingpadding-when-packing-a-sprite-atlas-with-blockoffset-value-set-to-0), 1125296)
    
*   2D: Fix exception when trimming Sprite alpha on a texture that is downsized ([1104094](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-error-is-thrown-when-trimming-a-sprite-that-has-a-greater-resolution-than-its-import-settings), 1113929)
    
*   2D: Fix Grid.GetCellCenterWorld returning an offset position when using an Isometric Grid layout ([1116814](https://issuetracker.unity3d.com/issues/grid-dot-getcellcenterworld-returns-a-value-offset-from-the-center-when-using-an-isometric-grid-layout), 1136013)
    
*   2D: Fix Sprite Editor Window module breakage when window is maximized and restore (1114929, 1114930)
    
*   2D: Fix Sprite Frame Inspector window overlaps the header and options when the window is shrunk diagonally ([1113250](https://issuetracker.unity3d.com/issues/sprite-editor-sprite-setting-window-overlaps-the-header-and-options-when-the-window-is-shrunk-diagonally), 1114470)
    
*   2D: Fix when entering negative values in width/height of Sprite Editor Window causes irregular sprite movement (1100307)
    
*   2D: Fixed an assertion message when `SpriteRenderer` was selected with no Sprite with the **Sprite Editor** window open. (1122260, 1122262)
    
*   2D: Fixed an issue where a Sprite was not generated from a texture when user selected the **Apply** action at the **Unapplied import** settings popup. (1117274, 1122263)
    
*   2D: Fixed an issue where the Editor crashed on clicking **Pack Preview** when same atlas was added in **Packables** in Debug View. ([1107235](https://issuetracker.unity3d.com/issues/2d-editor-crashes-on-clicking-pack-preview-when-same-atlas-is-added-in-packables-in-debug-view))
    
*   2D: Fixed an issue where the side of a Sprite was cut off when its **Max Size** property was changed. ([1101500](https://issuetracker.unity3d.com/issues/the-side-of-a-sprite-is-chopped-off-when-its-max-size-property-is-changed))
    
*   2D: Fixed issue where Sorting Groups did not update in Play Mode when Play Mode was paused in the Editor.
    
*   2D: Fixed issue where Sprites referenced both the original Sprite assets and Sprite Atlas, which resulted in increased memory usage. ([1071494](https://issuetracker.unity3d.com/issues/sprites-reference-both-the-original-sprite-assets-and-sprite-atlas-resulting-in-increased-memory-usage))
    
*   2D: Fixed issue where Sprites rendered through Command Buffers were not displayed until they were rendered once with a default Renderer. ([1097465](https://issuetracker.unity3d.com/issues/sprites-rendered-through-command-buffers-not-displayed-until-rendered-once-with-a-default-renderer))
    
*   2D: Fixed issue where SpriteShapeRenderer passed an invalid `_texelSize.zw`. ([1099636](https://issuetracker.unity3d.com/issues/spriteshaperenderer-passes-invalid-texelsize-dot-zw))
    
*   2D: Fixed the offset of the TilemapCollider2D collider for Isometric Tilemaps.
    
*   2D: Made a Sprite that is not packed into a Sprite Atlas remain invisible. (1083304)
    
*   2D: Made changes so that when you click and drag on an unselected Sprite, the Sprite Editor Window shows a normal cursor to indicate dragging a Sprite, instead of the resize cursor used for resizing a border. ([1077700](https://issuetracker.unity3d.com/issues/trying-to-move-the-green-outline-on-a-sprite-in-the-sprite-editor-moves-the-entire-rect-when-clicking-on-an-unselected-sprite))
    
*   2D: Made changes to allow users to reset the Sorting Layer and Sorting Order settings of Renderer components from the Inspector Settings (cog button). ([1096375](https://issuetracker.unity3d.com/issues/tilemap-renderer-properties-does-not-reset-when-resetting-the-component-using-cogwheel))
    
*   2D: PSB files do not get packed when added to Sprite Atlas (1114959, 1121775)
    
*   AI: Unity crashes when repathing agent destination ([1104500](https://issuetracker.unity3d.com/issues/unity-crashes-when-repathing-agent-destination))
    
*   Analytics: Fixed a bug that resulted in performance data still being sent from mobile devices when a developer disabled Analytics at runtime. ([1105108](https://issuetracker.unity3d.com/issues/performance-data-is-being-sent-when-analytics-are-disabled-in-runtime-on-mobile-devices))
    
*   Android: Added a fix in the new input system so Deadzoning is not performed in the native backend for game controller axes.
    
*   Android: Added a fix in the new input system so mouse delta is correctly calculated.
    
*   Android: Added detection for when the Editor does not manage to install the application to the device ([1086410](https://issuetracker.unity3d.com/issues/android-editor-doesnt-show-that-pushing-built-apps-to-android-4-dot-1-is-failing))
    
*   Android: Added the ability to opt-out from stopping Gradle daemons upon Editor exit. (1098578, 1138085)
    
*   Android: Added `StreamingAssets` folders starting with an underscore in Gradle builds
    
*   Android: Enabled EGL sRGB backbuffer in Android 9.0
    
*   Android: Fix black screen when PlayerSetting "Use 32-bit Display Buffer" is disabled ([1103404](https://issuetracker.unity3d.com/issues/android-app-shows-black-screen-when-built-without-use-32-bit-display-buffer-option))
    
*   Android: Fixed a crash on startup in Development Builds on older Android devices
    
*   Android: Fixed a problem with exceptions when exporting an Android Gradle project ([1089510](https://issuetracker.unity3d.com/issues/android-gradle-export-throws-trying-to-add-unity-classes-dot-jar-slash-androidmanifest-dot-xml-to-the-list-of-output-files))
    
*   Android: Fixed a Vulkan shader compile error when using `SV_RenderTargetArrayIndex` in the vertex shader output ([1098973](https://issuetracker.unity3d.com/issues/android-lwrp-pp-building-project-for-the-first-time-there-are-shader-errors-in-the-console-if-using-vulkan-graphics-api))
    
*   Android: Fixed an issue where a black screen appears when trying to use linear rendering with 16bit backbuffer
    
*   Android: Fixed an issue where Android quickly changing screen orientation twice stretches the view ([1098327](https://issuetracker.unity3d.com/issues/android-quickly-changing-screen-orientation-twice-stretches-view))
    
*   Android: Fixed an issue where Gradle builds fail when using quotes and backslashes in keystore passwords and aliases ([996504](https://issuetracker.unity3d.com/issues/android-gradle-build-fails-if-keystore-slash-key-password-contains-a-single-slash-double-quote), [1071288](https://issuetracker.unity3d.com/issues/android-gradle-build-system-does-not-escape-backslash-character-on-keystore-alias-password))
    
*   Android: Fixed an issue where redundant render pass was created for clear when using Vulkan
    
*   Android: Fixed an issue where the application froze when displaying the Android ProgressBar ([1053736](https://issuetracker.unity3d.com/issues/android-application-freezes-when-progressbar-appears-on-the-screen))
    
*   Android: Fixed an issue where the il2cpp library was relinked when building to Android (1089122)
    
*   Android: Fixed an issue where the `CrashReportint` module was not stripped on il2cpp when not used.
    
*   Android: Fixed an issue where `s_MainWindowRenderingOffscreen == false` and `CurrentThread::IsMainThread()` was firing on Android when using SRP. (1120743, 1133156)
    
*   Android: Fixed an OpenGL ES 3.0 shader compile error when generated code requires `bitfieldInsert`
    
*   Android: Fixed Android touch input scale when changing screen orientation with a custom resolution ([1085580](https://issuetracker.unity3d.com/issues/android-button-cannot-be-pressed-on-the-right-slash-bottom-half-of-the-screen-after-changing-resolution-and-screen-orientation-mode))
    
*   Android: Fixed automatic resolution scaling when using Vulkan (1108491, 1118293)
    
*   Android: Fixed dynamic resolution on some older Mali GPUs on Vulkan ([1065227](https://issuetracker.unity3d.com/issues/android-dynamic-resolution-doesnt-work-on-samsung-galaxy-s6-edge-plus))
    
*   Android: Fixed HDR rendering when using Vulkan on older Mali drivers ([1105065](https://issuetracker.unity3d.com/issues/lights-not-rendered-correctly-on-samsung-s6-edge-device-on-vulkan), 1115919)
    
*   Android: Fixed missing draws when using Vulkan on Adreno ([1094348](https://issuetracker.unity3d.com/issues/android-vulkan-meshes-with-standard-shader-and-gpu-instancing-enabled-are-not-rendered-correctly-on-adreno-gpus))
    
*   Android: Fixed shader compiler errors with Mali 450 drivers
    
*   Android: Fixed Terrain rendering when Vulkan on Adreno is used ([1102440](https://issuetracker.unity3d.com/issues/android-vulkan-terrain-with-draw-instanced-enabled-is-not-rendered-on-android-devices-with-adreno-gpu))
    
*   Android: Fixed the Bluetooth related crash on Android 5 devices when no headset is connected ([1089471](https://issuetracker.unity3d.com/issues/android-project-crashes-on-xiaomi-mi-4i))
    
*   Android: Fixed the load failure of il2cpp player using OBB files ([1124777](https://issuetracker.unity3d.com/issues/android-error-of-failed-to-extract-resources-needed-by-il2cpp-when-building-with-split-application-binary-set-to-true), 1130918)
    
*   Android: Fixed the wrong `\` director separator in `DIR_UNITYPROJECT&amp;DIR_GRADLEPROJECT` on Windows ([1088160](https://issuetracker.unity3d.com/issues/android-windows-template-variable-dir-unityproject-on-windows-does-not-escape-slash-characters))
    
*   Android: Fixed `Activity has leaked ServiceConnection` errors when calling `Application.Unload` ([1091255](https://issuetracker.unity3d.com/issues/activity-has-leaked-serviceconnection-errors-when-calling-application-dot-unload))
    
*   Android: Fixed `Android Screen.safeArea` coordinate system to be in screen space.
    
*   Android: Fixed `Application.Unload` sometimes crashing on Android ([1093574](https://issuetracker.unity3d.com/issues/android-application-dot-unload-causes-a-crash-after-multiple-openings-within-native-android-app))
    
*   Android: Fixed `GrabPass` when using linear rendering on Android ([1088699](https://issuetracker.unity3d.com/issues/android-object-becomes-brighter-when-grabpass-is-used-and-color-space-is-set-to-linear))
    
*   Android: Fixed `RenderTextureFormat ARGB2101010` when using Vulkan on Adreno
    
*   Android: GPU Instanced mesh renders with artifacts on Adreno 630 devices ([1079627](https://issuetracker.unity3d.com/issues/android-cube-using-displacement-pixel-map-is-not-rendered-or-rendered-with-artifacts-on-adreno-630-devices))
    
*   Android: Improved performance of **Cubemap** convolution on Mali GPUs ([989820](https://issuetracker.unity3d.com/issues/vr-android-very-poor-performance-on-galaxy-s8))
    
*   Android: Linker errors print to console when using il2cpp.
    
*   Android: Refactored and improved Android device detection and selection during builds ([1102133](https://issuetracker.unity3d.com/issues/android-retrying-build-on-authorized-android-device-which-was-unauthorized-when-starting-the-build-still-doesnt-build))
    
*   Android: Touch and mouse position's y-value is inverted in the native backend instead of managed code in the new input system
    
*   Android: `Keyboard.onTextInput` and `Keyboard.onIMECompositionChange` correctly calls for physical and virtual keyboard events
    
*   Animation: Fixed a crash in the avatar configurator when a faulty bone was selected after AutoMap. (1075651)
    
*   Animation: Fixed a crash when a cycle occurs in an animation graph. ([792020](https://issuetracker.unity3d.com/issues/playables-crash-on-cyclic-graphs))
    
*   Animation: Fixed a crash when opening the Animator window from a bad Animator Controller setup. ([1080436](https://issuetracker.unity3d.com/issues/unity-crashes-if-using-a-specific-animator-controller-on-play-mode-when-opening-animator-window))
    
*   Animation: Fixed a crash when the Animation window previewed a disabled GameObject. ([1125266](https://issuetracker.unity3d.com/issues/editor-crashes-with-mecanim-setvaluemask-when-enabling-animation-keyframe-recording-mode), 1127071)
    
*   Animation: Fixed a crash when the animator changed the bindings of the next animator. ([1099988](https://issuetracker.unity3d.com/issues/editor-crashes-with-unityengine-animation-setgenericfloatpropertyvalues-when-switching-timeline-with-constrains))
    
*   Animation: Fixed an issue where additive animations would build up values when other layers were not writing ([1094706](https://issuetracker.unity3d.com/issues/empty-animatorcontroller-on-animator-used-by-playables-breaks-layer-blending), 1127817)
    
*   Animation: Fixed an issue where AnimationClip.empty always returns true when Animation Type is set to Legacy. ([1061700](https://issuetracker.unity3d.com/issues/when-animation-type-is-set-to-legacy-animation-clip-could-not-be-loaded-from-assetbundle-in-build))
    
*   Animation: Fixed an issue where querying clips in partially-loaded Override Controllers would crash ([1118196](https://issuetracker.unity3d.com/issues/crash-in-animatoroverridecontroller-getoriginalclip-when-using-an-indexer-operator-to-access-an-animation-clip), 1127823)
    
*   Animation: Fixed an issue where the Animation window opened when an AnimationClip was double-clicked. ([1058422](https://issuetracker.unity3d.com/issues/double-clicking-animation-clip-does-not-open-animation-editor-window))
    
*   Animation: Fixed an issue with AnimationStreamSource.PreviousInputs when used with humanoid characters. (1102231)
    
*   Animation: Fixed an issue with frame rounding in the Animation window. (1101186)
    
*   Animation: Fixed an issue with the animator that occurred after instantiation. ([995978](https://issuetracker.unity3d.com/issues/animator-first-frame-of-animator-isnt-updated-by-playablegraph-after-being-instantiated))
    
*   Animation: Fixed an issue with \[burstcompile\] not working on animation jobs.
    
*   Animation: Fixed erroneous range when changing orders of sprite keyframes in AnimationClip (1076068)
    
*   Asset Import: Added a fix to properly assign the Diffuse Color when a HDRP/Lit materical is generated froma FBX standard material in HDRP projects. ([1087977](https://issuetracker.unity3d.com/issues/hdrp-material-imported-with-model-doesnt-preserve-original-base-color-and-set-texture), 1114076)
    
*   Asset Import: Changed the icon of the Assets generated using ScriptedImporters to match the icon of other model files.
    
*   Asset Import: Clamped the global scale in ModelImporter to at most 10 digits. ([1082327](https://issuetracker.unity3d.com/issues/editor-unity-crashes-when-the-fbx-adam-scale-factor-set-to-value-having-20-digits-or-above))
    
*   Asset Import: Fix Missing Avatar assignement in older projects ([1107242](https://issuetracker.unity3d.com/issues/missing-avatar-assignement-in-a$-mecanim-gdc2013-sample-project))
    
*   Asset Import: Fixed an issue where importing FBX files with skinned meshes and with Index Format set to 16-bit produced corrupt data and/or errors. ([1126943](https://issuetracker.unity3d.com/issues/bone-related-errors-and-animation-issues-when-importing-fbx-with-index-format-set-to-16bit), 1139690)
    
*   Asset Import: Fixed an issue with `ModelImporter` where imported materials had no textures assigned in HDRP projects.
    
*   Asset Import: Fixed error when selecting multiple fbx with different Material settings. Multi-selection is not supported on this panel. ([1118475](https://issuetracker.unity3d.com/issues/buildexternalobjectscache-throws-nullreferenceexception-when-inspecting-multiple-fbx-assets-at-once), 1121738)
    
*   Asset Import: Fixed import of Blender files with Blender 2.80. ([1115353](https://issuetracker.unity3d.com/issues/blender-2-dot-8-files-not-compatible-with-unity), 1140789)
    
*   Asset Import: Fixed issue where the Model Importer **Use File Scale** property did not display the multiple different values checkbox in multiple selection.
    
*   Asset Import: Fixed Sprite asset references are missing after upgrading ([1102809](https://issuetracker.unity3d.com/issues/sprite-asset-references-are-missing-after-upgrading))
    
*   Asset Import: Made changes so that ProjectBrowser icons refresh correctly when the Model Importer is applied.
    
*   Asset Import: Made changes to prevent the use of a previously created avatar in the AvatarCopy field of the ModelImporter Rig panel.
    
*   Audio: Added a slider for Cutoff Frequency in the Audio High Pass Filter component. ([818332](https://issuetracker.unity3d.com/issues/audio-high-pass-filter-component-has-no-slider), 1131466)
    
*   Audio: Fixed an issue in the profiler where the time spent collecting audio data depended on the number of audio clips with loaded audio data. ([1086988](https://issuetracker.unity3d.com/issues/profiler-dot-collectaudiostats-time-ms-is-very-high-when-preload-audio-data-is-enabled-on-many-audio-files))
    
*   Audio: Fixed an issue where the Edit key option displayed incorrect parameters in the Curve editor. (713681)
    
*   Audio: Fixed an issue with calling AudioSource.GetSpatializerFloat or AudioSource.SetSpatializerFloat before an AudioSource was played.
    
*   Audio: Fixed an issue with importing short audio files that caused importer errors. (882227)
    
*   Audio: Fixed the tree view for Audio Mixer groups in the Output object selector. ([1010156](https://issuetracker.unity3d.com/issues/audio-output-groups-are-not-shown-with-a-tree-structure-but-as-a-flat-list-in-output-group-object-selector), 1131468)
    
*   Build Pipeline: Added a fix so failed builds are not treated as "successful".
    
*   Build Pipeline: Added a fix to unload asset bundles before building a player or other asset bundles. ([1081760](https://issuetracker.unity3d.com/issues/editor-crashes-with-cachedwriter-write-when-building-project-with-missing-project-id))
    
*   Build Pipeline: Added a fixed to allow the **Scripting Define Symbols** line in **Player Settings** to be reverted with the Undo command. ([1083481](https://issuetracker.unity3d.com/issues/scripting-define-symbols-line-does-not-change-when-using-undo-command))
    
*   Build Pipeline: Fix rare data corruption when building asset bundles with LZMA compression.
    
*   Build Pipeline: Fixed an issue where `PlayerSettings.applicationIdentifier` would not return the identifier for the active build target when editing settings for a different build target. ([1041443](https://issuetracker.unity3d.com/issues/playersettings-dot-applicationidentifier-reports-incorrect-value))
    
*   Build Pipeline: Fixed an object ordering indeterminism issue in the results returned by ContentBuildInterface.PrepareScene
    
*   Build Pipeline: Removed duplicate mono folder in Mac standalone builds. Also removed around 500 kb of unnecessary data from builds.
    
*   Compute: Vulkan/Metal/OpenGL: compute shader compilation optimizations (1022026)
    
*   DX12: Fixed crash related to memory allocation issues when using a camera with the **Depth** or **Don't Clear** flags. ([969582](https://issuetracker.unity3d.com/issues/dx12-crash-with-memory-allocation-issues-when-using-a-camera-with-the-depth-or-dont-clear-flags))
    
*   DX12: Fixed exclusive fullscreen always reverting to windowed fullscreen.
    
*   DX12: Fixed issue where test runner crashed while running tests containing RenderTexture instantiation from the command prompt. (1015725)
    
*   Editor: Added **Main Menu/** prefix to main menu commands displayed in the Shortcuts Manager Command list with **Category** set to **All Unity Commands**.
    
*   Editor: Added a fix for consistent logfile option handling for all desktop platforms, the Editor, and the Player. This improves the handling of edge cases and scenarios with logfile parameter. ([900754](https://issuetracker.unity3d.com/issues/command-line-logfile-with-no-parameters-outputs-to-screen-on-os-x-but-not-on-windows), [960012](https://issuetracker.unity3d.com/issues/after-opening-and-building-project-in-the-appdata-slash-locallow-folder-appear-two-new-folders-with-and-and-dot-escaped-characters), 1068907)
    
*   Editor: Added a fix so that items can be activated with space bar input in the Linux Editor inspector. ([1061975](https://issuetracker.unity3d.com/issues/linux-editor-the-inspector-does-not-take-space-bar-input))
    
*   Editor: Added a fix so that selecting **Open** on the **Context Menu** performs actions on folders. (1079852)
    
*   Editor: Added a fix to disallow naming Assembly definitions as predefined assembly names. ([1081704](https://issuetracker.unity3d.com/issues/typeloadexception-is-thrown-when-highlighting-a-script-and-reflectiontypeloadexception-is-thrown-when-entering-play-mode))
    
*   Editor: Added a fix to improve performance when deserializing uint64 values from text serialized assets.
    
*   Editor: Added a fix to stop Android release builds from forwarding network traffic to device. ([1090170](https://issuetracker.unity3d.com/issues/android-slash-linux-unable-to-forward-network-traffic-to-device))
    
*   Editor: Added a horizontal scrollbar to Preset Manager settings. ([1087969](https://issuetracker.unity3d.com/issues/assigned-presets-are-not-visible-in-preset-manager-when-settings-window-is-shrinks-horizontally))
    
*   Editor: Added button to clear binding in Keys preferences.
    
*   Editor: Added diagnostic warning icon under text. (1093938)
    
*   Editor: Added missing size and style to `CacheFontForText`. (1087730)
    
*   Editor: Added null protection when iterating using `ExtendVisibleAsChild`. ([1083254](https://issuetracker.unity3d.com/issues/unity-crashes-on-extendvisibleaschild-when-onsceneguidelegate-references-a-method-which-calls-handleutility-dot-pickgameobject))
    
*   Editor: Bring back Imported Header for AssetImporter component ([1104131](https://issuetracker.unity3d.com/issues/imported-object-header-is-missing))
    
*   Editor: Corrected a typo in the tooltip for the 2D/3D switch in the Scene view control bar. ([1048139](https://issuetracker.unity3d.com/issues/2d-slash-3d-toggle-button-in-scene-view-has-toggled-mispelled-as-togggled))
    
*   Editor: Creating a new material while an item is selected in scene could yield "IndexOutOfRange" errors (1128724, 1131937)
    
*   Editor: Debug Internal inspector no displays all properties (1109531, 1118915)
    
*   Editor: EditorWindow notification is rendered behind UI elements when the elements are instantiated from UXML ([1116944](https://issuetracker.unity3d.com/issues/editorwindow-notifaction-is-rendered-behind-ui-elements-when-the-elements-are-instantiated-from-uxml), 1131498)
    
*   Editor: Enabled editing a script field when the script is missing. ([1117624](https://issuetracker.unity3d.com/issues/object-picker-cannot-be-used-to-assign-missing-script-when-having-missing-script-component-in-inspector-window), 1126282)
    
*   Editor: Fix a crash when using hyperlink tag without the closing tag. ([1113075](https://issuetracker.unity3d.com/issues/crash-on-textrenderingprivate-nativetextgenerator-getrectinstring-when-opening-a-project-with-textmeshpro-plugin), 1135091)
    
*   Editor: Fix an issue where asset store window could turn blank when redocking ([1100443](https://issuetracker.unity3d.com/issues/linux-editor-asset-store-window-turns-blank-after-docking-and-undocking))
    
*   Editor: Fix an issue where custom editors with scrollviews would be squashed in the inspector window (1103342)
    
*   Editor: Fix Crash on dragging Script to component in inspector (1124734, 1131934)
    
*   Editor: Fix crash on editor window destruction
    
*   Editor: Fix crash while setting version control mode to visible meta files ([1128867](https://issuetracker.unity3d.com/issues/unity-editor-crashes-on-gameobject-setsupportedmessagesdirty-when-changing-version-control-mode-to-visible-meta-files), 1132704)
    
*   Editor: Fix editor crash while saving a scene with missing script. (1111432, 1115552)
    
*   Editor: Fix Exceptions raised and Inspector is broken after user removes a component from multiselected GameObjects (1126938, 1131936)
    
*   Editor: Fix extra shift being present in some contextual menu shortcuts in Timeline.
    
*   Editor: Fix Inspector Window's uxml contains strings that are no longer localized (1122433, 1131929)
    
*   Editor: Fix issue where EditorApplication.quitting callbacks were not being called in batchmode
    
*   Editor: Fix keypad period and delete for input fields (Linux)
    
*   Editor: Fix menu shortcuts before first menu show on Linux
    
*   Editor: Fix selecting items with duplicate names in test hierarchy of Test Runner window ([987587](https://issuetracker.unity3d.com/issues/test-runner-hierarchy-doesnt-correctly-select-an-item), 1140566)
    
*   Editor: Fix SettingsWindow layout breaks from 18.3 ([1124696](https://issuetracker.unity3d.com/issues/project-settings-window-breaks-a-custom-layout-after-upgrading-to-2019-dot-1-and-2019-dot-2-when-the-layout-was-made-in-2018-dot-3), 1129237)
    
*   Editor: Fix: Copying and pasting selected text copies an additional letter that is not selected ([1107289](https://issuetracker.unity3d.com/issues/copying-and-pasting-selected-text-that-has-a-parenthesis-at-the-end-still-includes-the-even-if-its-not-selected), 1114040)
    
*   Editor: Fixed a Null Reference Exception thrown when multiple Assembly Definition Assets are added to the same folder. (1120826, 1120982)
    
*   Editor: Fixed an incorrect `Input.keyCode` value when keyboard layout changes on macOS.
    
*   Editor: Fixed an incorrect `Input.keyCode` value when using the Dvorak - QWERTY Command keyboard layout on macOS. ([1103558](https://issuetracker.unity3d.com/issues/macos-hotkeys-are-mapped-as-standard-dvorak-shortcuts-and-ignore-system-preferences-when-using-dvorak-qwerty-keyboard-layout), 1131774)
    
*   Editor: Fixed an issue in the Shortcuts Manager Commmand list where right-clicking an entry did not select that entry, and displayed the context menu from the previously selected entry. ([1110804](https://issuetracker.unity3d.com/issues/shortcut-manager-right-clicking-a-command-does-not-select-it), 1120069)
    
*   Editor: Fixed an issue in the Shortcuts Manager where changes were not saved to the profile when users unassigned shortcuts or reset shortcuts to their default settings.
    
*   Editor: Fixed an issue in the Shortcuts Manager where selecting a new category from the Category list did not reset the selected entry in the Command list. (1104559, 1120070)
    
*   Editor: Fixed an issue in the Shortcuts Manager where users could assign reserved modifier keys (**Shift**, **Ctrl/Cmd**, and so on) to commands. ([1110790](https://issuetracker.unity3d.com/issues/shortcut-manager-you-can-assign-commands-to-the-modifier-keys-by-dragging-and-dropping-via-the-keyboard-layout-panel), 1120071)
    
*   Editor: Fixed an issue on Linux where the progress bar window changed size repeatedly while creating or opening a project. (1100653)
    
*   Editor: Fixed an issue on macOS where entering Unity keyboard shortcuts while a project was loading crashed Unity. ([1004336](https://issuetracker.unity3d.com/issues/osx-holding-cmd-plus-while-creating-slash-opening-project-opens-preferences-window-before-editor-is-opened))
    
*   Editor: Fixed an issue on macOS where launching the Editor with `-batchmode` as the first argument caused a crash. ([1059028](https://issuetracker.unity3d.com/issues/macos-unity-crashes-with-segmentation-fault-11-or-bus-error-10-when-launching-with-batchmode-followed-by-projectpath))
    
*   Editor: Fixed an issue on macOS where opening and closing utility windows caused a crash. ([1046287](https://issuetracker.unity3d.com/issues/editor-crash-on-clicking-animation-curve-created-using-uielement-for-mac-osx))
    
*   Editor: Fixed an issue where artifacts appeared in Sprite sheets when users clicked drop-down menus in the Inspector. ([1055868](https://issuetracker.unity3d.com/issues/sprite-sheet-grid-artifact-appears-when-clicking-drop-down-menus))
    
*   Editor: Fixed an issue where assets from Unity's built-in resources could not be loaded by `AssetDatabase.LoadAllAssetsAtPath`. ([1104874](https://issuetracker.unity3d.com/issues/using-loadallassetsatpath-to-load-the-paths-does-not-load-objects-stored-at-paths-and-leaves-the-the-expecting-object-empty))
    
*   Editor: Fixed an issue where calling `RenderTexture.ReleaseTemporary` twice for same texture caused a crash. ([1091561](https://issuetracker.unity3d.com/issues/editor-crashes-with-renderbuffermanager-textures-garbagecollect-when-calling-rendertexture-dot-releasetemporary-twice))
    
*   Editor: Fixed an issue where changing the shortcut for a main-menu item using the Shortcuts Manager would not update the menu with the new shortcut.
    
*   Editor: Fixed an issue where closing the Editor while the Asset Store or Services window was loading caused a crash. ([1024048](https://issuetracker.unity3d.com/issues/closing-unity-while-a$-or-services-tab-is-loading-crashes-editor))
    
*   Editor: Fixed an issue where creating a parameter for an Animation condition after creating the condition sometimes threw a NullReferenceException. ([1127789](https://issuetracker.unity3d.com/issues/previously-empty-conditions-for-an-animation-transition-cannot-be-updated-after-creating-the-first-parameter), 1131535)
    
*   Editor: Fixed an issue where drag and dropping a texture onto a **GameObject** in the Scene created a material with no texture in HDRP projects.
    
*   Editor: Fixed an issue where dragging a GameObject to the position directly after a child object in the Hierarchy window inserted the dragged object in the wrong position. ([1069565](https://issuetracker.unity3d.com/issues/game-object-is-not-inserted-correctly-in-hierarchy-window-when-placed-after-child-object))
    
*   Editor: Fixed an issue where empty **Editor Settings** password fields were returning asterisks for empty fields. ([958884](https://issuetracker.unity3d.com/issues/vcs-password-field-still-shows-up-as-not-empty-after-deleting-password))
    
*   Editor: Fixed an issue where empty strings caused `TextField` to crash. ([1107172](https://issuetracker.unity3d.com/issues/shortcut-manager-an-assertion-failure-occurs-when-entering-a-user-profile-name-with-multiple-spaces-at-the-beginning))
    
*   Editor: Fixed an issue where having multiple GameObjects selected and using the Component context menu to call `GameObject.DestroyImmediate` on Components crashed Unity. ([1056115](https://issuetracker.unity3d.com/issues/crash-on-scripting-scriptingwrapperfor-when-destroying-component-with-gameobject-dot-destroyimmediate-after-re-adding-it))
    
*   Editor: Fixed an issue where keyboard shortcuts for main menu commands would not work if the key combination included the **Space** key. ([1106151](https://issuetracker.unity3d.com/issues/menuitem-functions-with-assigned-shortcuts-involving-the-space-key-are-not-called-when-the-corresponding-shortcut-is-pressed), 1120068)
    
*   Editor: Fixed an issue where layouts were saved and loaded incorrectly. (1078964)
    
*   Editor: Fixed an issue where lines were not drawn when using `Handles.DrawDottedLine` in a custom inspector. ([954149](https://issuetracker.unity3d.com/issues/handles-dot-drawdottedline-does-nothing-when-used-in-the-editor))
    
*   Editor: Fixed an issue where modifying an Avatar's **Per-Muscle Settings** caused a NullReferenceException. ([1068870](https://issuetracker.unity3d.com/issues/null-reference-exception-on-tweaking-the-pre-muscle-settings-of-a-avatar-when-scene-view-is-in-focus))
    
*   Editor: Fixed an issue where searching for an asset in the Project window, and then renaming it via the context menu would not work if the Project widow was using the one-column layout. ([1073306](https://issuetracker.unity3d.com/issues/renaming-asset-while-searching-in-the-project-view-does-not-work-in-one-column-layout))
    
*   Editor: Fixed an issue where selecting assets in the last row of the Project window made the scroll bar blink. ([1076266](https://issuetracker.unity3d.com/issues/project-window-scrollbar-disappears-after-selecting-assets-from-the-bottom-row))
    
*   Editor: Fixed an issue where SerializedProperty children were not visible when put in a horizontal group. ([1068811](https://issuetracker.unity3d.com/issues/serializedproperty-children-not-visible-when-put-in-horizontal-group))
    
*   Editor: Fixed an issue where switching platforms and recompiling scripts did not clear compile errors from the Console. (1078935)
    
*   Editor: Fixed an issue where Test Runner console messages could overlap the test menu. ([1094277](https://issuetracker.unity3d.com/issues/test-runner-result-console-tab-is-transparent))
    
*   Editor: Fixed an issue where the **Add Component** menu is not displayed in some cases. ([1104169](https://issuetracker.unity3d.com/issues/add-component-shortcut-ctrl-plus-shift-plus-a-no-longer-works))
    
*   Editor: Fixed an issue where the **Undo** command did not work after setting/resetting the layout to **Default**. ([1068662](https://issuetracker.unity3d.com/issues/windows-unable-to-use-undo-if-editor-layout-is-set-to-default))
    
*   Editor: Fixed an issue where the color picker ignored copied hex codes when they included the number sign (#) prefix. ([804231](https://issuetracker.unity3d.com/issues/color-picker-ignores-the-color-hex-code-when-copied-with))
    
*   Editor: Fixed an issue where the Editor recommended updating to an earlier version.
    
*   Editor: Fixed an issue where the Editor used the OS locale. ([1089361](https://issuetracker.unity3d.com/issues/windows-editor-uses-os-locale-settings-i-dot-e-commas-instead-of-dots-in-float-values-with-net-4-dot-6))
    
*   Editor: Fixed an issue where the Game view layout was not changing when the application was paused. ([1104417](https://issuetracker.unity3d.com/issues/editor-maximized-game-view-doesnt-get-minimized-after-disabling-the-maximize-on-play-and-toggling-pause-button))
    
*   Editor: Fixed an issue where the IME input was causing text duplication in the Editor. (1117859, 1117878)
    
*   Editor: Fixed an issue where the Inspector did not display GUI label tooltips. (1057359)
    
*   Editor: Fixed an issue where the Layers drop-down menu in the Inspector did not list grouped Layers properly. ([1068422](https://issuetracker.unity3d.com/issues/creating-layer-groups-with-the-slash-symbol-creates-multiple-groups-with-the-same-name-containing-only-a-single-layer))
    
*   Editor: Fixed an issue where the mouse position was offset in the Game view when using IMGUI. (1097051)
    
*   Editor: Fixed an issue where the preview icon for the Material Preset flickered. ([1099296](https://issuetracker.unity3d.com/issues/presets-material-preset-preview-icon-flickers-when-viewing-a-material-preset-in-the-inspector))
    
*   Editor: Fixed an issue where the RuntimeInitializeOnLoadMethodAttribute was ignored inside player-only code blocks (such as when using #if !UNITY\_EDITOR) and inside player-only assemblies created with an Assembly Definition. ([922692](https://issuetracker.unity3d.com/issues/conditional-compilation-problem-with-runtimeinitializeonloadmethod), 1071599)
    
*   Editor: Fixed an issue where the Scene icon was not updated after the png file was changed. (1084630)
    
*   Editor: Fixed an issue where `LoadSceneAsync` would not trigger subscribed callbacks on load. ([1049526](https://issuetracker.unity3d.com/issues/after-loading-editorapplication-dot-loadlevelasyncinplaymode-the-subscribed-completed-event-doesnt-triggers))
    
*   Editor: Fixed an issue with overriden main menu shortcuts.
    
*   Editor: Fixed an issue with project update from 2017.4 to 2019.1. ([1099240](https://issuetracker.unity3d.com/issues/2019-dot-1-a-fatal-error-is-thrown-after-updating-a-project-from-2017-dot-4-to-2019-dot-1))
    
*   Editor: Fixed arrow keys logging errors in editor log slowing down editor.
    
*   Editor: Fixed button style is not correct in texture inspector.
    
*   Editor: Fixed clutch shortcut stuck if key is released while editor is not in focus.
    
*   Editor: Fixed crash when building player with Services enabled, and using .NET 3.5. ([1103349](https://issuetracker.unity3d.com/issues/deployment-management-editor-crashes-when-building-a-project-for-any-platform-with-services-enabled))
    
*   Editor: Fixed custom layout menu items getting out of sync with Shortcut Manager. ([1097041](https://issuetracker.unity3d.com/issues/assigning-shortcuts-to-editor-layout-not-working))
    
*   Editor: Fixed CustomEditorAttributes scanning order (1108536)
    
*   Editor: Fixed default shortcuts for Cut/Copy/Paste/Select All/Undo/Redo menu items not usable for other commands in Shortcuts window.
    
*   Editor: Fixed Editor crashes on `HomeWindowHandler::LearnTabOpenedCallback` while opening Project or entering Play Mode. ([1090455](https://issuetracker.unity3d.com/issues/wild-crash-editor-crashes-on-homewindowhandler-learntabopenedcallback-while-opening-project-or-entering-play-mode))
    
*   Editor: Fixed game view dimensions to address issue where `Camera.ScreenPointToRay` returned slightly offset coordinates when drawing the Ray from the main camera to the mouse position. ([1083316](https://issuetracker.unity3d.com/issues/box-colliders-position-has-a-slight-offset-when-using-a-raycast-to-hit-it))
    
*   Editor: Fixed generic menu issue related to incorrect grouping of child menu item's when parent menu item contains space(" ") as its last character. ([1116792](https://issuetracker.unity3d.com/issues/guicontent-items-in-genericmenu-containing-spaces-before-the-slash-symbol-are-not-grouped-correctly), 1129941)
    
*   Editor: Fixed Hiding objects in the scene view does not work with SRP ([1105161](https://issuetracker.unity3d.com/issues/hiding-objects-in-the-scene-view-does-not-work-with-srp))
    
*   Editor: Fixed Hierarchy view hover issues (1131017, 1131031)
    
*   Editor: Fixed invalid screen parameters when multiple game views instances are active. ([1110671](https://issuetracker.unity3d.com/issues/game-view-does-not-scale-correctly-on-resizing-it-when-multiple-game-views-are-open-in-the-editor), 1131010)
    
*   Editor: Fixed issue where holding arrow keys sometimes caused editor to stop redrawing.
    
*   Editor: Fixed issue where Unity would crash when the Save Assets dialog box displayed before exiting the Editor. ([1062146](https://issuetracker.unity3d.com/issues/unity-crashes-when-saving-animation-clip-with-verify-saving-assets-setting-checked))
    
*   Editor: Fixed key down events dispatched twice if not used.
    
*   Editor: Fixed menu items forgetting their default shortcut bindings.
    
*   Editor: Fixed performance issues when using the Test Runner for Projects with many assemblies.
    
*   Editor: Fixed performance regressions related to UIElements moving out of experimental (1103391)
    
*   Editor: Fixed scene visibility column hiding the search path of the hierarchy ([1114645](https://issuetracker.unity3d.com/issues/hierarchy-search-path-display-is-obscured-by-the-visibility-icons-area-when-searching), 1122512)
    
*   Editor: Fixed serialization issue in which MonoBehaviours with no script would cause a crash while saving the Scene. ([925313](https://issuetracker.unity3d.com/issues/crash-in-output-l-when-saving-the-scene))
    
*   Editor: Fixed standard macOS text editing key bindings inside web views.
    
*   Editor: Fixed state propagation when a VisualElement is added to a hierarchy. (1093728)
    
*   Editor: Fixed strip debug info from release editor. (1070559, 1126323)
    
*   Editor: Fixed text fields in Save Scenes dialog window not being navigable using arrow keys.
    
*   Editor: Fixed the **Verify Save Assets** option to work in the Linux Editor. ([957853](https://issuetracker.unity3d.com/issues/linux-editor-files-are-not-saved-if-verify-saving-assets-is-enabled))
    
*   Editor: Fixed unhideable material's render queue for Scriptable Render Pipelines using Shader Graph. (1108637)
    
*   Editor: Generated for `mcs.rsp` references. (1053714)
    
*   Editor: Made changes so that Unity Test Runner won't execute the PrebuildSetup code for ignored playmode tests or tests disabled on the selected platform.
    
*   Editor: Made the `VisualElementAsset` id field deterministic. (1100451)
    
*   Editor: Made `MinMaxslider` `dragElement` position absolute. Previously it was relative, which broke layouts. (1090242)
    
*   Editor: Make sure that modules depeding on disabled modules are also disabled
    
*   Editor: Make sure that we bail out immediately when dragging a preset on a UnityObject that already has the dragged component ([1074291](https://issuetracker.unity3d.com/issues/endlayoutgroup-error-is-thrown-when-adding-preset-of-an-already-added-component))
    
*   Editor: Minimize button("-") does not work for Scene, Game, Hierarchy etc. windows on Mac. ([1117896](https://issuetracker.unity3d.com/issues/editor-minimize-button-doesnt-work-for-scene-game-hierarchy-etc-windows-on-mac), 1118033)
    
*   Editor: Null reference fix for semversion ([1129026](https://issuetracker.unity3d.com/issues/scripting-console-spammed-with-errors-when-version-defines-saved), 1141029)
    
*   Editor: Prefab Component overrides now remain visible in the Inspector after a domain reload. (1102487)
    
*   Editor: Recover from modal window being closed using the X button (windows)
    
*   Editor: Removed an extra separator from the context menu in the Hierarchy window. (1080882)
    
*   Editor: Removed cursor warning when calling `Cursor.SetCursor` on a texture loaded from an asset bundle. ([1028350](https://issuetracker.unity3d.com/issues/cursor-dot-setcursor-prints-invalid-texture-used-warning-when-the-texture-is-loaded-with-assetbundles))
    
*   Editor: Removed duplicate for Rider path discovery on Linux.
    
*   Editor: Renamed the **Child Controls Size** property to **Control Child Size** in the **Horizontal Layout Group** and **Vertical Layout Group** components. ([1090329](https://issuetracker.unity3d.com/issues/horizontal-layout-group-and-vertical-layout-group-child-controls-size-fields-are-mislabelled))
    
*   Editor: Renamed the UI **Transparency Priority** to **Renderer Priority** in the **MeshRenderer** component.
    
*   Editor: Show imported components on Model asset prefabs again (was hidden because we don't want to show components for normal prefab assets)
    
*   Editor: The **Strip Engine Code** setting is now available only in Player pettings for platforms that support stripping unused code.
    
*   Editor: The number of available glyphs is now a criterion in fallback font selection. The falback font system selects the matching font with the most available glyphs. ([1090134](https://issuetracker.unity3d.com/issues/linux-editor-symbol-characters-not-shown-slash-entered-in-text-fields))
    
*   Editor: Unity now displays an error message when recent projects contain an invalid or missing `ProjectSettings.txt` file. ([1002683](https://issuetracker.unity3d.com/issues/merge-conflict-in-projectversion-dot-txt-causes-unable-to-parse-file-error-on-any-project-opened))
    
*   Editor: Update OSX container window floating window icons (1102525)
    
*   Editor: Update toolbox handling for rider path detection
    
*   Editor: Updated Windows splash screen.
    
*   GI: Fix crash on application exit when GPU lightmapper openCL context is lost.
    
*   GI: Fixed a bug where a probeset with completely overlapping positions would cause the deringing settings array to become shifted.
    
*   GI: Fixed an issue in the GPU Lightmapper that stabilizes noise when iterating on lighting.
    
*   GI: Fixed an issue where GICache errors were thrown when baking Terrain with trees having deringing enabled on the light probes. ([1100362](https://issuetracker.unity3d.com/issues/gicache-errors-are-thrown-when-baking-terrain-with-trees-having-deringing-enabled-on-the-light-probes))
    
*   GI: Fixed an issue where running `UpdateMaterials` was causing performance issues.
    
*   GI: Fixed an issue where supersampling was introducing interdeterministic results with direct samples. It now uses round-robin sampling between supersamples. ([936693](https://issuetracker.unity3d.com/issues/plm-supersampling-renders-indeterministic-results-with-direct-samples))
    
*   GI: Fixed an issue where the bake could split out "Assertion failed on expression: 'm\_NumInstanceTransforms == m\_NumInstanceLODGroups'" and produce incorrect results for Scenes with LODs in them. It could occur when entering avatar configuration when baking or making sweeping changes to instances contained in the Scene. (1102752)
    
*   GI: Fixed an issue where the lightmap preview window didn't get cleared when lightmaps were removed. ([1082621](https://issuetracker.unity3d.com/issues/ui-per-renderer-lightmap-preview-is-not-cleared-after-disabling-gi-and-rebaking))
    
*   GI: Fixed an issue where the Reflection Probes progress bar didn't get cleared when cancelling.
    
*   GI: Fixed an issue where Unity would try to load incompatible serialized lighting data from cache and print out "Failed to load '\*\*\*' because it was serialized with a newer version of Unity. (Has a higher SerializedFile version).". (1112513, 1129760)
    
*   GI: Fixed file reading errors with hashID.ghd while baking lighting. ([1047087](https://issuetracker.unity3d.com/issues/plm-failed-reading-errors-with-hashid-dot-ghd-while-baking))
    
*   GI: Fixed hashing issue when writing out AO textures for PLM.
    
*   GI: Fixed issue where the UV Overlap preview didn't display after a manual bake. ([1087688](https://issuetracker.unity3d.com/issues/ui-baked-uv-overlap-mode-isnt-loaded-after-selecting-it-in-the-lightmap-preview-window))
    
*   GI: Fixed the API documentation for `Lightmapping.Clear` and `Lightmapping.ClearLightingDataAsset`.
    
*   GI: Fixed the Baked UV Charts debug lightmap. (1078533)
    
*   GI: Fixed the Editor log outputs ''d3d11: failed to lock buffer \[HASH\].'' while baking using CPU PLM. ([1095976](https://issuetracker.unity3d.com/issues/editor-log-outputs-d3d11-failed-to-lock-buffer-0000021b7f5b94e0-of-size-85222-0x8007000e-dot-while-baking-using-cpu-plm))
    
*   GI: Fixed the indirect intensity slider in the Progressive Lightmapper so that it now also affects indirect probe lighting. ([1060939](https://issuetracker.unity3d.com/issues/indirect-intensity-slider-has-no-effect-on-lightprobes-in-progressive-backends))
    
*   GI: GPU Lightmapper, fix number of bounces (was doing two extra).
    
*   GI: GPU Lightmapper, use interpolated vertex normal when shading bounce light, rather than plane normal.
    
*   GI: GPU Lightmapper: Ensure OpenCL kernel are recompiled on Nvidia even when only the include files changes.
    
*   GI: GPU Lightmapper: For baking default is to select the same graphic hardware as the editor.
    
*   GI: Improved sampling when baking lightmaps in scenes with translucent objects. ([1132640](https://issuetracker.unity3d.com/issues/cpu-plm-correlation-artifacts-when-using-semi-transparent-surfaces), 1133463)
    
*   GI: Renamed "Auto Bake On/Off" to "Auto Generate Lighting On/Off" in the app bar.
    
*   Graphics: Added a fix so HDR Mode in Graphics Settings is respected in LWRP. ([1104140](https://issuetracker.unity3d.com/issues/lwrp-graphics-settings-hdr-mode-is-being-ignored))
    
*   Graphics: Added extra validation for RT volumeDepth. (1096019)
    
*   Graphics: Assert '0 == m\_CurrentBuiltInBindMask' in HDRP test when Async Shader Compilation is ON (1117989, 1122369)
    
*   Graphics: Choose the correct occlusion camera when occlusion visualization is turned on
    
*   Graphics: Do not render the skybox in the scene view if using an SRP as the SRP will handle the skybox render.
    
*   Graphics: DX11: Fix for not being able to bind a a 2D Render Texture with a slice index of -1.
    
*   Graphics: Fix crash when stripping Umbra module on platforms supporting native code stripping. (1116487, 1118313)
    
*   Graphics: Fix crash when usign DrawMeshInsted with SRP batcher enabled (1122017, 1122357)
    
*   Graphics: Fix for postprocessing and instanced stereo rendering only a white screen in LWRP ([1100898](https://issuetracker.unity3d.com/issues/xr-graphics-lwrp-postprocess-when-using-post-process-effects-with-lwrp-and-instancing-stereo-rendering-only-a-white-screen))
    
*   Graphics: Fix issue with argument buffer not being bound properly (only a subset of the view was bound)
    
*   Graphics: Fix memory leak in Mac threaded texture creation (1126615, 1127347)
    
*   Graphics: Fixed a crash that happened when creating a `Texture2DArray` with a YUY2 `TextureFormat`. ([1094777](https://issuetracker.unity3d.com/issues/macos-creating-a-texture2darray-with-a-yuy2-textureformat-crashes-the-editor))
    
*   Graphics: Fixed a Frame Debugger texture tooltip, so it shows correct dimension info for 3D textures.
    
*   Graphics: Fixed a performance issue that prevented GPU drivers from utilizing internal texture compression. (Not applicable to RenderTexture.)
    
*   Graphics: Fixed a warning message in the Editor for Mac OS with an Android build target, where a warning would show up for decompressing ETC textures. (1115543, 1120074)
    
*   Graphics: Fixed an issue that would deplete memory when trying to compile Shaders that uses a self-referencing macro. ([1104217](https://issuetracker.unity3d.com/issues/mobile-os-restarts-because-of-high-memory-usage-when-compiling-shaders-for-opengles2))
    
*   Graphics: Fixed an issue where activated second display is not rendering when running the project in Standalone ([1099190](https://issuetracker.unity3d.com/issues/activated-second-display-is-not-rendering-when-running-the-project-in-standalone))
    
*   Graphics: Fixed an issue where copying raw depth buffers caused a crash. ([1040591](https://issuetracker.unity3d.com/issues/copying-directional-light-depthmap-in-rawdepth-mode-crashes-unity-editor))
    
*   Graphics: Fixed an issue where Frame Debugger was showing bad keywords when connected to a standalone Player. ([1070614](https://issuetracker.unity3d.com/issues/frame-debugger-does-not-display-all-additional-shader-keywords-when-debugging-a-built-player))
    
*   Graphics: Fixed an issue where Inspector Previews were using black cubemaps for environment reflection. ([1039018](https://issuetracker.unity3d.com/issues/metallic-objects-are-very-dark-in-the-preview-window))
    
*   Graphics: Fixed an issue where MeshTopology.Quads generated a draw call that uses 3 point patches instead of 4. ([1078885](https://issuetracker.unity3d.com/issues/meshtopology-dot-quads-generates-a-draw-call-that-uses-3-point-patches-instead-of-4-point))
    
*   Graphics: Fixed an issue where Reflection Probes weren't rebaking in the Editor after changes were made to the Shader code of the renderers used in the baked Reflection Probes. ([1020358](https://issuetracker.unity3d.com/issues/srp-template-template-geometry-is-hot-pink))
    
*   Graphics: Fixed an issue where the **Package Manager** UI was not rendering correctly on GLES2. ([1108286](https://issuetracker.unity3d.com/issues/package-manager-window-is-rendering-blobs-instead-of-letters-for-lwrp-in-glsl2), 1117897)
    
*   Graphics: Fixed an issue with Animator preview not rendering grids in Sciptable Render Pipelines. (1044281)
    
*   Graphics: Fixed async readback when using Vulkan.
    
*   Graphics: Fixed blicking when rendering at native resolution in fullscreen with OpenGL on Windows ([1039035](https://issuetracker.unity3d.com/issues/graphic-errors-slash-glitches-when-running-player-fullscreen))
    
*   Graphics: Fixed crash that infrequently occurred when instancing properties were absent from the MaterialPropertyBlock object sent to DrawMeshInstanced calls. (1115627, 1124733)
    
*   Graphics: Fixed Crash when calling Graphics.ExecuteCommandBuffer() if CommandBuffer.SetShadowSamplingMode() is used before it ([1102773](https://issuetracker.unity3d.com/issues/crash-when-calling-graphics-dot-executecommandbuffer-if-commandbuffer-dot-setshadowsamplingmode-is-used-before-it), 1124728)
    
*   Graphics: Fixed crash when user-created RT has an unsupported sample count. (1095433)
    
*   Graphics: Fixed Fog settings not being preserved for the additively loaded Scenes. ([1024864](https://issuetracker.unity3d.com/issues/lighting-settings-mix-settings-from-two-different-scenes-in-multi-scene-editing))
    
*   Graphics: Fixed graphics format that should support random writes. ([1096000](https://issuetracker.unity3d.com/issues/opengl-rendertexture-dot-create-failed-format-unsupported-for-random-writes-rgba4-unorm-7))
    
*   Graphics: Fixed loading of compressed textures with incomplete mipmap chains. ([1045189](https://issuetracker.unity3d.com/issues/opengl-unity-can-only-read-1-mipmap-from-dot-ktx-textures-when-the-texture-was-compressed-using-etc), 1115580)
    
*   Graphics: Fixed memory leak in metal threaded texture creation (1126615, 1127347)
    
*   Graphics: Fixed memory overwrites in the DX11 render target setting code.
    
*   Graphics: Fixed problem so that the correct SubShader is selected when rendering with the Editor Camera.
    
*   Graphics: Fixed RenderTexture asset UI preventing to select the color format ([1115203](https://issuetracker.unity3d.com/issues/render-texture-inspector-enum-broken), 1115204)
    
*   Graphics: Fixed RenderTexture asset UI to lose selected format data when the selected format is not supported. ([1116500](https://issuetracker.unity3d.com/issues/render-texture-enum-can-lose-users-data), 1116501)
    
*   Graphics: Fixed scene view rendering default skybox when SRP is enabled ([1076246](https://issuetracker.unity3d.com/issues/sceneview-renders-legacy-skybox-when-custom-rp-is-active))
    
*   Graphics: Fixed scissor/viewport handling when used with Dynamic Resolution feature.
    
*   Graphics: Fixed sRGB RenderTexture failing to be created when enableRandomWrite is on (1115223, 1115226)
    
*   Graphics: Fixed support for 32 bit vertex index buffer sub-mesh on dx11 during SRP batching. ([1117383](https://issuetracker.unity3d.com/issues/srp-batcher-doesnt-support-32-bit-vertex-index-buffer-mesh-on-dx11), 1120326)
    
*   Graphics: Fixed Texture.allowThreadedTextureCreation to correctly allow control of which thread textures are created on. (1131041, 1132127)
    
*   Graphics: Fixed Vulkan-Enabled GPU skinning for blend shapes. ([1134323](https://issuetracker.unity3d.com/issues/2019-dot-1-vulkan-directx-11-using-models-with-blend-shapes-causes-the-skinning-to-happen-on-the-cpu-instead-of-the-gpu), 1138973)
    
*   Graphics: Improved RenderTexture asset UI to store the user requested format ([1115203](https://issuetracker.unity3d.com/issues/render-texture-inspector-enum-broken), 1115204)
    
*   Graphics: Made changes to explicitly disallow the destroying of temporary render textures. ([1070564](https://issuetracker.unity3d.com/issues/calling-destroyimmediate-after-rendertexture-dot-releasetemporary-causes-the-crash-in-renderbuffermanager-textures-gettempbuffer))
    
*   Graphics: Made changes to skip shadow lights and shadow casters culling when shadows are disabled. ([1072624](https://issuetracker.unity3d.com/issues/osx-shadows-disabling-shadows-in-quality-settings-doesnt-stop-shadow-caster-culling))
    
*   Graphics: Optimizes single-colored ambient probe updates. ([1115645](https://issuetracker.unity3d.com/issues/the-rendersettings-dot-ambientlight-color-is-changing-inconsistenly-when-using-color-dot-lerp), 1136076)
    
*   Graphics: Reinstated support for reading Terrain Brush Textures. (1102243)
    
*   Graphics: Renamed **Renderer Priority** to **Priority** in the **Mesh Renderer** component.
    
*   Graphics: Vulkan: Disabled error messages when attempting to draw with missing bindings
    
*   Graphics: Vulkan: Fixed a race condition between updating ComputeBuffers from script and rendering from them within Graphics jobs.
    
*   Graphics: Vulkan: Fixed crash when rendering reflection probes on Android
    
*   Graphics: Vulkan: Fixed crash with certain shaders
    
*   Graphics: Vulkan: Fixed debug marker locations in RenderDoc trace
    
*   Graphics: Vulkan: Fixed various issues with FPS Samplegame
    
*   Graphics: (1086957)
    
*   IL2CPP: Add support for building with Xcode 10 and the macOS 10.14 SDK.
    
*   IL2CPP: Avoid using managed exceptions during time zone initialization. This cause cause crashes on some platforms. (1100856, 1117453)
    
*   IL2CPP: Correct a build error when script debugging is enabled for a project with no user scripts. ([1082185](https://issuetracker.unity3d.com/product/unity/issues/guid/1082185))
    
*   IL2CPP: Fixed IL2CPP build failing if Visual Studio 2019 is installed on the machine.
    
*   IL2CPP: Fixed invoking IEnumerable.GetEnumerator method on COM objects that implemenet Windows.Foundation.Collections.IIterable interface. ([878766](https://issuetracker.unity3d.com/issues/invoking-system-dot-collections-dot-ienumerable-dot-getenumerator-fails-on-native-objects-that-dont-implement-ibindablevector-interface), 1127105)
    
*   IL2CPP: Fixes a compilation error that can occur when the debugger is enabled but there are no source files specified in the symbol data. (1078027)
    
*   IL2CPP: Fixes an issue with UnsafeUtility.SizeOf() crashing IL2CPP when called with an enum type.
    
*   IL2CPP: Fixing an unhandled exception in IL2CPP. Adding support for pointer types when executing an initobj instruction.
    
*   IL2CPP: Prevent a compilation error in generated C++ code when the ldtoken opcode is used in some cases.
    
*   IL2CPP: Prevent a possible crash when a list of generic or nullable types with a field that is a struct with explicit layout is reallocated. (1121969, 1122739)
    
*   IL2CPP: Prevent finalizer from being incorrect injected for COM types.
    
*   IL2CPP: Support the AttributeType property of of the TypeInfo object.
    
*   Input: Added a fix in the new input system to correctly set and get sampling frequencies for sensors on iOS and Android platforms.
    
*   iOS: Added a fix so `DISABLE_TOUCH_DELAYS` does not create a warning on iOS 12 devices. ([1087337](https://issuetracker.unity3d.com/issues/ios-disable-touch-delays-define-causes-a-warning-on-ios-12-devices))
    
*   iOS: Added a fixed so `Screen.allowedOrientations` is not updated every frame. (1103167)
    
*   iOS: Fix warnings related to launch image when building for iOS in Xcode 10 ([1085602](https://issuetracker.unity3d.com/issues/ios-game-crashes-when-forcing-portrait-upside-down-orientation-on-iphone-xs-slash-xs-max))
    
*   iOS: Fixed a Lighweight Render Pipeline crash on several SoCs ([1098913](https://issuetracker.unity3d.com/issues/ios-lwrp-execution-of-the-command-buffer-was-aborted-error-is-being-thrown-when-launching-template-project))
    
*   iOS: Fixed an issue where a full screen movie reset after the app was minimized ([840951](https://issuetracker.unity3d.com/issues/handheld-dot-playfullscreenmovie-movie-resets-when-minimizing-and-maximizing-the-application))
    
*   iOS: Fixed an issue where changing `Screen.Orientation` on some iOS devices would not update the variable that holds the current orientation state ([1088729](https://issuetracker.unity3d.com/issues/ios-screen-dot-orientation-returns-wrong-value-on-some-devices-when-specific-orientation-was-forced-after-few-states))
    
*   iOS: Fixed an issue where particles were being rendered over non-transparent objects in a Low Poly Strategy Prototyper project ([1107546](https://issuetracker.unity3d.com/issues/metal-ios-some-particles-are-being-rendered-over-non-transparent-objects-in-low-poly-strategy-prototyper-project), 1122520)
    
*   iOS: Fixed crash on startup on 32bit devices using oldish iOS ([1109610](https://issuetracker.unity3d.com/issues/ios-bad-access-exception-thrown-on-deploying-build-on-devices-with-ios-version-10-or-lower), 1117891)
    
*   iOS: Fixed DiscardContents and GrabIntoRenderTexture interop on Metal ([1082159](https://issuetracker.unity3d.com/issues/ios-depth-texture-in-commandbuffer-and-customized-depth-of-field-shader-will-damage-the-rendertexture))
    
*   iOS: Fixed incorrect `Screen.safeArea` on plus sized iPhones ([1087954](https://issuetracker.unity3d.com/issues/ios-a-bunch-of-launch-image-warnings-are-thrown-when-building-for-ios-in-xcode-10))
    
*   iOS: Fixed issues with reporting orientation when autorotating and tweaked enabled orientations ([1075839](https://issuetracker.unity3d.com/issues/ios-screen-dot-orientation-returns-upsidedown-value-after-using-screen-dot-autorotatetoportrait-when-device-is-in-portrait-mode), [1075855](https://issuetracker.unity3d.com/issues/ios-unity-rendering-in-wrong-screen-orientation-after-auto-rotation-on-ios-using-screen-dot-orientation))
    
*   iOS: Fixed UnauthorizedAccessException when building for iOS (1108549)
    
*   iOS: Uncoupled the accelerometer from the gyroscope ([1085244](https://issuetracker.unity3d.com/issues/ios-the-accelerometer-stops-working-when-disabling-the-gyroscope-in-build))
    
*   iOS: `Gamepad.startButton` works correctly. The iOS `startButton` (or Menu button) only reports a down event and an up event is simulated immediately after to simulate a click. ([1093829](https://issuetracker.unity3d.com/issues/ios-gamepad-gamepad-dot-current-dot-startbutton-doesnt-return-expected-value), 1132630)
    
*   iOS: `Keyboard.onTextInput` and `Keyboard.onIMECompositionChange` correctly calls for physical and virtual keyboard events.
    
*   iOS: `Pen.tilt` values are correctly returned in the new input system ([1093816](https://issuetracker.unity3d.com/issues/ios-pen-tilt-dot-x-is-centered-on-1-dot-5-and-goes-to-0-when-tilting-both-left-and-right), 1132629)
    
*   Kernel: Fixed a temp job warning in C# jobs when the job was executing for longer than one frame.
    
*   Linux: Added a fix for touchpad sced an issue where touchpad scrolling was too sensitive in the Linux Editor. ([1073152](https://issuetracker.unity3d.com/issues/linux-scroll-sensitivity-of-touchpad-is-too-high))
    
*   Linux: Added a fix to allow Linux and Mac launch the BugReport crash handler when a SIGABRT is sent. ([1074324](https://issuetracker.unity3d.com/issues/linux-editor-forcecrash-forcedcrashcategory-dot-abort-not-being-caught-by-crash-reporter))
    
*   Linux: Fix crash on Editor startup when using -force-vulkan ([1109529](https://issuetracker.unity3d.com/issues/unity-cannot-start-if-force-vulkan-is-used-in-linux), 1123925)
    
*   Linux: Fix using multiple identical webcams on Linux ([1115884](https://issuetracker.unity3d.com/issues/linux-when-using-2-identical-webcams-with-same-name-second-webcam-does-not-return-frames), 1123759)
    
*   Linux: Fixed an Editor windows repaint bug in Ubuntu 16.04. (1107716)
    
*   Linux: Fixed an issue where tabs were incorrectly processed twice. ([1080441](https://issuetracker.unity3d.com/issues/linux-editor-android-key-creation-dialog-tabbing-skips-every-other-field))
    
*   Linux: Fixed annoying "'Unity' is not responding" message on Linux. ([1072712](https://issuetracker.unity3d.com/issues/gnome-pops-application-is-not-responding-dialog-behind-fullscreen-player-preventing-further-interaction-with-the-player), 1122090)
    
*   Linux: Fixed issue with keyboard input not being captured by the Game view when in Play mode ([1109908](https://issuetracker.unity3d.com/issues/linux-focus-cannot-be-properly-gained-on-play-mode-making-keyboard-input-switch-screens), 1118063)
    
*   Linux: Fixed Linux Editor executable being much larger than it used to be (1.2GB instead of ~350MB)
    
*   Linux: Fixed progress bar freeze when sprite assets have invalid names ([1106232](https://issuetracker.unity3d.com/issues/editor-freeze-when-creating-tile-assets-with-special-characters-star-in-the-name), 1115875)
    
*   Linux: Strong Input lag when locking cursor and using mouse with 1000hz polling rate ([1023587](https://issuetracker.unity3d.com/issues/linux-strong-input-lag-when-using-standart-asset-pack-and-mouse-with-1000hz-pooling-rate), 1118295)
    
*   Linux: Unity Editor and Build dips in Frame count when scrolling with the Mouse Wheel (1066760, 1117507)
    
*   Linux: \[Linux\]\[Editor\]Fixed Shift+tab selects previous window instead of previous tabbed element. (1107323, 1117698)
    
*   Lumin: Fixed an issue where the minimum platform API level in a custom manifest was not being respected.
    
*   LWRP: Fixed RenderTexture sRGB flag set incorrectly. ([1133874](https://issuetracker.unity3d.com/issues/lwrp-scene-darkens-when-using-antialiasing-in-gamma-lighting-if-hdr-is-not-on), 1136097)
    
*   Mobile: Added support for Bluetooth headphones' microphone for both Android and iOS ([946201](https://issuetracker.unity3d.com/issues/mobile-support-for-bluetooth-headphones-microphone))
    
*   Mobile: Fixed Ambient Occlusion in PostProcessing v2 ([1059893](https://issuetracker.unity3d.com/issues/ios-post-processing-ambient-occlusion-does-not-work))
    
*   Mobile: Fixed an issue where reflection was distorted when using baked reflection probes ([1114605](https://issuetracker.unity3d.com/issues/mobile-reflection-is-distorted-when-using-baked-reflection-probes), 1117116)
    
*   Mobile: Fixed an issue where the `TargetFPS` and `vSyncCount` has no effect on the FPS ([1078663](https://issuetracker.unity3d.com/issues/razer-phone-targetfps-and-vsynccount-has-no-effect-on-the-actual-fps), 1136554)
    
*   Mobile: Fixed Standard shader artifacts on mobiles
    
*   Mobile: Fixed the Crunch decoder to avoid access out of vector boundaries ([983436](https://issuetracker.unity3d.com/issues/ios-player-crashes-at-decode-alpha-selectors-etc-when-decoding-crunched-etc-texture), 1140135)
    
*   Multiplayer: Fixed issue where the unet hlapi package was not being automatically added to old projects opened in 2019.1, bumped version in editor manifest to 1.0.1 as well
    
*   OSX: Fix Empty Project builds for Mac/Win/Linux Standalone contain extra ~4MB of doc .xml files (1112215, 1125589)
    
*   OSX: Fixed an issue building the Mac Editor using customer source code distributions
    
*   OSX: Fixed an issue where Unity would crash if the resolution was set to invalid values via script. ([1070915](https://issuetracker.unity3d.com/issues/mac-standalone-after-set-the-width-and-height-to-be-0-player-quits-then-crashes))
    
*   OSX: Fixed GPU selector always being disabled. ([1055634](https://issuetracker.unity3d.com/issues/mac-cant-change-graphics-device-to-use-in-standalone-built-project))
    
*   OSX: Fixed issue where the option "Use Metal Editor" did not display on some versions of Unity. (1094058)
    
*   OSX: Fixed occasional crash when using Camera (be it FaceTime or coming from UnityRemote) ([1101944](https://issuetracker.unity3d.com/issues/ios-unity-remote-5-getting-assertion-failed-on-expression-uploaddstformat-equals-equals-format-errors-on-ios-device), [1110670](https://issuetracker.unity3d.com/issues/graphics-crash-when-running-a-particular-scene), 1115830, 1116526)
    
*   OSX: Fixed the icon at 128x128 being corrupt in macOS build ([1038984](https://issuetracker.unity3d.com/issues/macos-deployment-the-icon-at-128x128-is-corrupt-in-macos-build), 1132657)
    
*   OSX: Metal: Unity applications now correctly reported as "Requires High Perf GPU" in Activity Monitor (1055912)
    
*   Package Manager: A "Failed to fetch versions information" error would be displayed in Package Manager window for all unknown packages.
    
*   Package Manager: Add a warning message if you disable a package and that causes dependencies to also be disabled.
    
*   Package Manager: Add information to compiler errors explaining if a package has been disabled as a dependency of another package
    
*   Package Manager: Add information to info messages for disabled components in the inspector explaining if a package has been disabled as a dependency of another package
    
*   Package Manager: Added opening offline documentation when the online documentation is not accessible.
    
*   Package Manager: Fix an issue that prevented specific native plugins to be correctly identified the second time a project was loaded.
    
*   Package Manager: Fix an issue where packages would not be found because the project configured registry URL ended with an extraneous slash.
    
*   Package Manager: Fix Closing the 'Reset Packages to Defaults' confirmation window still resets the Packages. ([1134754](https://issuetracker.unity3d.com/issues/closing-the-reset-packages-to-defaults-confirmation-window-still-resets-the-packages), 1137060)
    
*   Package Manager: Fix for upgraded projects that use XR or Timeline and have disabled modules ([1111566](https://issuetracker.unity3d.com/issues/package-manager-ui-does-not-show-up-and-there-are-compilation-errors-when-upgrading-projects-to-2019-dot-1), 1115043)
    
*   Package Manager: Fix imcompatible packages showing up in the list of packages to install ([1066979](https://issuetracker.unity3d.com/issues/package-manager-window-is-empty-when-package-manager-ui-package-is-updated))
    
*   Package Manager: Fix incorrect text with the update button when a package is being installed (1124632, 1139328)
    
*   Package Manager: Fix Package Manager timeouts when opening a project inside a closed network.
    
*   Package Manager: Fix Package Manager UI refreshes the package list when entering play mode ([1135815](https://issuetracker.unity3d.com/issues/package-manager-ui-refreshes-the-package-list-when-entering-play-mode), 1135840)
    
*   Package Manager: Fixed a **Package Manager** error displaying "Input string was not in a correct format" when using Locales with the `,` number separator ([1131566](https://issuetracker.unity3d.com/issues/package-manager-throws-system-dot-formatexception-input-string-was-not-in-a-correct-format-errors-when-using-pl-pl-locale), 1139270)
    
*   Package Manager: Fixed an issue where an error message appeared when dragging the Packages folder in to the Favorites section. ([1084176](https://issuetracker.unity3d.com/issues/move-of-a-savedfilter-has-invalid-input-errors-appear-when-dragging-packages-folder-on-to-favorite-section-in-project-window))
    
*   Package Manager: Fixed an issue where native plugins inside a package would not get resolved on OSX
    
*   Package Manager: Made changes so packages that aren't installed are shown in package manager window. ([1098870](https://issuetracker.unity3d.com/issues/not-installed-packages-are-shown-in-package-manager-window))
    
*   Package Manager: Made changes so that packages, which are imported as dependencies for other packages, are not shown in Package Manager UI. ([1057210](https://issuetracker.unity3d.com/issues/packages-that-are-imported-as-dependencies-for-other-packages-are-not-shown-in-package-manager-ui))
    
*   Package Manager: The Asset Database refresh could hang when removing or updating the version of an installed package.
    
*   Package Manager: Use SemVer in core packages instead of 0.0.0-builtin
    
*   Particles: Apply collisions during the initial simulation step of newly spawned particles. ([1082981](https://issuetracker.unity3d.com/issues/some-particles-fail-to-collide-with-the-object-when-spawning-a-lot-of-particles-at-once), 1120773)
    
*   Particles: Apply the Simulation Speed modifier to the initial simulation step when spawning new particles ([1111729](https://issuetracker.unity3d.com/issues/particle-systems-height-slash-distribution-in-play-mode-is-affected-when-changing-the-simulation-speed), 1122166)
    
*   Particles: Fixed Prefabs with Sub emitters that have emit probability of 0 by default.
    
*   Particles: Opening a legacy Prefab with a ParticleSystem in Prefab Mode: ParticleSystemRenderer component is now correctly hidden in the Inspector.
    
*   Particles: Recompute particle bounds after executing a C# Job. ([1116569](https://issuetracker.unity3d.com/issues/iparticlesystemjob-bounding-box-is-not-recalculated-after-the-job), 1120793)
    
*   Physics: CharacterController will now ignore Rigidbodies that have their collision detection turned off. ([984035](https://issuetracker.unity3d.com/issues/charactercontroller-doesnt-respect-rigidbody-dot-detectcollisions-set-to-false))
    
*   Physics: Ensured that 2D trigger/collision exit callbacks occur when destroying a GameObject inside a 2D trigger/collision callback. ([1057320](https://issuetracker.unity3d.com/issues/ontriggerexit2d-not-triggered-when-collider-gameobject-is-destroyed-from-another-colliders-ontriggerenter2d))
    
*   Physics: Ensured that 2D trigger/collision exit callbacks occur when disabling a GameObject or 2D collider component. ([1071700](https://issuetracker.unity3d.com/issues/ontriggerexit2d-is-not-being-triggered-when-disabling-other-gameobject-with-a-trigger))
    
*   Physics: Fixed a crash in the 2D physics manager on iOS upon start-up when Physics2D package is disabled. ([1080899](https://issuetracker.unity3d.com/issues/ios-crash-in-initialize-at-physicsmanager2d-before-the-splash-screen))
    
*   Physics: Fixed a crash that occurred when adding a MeshCollider without CookingOptions.CookForFasterSimulation. Fixed by PhysX 3.4 Upgrade. ([1041838](https://issuetracker.unity3d.com/issues/adding-meshcollider-meshes-without-cookingoptions-dot-cookforfastersimulation-causes-crash-in-physx-subsortquick-sort4))
    
*   Physics: Fixed a spelling issue in the Physics settings (renamed Default Max Angular Speed). ([1104527](https://issuetracker.unity3d.com/issues/default-max-angular-speed-spelling-mistake-in-physics-settings), 1127096)
    
*   Physics: Fixed an issue that occurred when copying and pasting cloth component values. ([975495](https://issuetracker.unity3d.com/issues/pasting-cloth-component-values-causes-scene-view-to-break))
    
*   Physics: Fixed PhysicsScene.SphereCast having a set of default parameters that's inconsistent with the other queries. ([1096382](https://issuetracker.unity3d.com/issues/all-arguments-are-mandatory-for-int-physicsscene-dot-spherecast-even-though-they-shouldnt-be))
    
*   Physics: Fixed poor performance of self and inter collision gizmos for cloth. ([963985](https://issuetracker.unity3d.com/issues/having-the-self-and-inter-collision-gizmos-visible-lowers-performance-significantly))
    
*   Physics: Fixed `Rigidbody.AddExplosionForce` docs that were out of sync with code. ([1108989](https://issuetracker.unity3d.com/issues/addexplosionforce-s-added-force-to-rigidbodys-velocity-is-not-proportional-to-explosion-position), 1140551)
    
*   Physics: Made the bodies connected by `ConfigurableJoint` wake up when changing parameters, to match what happens when doing this in the Editor. ([1075514](https://issuetracker.unity3d.com/issues/changing-the-linear-limit-of-a-configurable-joint-does-nothing-when-its-being-changed-by-the-script), 1140550)
    
*   Physics: Physics Fix "Selected Object Info" in Physics Debug View being expanded incorrectly ([1122474](https://issuetracker.unity3d.com/issues/selected-object-info-foldout-is-misbehaving-in-the-physics-debugger), 1134269)
    
*   Physics: RelativeJoint2D now correctly handles rotation. ([1103365](https://issuetracker.unity3d.com/issues/physics2d-relativejoint2d-should-support-driven-rotations-as-per-box2d))
    
*   Physics: Stopped NullReferenceException due to sprite-snapping when dragging a Joint2D anchor when the same GameObject contains a SpriteRenderer without an assigned Sprite. ([1077680](https://issuetracker.unity3d.com/issues/nullreferenceexception-when-moving-around-a-springjoint2d-with-a-rigidbody-reference-to-an-empty-sprite))
    
*   Prefabs: Added localization to Overrides window and PrefabUtility dialogs.
    
*   Prefabs: Do not block saving a Prefab in Prefab Mode to a new Prefab when in Animation Mode
    
*   Prefabs: Don't include Importer Error Log in source prefab file when saving from PrefabMode
    
*   Prefabs: Fix handling of Transform replacement in Prefab instances and assets
    
*   Prefabs: Fix loosing selection of Prefab root in Prefab Mode after draggging script to Inspector.
    
*   Prefabs: Fix memory leak when calculating prefab dependencies during import.
    
*   Prefabs: More robust throwing of exceptions for invalid input to PrefabUtility apply and revert methods. (1090918)
    
*   Prefabs: Prefab Mode: Fix automatic UI reparenting to leave out the prefab itself when looking for a Canvas to render with
    
*   Prefabs: PrefabMode: For broken prefabs use the root that the PrefabImporter has chosen when opening the prefab file in Prefab Mode, other dangling roots are deleted.
    
*   Prefabs: Support reparenting prefab root in Awake and OnEnable when opening Prefab Mode.
    
*   Profiler: Fix ArgumentNullException thrown by "Show Related Object" pane of Profiler Window. ([1090876](https://issuetracker.unity3d.com/issues/profiler-argumentnullexception-thrown-in-the-console-when-show-related-object-option-is-selected-for-a-sample))
    
*   Profiler: Fixed an issue where Profiler stats was recording when profiling the Editor with runtime profiler API.
    
*   Profiler: Fixed issue with increased memory usage by the profiler for long-lasting background operations. (1094748)
    
*   SceneManager: Add 'Collapse All' functionality to the Hierarchy Window to easily collapse all rows in the Hierarchy. Added to the Hierarchy window context menu. (1137167, 1138476)
    
*   SceneManager: Fix SceneHierarchy throwing null ref exception in rare cases on LostFocus events. (1136536, 1138475)
    
*   SceneManager: Fix Unity hangs after dropping a parent transform into a SubScene below it. (1136535, 1138474)
    
*   Scripting: Added `System.Data.dll` in the references. ([1075265](https://issuetracker.unity3d.com/issues/the-project-cant-be-compiled-because-library-targeting-net-standard-2-dot-0-doesnt-work))
    
*   Scripting: Assigning a custom `Debug.logger.logHandler` now intercepts thrown exceptions. ([753944](https://issuetracker.unity3d.com/issues/assigning-a-custom-debug-dot-logger-dot-loghandler-doesnt-intercept-thrown-exceptions))
    
*   Scripting: Enabled empty assembly definition references and relaxed the need for a reference on an assembly. ([1130125](https://issuetracker.unity3d.com/issues/compilation-errors-after-reimporting-the-project-that-has-an-assembly-definition-that-references-another-assembly-definitions), 1136092)
    
*   Scripting: Fix compiler error reporting in Editor.log (1115012, 1115994)
    
*   Scripting: Fix potential crash when calling Editor.CreateEditor with a type that does not derive from UnityEditor.Editor. (1119535, 1126301)
    
*   Scripting: Fixed a bug where building players with "using alias" directives pointing to types in other assemblies would fail, if those types were not actually used.
    
*   Scripting: Fixed a crash where a whole hierarchy was destroyed when `GameObject` instantiated a new `GameObject` on the parent during an `OnDestroy` callback. ([1121506](https://issuetracker.unity3d.com/issues/crash-when-instantiating-new-gameobject-with-the-parent-of-the-gameobject-that-is-being-destroyed-and-exiting-play-mode), 1125293)
    
*   Scripting: Fixed an issue where the `originalProjection` variable in the `Camera.projectionMatrix` Scripting API example was not initialized. ([1097500](https://issuetracker.unity3d.com/issues/errors-are-throw-when-using-documentation-example-of-camera-dot-projectionmatrix))
    
*   Scripting: Fixed crash when adding multiple components of a disallowed type. ([959136](https://issuetracker.unity3d.com/issues/trying-to-add-two-same-script-components-with-disallowmultiplecomponent-via-test-causes-unity-to-crash))
    
*   Scripting: Fixed invalid UTF8 characters from imported assets. ([1086920](https://issuetracker.unity3d.com/issues/copyright-symbol-c-causes-invalid-utf8-string-error-when-observing-scripts-inspector-window), 1114945)
    
*   Scripting: Fixed issue where Unity couldn't stop `Coroutine` via `StopCoroutine()` if it had three or more nested yield return coroutines. ([1089467](https://issuetracker.unity3d.com/issues/coroutine-cant-be-stopped-via-stopcoroutine-if-it-has-3-or-more-nested-yield-return-coroutines))
    
*   Scripting: Fixes potential crash when an exception is thrown during domain unload ([879906](https://issuetracker.unity3d.com/issues/potential-crash-when-exception-is-raised-in-mono-domain-unload), 1115911)
    
*   Scripting: Made changes to disallow modifications of serialized data in `m_Component` on a GameObject. ([1022204](https://issuetracker.unity3d.com/issues/the-editor-crashes-when-exiting-the-play-mode-in-the-specific-project), [1082089](https://issuetracker.unity3d.com/issues/crash-on-gameobject-isactive-when-calling-prefabutility-dot-instantiateprefab))
    
*   Scripting: Make exception errors appear in Editor console when they're received from player. ([1103744](https://issuetracker.unity3d.com/issues/debug-dot-logexception-messages-arent-shown-in-the-editors-console-when-the-player-is-connected-using-an-ip-address), 1121783)
    
*   Scripting: NET\_LEGACY is now only set when NET 2.0 or .NET 2.0 Subset profile is used.
    
*   Scripting: Small performance improvement to `Renderer.bounds`. We were doing an unnecessary call to GetComponent()
    
*   Scripting Upgrade: Fix crash when debugging with Rider ([1111226](https://issuetracker.unity3d.com/issues/crash-on-clear-assembly-from-modifiers-when-entering-play-mode-from-rider-debug), 1118829)
    
*   Scripting Upgrade: Fix GC performing unnecessary full collections when incremental GC is enabled ([1129037](https://issuetracker.unity3d.com/issues/incremental-gc-doesnt-spread-collection-across-multiple-frames), 1132628)
    
*   Scripting Upgrade: Fixed a crash from a method with too many variables. ([1103205](https://issuetracker.unity3d.com/issues/allocating-too-many-variables-in-a-method-leads-to-a-crash), 1128765)
    
*   Scripting Upgrade: Fixed a crash in `Marshal.PtrToStructure` with a generic struct. ([1106422](https://issuetracker.unity3d.com/issues/if-marshal-dot-ptrtostructure-raises-an-exception-the-editor-crashes), 1123902)
    
*   Scripting Upgrade: Fixed a crash when a delegate constructor was invoked with the NULL method. ([1091693](https://issuetracker.unity3d.com/issues/editor-crashes-with-g-logv-when-entering-play-mode-with-active-flowcanvas-script), 1123904)
    
*   Scripting Upgrade: Fixed a crash when the method has Task return type. ([1111048](https://issuetracker.unity3d.com/issues/crash-on-mono-generic-class-get-class-when-function-has-task-return-type), 1123903)
    
*   Scripting Upgrade: Fixed a hang from race condition in C# sockets on Windows. ([1028819](https://issuetracker.unity3d.com/issues/streamreader-readline-stops-receiving-messages-after-the-server-hangs), 1128764)
    
*   Scripting Upgrade: Fixed a hang when using Photon networking on Windows. ([1054137](https://issuetracker.unity3d.com/issues/photon-unity-networking-messages-timeout-when-using-net-4-dot-x), 1128761)
    
*   Scripting Upgrade: Fixed excessive garbage collection allocations when using TLS. ([1084800](https://issuetracker.unity3d.com/issues/mono-net-4-dot-x-tls-1-dot-2-excessive-gc-usage-while-reading-from-tls-stream), 1128767)
    
*   Scripting Upgrade: Fixed random crash on x86 Linux with TLS connections ("GCHandle value belongs to a different domain")
    
*   Scripting Upgrade: Fixed sizes for `System.Numerics` types. ([1118631](https://issuetracker.unity3d.com/issues/system-dot-numerics-vector-sizes-are-all-16-bytes-instead-of-8-12-and-16-bytes), 1123901)
    
*   Scripting Upgrade: Fixed the use of `DataContractJsonSerializer` with `UseSimpleDictionaryFormat` option enabled. ([1070667](https://issuetracker.unity3d.com/issues/datacontractjsonserializer-usesimpledictionaryformat-doesnt-work-when-deserializing), 1128766)
    
*   Scripting Upgrade: Fixed `GetThreadContext failed` assertion message on Windows. ([1114668](https://issuetracker.unity3d.com/issues/gc-getthreadcontext-failed-crash-when-calling-gc-dot-collect-and-yielding-the-thread), 1131234)
    
*   Shaders: Added more clean and useful editor logs on shader compiler crashes. ([1097215](https://issuetracker.unity3d.com/issues/unity-displays-millions-of-lines-of-shader-source-in-editor-log-when-the-shader-compiler-crashes-during-builds))
    
*   Shaders: Added zero-init appdata in the domain surface shader to avoid a compiler error about the out parameter not being fully initialized.
    
*   Shaders: Fixed issue where edge/inside tessellation factors were improperly handled by the metal shader compiler. ([1065883](https://issuetracker.unity3d.com/issues/metal-edge-length-tessellation-throws-compilation-error-when-using-vertex-normal-on-the-vertex-function))
    
*   Shaders: Fixed issue where the surface shader analysis step sometimes had missing inputs when keepalpha was specified. ([864173](https://issuetracker.unity3d.com/issues/two-pass-surface-shader-does-not-include-vertex-color-data-in-the-second-pass))
    
*   Shaders: Made Particles StandardSurface shader support gles2 again ([1103043](https://issuetracker.unity3d.com/issues/gles2-particles-slash-standard-surface-shader-doesnt-render-on-devices))
    
*   Shaders: The XR wireframe shader now works correctly with OpenGL and DirectX. (1022184, 1131099)
    
*   SpeedTree: Fixed incorrect normal directionn on v7 assets.
    
*   SpeedTree: Fixed normal mapping on newly imported v8 assets.
    
*   SpeedTree: Fixed the import of collision objects from SpeedTree v8 Assets.
    
*   Terrain: Changed vertex/hull shader program translation into a tessellation compute kernel when there is no vertex input. ([1087072](https://issuetracker.unity3d.com/issues/terrain-crash-when-moving-terrain-in-scene-view))
    
*   Terrain: Fixed a rare crash loading in a corrupted Terrain Data asset. ([1132798](https://issuetracker.unity3d.com/issues/splatdatabase-checkconsistency-crash-when-opening-a-gaia-scene), 1139361)
    
*   Terrain: Fixed the Terrain selection outline so that it works from the back side as well. ([1098438](https://issuetracker.unity3d.com/issues/terrain-back-side-of-terrain-not-included-in-selection-pass))
    
*   Terrain: Made changes so the Remove Light Probe Ringing setting can be serialized and undone. ([1093751](https://issuetracker.unity3d.com/issues/terrain-remove-light-probe-ringing-not-serialized-and-tracked-by-undo-in-terrain-settings))
    
*   Terrain: Streamlined the experimental terrain tool API, to follow Unity conventions and reduce code complexity.
    
*   Timeline: Changed behaviour of the Timeline Window to apply modifications immediately during Playmode ([922846](https://issuetracker.unity3d.com/issues/timeline-mute-state-persists-from-first-played), 1111908, 1120859, 1120870)
    
*   Timeline: Clip edit mode clutch keys will not get stuck when holding multiple keys at the same time (1097216, 1120865)
    
*   Timeline: Clip inspector will no longer throw exceptions when changing values when the inspector is locked (1115984, 1120863)
    
*   Timeline: Double separator in context menu of animation track (1102911, 1117193)
    
*   Timeline: Fixed a Notifications crash when creating an instance of `GameObjects`. ([1129866](https://issuetracker.unity3d.com/issues/crash-on-scripting-scriptingwrapperfor-when-setting-gameobject-parent-via-timeline-signals), 1139320)
    
*   Timeline: Fixed an issue where a circular reference warning appeared in the Control Clip inspector even if there was no circular reference (1116520, 1121828)
    
*   Timeline: Fixed an issue where events were being sent twice near the end of a clip. ([1017658](https://issuetracker.unity3d.com/issues/timeline-sequence-doesnt-fire-animation-events-that-are-on-the-last-frames-when-several-clips-are-played), [1022016](https://issuetracker.unity3d.com/issues/timeline-animation-event-thats-close-to-the-last-frame-gets-called-twice-when-it-transitions-to-another-animation))
    
*   Timeline: Fixed an issue where it was difficult to select a marker at the edge of a clip. (1102591, 1120860)
    
*   Timeline: Fixed an issue where non-public custom tracks did not appear in the Add Track menu. (1122803, 1129914)
    
*   Timeline: Fixed an issue where Notifications with the Retroactive flag are triggered when the timeline loops. ([1137266](https://issuetracker.unity3d.com/issues/notifications-with-retroactive-flag-are-triggered-when-the-timeline-loops), 1141569)
    
*   Timeline: Fixed an issue where the Signal Receiver would throw exceptions if the Inspector was locked. ([1114526](https://issuetracker.unity3d.com/issues/selecting-a-signal-emitter-in-timeline-while-the-inspector-is-locked-causes-nullreferenceexceptions), 1120867)
    
*   Timeline: Fixed an issue where the Track context menu did not appear when right-clicking on a track header after a copy operation. (1131095, 1141893)
    
*   Timeline: Fixed an issue where you were able to select clips and markers located under the Timeline ruler and the Marker Header track. (1102598, [1117925](https://issuetracker.unity3d.com/issues/the-clip-is-selected-when-selecting-playhead-and-the-clip-is-partially-visible-in-the-timeline), 1118966, 1121827)
    
*   Timeline: Fixed appearance of muted tracks (1018643, 1120861)
    
*   Timeline: Fixed issue where performing undo after moving items on multiple tracks would not undo some items. (1131071, 1133964)
    
*   Timeline: Fixed Timeline Inspectors leaving _EditorGUI.showMixedValue_ in the wrong state. ([1123895](https://issuetracker.unity3d.com/issues/timeline-editorgui-dot-showmixedvalue-is-used-internally-in-the-clip-inspector-thus-causing-some-parts-of-the-editor-to-misbehave), 1133951)
    
*   Timeline: Fixed _Match Offsets_ commands causing improper animation defaults to be applied. (911678, 1133939)
    
*   Timeline: Inline curves dissappear from the timeline window. (1111871, 1117197)
    
*   Timeline: Marker Track shows up in the context menus. (1107586, 1117195)
    
*   Timeline: Pasted marker has "(Clone)" in its name. (1111899, 1117198)
    
*   Timeline: PlayableDirector.played event is now called after entering or exiting Playmode ([1088918](https://issuetracker.unity3d.com/issues/timelineeditor-dot-inspecteddirector-dot-played-event-isnt-called-after-entering-slash-exiting-play-mode), 1120858)
    
*   Timeline: Remap default prev/next shortcuts on OSX to avoid conflict with system shortcut.
    
*   Timeline: Removed warning that appeared when creating a new project ([1106556](https://issuetracker.unity3d.com/issues/timeline-warnings-are-produced-when-creating-a-new-project), 1117194)
    
*   Timeline: Signal is not triggered while playing when the time is manually set. (1111595, 1117196)
    
*   Timeline: Undoing a paste track operation in a group will no longer corrupt the timeline (1116052, 1120888)
    
*   UI: Added back-removed API for `Selectable.allSelectables` and options for a non-allocating version. ([1126186](https://issuetracker.unity3d.com/issues/ui-api-breaking-changes-on-upgrading-project-ffrom-2018-dot-3-to-2019-dot-1), 1126525)
    
*   UI: Cached `referencePixelsPerUnit` when the canvas parent is disabled. ([1066689](https://issuetracker.unity3d.com/issues/the-borders-of-an-image-change-when-disabling-and-re-enabling-a-canvas-after-changing-its-worldcamera))
    
*   UI: CanvasRenderer.SetMesh will now produce an error if a non-readable mesh is passed. ([1101813](https://issuetracker.unity3d.com/issues/application-crashes-when-rendering-non-read-slash-write-enabled-mesh-to-canvas-in-built-application), 1131495)
    
*   UI: Fix 4 split layout only showing perspective in scene views. ([1112970](https://issuetracker.unity3d.com/issues/ui-viewport-display-only-perspective-view-instead-of-top-front-and-right-after-switching-layout-to-4-split), 1114618)
    
*   UI: Fixed a breaking API change in `layoutGroup` where `scaleFactor` was added and inserted in the middle of the parameter list. ([1129157](https://issuetracker.unity3d.com/issues/undocumented-breaking-api-change-layoutgroup-dot-setchildalongaxis), 1133937)
    
*   UI: Fixed a bug where changing the Constraint Count for a Grid Layout Component caused a Division by Zero error. ([1075194](https://issuetracker.unity3d.com/issues/dividebyzeroexception-division-by-zero-error-when-changing-the-constraint-count-for-a-grid-layout-1))
    
*   UI: Fixed a bug where the drop-down menu sometimes didn’t close when clicking outside it. ([1064466](https://issuetracker.unity3d.com/issues/dropdown-doesnt-close-when-clicking-outside-it-under-certain-cicumstance))
    
*   UI: Fixed an issue where the Canvas was enabled and `RectTransform` data was polled in awake, it started returning incorrect values for root `RectTransform`s.
    
*   UI: Fixed an issue where Undo would break in the **Image** component when a Sprite is replaced. ([1114240](https://issuetracker.unity3d.com/issues/ui-image-component-breaks-when-the-sprite-is-replaced), 1119502)
    
*   UI: Fixed an issue where `IndexedSet` didn't return `-1` when the element is not found in the dictionary.
    
*   UI: Fixed an issue with UI Scrollbar blocking Prefab mode. (1115796, 1115799)
    
*   UI: Fixed issue where creating a ui element under a disabled canvas would create a new canvas ([1089472](https://issuetracker.unity3d.com/issues/creating-ui-on-a-disabled-ui-parent-also-adds-new-ui-element-thats-the-same-as-parent-every-time))
    
*   UI: Fixed issue where loading a Scene with an orphaned UI component caused a crash. ([1085469](https://issuetracker.unity3d.com/issues/unity-crashes-on-transform-getlocalposition-when-opening-a-specific-scene))
    
*   UI: Fixed issue where nested canvases with canvas groups and custom alphas didn’t work properly. ([1084745](https://issuetracker.unity3d.com/issues/canvas-group-children-with-canvas-component-are-faded-when-changing-alpha-parameter-in-the-canvas-group))
    
*   UI: Fixed issue where nested canvases with canvas scalers didn’t work properly. ([1033895](https://issuetracker.unity3d.com/issues/ui-removing-or-disabling-canvasscaler-corrupts-ui-which-cannot-be-undone))
    
*   UI: Fixed issue where the input field cursor wasn’t positioned properly. ([1083649](https://issuetracker.unity3d.com/issues/inputfields-image-doesnt-extend-to-fit-the-length-of-the-text-fields-value-when-editing-it-in-the-inspector))
    
*   UI: Fixed issue where UI filtering in Scene view didn't function properly. (1064210)
    
*   UI: Fixed issue where `ListView.Refresh` computed an incorrect offset for the first row when an item source changed.
    
*   UI: Fixed memory from being allocated every frame in `CanvasScaler.Update()`. ([1105332](https://issuetracker.unity3d.com/issues/2019-dot-1-canvasscaler-dot-update-allocates-memory-every-frame), 1118317)
    
*   UI: Fixed PopupField text overflow.
    
*   UI Elements: Fix GraphView badges behavior on zoom in/out
    
*   UI Elements: Fixed : Setting a TextField's "Password" attribute via C# doesn't work. (1109699, 1115308)
    
*   UI Elements: Fixed : Setting a TextField's "Password" attribute via UXML doesn't work. (1109697, 1115309)
    
*   UI Elements: Fixed an issue where closing a window from a scheduler callback gave errors. (1098721)
    
*   UI Elements: Fixed an issue where pressing delete did not clear the contents of the ObjectField. ([1062184](https://issuetracker.unity3d.com/issues/uielements-objectfield-pressing-delete-does-not-clear-contents-like-imgui-behaviour))
    
*   UI Elements: Fixed an issue where the List View selection was not dimmed when unfocused. (1085251)
    
*   UI Elements: Fixed an issue where the position of text elements was reset during layout. (1106914)
    
*   UI Elements: Fixed an issue where the UIElements scheduler ran expired items. (1138634, 1140174)
    
*   UI Elements: Fixed an issue where UIElements did not respond to the Return key, Enter key, and the spacebar with fields such as Toggle, GradientField, CurveField, ObjectField, EnumField, and popup-related fields.
    
*   UI Elements: Fixed an issue with GraphView where the group title name was not visible during editing. (1106992)
    
*   UI Elements: Fixed an issue with measuring text elements that were not added to a hierarchy. ([1108699](https://issuetracker.unity3d.com/issues/measurevisualelementtextsize-in-measurevisualelementtextsize))
    
*   UI Elements: Fixed an issue with setting the showVertical and showHorizontal properties of a Scrollview with a callback. (1137340, 1139666)
    
*   UI Elements: Fixed an issue with text and numeric fields where pressing Enter did not end editing. (1096200)
    
*   UI Elements: Fixed an issue with text and numeric fields where pressing Escape did not end editing and restore the previous value. (1096199)
    
*   UI Elements: Fixed an issue with UXML template instances where they always appeared at the end of their parent. (1104566)
    
*   UI Elements: Fixed an issue with VectorXXFields when the window is resized. (1049285)
    
*   UI Elements: Fixed GraphView getting blurred when reframing the view (1114357, 1117687)
    
*   UI Elements: Fixed inconsistent border width at non integer scaling. (1131952, 1136268)
    
*   UI Elements: Fixed incorrectly displayed selection state in Graphview (1136637, 1137863)
    
*   UI Elements: Fixed Line and Trail Renderers throw errors in the console when Inspector window is of certain dimensions (1121685, 1131006)
    
*   UI Elements: Fixed missing GraphView nodes on OpenGL (macOS) (1117681, 1117689)
    
*   UI Elements: Fixed Null Reference exception thrown on changing scale factor of the screen from Window's display settings ([1104793](https://issuetracker.unity3d.com/issues/editor-null-reference-exception-thrown-on-changing-scale-factor-of-the-screen-from-windows-display-settings), 1123854)
    
*   UI Elements: Fixed NullReferenceExceptions in GraphView when displaying elements with empty sizes (1111567, 1117688)
    
*   UI Elements: Fixed the delayed behaviour when mouse dragger is used on numeric input field. (1117379, 1131767)
    
*   UI Elements: Fixed the foldout visual triangle that changed to checkmark. (1116011, 1118229)
    
*   UI Elements: Fixed the GradientField not showing the alpha checker (1118985, 1123838)
    
*   UI Elements: Fixed the indentation of custom scripts variables into the Inspector Window ([1114055](https://issuetracker.unity3d.com/issues/2019-dot-1-variables-of-custom-script-components-are-indented-in-the-inspector), 1137231)
    
*   UI Elements: Fixed the Inspector Window not redrawing when switching from Normal to Debug and vice-versa (1125071, 1133805)
    
*   UI Elements: Fixed the layout struggling when opening a prefab in the window hierarchy (1120821, 1131003)
    
*   UI Elements: Fixed the multiline TextField not supporting Tab character ([984808](https://issuetracker.unity3d.com/issues/uielements-multi-lines-textfield-does-not-support-tab-character), 1115525)
    
*   UI Elements: Fixed the multiselection of animation clip showing debug output in the inspector ([1115027](https://issuetracker.unity3d.com/issues/animation-multi-selecting-animation-clips-in-project-window-show-debug-options), 1132587)
    
*   UI Elements: Fixed the ObjectPicker setting none in ObjectField when cancelling. ([1123688](https://issuetracker.unity3d.com/issues/cancelling-objectpicker-window-resets-objectfield-to-none-instead-of-an-already-set-value), 1131001)
    
*   UI Elements: Fixed the preview of UXML files in the Inspector. (1111250, 1128632)
    
*   UI Elements: Fixed the shortcutmanager where long names are not displayed correctly in the profile selector. ([1099039](https://issuetracker.unity3d.com/issues/long-names-are-not-displayed-properly), 1118262)
    
*   UI Elements: Fixed the Toolbar search cancel button not showing correctly. (1115354, 1124647)
    
*   UI Elements: Fixed the value not being in synch when doing a Cut or Paste action from contextual menu in TextFields ([1120588](https://issuetracker.unity3d.com/issues/ui-elements-context-menu-paste-makes-the-internal-state-of-a-textfield-come-out-of-sync-from-what-its-displaying), 1124654)
    
*   UI Elements: Fixed the visual output of the CurveField (1118999, 1131858)
    
*   UI Elements: Fixed the yoga layout not rounding values correctly. (1105567, 1123832)
    
*   UI Elements: Properly dirty repaint on nested VisualElement view-transforms (1117229, 1117951)
    
*   UI Elements: Reduced recurrent memory allocations performed by UIElements. (1135055, 1136266)
    
*   UI Elements: UIElements Debugger splitter resets after entering Play Mode ([1113790](https://issuetracker.unity3d.com/issues/uielements-debugger-splitter-resets-after-entering-play-mode), 1131497)
    
*   UI Elements: UIR: fix broken edge expansion system and tesselation (1125408, 1125417)
    
*   Unity Test Runner: Fixed issue where the test runner would not reopen the original scene after running playmode tests. ([1118111](https://issuetracker.unity3d.com/issues/unity-loads-new-untitled-scene-instead-of-previous-after-running-playmode-tests), 1123900)
    
*   Universal Windows Platform: Fixed "Open Download Page" button navigating to non-existent file ([1106517](https://issuetracker.unity3d.com/issues/editor-on-selecting-open-download-page-button-for-universal-windows-platform-directs-to-web-page-error))
    
*   Universal Windows Platform: Fixed build failure in generated VS project due to duplicate Extension nodes in the appx manifest (1123172, 1124732)
    
*   Universal Windows Platform: Fixed Enter and Tab keys not working in multiline InputField UI ([1108599](https://issuetracker.unity3d.com/issues/uwp-enter-key-is-not-working-for-inputfield-in-a-uwp-build), 1131081)
    
*   Universal Windows Platform: Fixed IL2CPP crashing when using certain new types (like Windows.Foundation.GuidHelper.Equals) in Windows SDK 17763 or newer.
    
*   Universal Windows Platform: Fixed InputField text selection so that it works on Windows 10 touch-enabled devices. ([1002834](https://issuetracker.unity3d.com/issues/uwp-input-fields-blinking-cursor-position-cant-be-change-on-devices-with-touch-input-enabled))
    
*   Universal Windows Platform: Fixed issue where WebCamTexture failed to play in certain rare situations. ([1044635](https://issuetracker.unity3d.com/issues/uwp-app-triggers-an-exception-when-starting-to-play-webcam-texture))
    
*   Universal Windows Platform: Fixed the Visual Studio warning from generated UWP projects concerning a missing VS2015 toolset. ([1091279](https://issuetracker.unity3d.com/issues/uwp-warning-is-printed-in-visual-studios-2017-for-a-missing-visual-studio-2015-v140-toolset))
    
*   Universal Windows Platform: Made builds fail if the certificate is expired. ([1022794](https://issuetracker.unity3d.com/issues/wsa-unity-allows-building-with-an-expired-uwp-certificate))
    
*   Video: Added VR single-pass instancing mode to the VideoPlayer component. (950205)
    
*   Video: Fix for multiple GameViews, Camera Preview, and manual Camera Render. ([1109551](https://issuetracker.unity3d.com/issues/video-player-video-clip-renders-only-in-single-game-window-when-multiple-game-windows-are-open), 1114623)
    
*   Video: Fixed a crash on iOS when switching between videos with 6 audio channels. ([935497](https://issuetracker.unity3d.com/issues/ios-videoplayer-video-with-6-audio-channels-crashes-when-switching-between-videos))
    
*   Video: Fixed a crash that occurred while importing the ARCore SDK for Unity 1.7.0 package. (1133177, 1139365)
    
*   Video: Fixed a crash with "-\[AVFoundationMediaLoader GetNumAudioChannels:\]" when entering Play Mode. ([1104510](https://issuetracker.unity3d.com/issues/unity-crashes-on-avfoundationmedialoader-getnumaudiochannels-when-entering-play-mode), 1139367)
    
*   Video: Fixed an issue where the Editor crashes on skipping transcoding twice for video. ([1104507](https://issuetracker.unity3d.com/issues/video-editor-crashes-on-skipping-transcoding-twice-for-video), 1139450)
    
*   Video: Fixed an issue with the "LZ4" or "LZ4HC" compression methods when viewing a video in the Standalone Player. ([1092265](https://issuetracker.unity3d.com/issues/using-lz4-or-lz4hc-compression-methods-results-in-an-error-in-standalone-player-when-viewing-a-video), 1139366)
    
*   Video: Fixed crash on specific AVI video files on Windows. ([1088203](https://issuetracker.unity3d.com/issues/crash-on-windowsvideomedia-copytorgba-when-importing-avi-file))
    
*   Video: Fixed crash on specific MPEG2 video files on Windows. ([1082071](https://issuetracker.unity3d.com/issues/editor-crashes-when-playing-mpeg2-video-in-inspector))
    
*   Video: Fixed issue where the frame rate dropped drastically when using Movie Recorder to record as WebM. ([1052060](https://issuetracker.unity3d.com/issues/recorder-frame-rate-drops-drastically-when-using-movie-recorder-to-record-as-webm))
    
*   Video: Improved VideoPlayer network error handling on Windows. ([1051461](https://issuetracker.unity3d.com/issues/windows-videoplayer-dot-errorreceived-callback-is-not-triggered-when-internet-connection-is-lost))
    
*   Video: Made changes so that VideoPlayer Camera Plane targets are visible in the SRP. ([1024877](https://issuetracker.unity3d.com/issues/video-player-doesnt-show-anything-on-hd-scriptable-render-pipeline))
    
*   Video: Made changes to disregard unsupported streams on Windows. ([1065499](https://issuetracker.unity3d.com/issues/an-error-is-thrown-when-playing-mov-file-which-was-made-on-iphone-ios-10))
    
*   Video: \[WINDOWS 7\] Imported Video File cannot be played in 2019.1 (1133061, 1133666)
    
*   VR: \[Lumin\] Fixed an issue where including TrackedPoseDriver in a scene would produce incorrect headpose results (1105315, 1118305)
    
*   WebGL: Fixed an issue where the Editor prevented builds for WebGL when linear color space was enabled. ([1103083](https://issuetracker.unity3d.com/issues/webgl-cant-build-with-linear-color-space-due-to-wrong-error))
    
*   WebGL: Fixed an issue where WebGL froze when switching to full-screen. ([1106442](https://issuetracker.unity3d.com/issues/webgl-switching-to-full-screen-causes-webgl-player-freeze), 1144828)
    
*   WebGL: Fixed the Build window Linear Color Space compatibility check. ([1105479](https://issuetracker.unity3d.com/issues/linear-color-space-build-can-be-started-with-webgl-1-dot-0-in-the-api-list))
    
*   WebGL: Fixed the Performance Reporting integer overflow in WebAssembly development builds.
    
*   WebGL: Fixed WebGL build failure when python is already installed ([938826](https://issuetracker.unity3d.com/issues/webgl-build-fails-conflicting-with-existing-emscripten-and-python-installation))
    
*   WebGL: Fixed `Application.Quit()` and memory cleanup. ([1032870](https://issuetracker.unity3d.com/issues/webgl-player-continues-to-run-after-webgl-content-is-removed-from-dom))
    
*   WebGL: WebGL: Fix build&run with wasm streaming enabled. ([1104514](https://issuetracker.unity3d.com/issues/wasm-streaming-doesnt-work-using-build-and-run), 1125367)
    
*   Windows: Fixed an issue where the Editor froze when certain devices (Steinberg UR 22 mk II, Cronus MAX) were connected to the computer. ([917526](https://issuetracker.unity3d.com/issues/unity-hangs-when-opening-project-with-steinberg-ur-22-mk-ii-connected))
    
*   Windows: Fixed cursor confinement to window not matching window bounds visually
    
*   Windows: Fixed headless build crashing if closed via the "X" button in the console
    
*   Windows: Fixed WinPixEventRuntime.dll deployed with non-development builds ([1118833](https://issuetracker.unity3d.com/issues/building-an-application-generates-winpixeventruntime-dot-dll-when-development-build-is-unchecked-and-architecture-is-x86-64), 1131483)
    
*   Windows: Improved error messages after failing to load native plugins on Windows Standalone and UWP if one of their dependencies is missing. (1083178, 1116537)
    
*   XR: Fix invalid return when using XRDevice.GetNativePointer with Oculus
    
*   XR: Fix white flash before splash screen on Gear VR applications ([893599](https://issuetracker.unity3d.com/issues/gearvr-when-returning-from-the-oculus-menu-to-app-there-is-a-white-flash))
    
*   XR: Fixed a regression where Android based VR was locked to 30fps. ([1135328](https://issuetracker.unity3d.com/issues/oculus-go-apllications-are-capped-at-30-fps-when-building-a-project-for-oculus-go), 1140824)
    
*   XR: Fixed head-tracking and rendering for in-editor remoting to HoloLens devices ([1138473](https://issuetracker.unity3d.com/issues/hololens-remoting-hololens-device-does-not-render-anything-when-emulation-mode-is-set-to-remote-to-device), 1140716)
    
*   XR: Fixed issue that caused the player to crash when using Google Cardboard API with both GLES3 and Vulkan included in the graphics APIs. ([1102049](https://issuetracker.unity3d.com/issues/xr-android-application-crashes-and-does-not-fall-back-to-gles3-when-having-both-gles3-and-vulkan-included-in-graphics-apis))
    
*   XR: Fixed issue where VR Billboarded trees were improperly lit on macOS if VR was enabled. (1025108)
    
*   XR: Fixed issue where VR tree shader used alpha to coverage multi-sampling when multi-sample anti-aliasing (MSAA) was disabled. ([1074421](https://issuetracker.unity3d.com/issues/details-are-lost-too-early-for-terrain-trees-in-vr))