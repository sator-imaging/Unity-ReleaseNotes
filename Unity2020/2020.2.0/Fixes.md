# Unity 2020.2.0
https://unity3d.com/unity/whats-new/2020.2.0

## Fixes

<ul>
<li><p>2D: Added a tootlip for the Tile Palette Gizmos button. (<a href="https://issuetracker.unity3d.com/issues/2d-tooltip-is-missing-for-the-gizmos-button-in-the-tile-palette">1254646</a>)</p></li>
<li><p>2D: Added the <em>Always Update</em> property to the Sprite Skin component so that when enabled, the Sprite Skin will always deforms even when its associated Sprite Renderer is culled.</p></li>
<li><p>2D: Ensured that the "Unapplied import settings" prompt appears you select <em>Apply</em> when  there are changes in both the Sprite Editor and Texture Importer windows. (<a href="https://issuetracker.unity3d.com/issues/2d-unapplied-import-settings-doesnt-prompt-on-generating-custom-outline-with-mosaic-property-unchecked">1244077</a>)</p></li>
<li><p>2D: Fixed a crash caused by using a Sprite Atlas with Secondary Textures assigned to it. (<a href="https://issuetracker.unity3d.com/issues/crash-when-opening-unity-project-that-has-sprite-atlas-with-normalmap-secondary-texture">1288572</a>)</p></li>
<li><p>2D: Fixed a crash when undoing and redoing after a Tile Palette is saved. (<a href="https://issuetracker.unity3d.com/issues/2d-editor-crashes-when-undo-and-redo-operation-is-performed-with-tile-palette">1280263</a>)</p></li>
<li><p>2D: Fixed an issue causing Editor crashes when packing Sprites. (<a href="https://issuetracker.unity3d.com/issues/2d-spriteatlas-v2-editor-crashes-when-packing-sprites">1259149</a>)</p></li>
<li><p>2D: Fixed an issue preventing you from creating Sprite Shape Profiles along with <code>ArgumentNullException</code> being thrown in the Project window. (<a href="https://issuetracker.unity3d.com/issues/2d-spriteshape-unable-to-create-sprite-shape-profile-along-with-argumentnullexception-thrown-in-the-project-window">1280016</a>)</p></li>
<li><p>2D: Fixed an issue so that a <code>NullReferenceException</code> is no longer thrown when you perform the Redo operation after creating the <em>Range</em> property in the Sprite Shape profiler preset. (<a href="https://issuetracker.unity3d.com/issues/2d-nullreferenceexception-thrown-on-performing-redo-operation-after-creating-range-property-in-the-spriteshape-profiler-preset">1274776</a>)</p></li>
<li><p>2D: Fixed an issue so that dragging a Sprite Shape Profile to the Hierarchy window while in Prefab Mode now no longer creates a GameObject in the in the main Scene. (<a href="https://issuetracker.unity3d.com/issues/dragging-sprite-shape-profile-to-hierarchy-creates-a-game-object-in-main-scene-when-being-in-prefab-mode">1265846</a>)</p></li>
<li><p>2D: Fixed an issue so that Sprites with no animation data are not processed during <code>AssetPostProcessor</code>.</p></li>
<li><p>2D: Fixed an issue so that the Shift+Erase keyboard shortcut now returns to the Paint Tool when painting with the Tool in the Tile Palette.</p></li>
<li><p>2D: Fixed an issue so that the Sprite Editor window now shows the Sprite when the Inspector is locked and the Sprite is selected in the Project window.</p></li>
<li><p>2D: Fixed an issue that a assertion failed exception is no longer thrown when undoing after clicking the <em>Create Range</em> button. (<a href="https://issuetracker.unity3d.com/issues/2d-sprite-shape-assertion-failed-exception-is-thrown-on-undoing-after-clicking-on-create-range-button">1273705</a>)</p></li>
<li><p>2D: Fixed an issue where a Sprite Shape's bounding box did not take into account certain vertices. (<a href="https://issuetracker.unity3d.com/issues/2d-spriteshape-spriteshape-bounding-box-does-not-take-into-account-certain-vertices">1274400</a>)</p></li>
<li><p>2D: Fixed an issue where the preview of a deleted Secondary Texture entry remained visible in the Sprite Editor. (<a href="https://issuetracker.unity3d.com/issues/2d-sprite-preview-of-secondary-textures-is-not-updated-on-deleting-first-texture">1211176</a>)</p></li>
<li><p>2D: Fixed an issue where the vertical scroll bar of the Secondary Textures module in the Sprite Editor did not react to the mouse wheel. (<a href="https://issuetracker.unity3d.com/issues/sprite-editor-vertical-scrollbar-for-secondary-textures-does-not-scroll-up-with-mouse-wheel">1204429</a>)</p></li>
<li><p>2D: Fixed an issue where <code>Sprite.GetVertexAttribute (TexCoord0)</code> did not return the correct UV data if the Sprite was not rendered yet. (1266065)</p></li>
<li><p>2D: Fixed inconsistent positions in the 2D menu. (1268024)</p></li>
<li><p>2D: Fixed Sprite Skin deformation not being updated when the Sprite Skin component is enabled for a GameObject.</p></li>
<li><p>2D: Fixed the auto-sizing of the Tile Palette when the Tile Palette's <em>Cell Swizzle</em> is set to <em>YXZ</em>.</p></li>
<li><p>2D: Fixed the broken documentation links in the Inspectors windows of components from the <a href="https://docs.unity3d.com/Packages/com.unity.2d.animation@latest/">2D Animation</a> package.</p></li>
<li><p>2D: Fixed the broken documentation links in the PSD Importer Inspector view.</p></li>
<li><p>2D: Fixed the broken documentation URL of the Pixel Perfect component.</p></li>
<li><p>2D: Fixed the exception error caused by reverting newly created vertices and edges in the <a href="https://docs.unity3d.com/Packages/com.unity.2d.animation@5.0/manual/SkinningEditor.html">Skinning editor module</a>.</p></li>
<li><p>2D: Fixed the generation of Collider shapes with Tilemap Collider 2D, when a Tile is animated with Animated Tiles.</p></li>
<li><p>2D: Fixed the issue causing the Sprite Asset used by the Sprite Skin component to be deleted in the Scene.</p></li>
<li><p>2D: Fixed the issue causing the <code>Invalid worldAABB</code> error message when the Pack Preview button was repeatedly pressed. (1270150)</p></li>
<li><p>2D: Fixed the issue where '_NormalMap' <a href="https://docs.unity3d.com/Manual/SpriteEditor-SecondaryTextures.html">Secondary Textures</a> were not streched to the *Max Texture Size* when the Atlas Texture's size is larger than the  _NormalMap Texture. (<a href="https://issuetracker.unity3d.com/issues/lwrp-normalmap-secondary-texture-is-streched-to-atlassize-when-atlas-texture-size-is-larger-than-normal-map-texture-size">1167829</a>)</p></li>
<li><p>2D: Fixed the issue where the PSD Importer created empty GameObjects in certain cases.</p></li>
<li><p>2D: Fixed the issue where <code>Bounds/RectInt.allPositionsWithin</code> kept returning positions of size 0 for any axis. (<a href="https://issuetracker.unity3d.com/issues/boundsint-allpositionswithin-return-points-when-boundsint-x-or-y-size-is-zero-and-non-zero-in-other-axes">1227811</a>)</p></li>
<li><p>2D: Fixed the memory leak from the Sprite Shape Controller when no control points are used.</p></li>
<li><p>2D: Fixed the Sprite Editor not showing the Sprite when the Inspector is locked and the Sprite is not selected in the Project window. (<a href="https://issuetracker.unity3d.com/issues/the-sprite-editor-doesnt-show-the-sprite-when-the-inspector-is-locked-and-the-sprite-is-not-selected-in-the-project-window">1215581</a>)</p></li>
<li><p>2D: Fixed the Sprite Packer preview image of a loaded AssetBundle so that it properly displays after the Editor is refocused. (<a href="https://issuetracker.unity3d.com/issues/sprite-packed-image-is-blank-in-loaded-assetbundle-after-editor-re-focus">1243177</a>)</p></li>
<li><p>2D: Fixed the visual defect that occurs after undoing changes to the <em>Bone Transform</em> properties in the Sprite Skin components' Inspector window.</p></li>
<li><p>2D: Fixed <code>OnDrawGizmos</code> to work with <code>Rendering.CommandBuffer.GetTemporaryRT</code> and <code>CommandBuffer.ReleaseTemporaryRT</code>.</p></li>
<li><p>2D: Modified Colliders to respect the <em>Pivot</em> property of Edge Sprites in Sprite Shape.</p></li>
<li><p>2D: Modified Path tool returns usage.</p></li>
<li><p>2D: Modified Sprite Shapes so that they are not generated when not in view during runtime.</p></li>
<li><p>2D: Modified the <em>Depth</em> column label so that is is no longer clipped in the Visibility Tool window. (<a href="https://issuetracker.unity3d.com/issues/2d-depth-keyword-gets-clipped-in-the-visibility-tool-window-in-the-skinning-editor">1257991</a>)</p></li>
<li><p>2D: Modified the Grid Brush property to retain cells set when moving Tiles with the Move tool. (<a href="https://issuetracker.unity3d.com/issues/2d-tilemap-get-erased-while-using-flood-fill-brush-when-select-and-mover-brush-is-used-earlier">1244347</a>)</p></li>
<li><p>2D: Modified the properties under the Sprite Library Asset that they no longer over lap in the Inspector window. (<a href="https://issuetracker.unity3d.com/issues/2d-properties-under-the-new-sprite-library-asset-are-overlapping-on-each-other-in-the-inspector">1280017</a>)</p></li>
<li><p>2D: Modified the Sprite Editor window so that the Visibility window no longer overlaps with the Weights and Geometry window when the Sprite Editor window is resized. (1263353)</p></li>
<li><p>2D: Modified the Tilemap Painting editor so that when painting or erasing Tiles from the Tile Palette, the active editor tool is automatically set to the Paint tool if the Shift key is released before the mouse button is released. (<a href="https://issuetracker.unity3d.com/issues/tile-eraser-tool-is-not-deselected-when-shift-key-is-let-go-of-before-letting-go-of-the-left-mouse-button">1231123</a>)</p></li>
<li><p>2D: Modified the vertical slider handle so it is now properly aligned in the Bone Influence window. (<a href="https://issuetracker.unity3d.com/issues/2d-animation-vertical-slider-handle-is-not-aligned-and-placed-slightly-to-the-right-side-in-the-bone-influence-window">1260568</a>)</p></li>
<li><p>2D: Modified Tile Palette so that when dragging in Sprites and Tiles to the Tile Palette,  the layout of Tiles are kept equal in width and height where possible</p></li>
<li><p>2D: Modified Tilemap Renderer so that individual Sprites are culled when the Renderer is set to <em>Individual</em> mode, instead of using chunk culling.</p></li>
<li><p>2D: Updated the documentation for <code>Bounds</code>/<code>RectInt</code> when setting a minimum position that is greater than the maximum position or vice versa.</p></li>
<li><p>AI: Added OffMeshLink component Reset functionality. (<a href="https://issuetracker.unity3d.com/issues/navigation-reset-functionality-is-not-working-for-off-mesh-link">1155287</a>)</p></li>
<li><p>AI: Baking ignores FBX files with Mesh Compression set to Low or Medium when baking NavMesh. (<a href="https://issuetracker.unity3d.com/issues/navmesh-baking-ignores-fbx-files-with-mesh-compression-set-to-low-or-medium-when-baking-navmesh">1152594</a>)</p></li>
<li><p>AI: Fixed a crash when specified node pool size for a new NavMeshQuery is too small. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-when-using-navmeshquery-beginfindpath-on-navmeshnodepool-getnode">1104755</a>)</p></li>
<li><p>AI: Fixed a missing override indicators in NavMesh editors for the size of NavMeshObstacle and Area Mask for NavMeshAgent. (<a href="https://issuetracker.unity3d.com/issues/prefabs-blue-highlight-override-indicator-is-missing-for-radius-and-height-properties-in-nev-mesh-obstacle">1269446</a>)</p></li>
<li><p>AI: Fixed an editor crash when building a NavMesh with excessively distant sources. (<a href="https://issuetracker.unity3d.com/issues/crash-on-schedulenavmeshdataupdate-when-building-navmeshsurface-while-another-gameobject-is-far-away">1231244</a>)</p></li>
<li><p>AI: Fixed an issue where NavMesh agent 'Area Mask' dropdown displayws when all values are selected. (<a href="https://issuetracker.unity3d.com/issues/ai-area-mask-dropdown-doesnt-display-everything-as-selected-when-all-options-are-checked">1117300</a>)</p></li>
<li><p>AI: Fixed an issue where pathfinding returned the end point on the wrong "floor" of the NavMesh. (<a href="https://issuetracker.unity3d.com/issues/navmesh-dot-sampleposition-finds-the-closest-point-on-the-different-y-position-when-an-agent-cannot-find-a-path">1124570</a>)</p></li>
<li><p>AI: Fixed NavMesh link cost modifiers improper behavior. (<a href="https://issuetracker.unity3d.com/issues/navmeshpath-partial-path-calculation-gets-stuck-on-navmeshlink">1281314</a>)</p></li>
<li><p>Android: Automatically enable 'Custom ... Manifest' and 'Custom ... Template' checkboxes in Player Settings if appropriate files are added to Plugins/Android directory. (<a href="https://issuetracker.unity3d.com/issues/custom-grandle-settings-are-not-exported-to-build-dot-gradle">1227315</a>)</p></li>
<li><p>Android: Avoid using depthClamp on GPUs that don't support it when using Vulkan.</p></li>
<li><p>Android: Disabled Optimized Frame Pacing on Android 4.4-5.1 to fix crash/freeze. (<a href="https://issuetracker.unity3d.com/issues/android-4-dot-4-crash-on-dvmgetvirtualizedmethod-cause-null-pointer-dereference-when-optimized-frame-pacing-is-enabled">1268910</a>)</p></li>
<li><p>Android: Fixed a regression with playing back uncompressed, on-disk asset bundles on Android versions before Pie.</p></li>
<li><p>Android: Fixed a super-slow playback of video issue in asset bundles on Android. (<a href="https://issuetracker.unity3d.com/issues/android-video-player-unable-to-play-video-from-asset-bundles">1287770</a>)</p></li>
<li><p>Android: Fixed a Vulkan validation error when using Optimized Frame Pacing with Vulkan. (1255060)</p></li>
<li><p>Android: Fixed an issue when accessing streamable assets time is increased due to incorrect compression settings. (<a href="https://issuetracker.unity3d.com/issues/android-loading-the-viking-village-scene-takes-a-couple-of-minutes">1276114</a>)</p></li>
<li><p>Android: Fixed an issue when using storage buffer object in both vertex and fragment shader on Adreno. (<a href="https://issuetracker.unity3d.com/issues/drawmeshinstancedindirect-fails-to-render-opaque-pass-when-using-opengl-es-with-android-or-dx12-with-standalone">1251305</a>)</p></li>
<li><p>Android: Fixed an issue where Android cutout's y coordinate in windowed mode. (<a href="https://issuetracker.unity3d.com/issues/screen-cutout-values-are-not-adjusted-when-device-is-in-windowed-mode-on-portrait-orientation">1248638</a>)</p></li>
<li><p>Android: Fixed an issue where Multithreaded Rendering setting would use the incorrect platform settings.</p></li>
<li><p>Android: Fixed an issue with android's window pixel format when rendering over native UI. (<a href="https://issuetracker.unity3d.com/issues/android-camera-background-set-to-solid-color-ignores-alpha-value-on-android-devices">1244553</a>)</p></li>
<li><p>Android: Fixed artifacts on older Adreno devices when using compute skinning with blend shaped with OpenGL ES. (<a href="https://issuetracker.unity3d.com/issues/graphics-android-build-with-compute-skinning-option-causes-broken-blend-shapes">1260887</a>)</p></li>
<li><p>Android: Fixed Autoconnect Profiler option when device is connected with USB only. (<a href="https://issuetracker.unity3d.com/issues/android-autoconnect-profiler-option-does-not-work-with-usb-only">1244618</a>)</p></li>
<li><p>Android: Fixed BuildOptions.ConnectToHost option, when Android is only connected to PC via USB and Wifi is disabled. Previously BuildOptions.ConnectToHost would only work through Wifi connection, now the app should automatically connect to Editor. (1233567)</p></li>
<li><p>Android: Fixed depth when rendering to backbuffer with BlitType Auto/Never.</p></li>
<li><p>Android: Fixed performance regression on Mali GPUs when using CBUFFERs. (1157313)</p></li>
<li><p>Android: Fixed RenderPass API implementation when using OpenGL ES. (1219327)</p></li>
<li><p>Android: With sporadic freeze when using Vulkan on Mali devices.</p></li>
<li><p>Animation: Added documentation for AnimatorControllerPlayable methods. (1195131)</p></li>
<li><p>Animation: Ensured that deactivating GameObjects does not deallocate memory used by TransformStreamHandle. (<a href="https://issuetracker.unity3d.com/issues/memory-leak-occurs-due-to-transformstreamhandle-memory-not-being-deallocated-when-deactivating-gameobjects">1167280</a>)</p></li>
<li><p>Animation: Fixed a crash casued by <code>animation.Play(AnimationPlayMode.Queue)</code> being called at every frame. (<a href="https://issuetracker.unity3d.com/issues/crash-in-animationcurvetpl-evaluateclamp-when-animation-dot-play-animationplaymode-dot-queue-is-called-in-update">1218218</a>)</p></li>
<li><p>Animation: Fixed a crash that occurred when AnimationPlayables were destroyed. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-destroying-a-playable-object-during-ondestroy-function-call">1231355</a>)</p></li>
<li><p>Animation: Fixed a crash that would happen when calling the GetBoneTransform on a humanoid with no left finger. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-calling-getbonetransform-on-an-animator-with-generated-avatar-and-specific-bone-mapping">1228811</a>)</p></li>
<li><p>Animation: Fixed a crash where the animation clip custom target was null as it was still in a transform binding mode. (<a href="https://issuetracker.unity3d.com/issues/crash-on-unityengine-animation-setboundcurvefloatvalue-when-animationclip-properties-are-displayed-in-the-inspector">1228823</a>)</p></li>
<li><p>Animation: Fixed an issue in the Animation window where the Esc key did not cancel renaming. (<a href="https://issuetracker.unity3d.com/issues/the-changes-are-applied-when-renaming-animation-property-in-the-animation-tab-and-pressing-esc">1157048</a>)</p></li>
<li><p>Animation: Fixed an issue in the Stats window that dispalyed an incorrect number of playing animations. (<a href="https://issuetracker.unity3d.com/issues/animation-count-in-scene-from-the-stats-window-does-not-drop-down-when-all-of-the-animation-are-finished-in-the-scene">1201251</a>)</p></li>
<li><p>Animation: Fixed an issue where blending playables that animated different set of properties would not correctly blend with the scene values. (<a href="https://issuetracker.unity3d.com/issues/wrong-animation-is-played-when-multiple-animation-tracks-are-blended-in-timeline">1252312</a>)</p></li>
<li><p>Animation: Fixed an issue where changes to an entry transition would not rebuild the state machine. (<a href="https://issuetracker.unity3d.com/issues/the-mute-transition-flag-in-the-sub-state-machine-gets-ignored-after-switching-muted-transitions">1282801</a>)</p></li>
<li><p>Animation: Fixed an issue where creating Motions for a BlendTree node would overlap and hide surrounding BlendTree nodes. (<a href="https://issuetracker.unity3d.com/issues/animation-blendtree-overlaps-and-hides-another-blendtree-on-adding-the-motion-field">1193229</a>)</p></li>
<li><p>Animation: Fixed an issue where Light.innerSpotAngle could not be animated. (<a href="https://issuetracker.unity3d.com/issues/urp-no-keyframe-is-added-when-animating-the-spot-lights-inner-spot-angle-variable">1270159</a>)</p></li>
<li><p>Animation: Fixed an issue where OnStateEnter was not being called when StateMachineBehaviour stop Timelines. (<a href="https://issuetracker.unity3d.com/issues/onstateenter-is-not-called-when-using-the-timeline-with-an-animator-on-the-same-gameobject">1257833</a>)</p></li>
<li><p>Animation: Fixed an issue where OnStateUpdate was not called when attaching a new AnimatorControllerPlayable. (<a href="https://issuetracker.unity3d.com/issues/onstateupdate-will-not-be-called-when-a-new-animatorcontrollerplayable-is-attached-by-the-first-time">1168332</a>)</p></li>
<li><p>Animation: Fixed an issue where the editor crashes when opening Animator transition settings with specific hierarchy. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-opening-animator-transition-settings-with-specific-hierarchy">1242608</a>)</p></li>
<li><p>Animation: Fixed an issue where the Layers and Parameters view in the Animator component where unhidden when entering Play Mode. (<a href="https://issuetracker.unity3d.com/issues/hidden-animator-layers-slash-parameter-view-opens-back-again-after-entering-play-mode">1219412</a>)</p></li>
<li><p>Animation: Fixed an issue where threshold values with commas would not save in blend tress. (<a href="https://issuetracker.unity3d.com/issues/blendtree-writing-treshold-value-with-comma-doesnt-save-the-value">817322</a>)</p></li>
<li><p>Animation: Fixed an issue with animations in built projects that occurred when the Disable Unity Audio setting was enabled in the Project Settings. (<a href="https://issuetracker.unity3d.com/issues/checking-the-disable-unity-audio-checkbox-breaks-the-playable-graph-with-animations-in-the-built-player">1187693</a>)</p></li>
<li><p>Animation: Fixed an issue with the Animator window layout not persisting. (<a href="https://issuetracker.unity3d.com/issues/the-animator-window-defaults-its-layout-when-opened">1197028</a>)</p></li>
<li><p>Animation: Fixed root transform offsets introduced on nested humanoid characters running Animation C# Jobs. (<a href="https://issuetracker.unity3d.com/issues/animation-rigging-with-humanoid-rig-multi-xxxx-constraint-moving-the-animators-parent-node">1259490</a>)</p></li>
<li><p>Asset Import: Fixed an issue in ModelImporter when the Preserve Hierarchy was ignored in some cases after applying a Preset to it. (1243047)</p></li>
<li><p>Asset Import: Fixed an issue that was throwing errors in the console when Rig settings of multiple models were all changed at once. (<a href="https://issuetracker.unity3d.com/issues/argumentoutofrange-exception-is-thrown-when-applying-rig-changes-to-multiple-selected-fbx-models">1264463</a>)</p></li>
<li><p>Asset Import: Fixed an issue when using ClearImporterOverride on Model assets (fbx files and other formats using the ModelImporter) that caused a memory leak and console errors. (<a href="https://issuetracker.unity3d.com/issues/using-clearimporteroverride-to-revert-an-asset-that-is-using-a-modelimporter-creates-memory-leaks-and-logs-errors-in-the-console">1218841</a>)</p></li>
<li><p>Asset Import: Fixed an issue where RE2 generated warnings on old versions of macOS. (1259551)</p></li>
<li><p>Asset Import: Fixed an issue with the model rotated 90 degrees when upgrading project from version 2020.2.0a20 and below to 2020.2.0a21 and above. (<a href="https://issuetracker.unity3d.com/issues/model-rotates-90-degrees-when-upgrading-project-from-version-2020-dot-2-0a20-and-below-to-2020-dot-2-0a21-2020-dot-2-0b3">1276677</a>)</p></li>
<li><p>Asset Import: Fixed AssetImportWorker taking autoconnect player connections.</p></li>
<li><p>Asset Import: Importers does not lose selection anymore when the imported asset changes its type. (<a href="https://issuetracker.unity3d.com/issues/an-asset-is-deselected-when-its-texture-shape-value-is-changed-and-the-changes-are-applied">1182598</a>)</p></li>
<li><p>Asset Import: LoadImage now returns PNGs in the authored colorspace when gAMA block is authored, instead of gamma 2.0. A new static flag has been added to the ImageConversion class to disable this behavior. See Texture2D.LoadImage for additional details. (1199896)</p></li>
<li><p>Asset Import: Solved an issue so that AssetDatabaseExperimental.GetAvailableImporterTypes returns all expected registered importers for a given asset path. (<a href="https://issuetracker.unity3d.com/issues/scriptedimporter-does-not-register-autoselect-properly">1218830</a>)</p></li>
<li><p>Asset Pipeline: ArtifactID is now unique for an import result. (1193231)</p></li>
<li><p>Asset Pipeline: Changed behavior in Refresh<br></p> 
<ul>
<li>Empty folders that don't have .meta files get deleted if the folders were known before.<br></li>
<li>If an orphaned .meta file is marked as folderAsset the folder is recreated.<br>
These changes address issues related to creating/deleting folders in certain (p4, git) version controlled projects where empty folders don't get created/deleted when the user gets latest version on the client.</li>
</ul></li>
<li><p>Asset Pipeline: Changing the platform is not propagated to the asset import worker process.</p></li>
<li><p>Asset Pipeline: Disabled editors for removed assets. (<a href="https://issuetracker.unity3d.com/issues/targets-are-null-in-custom-editors-during-ondisable-when-deleting-an-asset-in-adb2">1158081</a>)</p></li>
<li><p>Asset Pipeline: Fixed a crash in GetHashOfImportedAssetDependencyHints when scripted importer returns null inside GatherDependenciesFromSourceFile during unity startup. (1234968)</p></li>
<li><p>Asset Pipeline: Fixed a crash when a preview image was destroyed indirectly. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-returning-asset-preview-for-a-custom-scriptable-object-using-assetpreview-dot-getassetpreview">1163297</a>)</p></li>
<li><p>Asset Pipeline: Fixed a Project Startup slow time issue due to an unmatched Custom Dependencies. (<a href="https://issuetracker.unity3d.com/issues/project-startup-time-slow-due-to-unmatched-custom-dependencies">1276078</a>)</p></li>
<li><p>Asset Pipeline: Fixed a scalability issue of increasing number of revisions of long dependency chains (e.g. iterating on nested prefabs). (1250294)</p></li>
<li><p>Asset Pipeline: Fixed a small performance regression when batch copying assets via scripts. (1238732)</p></li>
<li><p>Asset Pipeline: Fixed an issue where ''GetCurrentCacheServerIp' was returning an empty string instead of actual value.</p></li>
<li><p>Asset Pipeline: Fixed an issue where an imported asset dependency on a source asset could lead to a wrong import.</p></li>
<li><p>Asset Pipeline: Fixed an issue where an unused artifact dependency would lead to infinite import.</p></li>
<li><p>Asset Pipeline: Fixed an issue where Artifacts for deleted asset didn't get deleted in artifact garbage collection.</p></li>
<li><p>Asset Pipeline: Fixed an issue where custom dependencies changes are rejected in initial domain load.</p></li>
<li><p>Asset Pipeline: Fixed an issue where Forced import of an new asset which already have a meta file (and thereby a GUID) don't get force reimported.</p></li>
<li><p>Asset Pipeline: Fixed an issue where the current directory was changed in beginning of refresh. (<a href="https://issuetracker.unity3d.com/issues/fatal-error-is-not-thrown-and-editor-continues-to-function-when-working-directory-is-changed-with-directory-dot-setcurrentdirectory">1278242</a>)</p></li>
<li><p>Asset Pipeline: Fixed Binary to YAML UInt16 conversion error when importing a specific binary serialized package into a project with Force Text serialization enabled. (<a href="https://issuetracker.unity3d.com/issues/binary-to-yaml-conversion-error-is-thrown-importing-certain-packages-and-asset-serialization-mode-is-set-to-force-text">1225913</a>)</p></li>
<li><p>Asset Pipeline: Fixed bug where renaming a script doesn't properly take effect on asset import workers. (<a href="https://issuetracker.unity3d.com/issues/prefab-in-subscene-does-not-update-after-component-script-changes">1258644</a>)</p></li>
<li><p>Asset Pipeline: Fixed for bug where the main object would change after renaming a native asset. (<a href="https://issuetracker.unity3d.com/issues/parent-and-child-nested-scriptable-object-assets-switch-places-when-parent-scriptable-object-asset-is-renamed">1189089</a>)</p></li>
<li><p>Asset Pipeline: Fixed for instability where .meta files are not parsed right. (<a href="https://issuetracker.unity3d.com/issues/investigate-why-meta-files-are-sometimes-not-parsed-right">1214122</a>)</p></li>
<li><p>Asset Pipeline: Fixed issue where postprocessors with version 0 wouldn't be used.</p></li>
<li><p>Asset Pipeline: Having information that says "version 2" is selected, can be confusing, since users could assume that the "version 1" of the asset import pipeline could be selected. This has been removed completely as 2020.1 can on the Asset Import Pipeline that was re-written for 2019.3.</p></li>
<li><p>Asset Pipeline: If the license is not valid asset import worker processes will fail and block the main editor. (1224855)</p></li>
<li><p>Audio: Changing audio mixer attenuation to or from 0 dB resulted in popping / spiking sounds. (<a href="https://issuetracker.unity3d.com/issues/changing-audiomixer-volume-from-any-volume-in-db-to-0-db-results-in-popping-slash-spiking-sound">1101442</a>)</p></li>
<li><p>Audio: Chorus and Flange filters didn't apply initial parameters correctly under certain situations when used in the audio mixer or as audio filter components. (579690)</p></li>
<li><p>Audio: Fixed "Assertion failed on expression" message in console when disabling the audio system from the project settings while an audio clip preview is playing. Also, the preview playback will now stop in this scenario. (<a href="https://issuetracker.unity3d.com/issues/audio-assertion-failed-on-expression-is-thrown-while-playing-an-audio-preview-when-unity-audio-is-disabled">1232267</a>)</p></li>
<li><p>Bug Reporter: Added a name of the file causing the error to the project packer error message. (<a href="https://issuetracker.unity3d.com/issues/bugreporter-does-not-print-out-failing-filename-then-project-packing-fails">1223660</a>)</p></li>
<li><p>Build Pipeline: Added scroll viewer to build settings. (<a href="https://issuetracker.unity3d.com/issues/build-settings-window-uwp-gets-overlapping-elements-when-its-height-goes-beyond-a-certain-treshold">1211918</a>)</p></li>
<li><p>Build Pipeline: Added support for baked collision mesh writing in the Scriptable Build Pipeline.</p></li>
<li><p>Build Pipeline: Fixed a build corrupted issue when a field coming from an assembly override was serialized in assets/scenes. (1265330)</p></li>
<li><p>Build Pipeline: Fixed an edge case issue where generated sprite texture case were being mangled and caused build errors on case sensitive file systems.</p></li>
<li><p>Build Pipeline: Fixed an issue where StreamingAssets AssetBundle manifest were not provided by default to PlayerBuild, which resulted in types being referred by AssetBundle being kept in the build even if Player.Optimization.Managed Stripping Level was set to Medium or High.</p></li>
<li><p>Build Pipeline: Fixed bug in the Managed SpookyHash algorithm that was causing some bytes at the end of the buffer to not be incorporated into the hash for specific buffer sizes.</p></li>
<li><p>Build Pipeline: Reduced amount of garbage collection performed inside the ContentBuildInterface.</p></li>
<li><p>Burst: Fixed a compatibility issues between burst and older linux distros.</p></li>
<li><p>Burst: Fixed a potential error when running the linker with a failure on lld command.</p></li>
<li><p>Burst: Fixed a regression that could break usage of native plugins.</p></li>
<li><p>Burst: Fixed an issue preventing player builds to succeed when burst compilation is disabled.</p></li>
<li><p>Burst: Fixed an issue that prevented burst from resolving functions on platforms when it's statically linked such as iOS.</p></li>
<li><p>Burst: Fixed an issue where if a path to the package contained spaces, then native command execution would fail. This manifiested as weird errors with 'lld' or 'vswhere' or other native tools.</p></li>
<li><p>Burst: Fixed Debug.Log by re-enabling it when used in function pointers or jobs.</p></li>
<li><p>Burst: Fixed errors when opening Inspector with a non-public Execute method on a job producer type.</p></li>
<li><p>CodeEditor: Added support for solution folders.<br> Only bind the messenger when the VS editor is selected.<br>
Warn when unable to create the messenger.<br>
Fixed an initialization issue triggering legacy code generation.<br>
Allow package source in assembly to be generated when referenced from asmref.</p></li>
<li><p>CodeEditor: Fixed and issue where teh assembly references to package assemblies break IDE projects.</p></li>
<li><p>CodeEditor: RIDER - "The specified path is not of a legal form (empty)".</p></li>
<li><p>CodeEditor: RIDER - Guarantee that sln and csproj files are present, when OpenProject is called.</p></li>
<li><p>Core: Fixed crash when IME Strings got too long. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-when-typing-long-cangjie-keyboard-characters-into-the-input-field">1226610</a>)</p></li>
<li><p>DX12: Fixed a performance issue when invoking dynamic vertex buffer updates. (<a href="https://issuetracker.unity3d.com/issues/d3d12-large-performance-losses-when-invoking-dynamic-vertex-buffer-updates">1204804</a>)</p></li>
<li><p>DX12: Fixed an issue with MSAA which resolved on 2D texture arrays.</p></li>
<li><p>DX12: FrameTimingManager now works on DX12 Windows Standalone and UWP. (<a href="https://issuetracker.unity3d.com/issues/directx12-frametimingmanager-does-not-return-useful-data">1212335</a>)</p></li>
<li><p>Editor: "Generate all .csproj files" setting needs to be toggled on every startup for all the csproj files to actually be generated.</p></li>
<li><p>Editor: (case 1215825) UnityEngine.Diagnostics.ForceCrash does not produce crash dump when editor exits due to fatal error log message. (1215825)</p></li>
<li><p>Editor: Active Tool window now saves properly in the layout. (<a href="https://issuetracker.unity3d.com/issues/editortool-active-tool-window-isnt-save-in-the-project-layout">1224432</a>)</p></li>
<li><p>Editor: Allow pasting float numbers with a trailing f into number fields.</p></li>
<li><p>Editor: Automatic "unity is busy" progress dialogs on Windows no longer steal focus or pop up while the editor is not the active application.</p></li>
<li><p>Editor: Changed CTRL+click in Hierarchy so it changes the active object to reflect the Scene View behavior. (1154444)</p></li>
<li><p>Editor: Com.unity.test-framework does not print any messages when loaded into a project. (1214217)</p></li>
<li><p>Editor: Create Empty Parent' added to the hierarchy window context menu.</p></li>
<li><p>Editor: Cut' and 'Paste As a Child' functionality added to Scene View. (1215583)</p></li>
<li><p>Editor: Do not generate invalid project files when 'Open by file extension' is chosen. (<a href="https://issuetracker.unity3d.com/issues/unity-generates-broken-c-number-solution-and-project-files-if-external-script-editor-preference-is-set-to-open-by-file-extension">1246567</a>)</p></li>
<li><p>Editor: Don't display blank GameObject preview for Camera Prefab Assets. Instead, treat it the same as other Prefabs that don't have renderer components. (<a href="https://issuetracker.unity3d.com/issues/camera-prefab-icon-is-blank-in-inspectors-improved-prefab-section-and-project-window">1182438</a>)</p></li>
<li><p>Editor: Ensur EditorSettings works as preset. (<a href="https://issuetracker.unity3d.com/issues/dot-preset-files-properties-value-changes-are-not-reflected-when-the-values-are-modified-in-the-inspector-window">1223623</a>)</p></li>
<li><p>Editor: Fixed "Handles.Repaint called outside an editor OnGUI" error when folding out an Avatar Mask's Node Name property. (<a href="https://issuetracker.unity3d.com/issues/handles-dot-repaint-called-outside-an-editor-ongui-error-is-thrown-when-folding-out-an-avatar-masks-node-name-property">1244003</a>)</p></li>
<li><p>Editor: Fixed 3D texture preview drag rotation.</p></li>
<li><p>Editor: Fixed a bug where UTR fails with "No tests have been selected to run message" when in fact we attempt to run playmode tests in standalone player and connection times out.</p></li>
<li><p>Editor: Fixed a canceling rect selection that was breaking the inspector. (<a href="https://issuetracker.unity3d.com/issues/inspector-freezes-when-esc-key-is-pressed-while-editing-a-collider-and-drawing-a-selection-rectangle-in-the-scene-window">1253694</a>)</p></li>
<li><p>Editor: Fixed a class of GTK warnings showing up in the editor log when running the Linux editor. (<a href="https://issuetracker.unity3d.com/issues/multiple-gtk-warnings-pop-up-in-the-log-when-running-the-linux-editor">1268468</a>)</p></li>
<li><p>Editor: Fixed a crash that could occur when Burst compilation was scheduled before Burst had been initialized.</p></li>
<li><p>Editor: Fixed a crash when several editors were opened at the same time.</p></li>
<li><p>Editor: Fixed a crashed when a Transform was accessed during OnValidate. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-with-transform-getposition-when-exiting-play-mode-after-scene-reload">1114911</a>)</p></li>
<li><p>Editor: Fixed a float point imprecision with the rect tool. (<a href="https://issuetracker.unity3d.com/issues/cube-scales-in-x-axis-too-when-it-is-scaled-in-z-axis-while-using-rect-tool">1246267</a>)</p></li>
<li><p>Editor: Fixed a performance regression caused by Preferences 'Developer Mode' writing and reading preferences each frame. (1261270)</p></li>
<li><p>Editor: Fixed a race condition during input shutdown when unloading an input library on Windows. (<a href="https://issuetracker.unity3d.com/issues/crash-on-win-xinputdevice-poll-when-closing-the-editor">1250096</a>)</p></li>
<li><p>Editor: Fixed a ShortcutWindow profile dropdown that was missing the dropdown arrow. (<a href="https://issuetracker.unity3d.com/issues/shortcut-manager-profile-context-menu-dropdown-icon-is-missing-in-the-shortcuts-manager-window">1232757</a>)</p></li>
<li><p>Editor: Fixed a Unity crash in BroadcastMessageAny when parenting RectTransform in OnCanvasHierarchyChanged. (<a href="https://issuetracker.unity3d.com/issues/crash-on-transform-broadcastmessageany-when-parenting-recttransform-in-oncanvashierarchychanged">1255755</a>)</p></li>
<li><p>Editor: Fixed an alignment issue with the sorting group component in the inspector. (<a href="https://issuetracker.unity3d.com/issues/sorting-group-components-fields-have-no-margins-in-the-inspector-window">1264073</a>)</p></li>
<li><p>Editor: Fixed an Editor crash with TLSAllocator::GetAllocatedMemorySize() const when connecting wire-free earbuds in the Play mode. (<a href="https://issuetracker.unity3d.com/issues/macos-editor-crashes-with-tlsallocator-getallocatedmemorysize-const-when-connecting-wire-free-earbuds-in-the-play-mode">1261961</a>)</p></li>
<li><p>Editor: Fixed an error in player settings caused by switching platforms. (<a href="https://issuetracker.unity3d.com/issues/opening-player-setting-throws-exceptions-after-defining-a-scripting-symbol-and-switching-a-platform">1284565</a>)</p></li>
<li><p>Editor: Fixed an error that occurred when creating a new swatch preset library with a name containing "/". (<a href="https://issuetracker.unity3d.com/issues/imgui-could-not-determine-location-error-is-thrown-when-a-new-swatch-preset-library-is-created-by-name-starting-with-slash">1254004</a>)</p></li>
<li><p>Editor: Fixed an incompatibility issues with scripting based PlayerSettings and Presets. (1232077)</p></li>
<li><p>Editor: Fixed an incompatibility issues with scripting based PlayerSettings and Presets. (1232092)</p></li>
<li><p>Editor: Fixed an incompatibility issues with scripting based PlayerSettings and Presets. (1232095)</p></li>
<li><p>Editor: Fixed an incompatibility issues with scripting based PlayerSettings and Presets. (1232100)</p></li>
<li><p>Editor: Fixed an incompatibility issues with scripting based PlayerSettings and Presets. (1232104)</p></li>
<li><p>Editor: Fixed an incompatibility issues with scripting based PlayerSettings and Presets. (1232112)</p></li>
<li><p>Editor: Fixed an incompatibility issues with scripting based PlayerSettings and Presets. (1232117)</p></li>
<li><p>Editor: Fixed an incompatibility issues with scripting based PlayerSettings and Presets. (1232141)</p></li>
<li><p>Editor: Fixed an incorrect drag indicator issue when dragging sprites to the hierarchy. (<a href="https://issuetracker.unity3d.com/issues/gameobject-is-added-as-a-child-when-dragged-from-project-window-in-between-two-gameobjects">1178106</a>)</p></li>
<li><p>Editor: Fixed an issue by adding null check. (<a href="https://issuetracker.unity3d.com/issues/argumentoutofrangeexception-is-thrown-when-right-clicking-scriptableobjects-label-in-the-inspector">1211302</a>)</p></li>
<li><p>Editor: Fixed an issue by Calling UpdateCachedData to get updated info before updating the m_traker. (<a href="https://issuetracker.unity3d.com/issues/deleting-a-scrollbar-on-the-scrollview-causes-scene-to-become-dirty-multiple-times-in-a-row">1202591</a>)</p></li>
<li><p>Editor: Fixed an issue by setting the font size property value to zero in reset function. (<a href="https://issuetracker.unity3d.com/issues/imgui-font-size-property-from-text-mesh-component-is-not-resetting-on-selecting-reset">1239786</a>)</p></li>
<li><p>Editor: Fixed an issue in the Linux editor where mouse input in one window could create undesired visual changes in other windows upon repaint. (<a href="https://issuetracker.unity3d.com/issues/linux-hovering-over-console-messages-also-hovers-over-hierarchy-elements">1131492</a>)</p></li>
<li><p>Editor: Fixed an issue on Linux where the prefab overrides popup could overflow the available vertical screen space. (<a href="https://issuetracker.unity3d.com/issues/if-the-overrides-screen-is-taller-than-screen-part-of-the-screen-goes-out-of-display">1119679</a>)</p></li>
<li><p>Editor: Fixed an issue to enable scroll down automatically when first frame of logs does not fit in console window. (<a href="https://issuetracker.unity3d.com/issues/console-window-doesnt-scroll-down-automatically-when-initial-slash-first-frame-of-logs-does-not-fit">1241533</a>)</p></li>
<li><p>Editor: Fixed an issue wehre tvOS player settings would not work with presets. (1254898)</p></li>
<li><p>Editor: Fixed an issue when importing an Asset from a .unitypackage that has the same GUID as an existing Asset in the project wasn't displaying a warning. (<a href="https://issuetracker.unity3d.com/issues/unity-overrides-certain-scripts-even-when-they-are-named-differently">1250673</a>)</p></li>
<li><p>Editor: Fixed an issue where a prefab selection in the Scene View was not respecting user set picking flags. (1234665)</p></li>
<li><p>Editor: Fixed an issue where AllowSceneActivation was not respected during enter playmode. (<a href="https://issuetracker.unity3d.com/issues/allowsceneactivation-equals-false-is-ignored-when-particular-set-of-audio-files-are-present-in-the-scene">1153187</a>)</p></li>
<li><p>Editor: Fixed an issue where Alt+numpad Unicode character input would not works in the Windows editor. (<a href="https://issuetracker.unity3d.com/issues/no-input-appears-when-using-keyboard-character-shortcuts-with-alt-code-in-a-textfield">1174605</a>)</p></li>
<li><p>Editor: Fixed an issue where an exception was thrown when trying to show the contextual menu for an unloaded scene in the hierarchy window. (<a href="https://issuetracker.unity3d.com/issues/argumentexception-thrown-after-unloading-a-scene-and-right-clicking-in-the-hierarchy">1233432</a>)</p></li>
<li><p>Editor: Fixed an issue where assembly reloading happened more than once when switching to the Unity Editor from another app or between Unity Editor windows. (1272211)</p></li>
<li><p>Editor: Fixed an issue where certain dropdowns are misaligned in the player settings preset editor. (<a href="https://issuetracker.unity3d.com/issues/preset-supported-aspect-ratios-dropdown-icon-overlaps-with-window-layout-when-a-preset-of-player-settings-is-created">1218668</a>)</p></li>
<li><p>Editor: Fixed an issue where clicking the right edge of textures icon in material inspector would open a asset selection window. (<a href="https://issuetracker.unity3d.com/issues/texture-icon-box-opens-asset-selector-window-instead-of-revealing-the-asset-in-project-browser-when-clicking-on-its-right-side">1248553</a>)</p></li>
<li><p>Editor: Fixed an issue where ColorField had no border when showEyeDropper was set to false. (<a href="https://issuetracker.unity3d.com/issues/colorfield-has-no-outer-border-when-showeyedropper-is-set-to-false">1244882</a>)</p></li>
<li><p>Editor: Fixed an issue where dragging from a closed window in the mac Editor would crash. (1257002)</p></li>
<li><p>Editor: Fixed an issue where DrawGizmo attribute was not supporting interfaces. (1271985)</p></li>
<li><p>Editor: Fixed an issue where extra symbols were added to the field, when double clicking on non-equal values and trying to type over them. (<a href="https://issuetracker.unity3d.com/issues/double-clicking-on-non-equal-values-and-trying-to-type-over-them-results-in-symbols-added-to-the-field">1256909</a>)</p></li>
<li><p>Editor: Fixed an issue where Handles.Button prevented Scene View navigation. (<a href="https://issuetracker.unity3d.com/issues/handles-dot-button-doesnt-allow-camera-rotation-when-mouse-hovering-over-the-button">1250996</a>)</p></li>
<li><p>Editor: Fixed an issue where hidden components were not visible in the Inspector, even after the attached script was deleted. (<a href="https://issuetracker.unity3d.com/issues/component-with-hideflags-set-to-hideininspector-remains-hidden-when-the-referenced-script-is-removed">1250355</a>)</p></li>
<li><p>Editor: Fixed an issue where hierarchy search field was not always resetting when exiting prefab edit mode. (<a href="https://issuetracker.unity3d.com/issues/hierarchy-search-field-does-not-reset-when-searching-in-prefab-edit-mode-and-returning-back-to-scene">1265782</a>)</p></li>
<li><p>Editor: Fixed an issue where iOS player settings were not working with presets. (1232103)</p></li>
<li><p>Editor: Fixed an issue where Material Validation color swatches did not render after domain reload. (<a href="https://issuetracker.unity3d.com/issues/scene-slash-game-view-color-patches-are-missing-in-pbr-validation-settings-preview-window-for-all-the-three-sections">1250913</a>)</p></li>
<li><p>Editor: Fixed an issue where meta file info was not preserved when drag-copying assets in the Project Window. (<a href="https://issuetracker.unity3d.com/issues/scriptableobjects-mainobjectfileid-is-reset-when-duplicating-it-to-another-folder">1220825</a>)</p></li>
<li><p>Editor: Fixed an issue where multiple EventSystem instances could be created from a prefab in one scene. (<a href="https://issuetracker.unity3d.com/issues/multiple-eventsystem-instances-can-be-created-from-a-prefab-in-one-scene">1210254</a>)</p></li>
<li><p>Editor: Fixed an issue where no warning was occurring when duplicating an Asset from the Packages folder. (<a href="https://issuetracker.unity3d.com/issues/asset-does-not-get-duplicated-and-no-warning-occur-when-duplicating-an-asset-from-the-packages-folder">1265856</a>)</p></li>
<li><p>Editor: Fixed an issue where plugin resolution would fail if a plugin had two chained library extensions. (<a href="https://issuetracker.unity3d.com/issues/dllnotfoundexception-is-thrown-in-console-window-when-entering-the-play-mode">1217894</a>)</p></li>
<li><p>Editor: Fixed an issue where ProBuilder window stole focus on MacOS. Also ensures Application.isFocused only returns true in the Editor when GameView is focused (as is the documented behavior). (<a href="https://issuetracker.unity3d.com/issues/macos-hovering-the-mouse-on-probuilder-windows-buttons-regains-focus-on-the-unity-editor">1254752</a>)</p></li>
<li><p>Editor: Fixed an issue where right-clicking assets in the Hierarchy and Project window did not correctly highlight them. (<a href="https://issuetracker.unity3d.com/issues/mac-right-clicking-assets-in-the-hierarchy-and-project-window-does-not-correctly-select-slash-highlight-them">1222945</a>)</p></li>
<li><p>Editor: Fixed an issue where Scene View picking always returning the selection base when a prefab is the first selected object with a non-prefab GameObject behind. (<a href="https://issuetracker.unity3d.com/issues/cycling-through-objects-by-clicking-on-them-in-the-scene-view-gets-stuck-on-the-prefab-object-when-the-last-object-is-a-pref">1166101</a>)</p></li>
<li><p>Editor: Fixed an issue where SearchField style of custom editors does not match with other Search Fields in the editor. (<a href="https://issuetracker.unity3d.com/issues/imgui-searchfield-style-in-a-custom-editors-window-does-not-match-editors-searchfield-style">1243420</a>)</p></li>
<li><p>Editor: Fixed an issue where selected text is not replaced in Input Field. (<a href="https://issuetracker.unity3d.com/issues/typed-text-is-added-to-the-selected-text-when-using-inputfield-dot-onvalidateinput">1253193</a>)</p></li>
<li><p>Editor: Fixed an issue where Settings Window was not refreshing after selecting a Preset. (<a href="https://issuetracker.unity3d.com/issues/editor-values-under-project-settings-window-doesnt-update-on-selecting-its-preset-until-the-mouse-cursor-is-hovered-over-the">1268130</a>)</p></li>
<li><p>Editor: Fixed an issue where snapping didn't work only lines were showing.</p></li>
<li><p>Editor: Fixed an issue where switching between tabs in the Preferences window resized the Cinemachine tab's UI. (<a href="https://issuetracker.unity3d.com/issues/cinemachine-switching-between-different-tabs-in-preferences-window-resizes-cinemachine-tabs-ui">1258316</a>)</p></li>
<li><p>Editor: Fixed an issue where the -api-profile flag caused the editor to write to ProjectSettings/ProjectSettings.asset using binary serialization mode despite ForceText was configured in ProjectSettings/EditorSettings.asset.</p></li>
<li><p>Editor: Fixed an issue where the Build Settings window was not dockable. (1259782)</p></li>
<li><p>Editor: Fixed an issue where the context menu <code>Reset</code> was not functioning as intended with Assembly Definition and Reference files. (<a href="https://issuetracker.unity3d.com/issues/testrunner-reset-functionality-is-not-working-in-test-import-settings">1217217</a>)</p></li>
<li><p>Editor: Fixed an issue where the Editor crashed when maximizing and minimizing the docked IMGUI debugger window. (<a href="https://issuetracker.unity3d.com/issues/imgui-editor-crashes-on-maximizing-and-minimizing-imgui-debugger-window-when-inspected-view-is-selected">1257185</a>)</p></li>
<li><p>Editor: Fixed an issue where the first item was executed when pressing enter, even if nothing was selected. (<a href="https://issuetracker.unity3d.com/issues/quick-search-2-dot-0-0-first-entry-is-no-longer-active-by-default-must-press-down-first-before-pressing-enter">1258382</a>)</p></li>
<li><p>Editor: Fixed an issue where the Gizmos FoldOut does not expand until the mouse cursor is moved. (<a href="https://issuetracker.unity3d.com/issues/imgui-property-dropdown-of-gizmos-doesnt-expand-until-the-mouse-cursor-is-moved-under-physics-2d-in-the-project-settings">1228330</a>)</p></li>
<li><p>Editor: Fixed an issue where the input handler was set incorrectly when upgrading projects. (1287791)</p></li>
<li><p>Editor: Fixed an issue where the keyboardLayout was not returning correct value on linux. (<a href="https://issuetracker.unity3d.com/issues/linux-keyboardlayout-always-return-us">1167021</a>)</p></li>
<li><p>Editor: Fixed an issue where the Line Renderer Simplify toggle would not refresh the scene view. (<a href="https://issuetracker.unity3d.com/issues/line-renderers-simplify-preview-does-not-update-the-line-until-the-mouse-cursor-enters-the-scene-view">1258815</a>)</p></li>
<li><p>Editor: Fixed an issue where the Renderer component editor did not list the reflection probes when they were disabled in the SupportedRenderingFeatures. (1254082)</p></li>
<li><p>Editor: Fixed an issue where the Save Asset window does not close automatically after saving all assets. (<a href="https://issuetracker.unity3d.com/issues/imgui-save-asset-window-doesnt-close-automatically-and-appears-blank-after-saving-assets">1222647</a>)</p></li>
<li><p>Editor: Fixed an issue where the Scene View's Select All would not taking into account scene picking/visibility state. (<a href="https://issuetracker.unity3d.com/issues/sceneviz-select-all-shortcut-ignores-the-pickable-property-of-game-object">1250345</a>)</p></li>
<li><p>Editor: Fixed an issue where the Unity Download Assistant on Windows did not correctly displays progress as a positive percentage. (<a href="https://issuetracker.unity3d.com/issues/installer-installation-process-shows-a-negative-percentage-value-in-the-progress-bar-when-using-the-windows-download-assistant">1294162</a>)</p></li>
<li><p>Editor: Fixed an issue where the Unity Download Assistant on Windows did not correctly prompts for the download and install path. (<a href="https://issuetracker.unity3d.com/issues/the-unitydownloadassistant-no-longer-asks-for-the-install-path-on-windows">1294753</a>)</p></li>
<li><p>Editor: Fixed an issue where there were duplicate results from AssetDatabase.FindAssets. (<a href="https://issuetracker.unity3d.com/issues/assetdatabase-dot-findassets-returns-multiple-results-with-the-same-guid-for-one-fbx-file">1242371</a>)</p></li>
<li><p>Editor: Fixed an issue where tool tips in camera inspector were missing. (<a href="https://issuetracker.unity3d.com/issues/camera-tooltip-is-missing-for-the-target-display-property-under-camera-component">1263085</a>)</p></li>
<li><p>Editor: Fixed an issue where when "Add Component" button jumps in the inspector when resizing if has custom expandable UI Group elements. (<a href="https://issuetracker.unity3d.com/issues/add-component-button-jumps-on-top-of-other-properties-in-the-inspector-window-when-resizing-the-inspector-window">1230277</a>)</p></li>
<li><p>Editor: Fixed an issue where width of the border of the Alpha Value is not enclosed within boundary in the color picker. (<a href="https://issuetracker.unity3d.com/issues/color-picker-width-of-the-border-of-the-alpha-value-is-not-enclosed-within-boundary">1237286</a>)</p></li>
<li><p>Editor: Fixed an issue where windows overlapped over other windows on resizing. (<a href="https://issuetracker.unity3d.com/issues/imgui-hierarchy-and-project-window-overlaps-when-resizing-the-package-manager-window">1255867</a>)</p></li>
<li><p>Editor: Fixed an issue where you could not drag and drop from outside the project folder. (<a href="https://issuetracker.unity3d.com/issues/failed-copying-file-error-message-appears-while-dragging-file-from-explorer-to-the-editor">1270452</a>)</p></li>
<li><p>Editor: Fixed an issue with "Select Shader" option in inspector shader context menu. (<a href="https://issuetracker.unity3d.com/issues/linux-shader-selection-dropdowns-context-menus-select-shader-option-doent-work">1231531</a>)</p></li>
<li><p>Editor: Fixed an issue with Cancelling Display Dialog error when switching active input handling setting. (<a href="https://issuetracker.unity3d.com/issues/active-input-handling-mac-error-thrown-when-switching-active-input-handling">1283400</a>)</p></li>
<li><p>Editor: Fixed an issue with Linux using FitRectToScreen instead of FitWindowRectToScreen. (1263999)</p></li>
<li><p>Editor: Fixed an issue with object sorting in the Profiler window. (<a href="https://issuetracker.unity3d.com/issues/profiler-nullreferenceexception-thrown-when-sorting-columns-in-ui-details">1240861</a>)</p></li>
<li><p>Editor: Fixed an issue with Properties in the Canvas Scaler component not matching the properties in its Preset. (<a href="https://issuetracker.unity3d.com/issues/ui-properties-in-the-canvas-scaler-component-doesnt-match-with-the-properties-in-its-preset">1252603</a>)</p></li>
<li><p>Editor: Fixed an issue with restoring of Rect Transform on UNDO after a render mode change. (<a href="https://issuetracker.unity3d.com/issues/undo-doesnt-restore-ui-canvas-rect-transform-after-changing-canvas-render-from-world-space-to-screen-space">1246899</a>)</p></li>
<li><p>Editor: Fixed an issues related to labels that disappeared and Overlaping of labels in Layer Collision Matrix. (<a href="https://issuetracker.unity3d.com/issues/vertical-labels-of-the-layer-collision-matrix-overlap-with-the-rest-of-the-project-settings-ui">1259361</a>)</p></li>
<li><p>Editor: Fixed an issuey where the Editor toggle boxes' height did not adjusted to align with their label. (<a href="https://issuetracker.unity3d.com/issues/hdrp-enabled-checkboxes-are-misaligned-under-custom-passes-from-custom-pass-volume-component-in-the-inspector">1260494</a>, <a href="https://issuetracker.unity3d.com/issues/adaptive-performance-samsung-android-provider-property-is-not-aligned-with-its-checkbox-in-project-settings-menu">1267326</a>)</p></li>
<li><p>Editor: Fixed an object sixing issue when the Center scale handle was not given an initial scale that was [1,1,1]. (<a href="https://issuetracker.unity3d.com/issues/object-size-is-doubled-when-center-scaling-it-with-custom-script-using-handles-dot-scalehandle-method">1264038</a>)</p></li>
<li><p>Editor: Fixed an overflow issue where keycode mappings were  not using the  std maps. (1270330)</p></li>
<li><p>Editor: Fixed Android Target DPI player setting to work with presets. (1254906)</p></li>
<li><p>Editor: Fixed assembly hot reload inside the editor. (1251134)</p></li>
<li><p>Editor: Fixed camera speed slider not getting to min-max when setting min/max values with more than 2 decimals. (<a href="https://issuetracker.unity3d.com/issues/scenecamera-slider-handle-of-camera-speed-disappears-when-min-value-is-set-98-dot-99">1190430</a>)</p></li>
<li><p>Editor: Fixed cancel of multiple objects rename that would set their names to "&lt;multi&gt;" instead of keeping their original names. (<a href="https://issuetracker.unity3d.com/issues/multiple-selected-game-objects-with-different-names-are-renamed-to-when-pressing-esc-key-while-typing-a-new-name">1218183</a>)</p></li>
<li><p>Editor: Fixed disappearing "Edit..." button next to Shader dropdown list on Material UI.</p></li>
<li><p>Editor: Fixed dragging on Empty Favorites. (<a href="https://issuetracker.unity3d.com/issues/new-favorites-cannot-be-added-if-there-are-no-folders-in-the-favorite-section">1224386</a>)</p></li>
<li><p>Editor: Fixed error in import by adding support for the conversion of SkinWeights using UNorm16 and SNorm16 format. (1218889)</p></li>
<li><p>Editor: Fixed flickering when multiple windows were shown on macOS Editor. (<a href="https://issuetracker.unity3d.com/issues/osx-editor-windows-flicker-in-play-mode-when-dragging-and-docking-windows">1221722</a>)</p></li>
<li><p>Editor: Fixed foldout alignment in Physics2D Settings window. (<a href="https://issuetracker.unity3d.com/issues/imgui-properties-under-physics-2d-are-misaligned-in-the-project-setting-window">1228331</a>)</p></li>
<li><p>Editor: Fixed Frame Debugger to show Compute Shader dispatch information properly.</p></li>
<li><p>Editor: Fixed Highlighter APIs. (<a href="https://issuetracker.unity3d.com/issues/gui-items-are-not-found-and-highlighted-when-using-highligher-dot-highlight-method">1223530</a>)</p></li>
<li><p>Editor: Fixed incorrect GUI style for Influence Mask field in the ParticleSystem External Forces Module.</p></li>
<li><p>Editor: Fixed issue where an incorrect mesh index count was being displayed in the Mesh Inspector. (<a href="https://issuetracker.unity3d.com/issues/inspector-shows-indices-count-equal-to-a-sum-of-all-sub-meshes-even-when-the-sub-meshes-are-overlapping">1268635</a>)</p></li>
<li><p>Editor: Fixed issue where the free move's surface snap (shift+control) didn't use the new HandleUtility.PlaceObject extendable API.</p></li>
<li><p>Editor: Fixed issue with event data not being reset on subsequent clicks after the first one. (<a href="https://issuetracker.unity3d.com/issues/the-value-of-the-property-abstracteventdata-dot-used-does-not-reset-after-the-first-right-click-when-using-abstracteventdata-dot-use">1219722</a>)</p></li>
<li><p>Editor: Fixed issues caused when components required by other components do not exist. (<a href="https://issuetracker.unity3d.com/issues/crashes-when-removing-a-rigidbody-from-prefab-when-instance-of-a-prefab-has-a-configurable-joint-attached">876288</a>, <a href="https://issuetracker.unity3d.com/issues/crash-in-unity-fixedjoint-create-when-loading-a-specific-scene">887641</a>, 888143, <a href="https://issuetracker.unity3d.com/issues/editor-crashes-with-unity-characterjoint-create-when-removing-rigidbody-from-a-prefab-while-an-instance-has-a-character-joint">1086961</a>)</p></li>
<li><p>Editor: Fixed issues with AspectRatioFitter component. (<a href="https://issuetracker.unity3d.com/issues/aspect-ratio-fitters-fit-in-parent-aspect-mode-causes-scene-to-update-indefinitely">1199877</a>)</p></li>
<li><p>Editor: Fixed main editor window is no longer maximized when resetting the layout. (<a href="https://issuetracker.unity3d.com/issues/windows-editor-window-is-no-longer-maximized-when-changing-or-resetting-the-layout">1179646</a>)</p></li>
<li><p>Editor: Fixed New InputSystem not handling absolute mouse positions including those sent over RDP.</p></li>
<li><p>Editor: Fixed player settings visual glitch issue where "Metal API Validation" checkbox had an extra indentation level.</p></li>
<li><p>Editor: Fixed Preset incompatibilities in Player Settings (Default/Standalone). (1232067)</p></li>
<li><p>Editor: Fixed property dropdown of "Surface Effector 2D" doesn't expand until the mouse cursor is moved in Properties Window. (<a href="https://issuetracker.unity3d.com/issues/2d-options-property-dropdown-of-surface-effector-2d-doesnt-expand-until-the-mouse-cursor-is-moved-in-properties-window">1243958</a>)</p></li>
<li><p>Editor: Fixed property window cascading even though no property windows are opened. (1251625)</p></li>
<li><p>Editor: Fixed rare unstable asset hash.</p></li>
<li><p>Editor: Fixed rebuilding gizmo renderers caused an performance regressions. (1238713)</p></li>
<li><p>Editor: Fixed Scene View not accepting input after Maximizing and Un-maximizing while holding the right mouse button. (<a href="https://issuetracker.unity3d.com/issues/scene-window-freezes-when-holding-right-mouse-button-in-maximized-scene-window-and-minimizing-it-with-shift-plus-space-keys">1186624</a>)</p></li>
<li><p>Editor: Fixed script execution order values being cropped when using certain UI scaling values (mostly 125%). (<a href="https://issuetracker.unity3d.com/issues/script-execution-order-values-are-cropped-when-ui-scaling-is-set-to-125-through-display-settings">1182109</a>)</p></li>
<li><p>Editor: Fixed skybox persisting in scene after drag cancellation.</p></li>
<li><p>Editor: Fixed test ShortcutEntryConstructor_MethodWithShortcutArgs_FromAttribute in debug mode. (1233242)</p></li>
<li><p>Editor: Fixed Texture 2D Array support to the Render Texture Editor. (<a href="https://issuetracker.unity3d.com/issues/hdr-texture-rbg111110-in-inspector-preview-is-white-when-rendertexture-format-is-tex2darray">1238898</a>)</p></li>
<li><p>Editor: Fixed the Click Offset area for a GUI Button. (<a href="https://issuetracker.unity3d.com/issues/button-click-region-is-offset-when-the-ui-scaling-is-higher-than-100-percent">1240174</a>)</p></li>
<li><p>Editor: Fixed the crash when "Right click" is used to close an undocked preview window on Windows. (<a href="https://issuetracker.unity3d.com/issues/editor-occasionally-crashes-when-docking-slash-undocking-the-inspector-preview-window">1231889</a>)</p></li>
<li><p>Editor: Fixed the FillOrigin Enumpopup issue. (<a href="https://issuetracker.unity3d.com/issues/ui-image-fill-origin-is-changed-when-selecting-multiple-filled-type-images-with-different-fill-origin">1254876</a>)</p></li>
<li><p>Editor: Fixed the issue where the Grid opacity Input field is highlighted on changing the Grid Axis from the scene view grid settings window. (<a href="https://issuetracker.unity3d.com/issues/windows-on-changing-the-grid-axis-from-scene-view-grid-visibility-toggle-button-grid-opacity-input-field-gets-highlighted">1221530</a>)</p></li>
<li><p>Editor: Fixed the Object Selector window preventing object selection in the Scene View when searching for certain types. (<a href="https://issuetracker.unity3d.com/issues/editorguilayout-dot-objectfield-selection-pop-up-for-some-components-prevents-mouse-drag-multi-selection-in-scene-view">1241020</a>)</p></li>
<li><p>Editor: Fixed the warning thrown by the Clang compiler at Line 134 of "RuleSetFiles.cpp"  "warning- returning reference to local temporary object<br> [-Wreturn-stack-address]<br>
return core::string("");".</p></li>
<li><p>Editor: Fixed toggling Scene View from 2D to 3D locking the camera motion to the last direction of movement. (<a href="https://issuetracker.unity3d.com/issues/scene-slash-game-view-switching-to-3d-view-while-navigating-using-arrow-keys-in-2d-view-breaks-the-navigation-tool">1232270</a>)</p></li>
<li><p>Editor: Fixed Transform manipulator to use Undo.RecordObject so it works with livelink.</p></li>
<li><p>Editor: Fixed Unity Editor existing fullscreen mode when layout is changed. (<a href="https://issuetracker.unity3d.com/issues/unity-editor-gets-minimized-when-layout-is-changed">1232706</a>)</p></li>
<li><p>Editor: Fixed unselected Scene Views not respecting the mouse scroll wheel zoom shortcut. (<a href="https://issuetracker.unity3d.com/issues/unable-to-zoom-in-slash-out-in-other-than-the-last-selected-scene-windows-when-they-are-not-selected">1216819</a>)</p></li>
<li><p>Editor: Fixed usage of <code>restore_saved_layout</code> when <code>bottom_view</code> and <code>top_view</code> are null for an editor mode dynamic layout. (1244524)</p></li>
<li><p>Editor: Fixed vertex snapping incorrectly snapping to objects hidden by Scene Visibility flags. (1222442)</p></li>
<li><p>Editor: Fixed <code>EndLayoutGroup</code> errors when GUI items are highlighted by PrefixLabel. (<a href="https://issuetracker.unity3d.com/issues/themes-endlayoutgroup-errors-are-thrown-when-gui-items-are-highlighted-by-prefixlabel">1238526</a>)</p></li>
<li><p>Editor: Forces normal windows to open in the active space (on top of the editor) when editor is full screened on mac. This prevents a 'hidden' window. (<a href="https://issuetracker.unity3d.com/issues/macos-floating-windows-open-behind-other-fulls-screen-applications-when-full-screen-editor-is-opened-on-the-external-display">1218891</a>)</p></li>
<li><p>Editor: Game tab no longer undocks when switching between tabs while cursor is locked. Cursor no longer locks on focus, only on a click in the Game tab. Also fixes an issue where cursor lock would not function properly (e.g. lock without hiding) when moving docked window to a new location in the editor. All fixes are specific to the editor on Windows. (<a href="https://issuetracker.unity3d.com/issues/game-view-tab-becomes-undocked-when-switching-focus-to-it-from-another-tab-and-cursor-becomes-locked">1246445</a>)</p></li>
<li><p>Editor: GameObjects are not draggable when using the scroll wheel in macOS. (<a href="https://issuetracker.unity3d.com/issues/gameobjects-are-not-draggable-when-using-the-scroll-wheel">1175328</a>)</p></li>
<li><p>Editor: Gizmo icons are now displayed on all objects all the time unless object is selected. (1223375)</p></li>
<li><p>Editor: Hierarchy items are not considered hovered when scrolling the vertical scrollbar. (<a href="https://issuetracker.unity3d.com/issues/gameobjects-are-being-highlighted-when-dragging-the-scroll-bar-in-hierarchy-window">1229149</a>)</p></li>
<li><p>Editor: Implemented Getter and Setter for Blocking Mask property, so that it can be accessed through script. (<a href="https://issuetracker.unity3d.com/issues/graphic-raycaster-blocking-mask-is-accessible-through-the-inspector-but-not-through-script">1210118</a>)</p></li>
<li><p>Editor: In the linux editor, guiviews no longer gain focus on scroll events (scroll still occurs), which has the effect of preventing the editor from stealing focus on scrolls over guiviews that were previously unfocused. (1270605)</p></li>
<li><p>Editor: Including a trailing semi-colon in a testName filter no longer results in all tests being run. (<a href="https://issuetracker.unity3d.com/issues/testfilter-command-line-argument-does-not-filter-tests-when-test-names-are-separated-by-a-semicolon-and-an-empty-space">1171200</a>)</p></li>
<li><p>Editor: Inspector property copy/paste no longer allows pasting unrelated enum values. (<a href="https://issuetracker.unity3d.com/issues/imgui-copy-paste-feature-for-same-component-field-types-have-missing-validations">1222717</a>)</p></li>
<li><p>Editor: Internal.</p></li>
<li><p>Editor: Light icons in scene view now update immediately after light type is changed in inspector. (<a href="https://issuetracker.unity3d.com/issues/scene-slash-game-view-changing-the-light-type-doesnt-update-its-respective-gizmo-until-gameobject-loses-focus">1229003</a>)</p></li>
<li><p>Editor: Makes sure proper selected items are within hierarchy view after "selecte prefab root" and "invert selection", previously items would be properly selected but not in view of the hierarchy. (<a href="https://issuetracker.unity3d.com/issues/improved-prefab-prefab-root-is-not-displayed-in-hierarchy-on-selecting-root-if-its-not-in-current-hierarchy-view">1228117</a>)</p></li>
<li><p>Editor: Modified Android Icons PlayerSettings to work with presets. (1232114)</p></li>
<li><p>Editor: Modified arrays to be reorderable by default, and present non-reorderable arrays using legacy control.</p></li>
<li><p>Editor: Modified iOS Icons PlayerSettings to work with presets. (1232101)</p></li>
<li><p>Editor: Modified the LineRenderer editor positions view to always display the <code>index</code> column. (<a href="https://issuetracker.unity3d.com/issues/shuriken-removing-all-visible-columns-from-the-line-renderer-component-of-line-object-leads-to-argumentexception">1260526</a>)</p></li>
<li><p>Editor: Modified the settings provider example for how to write UI for a SettingsProvider to save the property editing. (1263452)</p></li>
<li><p>Editor: Modified the title of the splash screen window to clarify activity name on CentOS. (1232562)</p></li>
<li><p>Editor: Modified the tooltip text for the <em>Disable</em> button. (<a href="https://issuetracker.unity3d.com/issues/imgui-frame-debuggers-enable-slash-disable-button-displays-the-same-tooltip-irrespective-of-its-state">1240815</a>)</p></li>
<li><p>Editor: Modified the Unity menu to display the Windows menu item second from last. (<a href="https://issuetracker.unity3d.com/issues/linux-editor-window-and-help-menu-items-are-in-different-order-than-on-win">775676</a>)</p></li>
<li><p>Editor: Modified tvOS Icons PlayerSettings to work with presets. (1232093)</p></li>
<li><p>Editor: Mouse hover event is fixed in situations when windows are overlapping on macOS. (1222681)</p></li>
<li><p>Editor: Presets modifications array inconsistent size when excluding some properties. (<a href="https://issuetracker.unity3d.com/issues/presets-inconsistent-behaviour-of-preset-dot-propertymodifications-when-excluding-slash-including-properties">1229273</a>)</p></li>
<li><p>Editor: Project does not contain all .csproj files when "Generate All .csproj files" option is selected in preferences.</p></li>
<li><p>Editor: Re-added Mesh info to the Mesh Inspector Preview.</p></li>
<li><p>Editor: Removed extra spacing added to some fields in the inspector. (<a href="https://issuetracker.unity3d.com/issues/there-are-inconsistent-margins-between-position-rotation-and-scale-properties-in-the-transform-component">1235884</a>)</p></li>
<li><p>Editor: Static Analysis found I missed a spot to check if a pointer was NULL. (1229276)</p></li>
<li><p>Editor: The projection property in the Camera inspector is now properly getting the blue indicator, if changed in a prefab. (<a href="https://issuetracker.unity3d.com/issues/improved-prefab-blue-highlight-is-missing-on-making-changes-in-projection-of-main-camera-prefab">1197771</a>)</p></li>
<li><p>Editor: Transform shift rotate always reset the rotation value when used. (<a href="https://issuetracker.unity3d.com/issues/transformtool-shift-rotate-always-reset-the-rotation-value-when-used">1221620</a>)</p></li>
<li><p>Editor: Unity remote is no longer deprecated in the editor.</p></li>
<li><p>Editor: Updated cancel button when using SetValueWithoutNotify. (1246292)</p></li>
<li><p>Editor: Updated Collab package to 1.3.9.  See the package changelog for full details.</p></li>
<li><p>Editor: Updated the Doc URL server with the official public server. (1255912)</p></li>
<li><p>Editor: Updated the documentation for CreateEditor API to indicate that it has to be destroyed explicitly. (<a href="https://issuetracker.unity3d.com/issues/memory-leak-when-calling-editor-dot-createeditor">1250942</a>)</p></li>
<li><p>Editor: Updated the error message that is displayed when creating a swatch preset library with a filename beginning with a colon. (<a href="https://issuetracker.unity3d.com/issues/imgui-moving-file-failed-window-opens-when-a-swatch-preset-library-is-created-by-name-starting-with-colon">1254007</a>)</p></li>
<li><p>Editor: Updated the Profile Analyzer (com.unity.performance.profile-analyzer) to version 1.0.1, with various fixes included. See https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.0/changelog/CHANGELOG.html. (<a href="https://issuetracker.unity3d.com/issues/profile-anlyzer-timing-data-in-tooltip-for-top-10-markers-looks-incorrect">1253426</a>, 1254017, <a href="https://issuetracker.unity3d.com/issues/profile-analyzer-marker-summary-count-values-arent-sorted-descending">1254572</a>, <a href="https://issuetracker.unity3d.com/issues/profile-analyzer-blue-line-appeared-in-the-bottom-left-corner-of-the-compare-tab-in-the-profile-analyzer-window">1254868</a>, <a href="https://issuetracker.unity3d.com/issues/profile-analyzer-description-text-is-misaligned-in-the-single-tab-of-the-profile-analyzer-window">1254869</a>, <a href="https://issuetracker.unity3d.com/issues/profile-anayzer-marker-table-export-returns-different-information-on-5-dot-6-vs-2019-dot-3">1254870</a>, <a href="https://issuetracker.unity3d.com/issues/profile-analyer-histogram-buckets-for-count-values-look-to-be-out-or-maybe-a-rounding-issue">1256243</a>)</p></li>
<li><p>Editor: Updated the toolbar search field in the Settings window to be a fixed width. (<a href="https://issuetracker.unity3d.com/issues/adaptive-performance-search-bar-flickers-on-enabling-device-simulator-provider-while-adaptiveperformancesettings-is-selected">1257235</a>)</p></li>
<li><p>Editor: VSync gets disabled after Maximize on Play is disabled and Play Mode is unpaused after pausing. (<a href="https://issuetracker.unity3d.com/issues/gameview-vsync-gets-disabled-in-game-view-after-maximize-on-play-is-disabled-and-play-mode-is-unpaused-after-pausing">1230428</a>)</p></li>
<li><p>Editor: When attempting to create a new file beginning with a dot, auto-convert the character to an underscore, similar to what we do for other invalid characters, instead of displaying an error. (<a href="https://issuetracker.unity3d.com/issues/unable-to-create-a-prefab-when-gameobjects-name-starts-with-a-period">1117029</a>)</p></li>
<li><p>Editor: When creating a new asset in the project window of the Editor Unity will now no longer add the required file extension if the entered name already ends with it.  So for example creating a script called "Foo.cs" in the project will now create the file "Foo.cs" rather than "Foo.cs.cs".  The behaviour when the file extension is omitted is unchanged - creating the script "Foo" will create the file "Foo.cs" as normal. (<a href="https://issuetracker.unity3d.com/issues/new-c-number-script-is-appended-an-additional-cs-extension-when-its-name-already-contains-cs-extension">1251423</a>)</p></li>
<li><p>Editor: When deleting the last subfolder of an expanded folder, the icon stays the expanded folder one.<br> In fact the expanded status of the folder is not updated.<br>
This updates the status correctly.
(<a href="https://issuetracker.unity3d.com/issues/project-view-folder-icon-keeps-the-expanded-icon-when-subfolder-is-deleted-while-the-parent-folder-is-expanded">1233024</a>)</p></li>
<li><p>GI: Added convergence statistics for additional probes (Lightmapping.SetAdditionalBakedProbes) in the Lighting window.</p></li>
<li><p>GI: Baking light probes and additional probes  (Lightmapping.SetAdditionalBakedProbes) is faster.</p></li>
<li><p>GI: Ensured Prefab Mesh Renderers are properly affected when a user changes Receive GI, Lightmap Parameter, or Optimize UVs settings. (<a href="https://issuetracker.unity3d.com/issues/improved-prefabs-blue-highlight-is-not-available-for-contribute-and-receive-gi-in-mesh-renderer">1179530</a>)</p></li>
<li><p>GI: Ensured that all tooltips for Light Probe Proxy Volumes are present. (<a href="https://issuetracker.unity3d.com/issues/lppv-imgui-tool-tip-missing-for-refresh-mode-in-light-probe-proxy-volume">1245432</a>)</p></li>
<li><p>GI: Ensured that Contribute GI is enabled for Presets where appropriate. (<a href="https://issuetracker.unity3d.com/issues/preset-meshrenderer-does-not-save-changes-on-creating-its-preset-when-contribute-global-illumination-is-enabled">1223708</a>)</p></li>
<li><p>GI: Ensured that distance values for objects using level of detail (LOD) groups are correct.</p></li>
<li><p>GI: Ensured that GPU VRAM is released following a Progressive GPU Lightmapper bake. (<a href="https://issuetracker.unity3d.com/issues/gpulm-vram-not-released-following-a-gplum-bake">1204993</a>)</p></li>
<li><p>GI: Ensured that inspecting a mesh renderer with no vertex buffer or no index buffer does not cause crashes. (<a href="https://issuetracker.unity3d.com/issues/crash-in-spookyhash-short-when-marking-a-model-loaded-from-asset-bundles-as-static">1197692</a>)</p></li>
<li><p>GI: Ensured that LightmapParameters class is not null for new scenes and is accessible via the C# API, along with pushOff. Corrected the docs accordingly. (<a href="https://issuetracker.unity3d.com/issues/lightning-parameters-cant-be-accessed-by-c-number-api-reflection-usage-needed">1215629</a>)</p></li>
<li><p>GI: Ensured that moving an Object while baking does not break directionality while using the Progressive GPU Lightmapper. (<a href="https://issuetracker.unity3d.com/issues/moving-an-object-while-baking-breaks-uvs">1238156</a>)</p></li>
<li><p>GI: Ensured that RadeonRays::PlainBvhTranslator::Process does not cause the Editor to crash when using the Progressive GPU Lightmapper for neighboring Terrains. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-radeonrays-plainbvhtranslator-process-when-generating-lighting-with-gpu-lightmapper-for-neighboring-terrains">1198965</a>)</p></li>
<li><p>GI: Ensured that SceneLights in EnlightenBakeManager and ProgressiveRuntimeManagre do not have any memory leaks.</p></li>
<li><p>GI: Ensured that selecting a GPU, restarting the Editor, or unplugging the eGPu will not crash the Editor. (<a href="https://issuetracker.unity3d.com/issues/out-of-bounds-access-when-selecting-egpu-restarting-editor-unplugging-egpu">1272640</a>)</p></li>
<li><p>GI: Ensured that selective RGB, R, G, and B view access functions in the Lightmap thumbnail preview. (<a href="https://issuetracker.unity3d.com/issues/lighting-rgb-r-g-and-b-button-does-nothing-in-lightmap-thumbnail-preview">1199790</a>)</p></li>
<li><p>GI: Ensured that Static Batching does not corrupt Baked Lightmap scene visualizations on Play. (<a href="https://issuetracker.unity3d.com/issues/static-batching-corrupts-lightmap-uvs-on-play">1059722</a>)</p></li>
<li><p>GI: Ensured that the Custom Cache Folder Location updates correctly. (<a href="https://issuetracker.unity3d.com/issues/gi-cache-custom-cache-folder-location-updates-only-after-disabling-cache-compression">1228137</a>)</p></li>
<li><p>GI: Ensured that the Editor does not hang on close or when baking is canceled. (<a href="https://issuetracker.unity3d.com/issues/editor-hangs-on-close-when-baking-is-canceled-and-cpu-usage-is-100-percent">1235769</a>)</p></li>
<li><p>GI: Ensured that the Force Stop button functions properly when the user is running a bake with the Progressive Lightmapper and composite lightmaps are in their current state. (<a href="https://issuetracker.unity3d.com/issues/plm-force-stop-operation-takes-a-long-time-to-finish-when-baking-a-large-number-of-lightmaps">1069481</a>)</p></li>
<li><p>GI: Ensured that the GPU Lightmapper will not fall back to the CPU Lightmapper when the user moves the viewport during baking with progressive updates enabled. (<a href="https://issuetracker.unity3d.com/issues/gpu-plm-fallback-to-cpu-plm-with-various-open-cl-errors-when-moving-the-viewport-during-baking-with-progressive-updates-on">1286418</a>)</p></li>
<li><p>GI: Ensured that the Inspectors Float Range slider correctly functions in linear colour space on gamma properties. (<a href="https://issuetracker.unity3d.com/issues/urp-shaders-exposure-handler-disappeared-on-dragging-to-its-max-value-in-skybox-slash-6-sided-shader">1245429</a>)</p></li>
<li><p>GI: Ensured that the labels for the Lightmap thumbnail preview window is are properly aligned. (<a href="https://issuetracker.unity3d.com/issues/global-illumination-title-is-overlapping-on-rgb-menu-in-lightmap-thumbnail-preview">1113043</a>)</p></li>
<li><p>GI: Ensured that the miss marker for first bounce ray is correct.</p></li>
<li><p>GI: Ensured that the Progressive GPU Lightmapper will run on Apple Silicon.</p></li>
<li><p>GI: Ensured that the Progressive Lightmapper does not crash when using a rendertarget as a cookie texture. (1261117)</p></li>
<li><p>GI: Ensured that the Sun fields enum is the correct width. (<a href="https://issuetracker.unity3d.com/issues/imgui-sun-dropdown-icon-overlaps-with-text-when-the-high-quality-option-is-selected">1244279</a>)</p></li>
<li><p>GI: Ensured that Unity displays an error message when a user selects an unavailable denoiser. (<a href="https://issuetracker.unity3d.com/issues/ui-unable-to-select-optix-option-in-direct-denoiser-once-other-options-selected-in-filtering-under-lighting-window">1254973</a>)</p></li>
<li><p>GI: Ensured that users can select UV colors for a Lightmap Preview. (<a href="https://issuetracker.unity3d.com/issues/ui-unable-to-provide-custom-color-selection-for-uvs-in-lightmaps">1252445</a>)</p></li>
<li><p>GI: Ensured thatTempBuffer&lt;RenderTexture&gt; is not released in memory when users are using deprecated Realtime Global Illumination functionality.</p></li>
<li><p>GI: Make Experimental.Lightmapping.Bake and BakeAsync docs less confusing by calling out which objects are affecting the bake. (<a href="https://issuetracker.unity3d.com/issues/experimental-dot-lightmapping-dot-bake-docs-are-a-bit-confusing">1246519</a>)</p></li>
<li><p>GI: Reduced the incidence of invalid texels in Progressive Lightmapper bakes. (<a href="https://issuetracker.unity3d.com/issues/gpu-lightmapper-produces-invalid-texels-in-a-certain-scene">1217996</a>)</p></li>
<li><p>GI: Updated labels for Contribute and Receive GI mode in the Scene view. (1261852)</p></li>
<li><p>GI: When the Progressive GPU Lightmapper falls back to CPU Unity only creates OpenCL contexts. (<a href="https://issuetracker.unity3d.com/issues/lighting-baking-stucks-when-the-static-object-starts-to-bake-with-progressive-gpu-lightmapper">1208704</a>)</p></li>
<li><p>Graphics: - Fixed performance slowdown when releasing large amounts of buffers at once in Vulkan. Affects SRP batcher the most. (1102159)</p></li>
<li><p>Graphics: Added a warning message when intermediate renderers reset non-finite bounds to zero. (<a href="https://issuetracker.unity3d.com/issues/drawmeshinstanceindirect-does-not-render-an-instance-when-using-a-vector3-static-property-as-the-dimensions-of-the-bounds">1225021</a>)</p></li>
<li><p>Graphics: Added additional return code validation to various QueryInterface calls. (1229903)</p></li>
<li><p>Graphics: Added parameter to SkinnedMeshRenderer.BakeMesh(Mesh mesh, bool useScale) to take scaling into account when baking a mesh. By default this value is set to false to keep backwards compatibility. (<a href="https://issuetracker.unity3d.com/issues/meshes-vertices-are-not-relative-to-the-skinnedmeshrenderers-scale-when-executing-skinnedmeshrenderer-dot-bakemesh">1013310</a>)</p></li>
<li><p>Graphics: Added prompt when switching colors space in editor.<br> Setting color space to uninitialized via script is no longer valid.<br>
Updated RenderTextureDesc documentation.
(<a href="https://issuetracker.unity3d.com/issues/crash-color-space-uninitialised-can-be-set-via-c-number-script-but-build-player-will-crash">1274452</a>, <a href="https://issuetracker.unity3d.com/issues/ux-color-space-cancel-button-greyed-out-when-switching-color-space">1274453</a>)</p></li>
<li><p>Graphics: Added ScriptableCamera that can extend a Camera by inheritence.</p></li>
<li><p>Graphics: API to modify Virtual Texturing settings was changed to be more user friendly and finer grained.<br> Changing settings will now cause existing caches to be recreated instead of only affecting the sizes of new caches.</p></li>
<li><p>Graphics: CopyTexture with explicit mips and regions now copies the full texture when both textures have no mips specified and Texture Quality is not FullRes. This also adds a warning when Texture Quality is set and CopyTexture is used to copy textures with mismatched mips. (<a href="https://issuetracker.unity3d.com/issues/graphics-dot-copytextures-overload-with-region-parameters-copies-a-quarter-of-the-source-texture-when-texture-quality-is-half-res">1215135</a>)</p></li>
<li><p>Graphics: Corrected the condition that is used to display the copy texture warning about mip inconsistency. (1254356)</p></li>
<li><p>Graphics: Enabled valid tessellation behavior for HDRP on Metal API platforms.</p></li>
<li><p>Graphics: Ensure that when you have &gt; 63 material inspectors displayed that they will render and not throw an exception. (<a href="https://issuetracker.unity3d.com/issues/invalidoperationexception-thrown-and-performance-drop-when-selecting-a-mesh-inside-scene-view-with-more-than-63-submeshes">1156199</a>)</p></li>
<li><p>Graphics: Expose EmitGeometryForCamera to C# for SRP UI rendering. (1155022)</p></li>
<li><p>Graphics: Fixed 16-bit texture quantized to 8 bits during importing. (1212098)</p></li>
<li><p>Graphics: Fixed a bad sort operation that  caused random crashes during lightmap baking on OSX. (<a href="https://issuetracker.unity3d.com/issues/osx-crash-on-preparing-bake-stage-when-rebaking-gi-after-changing-lighting-settings-and-clearing-baked-data">1271626</a>)</p></li>
<li><p>Graphics: Fixed a calculation of disk read data issue. (1274963)</p></li>
<li><p>Graphics: Fixed a crash in the Editor when switching from HDRP to builtin pipeline in Graphics Settings. (<a href="https://issuetracker.unity3d.com/issues/editor-crash-when-switching-from-hdrp-to-builtin">1246590</a>)</p></li>
<li><p>Graphics: Fixed a crash on DirectX11 that happened when you created a texture with a partial mip chain. (<a href="https://issuetracker.unity3d.com/issues/crash-when-creating-a-new-texture2d-with-a-resolution-greater-or-equal-to-2048-and-the-mipcount-higher-than-1">1213005</a>)</p></li>
<li><p>Graphics: Fixed a crash that occured while calling VFX.VisualEffect.SetGradient with null. (<a href="https://issuetracker.unity3d.com/issues/visualeffectgraph-crash-on-unityengine-dot-vfx-dot-visualeffect-dot-setgradient-when-setting-gradient-to-null-value-with-setgradient">1271839</a>)</p></li>
<li><p>Graphics: Fixed a crash when calling Graphics.DrawMeshNow without first having called material.SetPass successfully. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-graphics-dot-drawmeshnow-is-called">1236602</a>)</p></li>
<li><p>Graphics: Fixed a crash when running Virtual Texturing with NativeGfxJobs enabled. (1254545)</p></li>
<li><p>Graphics: Fixed a crash when using invalid ScriptableCullingParameters inside a custom SRP. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-assigning-an-srp-asset-which-calls-a-cull-method-with-default-parameters">1218248</a>)</p></li>
<li><p>Graphics: Fixed a DXGI swapchain update regression from 2020.1.0a21, and changed a texture format that could cause Unity to crash.</p></li>
<li><p>Graphics: Fixed a mesh rendering issue in SRP Batcher when using Polybrush. (1220956)</p></li>
<li><p>Graphics: Fixed a missing memory barrier issue when abimage was repeatedly bound for writing between dispatch calls.</p></li>
<li><p>Graphics: Fixed a potential crash in VFX when effect was updated out of frustum in indirect mode. (1256791)</p></li>
<li><p>Graphics: Fixed a potential crash when enabling hardware dynamic resolution using DX12 renderer. (1158661)</p></li>
<li><p>Graphics: Fixed a potential crash when switching vsync at runtime. (<a href="https://issuetracker.unity3d.com/issues/android-player-crashes-when-changing-vsync-settings">1251670</a>)</p></li>
<li><p>Graphics: Fixed a prefab creation issue of non-MonoBehaviour ManagedObject component.</p></li>
<li><p>Graphics: Fixed a slow destruction of RenderTexture's internal resources when using Vulkan.</p></li>
<li><p>Graphics: Fixed a SystemInfo.minConstantBufferOffsetAlignment return type issue. (<a href="https://issuetracker.unity3d.com/issues/scriptreference-slash-systeminfo-minconstantbufferoffsetalignment-dot-html">1191780</a>)</p></li>
<li><p>Graphics: Fixed a TextureID leak when async loaded to a texture that was already loaded. (1266477)</p></li>
<li><p>Graphics: Fixed an exception that was thrown when creating unsupported Crunched Cubemap from script, Crunched Texture3D, CubemapArray, Texture2DArray and SparseTexture. (1278154)</p></li>
<li><p>Graphics: Fixed an int32 overflow issue that occured during RenderTexture runtime memory calculations. (<a href="https://issuetracker.unity3d.com/issues/creating-a-render-texture-throws-assertion-error-when-size-is-set-to-16384x16384-and-color-format-is-set-to-r16g16b16a16-sfloat">1263913</a>)</p></li>
<li><p>Graphics: Fixed an issue in RenderTargetIdentifier when comparing instances with different default values for m_DepthSlice. The default value is now -1, which is required by XR code.</p></li>
<li><p>Graphics: Fixed an issue whene import of 16 bit cubemaps with spherical or cylindrical mapping would fail. (<a href="https://issuetracker.unity3d.com/issues/project-enviroment-image-is-yellow-after-upgrading-projet-to-2020-dot-2">1284767</a>)</p></li>
<li><p>Graphics: Fixed an issue where copying compressed volume textures did not uses correct volume slice sizes. (1266585)</p></li>
<li><p>Graphics: Fixed an issue where CopyTexture might not respect the ignore texture limit flag resulting in wrong copies.</p></li>
<li><p>Graphics: Fixed an issue where GetShadowCasterBounds method were not correctly returning false when casters were beyond the set shadow distance. (<a href="https://issuetracker.unity3d.com/issues/getshadowcasterbounds-ignores-shadow-distance">1250914</a>)</p></li>
<li><p>Graphics: Fixed an issue where in some cases, Custom Render Textures would not be rendered (generally with asset bundles or in a standalone build). (<a href="https://issuetracker.unity3d.com/issues/custom-render-textures-are-not-rendered-in-a-standalone-build">1282195</a>)</p></li>
<li><p>Graphics: Fixed an issue where material references were getting discarded when a Renderer is Reset. (<a href="https://issuetracker.unity3d.com/issues/material-references-are-missing-when-replacing-a-mesh-renderer-component-by-skinned-mesh-renderer-component">1186957</a>)</p></li>
<li><p>Graphics: Fixed an issue where m_PreWarmDeltaTime had negative values. (<a href="https://issuetracker.unity3d.com/issues/prewarm-total-time-can-go-into-negatives-throwing-a-thread-group-size-must-be-above-zero-error">1167237</a>)</p></li>
<li><p>Graphics: Fixed an issue where rendertarget readback was not respecting channel layout. (<a href="https://issuetracker.unity3d.com/issues/command-buffer-blit-between-active-render-texture-into-bgra32-render-texture-is-rendered-black">1256612</a>)</p></li>
<li><p>Graphics: Fixed an issue where RenderTexture.Create with bindTextureMS option would fail silently if the used MSAA antiAliasing value was unsupported with the active graphics device.</p></li>
<li><p>Graphics: Fixed an issue where shadows were not taken into account on any light type if object was not on Default Light Layer. (1289846)</p></li>
<li><p>Graphics: Fixed an issue where some of the fields on the SkinnedMeshRenderer were missing tooltips. (<a href="https://issuetracker.unity3d.com/issues/mesh-renderer-tooltips-are-missing-for-properties-under-skinned-mesh-renderer-component">1263903</a>)</p></li>
<li><p>Graphics: Fixed an issue where tree billboards were not rotated correctly when the camera was moving on mobile platforms. (<a href="https://issuetracker.unity3d.com/issues/mobile-terrain-tree-billboards-not-rotating-while-camera-moving">1242389</a>)</p></li>
<li><p>Graphics: Fixed an issue where unexpected continue was causing a missing update in VisualEffect after Reset Override. (<a href="https://issuetracker.unity3d.com/issues/vfx-resetoverride-doesnt-serialize-correctly">1206890</a>)</p></li>
<li><p>Graphics: Fixed an issue where vulkan scratchbuffer int32 overflowed. (1272953)</p></li>
<li><p>Graphics: Fixed an issue with blend shape on Mali GPU. (1285097)</p></li>
<li><p>Graphics: Fixed an issue with drag and drop of non-MonoBehaviour ManagedObject's child component onto inspector.</p></li>
<li><p>Graphics: Fixed an issue with invalid state transitions in DX12 back-end. (1259951)</p></li>
<li><p>Graphics: Fixed an issue with missing support for texture 2d (ms) arrays.</p></li>
<li><p>Graphics: Fixed an issue with shadow caster culling for HDRP. (<a href="https://issuetracker.unity3d.com/issues/hdrp-box-lights-shadow-flicker-at-certain-camera-angles">1185407</a>)</p></li>
<li><p>Graphics: Fixed and issue where RenderPass api did not sample stencil input attachment.</p></li>
<li><p>Graphics: Fixed buffer over-read when decoding BC4/5 texture data. (1270857)</p></li>
<li><p>Graphics: Fixed build time regression in the built-in shader.</p></li>
<li><p>Graphics: Fixed crash when null is passed in to Material.GetTexturePropertyName().</p></li>
<li><p>Graphics: Fixed crash when null is passed in to Material.GetTexturePropertyNameIDs(). (<a href="https://issuetracker.unity3d.com/issues/crash-in-materialscripting-gettexturepropertynameidsinternal-when-calling-material-dot-gettexturepropertynameids-with-a-null-arg">1238775</a>)</p></li>
<li><p>Graphics: Fixed crash when trying to assign RenderTexture as input for a VT stack. (1235243)</p></li>
<li><p>Graphics: Fixed crash when using out-of-bounds indices with RenderPass API. (1226312)</p></li>
<li><p>Graphics: Fixed crash when using shader pass uses not first input attachment.</p></li>
<li><p>Graphics: Fixed Editor crash when using 2bpp PVRTC for 3D textures.</p></li>
<li><p>Graphics: Fixed flipped view when using RenderPass API.</p></li>
<li><p>Graphics: Fixed for UVMeshMetric calculation. (1248992)</p></li>
<li><p>Graphics: Fixed Frame Debugger when using RenderPass API.</p></li>
<li><p>Graphics: Fixed half precision support in compute shaders. (<a href="https://issuetracker.unity3d.com/issues/mobile-android-and-ios-do-not-support-fp16-on-compute-shader">1227467</a>)</p></li>
<li><p>Graphics: Fixed incorrect gamma decoding at import of LDR textures that target a HDR graphics format in a gamma colorspace project.</p></li>
<li><p>Graphics: Fixed incorrect input attachment indexing on fallback platforms.</p></li>
<li><p>Graphics: Fixed incorrect NativeArray aliasing when using CPU PVT. (1232623)</p></li>
<li><p>Graphics: Fixed Indirect drawcalls on Metal binding buffers with wrong offset. (1211151)</p></li>
<li><p>Graphics: Fixed inheritance of custom editors for renderpipeline when inheriting RenderPipelines. (<a href="https://issuetracker.unity3d.com/issues/inspector-showing-built-in-rp-gui-when-using-extended-universalrp-asset">1263659</a>)</p></li>
<li><p>Graphics: Fixed initialization of Camera's state which was causing an issue on Camera's child component's Reset.</p></li>
<li><p>Graphics: Fixed invalid GLSL code generation with result variable participating in comparisons. (<a href="https://issuetracker.unity3d.com/issues/hdrp-vulkan-sss-not-working-correctly-on-vulkan">1229297</a>)</p></li>
<li><p>Graphics: Fixed issue where one object in the scene would need ReceiveShadows set to true for Screen Space Shadows to be enabled when using deferred path. (<a href="https://issuetracker.unity3d.com/issues/skinnedmeshrenderer-not-receiving-shadows-in-game-view-if-its-the-only-gameobject-rendered-by-the-camera">1218683</a>)</p></li>
<li><p>Graphics: Fixed Metal RenderPass crash when there is no depth.</p></li>
<li><p>Graphics: Fixed offset calculations of volume slices for compressed texture formats. (<a href="https://issuetracker.unity3d.com/issues/an-error-is-thrown-in-the-console-window-when-copying-a-compressed-texture2d-with-graphics-dot-copytexture-to-texture3d">1249421</a>)</p></li>
<li><p>Graphics: Fixed RenderBufferLoadAction.Clear when using SRP RenderPass API. (1225431)</p></li>
<li><p>Graphics: Fixed RenderPass API Validation, SystemInfo.supportedRenderTargetCount is per subpass.</p></li>
<li><p>Graphics: Fixed ScreenCapture.CaptureScreenshotAsTexture crashing on Metal under some circumstances. (<a href="https://issuetracker.unity3d.com/issues/macos-crash-in-amdmtlbronzereadpixelbypixel2-when-calling-screencapture-dot-capturescreenshotastexture">1262959</a>)</p></li>
<li><p>Graphics: Fixed several performance issues with reflection probe anchors when reloading scenes.</p></li>
<li><p>Graphics: Fixed some VFX failing validation on metal, crashing editor/player. (<a href="https://issuetracker.unity3d.com/issues/unity-editor-crashes-when-opening-vfx-graph-or-dragging-vfx-asset-into-the-hierarchy">1231313</a>)</p></li>
<li><p>Graphics: Fixed static analysis defect - class member not initialized in constructor. (1240445)</p></li>
<li><p>Graphics: Fixed static analysis defect - class members not initialized in constructor. (1248294)</p></li>
<li><p>Graphics: Fixed static analysis defect - invalid error check. (1262795)</p></li>
<li><p>Graphics: Fixed the ObjectToWorld matrix used by the BatchRendererGroup when the shader opts for nomatrices instancing.</p></li>
<li><p>Graphics: Fixed transparent shaders with no _MainTex property not having offset and scale uniforms set when rendering for picking in the Scene View. (<a href="https://issuetracker.unity3d.com/issues/2d-unable-to-select-sprite-by-clicking-in-scene-view-when-another-sprite-is-using-maintex-property-with-tiling-slash-offset-values">1232257</a>)</p></li>
<li><p>Graphics: Fixed two gfx memory leaks that occurred when running HDRP and using a custom rendering solution in client/worker rendering mode.</p></li>
<li><p>Graphics: Fixed uninitialized variable in MeshRenderer. (1226229)</p></li>
<li><p>Graphics: Ignore points/line topology when raytracing mesh in editor for selection. (<a href="https://issuetracker.unity3d.com/issues/scrollwheel-click-to-center-on-gameobject-prints-errors-when-clicking-on-non-triangle-only-meshes">1183667</a>)</p></li>
<li><p>Graphics: Improved documentation for <code>Texture.allowThreadedTextureCreation</code>.</p></li>
<li><p>Graphics: Made export to png use grayscale image for R8. (<a href="https://issuetracker.unity3d.com/issues/texture-has-blue-tint-when-textureformat-dot-r8-is-used">1239813</a>)</p></li>
<li><p>Graphics: Metal: Fixed a compatibility issues with MSAA/filtering on Apple Silicon and macOS 11.</p></li>
<li><p>Graphics: Metal: Fixed a constant buffer binding issue with HDRP 9.x Decals shader.</p></li>
<li><p>Graphics: Metal: Fixed a regression with Time.deltaTime and disabling vsync.</p></li>
<li><p>Graphics: Metal: Fixed a system instability/hang issue with texture versioning. (1256106)</p></li>
<li><p>Graphics: Metal: Fixed HLSL compatibility issue with DrawProceduralIndirect. SV_InstanceID always starts at 0 but with Metal, a base instance was not subtracted for equal behavior.</p></li>
<li><p>Graphics: Metal: Fixed MSAA ResolveDepthIntoTexture to use the resolved texture as a source when doing blit into destination.</p></li>
<li><p>Graphics: Metal: Fixed shader compiler warnings that could appear on macOS 11 Big Sur/iOS 14.</p></li>
<li><p>Graphics: Removed a hitch on creation of large textures on DX12.</p></li>
<li><p>Graphics: Removed a unneeded PIX related assert.</p></li>
<li><p>Graphics: Shader Memory usage optimization in player. (1223610)</p></li>
<li><p>Graphics: SRP Batcher doesn't break at first element anymore when rendering hybrid v2 objects. (1263322)</p></li>
<li><p>Graphics: The DX12 renderer performance has been improved by only adding IASetPrimitiveTopology to a command list when the topology has changed.</p></li>
<li><p>Graphics: This fixes the crash during command buffer reading in d3d12 mode. (1233711)</p></li>
<li><p>Graphics: Thread safety fix to texture streaming manager. (1229887)</p></li>
<li><p>Graphics: Throw an exception when creating mesh with more streams than supported for mesh. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-mesh-dot-setvertexbufferparams-function-is-provided-with-a-vertexattributedescriptor-of-length-5-or-greater">1226104</a>)</p></li>
<li><p>Graphics: Tipfix uninitialized variables in TextureUploadMemoryDX11. (1231159)</p></li>
<li><p>Graphics: TotalTime is inconsistent with sum of deltaTime. (1237608)</p></li>
<li><p>Graphics: Updated message that is shown in Inspector when using a mesh without animation data for SkinnedMeshRenderer. (<a href="https://issuetracker.unity3d.com/issues/skinnedmeshrenderer-not-being-rendered-in-build">1229548</a>)</p></li>
<li><p>Graphics: Updated QualitySettings.streamingMipmapsRenderersPerFrame to support setting at runtime. (<a href="https://issuetracker.unity3d.com/issues/qualitysettings-dot-streamingmipmapsrenderersperframe-is-read-only-in-a-built-project">1222432</a>)</p></li>
<li><p>Graphics: When creating shaders for desktop metal, do not forcibly generate constexpr shader for comparison (this is needed for ios where older devices do not support setting comparison from the application side). (<a href="https://issuetracker.unity3d.com/issues/mac-urp-toon-shader-is-not-rendered-and-no-errors-are-shown-when-its-compiled">1201857</a>)</p></li>
<li><p>IL2CPP: Fixed an exception that could be throw if System.Data.DataCommonEventSource.ExitScope was called at runtime on a non-windows platform when managed code stripping is enabled. (1278839)</p></li>
<li><p>IL2CPP: Fixed building Universal Windows Platform player when using Windows SDK versions 15063 or 16299.</p></li>
<li><p>IL2CPP: Respect the DllImportAttribute.PreserveSig property on PInvoke definitions.</p></li>
<li><p>IL2CPP: Respect the PreserveSigAttribute on COM interop types. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-preservesig-attribute-is-ignored-when-building-with-il2cpp">1202914</a>)</p></li>
<li><p>IMGUI: Fixed a scroll bar thumb overlapping with arrow icons issue in the console window. (<a href="https://issuetracker.unity3d.com/issues/imgui-console-scrollbars-down-directional-arrow-button-overlaps-on-scrollbar-handles-on-reducing-error-description-panel">1269928</a>)</p></li>
<li><p>IMGUI: Fixed an issue where NotImplementedException is thrown on double clicking instructions from Inspected view when mode set to Clip. (<a href="https://issuetracker.unity3d.com/issues/imgui-debugger-notimplementedexception-is-thrown-on-selecting-instructions-from-inspected-view-when-mode-set-to-clip">1251517</a>)</p></li>
<li><p>IMGUI: Fixed an issue with pop up menus needing additional click to switch. (<a href="https://issuetracker.unity3d.com/issues/popup-menus-are-modal-and-blocking-requiring-two-clicks-to-switch">1247542</a>)</p></li>
<li><p>IMGUI: Fixed IndexOutOfRangeException when loading the editor. (<a href="https://issuetracker.unity3d.com/issues/splitter-indexoutofrangeexception-when-opening-the-editor">1241206</a>)</p></li>
<li><p>IMGUI: Fixed text input field not scrolling issue when cursor is moved. (<a href="https://issuetracker.unity3d.com/issues/transform-values-that-do-not-fit-their-input-field-in-the-inspector-window-cannot-be-viewed-after-their-cutoff-point">1268088</a>)</p></li>
<li><p>IMGUI: Fixed the issue where the last selection is shown as focused even after selection another window. (<a href="https://issuetracker.unity3d.com/issues/imgui-options-dont-lose-focus-completely-on-deselection-in-inspector-slash-project-settings-slash-preferences">1241127</a>)</p></li>
<li><p>IMGUI: Fixed the slider thumb artifact when multi editing. (<a href="https://issuetracker.unity3d.com/issues/undoing-slider-fields-when-multi-selecting-from-one-common-value-to-a-non-equal-value-state-leaves-a-slider-handle-artifact">1256600</a>)</p></li>
<li><p>iOS: Fixed a xcode warning when UnityAppController.h was included in .m file. (<a href="https://issuetracker.unity3d.com/issues/ios-xcode-exported-unityappcontroller-dot-h-throws-2-this-block-declaration-is-not-a-prototype-warnings">1267931</a>)</p></li>
<li><p>iOS: Fixed an issue where active/visible status of ipad floating keyboard were mishandled. (<a href="https://issuetracker.unity3d.com/issues/ipados-13-touchscreenkeyboard-dot-visible-isnt-updated-if-using-floating-keyboard">1217147</a>)</p></li>
<li><p>iOS: Fixed an issue where Arcade's application was using a prohibited API when using Social API function.</p></li>
<li><p>iOS: Fixed an issue where GetKeyUp and GetKeyDown functions were  returning true on every frame. (<a href="https://issuetracker.unity3d.com/issues/ios-controller-getkeyup-and-getkeydown-are-called-every-frame-when-a-button-on-controller-is-being-pressed">1218784</a>)</p></li>
<li><p>iOS: Fixed an occassional crash on exit coming from iOS calling [UIViewController prefersHomeIndicatorAutoHidden] or [UIViewController preferredScreenEdgesDeferringSystemGestures] after unity has been killed.</p></li>
<li><p>iOS: Fixed default specular cubemap format for iOS and tvOS to be PVRTC.</p></li>
<li><p>iOS: Fixed game crashing after using Social.LoadUsers and then changing scene. (<a href="https://issuetracker.unity3d.com/issues/ios-il2cpp-crash-on-il2cpp-vm-livenessstate-addprocessobject-when-using-social-dot-loadusers-and-then-changing-scenes">1270230</a>)</p></li>
<li><p>iOS: Fixed sound becoming muted after quickly swapping to voice dictation and back to app. (<a href="https://issuetracker.unity3d.com/issues/ios-sound-becomes-muted-after-quickly-swapping-to-voice-dictation-and-back-to-app">1176463</a>)</p></li>
<li><p>Kernel: AlignOf&lt;T&gt; returns C# required structure alignment, instead of 4.</p></li>
<li><p>Kernel: Fixed a stall issue when entering playmode with many pending Burst jobs to compile.</p></li>
<li><p>Kernel: Fixed an issue where worldPositionStays argument was missing from Undo.SetTransformParent. (<a href="https://issuetracker.unity3d.com/issues/worldpositionstays-argument-is-missing-from-unity-dot-undo-dot-settransformparent-in-comparison-with-transform-dot-setparent">1247086</a>)</p></li>
<li><p>Kernel: Fixed issue with debug assert raised in unique_ptr, when move-from is either default constructed or already moved-from. (<a href="https://issuetracker.unity3d.com/issues/error-unique-ptr-move-assignment-error-rhs-memory-label-does-not-match-when-docking-windows">1226908</a>)</p></li>
<li><p>Kernel: Fixed rounding when undoing parenting. (<a href="https://issuetracker.unity3d.com/issues/transform-values-change-by-a-tiny-amount-when-undoing-parenting">1214246</a>)</p></li>
<li><p>Kernel: NativeArray.Dispose behavior to not throw when Allocator.None is used.</p></li>
<li><p>License: Fixed an issue where Report/log licensing errors were not sent by the client. (1273213)</p></li>
<li><p>Linux: Disabled unstable DrawHeader_WhenInvokedManually_FromPrefabOverridesTreeView_InvokesCallback test for case 1179487.</p></li>
<li><p>Linux: Fixed a highlighting issue in the hierarchy window while dragging assets. (<a href="https://issuetracker.unity3d.com/issues/linux-gameobjects-in-the-hierarchy-window-are-not-highlighted-when-dragging-an-asset-from-the-project-window-over-them">1251614</a>)</p></li>
<li><p>Linux: Fixed an Editor crashes if there was not a X11 window desktop environment. (1264934)</p></li>
<li><p>Linux: Fixed an issue where the eyedropper tool in the color picker did not work on Linux. (<a href="https://issuetracker.unity3d.com/issues/linux-editor-color-picker-does-not-work">1174814</a>)</p></li>
<li><p>Linux: Fixed keyboard modifiers from being incorrectly munged while moving between editor windows. (<a href="https://issuetracker.unity3d.com/issues/linux-cannot-move-object-when-rect-tool-is-selected-after-resizing-while-keeping-shift-held-down">1218006</a>, <a href="https://issuetracker.unity3d.com/issues/linux-scene-view-navigation-functionality-does-not-adjust-properly-when-ctrl-and-alt-keys-are-swapped">1236681</a>)</p></li>
<li><p>Linux: Fixed performance regression while running in Play mode inside the editor. (<a href="https://issuetracker.unity3d.com/issues/linux-performance-regression-in-play-mode-while-using-the-editor-on-linux-play-mode-is-unable-to-reach-more-than-10fps">1271213</a>)</p></li>
<li><p>Linux: Fixed sporadic errors in the console due to sending invalid drag events. (<a href="https://issuetracker.unity3d.com/issues/linux-assertion-failed-errors-are-occasionally-thrown-when-reordering-gameobjects-in-the-hierarchy-window">1251591</a>)</p></li>
<li><p>Linux: Fixed UnitySetup -L option incorrectly showing defaults. (<a href="https://issuetracker.unity3d.com/issues/linux-installer-installs-only-editor-if-unattended-although-all-components-are-marked-as-default">1160471</a>)</p></li>
<li><p>macOS: CPU usage decreased for Player built with 'Run in Background'. (<a href="https://issuetracker.unity3d.com/issues/macos-cpu-usage-increases-instead-of-decreasing-when-unfocusing-a-player-built-with-run-in-background-option-disabled">1240835</a>)</p></li>
<li><p>macOS: Fixed a -screen-quality command line argument issue for the player on all desktop platforms. (<a href="https://issuetracker.unity3d.com/issues/screen-quality-command-argument-has-no-effect-on-built-application">1094263</a>)</p></li>
<li><p>macOS: Fixed an issue where macOS Standalone player would not build on case sensitive file systems. (<a href="https://issuetracker.unity3d.com/issues/macos-x64arm64-builds-fail-on-case-sensitive-file-systems">1293383</a>)</p></li>
<li><p>macOS: Fixed an issue where MONO variable path did not have quotes in generated .sh script when exporting the Xcode project. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-macos-mono-variable-path-has-no-quotes-in-generated-sh-script-when-exporting-the-xcode-project">1274999</a>)</p></li>
<li><p>macOS: Fixed an issue where shader pre-warming would crash when a fragment shader returns something else than the usual 4 components. (<a href="https://issuetracker.unity3d.com/issues/ios-urp-metal-gpu-crashes-and-compiler-failed-to-build-request-error-is-thrown-on-shader-warm-up">1264839</a>)</p></li>
<li><p>macOS: Fixed an issue where target .xcodeproj was used instead of the target directory when building MacOS Xcode Project. (<a href="https://issuetracker.unity3d.com/issues/mac-os-building-standalone-project-for-mac-when-generate-xcode-project-is-enabled-generates-both-a-folder-and-xcodeproj">1288729</a>)</p></li>
<li><p>macOS: Fixed an issue where the Build Settings window would not minimizes with the editor window. (<a href="https://issuetracker.unity3d.com/issues/mac-build-settings-window-doesnt-minimize-after-minimizing-the-editor">1199503</a>)</p></li>
<li><p>macOS: Fixed an issue where the Catalina system font directory to font search paths was not added. (1249128)</p></li>
<li><p>macOS: Fixed assets cannot be saved if the project name contains certain Unicode characters. (<a href="https://issuetracker.unity3d.com/issues/macos-assets-cannot-be-saved-if-the-project-name-contains-certain-unicode-characters">1229500</a>)</p></li>
<li><p>macOS: Fixed console window lose focus when status bar is clicked to show it. (<a href="https://issuetracker.unity3d.com/issues/mac-console-window-does-not-maintain-focus-when-the-status-bar-is-repeatedly-clicked-to-show-the-console-window">1227963</a>)</p></li>
<li><p>macOS: Fixed duplicate "Replace" dialog when building iOS target on macOS 10.15. (<a href="https://issuetracker.unity3d.com/issues/ios-cannot-append-build">1265065</a>)</p></li>
<li><p>macOS: Fixed Input Method Editor on macOS so that the user's cursor appears in the location they intend.</p></li>
<li><p>macOS: Fixed issue on MacOS where VSync was not locking framerate when in fullscreen. (<a href="https://issuetracker.unity3d.com/issues/macos-opengl-vsync-count-does-not-lock-the-framerate-upon-launching-the-player-with-qualitysettings-dot-vsynccount-equals-1">1239354</a>)</p></li>
<li><p>macOS: Fixed issue where using the CanvasScalar with Physical Constraint set would cause a performance regression. (1241982)</p></li>
<li><p>Mobile: Fixed iOS/tvOS bundle ID format restrictions to match Apple requirements. (<a href="https://issuetracker.unity3d.com/issues/ios-build-fails-when-bundle-id-doesnt-contain-a-period">1240017</a>)</p></li>
<li><p>Mobile: Fixed ProjectCapabilityManager adding corresponding frameworks to the wrong target. (<a href="https://issuetracker.unity3d.com/issues/ios-projectcapabilitymanager-dot-addsigninwithapple-adds-authenticationservices-framework-for-the-wrong-target">1245194</a>)</p></li>
<li><p>Mobile: Fixed several InputField errors when selecting text with Hide Mobile Input enabled. (<a href="https://issuetracker.unity3d.com/issues/mobile-selecting-text-from-input-field-throws-exceptions-when-hide-mobile-input-is-enabled">1247399</a>)</p></li>
<li><p>Mobile: Removed Game SDK 3.1 initialization due to issues in GameSDK 3.1. Any other GameSDK version is still supported.</p></li>
<li><p>Mobile: Removed notification package from Tests/GeneratedTests/PackageIsolationTests/Assets/Resources/ExemptionList.json to clean the console test. (1252209)</p></li>
<li><p>Multiplayer: Added and/or fixing range validation of indexes coming from network to be in-bound before using them.</p></li>
<li><p>Package: Fixed an issue where CinemachineBlendListCamera was incorrectly holding 0-length camera cuts.</p></li>
<li><p>Package Manager: Adjusted package 'Preview' and 'Verified' tag colors in Light mode to meet minimum legal contrast requirements.</p></li>
<li><p>Package Manager: Changed function signature and comments.</p></li>
<li><p>Package Manager: Changed Package Manager window to use UIElements VisualSplitter instead of custom splitter class. This makes the window behave more consistently with other application windows with a split view, i.e. Preferences Window. Split view resizing with window resizing now works in Package Manager window.</p></li>
<li><p>Package Manager: Created a proxy for AssetDatabase, such that in the test environment we never rely on the state of the real AssetDatabase.</p></li>
<li><p>Package Manager: Fixed a issue where samples for a package were not refreshed after modifying in package.json. (<a href="https://issuetracker.unity3d.com/issues/packman-package-manager-does-not-refresh-slash-update-on-package-dot-json-changes-only-after-editor-restart">1233444</a>)</p></li>
<li><p>Package Manager: Fixed a possible null error in console when listing samples.</p></li>
<li><p>Package Manager: Fixed an issue in the <code>UnityEngine.PackageManager.Client.Pack</code> method did not properly use the contents of <code>.gitignore</code> when <code>.npmignore</code> was missing.</p></li>
<li><p>Package Manager: Fixed an issue in the <code>UnityEngine.PackageManager.Client.Pack</code> method which could sometimes result in file permission issues.</p></li>
<li><p>Package Manager: Fixed an issue where  a deleted custom package still was displayed in project window. (<a href="https://issuetracker.unity3d.com/issues/deleted-custom-package-still-displayed-in-project-window">1266789</a>)</p></li>
<li><p>Package Manager: Fixed an issue where a network requests sometime mislabeling the host as <code>undefined</code> when unsuccessful.</p></li>
<li><p>Package Manager: Fixed an issue where Asset Store package download progress tracking UX was inconsistent in the Package Manager window. (1272970)</p></li>
<li><p>Package Manager: Fixed an issue where download and import was enabled for an asset that was not available on the Asset Store.</p></li>
<li><p>Package Manager: Fixed an issue where npm authentication configuration was ignored when there was an extraneous slash at the end of the configured registry URL.</p></li>
<li><p>Package Manager: Fixed an issue where preview packages from Scoped Registries where filtered out.</p></li>
<li><p>Package Manager: Fixed an issue where samples showed randomly when package was not installed and Sample.FindByPackage API did not work if the package manager window was not open.</p></li>
<li><p>Package Manager: Fixed an issue where the Diagnose button in the critical startup failure dialog would not launch a diagnostics window on Linux.</p></li>
<li><p>Package Manager: Fixed an issue where the same git package twice could not be added twice. (<a href="https://issuetracker.unity3d.com/issues/adding-a-new-git-package-section-doesnt-go-away-when-adding-an-already-installed-package-from-git-url">1263238</a>)</p></li>
<li><p>Package Manager: Fixed an issue where the Unity Package Manager could take more time to start up than the 10 seconds allotted by Unity.</p></li>
<li><p>Package Manager: Fixed an issue where the <code>Client.GetAllPackageInfo</code> method would silence errors and return an empty list of packages when there were registry reachability issues.</p></li>
<li><p>Package Manager: Fixed an issue where tooltip doesn't show up  for the GroupName label.</p></li>
<li><p>Package Manager: Fixed an issue where <code>PackageManager.Client.Remove</code> request was still proceeding after input package name contained unsupported characters like carriage return or line feed failed validation.</p></li>
<li><p>Package Manager: Fixed an issue with search query after manual refresh.</p></li>
<li><p>Package Manager: Fixed an null error issue in Scoped Registries Settings.</p></li>
<li><p>Package Manager: Fixed and issue with  label superposition of the toggle button when using 4k screen. (<a href="https://issuetracker.unity3d.com/issues/enable-preview-packages-setting-name-is-clipping-with-the-checkbox-on-high-resolution-displays">1243974</a>)</p></li>
<li><p>Package Manager: Fixed AssetStore package display issue with poor internet connection.</p></li>
<li><p>Package Manager: Fixed defect in AssetStorePackage reported by static code analysis. (1237761)</p></li>
<li><p>Package Manager: Fixed defect in AssetStoreProductInfo reported by static code analysis. (1237762)</p></li>
<li><p>Package Manager: Fixed issue where 'user not logged in' error sometimes occurs on opening Unity Editor with Package Manager window opened to My Assets.</p></li>
<li><p>Package Manager: Fixed issue where Package Manager UI shows empty list when there's an error in ScopedRegistry settings.</p></li>
<li><p>Package Manager: Fixed Package Manager dialog box could be empty if the error message was too long.</p></li>
<li><p>Package Manager: Fixed potential null error in Package Database.</p></li>
<li><p>Package Manager: Fixed scroll for package dev description.</p></li>
<li><p>Package Manager: Fixed the blurry dropdown button for preview packages.</p></li>
<li><p>Package Manager: Fixed the issue where ArgumentException will be thrown when opening Asset Store page in Package Manager window when Charles Proxy is running.</p></li>
<li><p>Package Manager: Fixed the issue where Packman UI won't refresh on package.json update.</p></li>
<li><p>Package Manager: Fixed the superposition of the text packages and load next in package load bar.</p></li>
<li><p>Package Manager: Fixed when viewing offline docs not working if there is no program associated to markdown files in the operation system.</p></li>
<li><p>Package Manager: Fixed <code>PackageInfo.FindForAssetPath</code> performance overhead. (1221526)</p></li>
<li><p>Package Manager: Grey out package in inspector.</p></li>
<li><p>Package Manager: Internal changes, moved DownloadImageAsync function into AssetStoreCache class so it is with the Load and Save Image functions.</p></li>
<li><p>Package Manager: Match download bar to windows size.</p></li>
<li><p>Package Manager: Moved storage of npm credentials from system/global configuration to user configuration. The file format was also changed to TOML.</p></li>
<li><p>Package Manager: Removing a custom package in development was not updated in the UI.</p></li>
<li><p>Package Manager: Set actif remove button when element present.</p></li>
<li><p>Particles: Added error message when using sub-emitters outside the hierarchy of the parent system. (<a href="https://issuetracker.unity3d.com/issues/non-child-sub-emitter-particles-move-slash-shift-slash-teleport-when-modifying-transform-and-play-on-awake-is-off">1230728</a>)</p></li>
<li><p>Particles: Disabled Particle System "Open In Editor" button when editing a preset.</p></li>
<li><p>Particles: Display a warning message if a Stop Action is used on a sub-emitter. (<a href="https://issuetracker.unity3d.com/issues/sub-emitter-doesnt-call-onparticlesystemstopped-function-if-the-parent-particle-system-is-still-alive">1218545</a>)</p></li>
<li><p>Particles: Fixed a crash when using BakeTrails with <code>Attach Ribbons to Transform</code>.</p></li>
<li><p>Particles: Fixed particle lights being re-rendered over multiple frames.</p></li>
<li><p>Particles: Hide scene view controls from the Particle System Inspector when viewing Prefab overrides. (<a href="https://issuetracker.unity3d.com/issues/shuriken-shape-transform-tool-goes-out-of-layout-under-shape-module-from-particle-system-in-prefab-override-window">1242874</a>)</p></li>
<li><p>Particles: Hide the noise preview Texture when viewing Prefab overrides. (<a href="https://issuetracker.unity3d.com/issues/shuriken-quality-dropdown-icon-overlaps-with-text-under-noise-module-from-particle-system-in-prefab-override-window">1242905</a>)</p></li>
<li><p>Particles: IsEmitting script API should return false if the emission module is disabled. (<a href="https://issuetracker.unity3d.com/issues/particlesystem-dot-isemitting-returns-true-when-the-emission-module-is-disabled">1240811</a>)</p></li>
<li><p>Physics: Fixed  an issue where the changes and the prefab override conditions were not being properly handled and displayed by the MeshCollider inspector for the Cooking Options property. (<a href="https://issuetracker.unity3d.com/issues/prefabs-blue-highlight-override-indicator-is-missing-for-cooking-options-dropdown-in-mesh-collider">1267893</a>)</p></li>
<li><p>Physics: Fixed a crash when a BoxCollider produced more than 64 contact points with another convex collider. (<a href="https://issuetracker.unity3d.com/issues/macos-hinge-joint-with-mesh-collider-causes-a-crash-on-a-specific-project">1269931</a>)</p></li>
<li><p>Physics: Fixed a memory leak than occured when a physics scene was unloaded. (1257745)</p></li>
<li><p>Physics: Fixed an issue with ray casts not working correctly with colliders that have attached ArticulationBody components.</p></li>
<li><p>Physics: Fixed an issue with the Cloth component's virtual particles being set incorrectly at creation.</p></li>
<li><p>Physics: Fixed ArticulationBody.immovable property setter to have effect when set during runtime.</p></li>
<li><p>Physics: Fixed ArticulationBody.jointPosition crash that happened sometimes in articulations more than two objects deep.</p></li>
<li><p>Physics: Fixed Component Reset functionality for: Hinge Joints (all parameters relating to Motor, Spring, Limits), Joints (Enable Collision, Enable Preprocessing, Break Force, Break Torque), Character Joints (Swing Axis, Enable Projection). (<a href="https://issuetracker.unity3d.com/issues/hingejoint-reset-functionality-is-not-working-forspring-motor-and-limit-for-hinge-joint">1157026</a>)</p></li>
<li><p>Physics: Fixed crash while accessing Collider.attachedRigidbody property if ArticulationBody component is attached instead of Rigidbody.</p></li>
<li><p>Physics: Fixed various crashes related to activation/deactivation of ArticulationBody components attached to game objects, like changing game object parent, enabling/disabling of game objects, enabling/disabling/removal of ArticulationBody components, removal of game objects with ArticulationBody attached.</p></li>
<li><p>Physics: Updated the profiler entry name for Physics.CheckSphere. (<a href="https://issuetracker.unity3d.com/issues/profiler-marker-is-named-as-test-dot-dot-dot-and-not-check-dot-dot-dot">1215381</a>)</p></li>
<li><p>Player: Changed AsyncReadManagerMetricsFilters to be passed by reference in relevant methods. (1242611)</p></li>
<li><p>Player: Explicitly stopping games after test runs to ensure clean test environment.</p></li>
<li><p>Player: Fixed issue where output from Stadia commands were not printing stderr.</p></li>
<li><p>Player: Re-enabled OnAudioConfigChanged and AudioRenderTest tests on the Stadia Platform.</p></li>
<li><p>Player: Updated automation player to use most recent stadia sdk.</p></li>
<li><p>Plugins: Fixed an issue where the XboxOne native extension dll to fail gracefully if required dll's are not found.</p></li>
<li><p>Prefabs: "Find References In Scene" did not work with nested prefabs. (1213528)</p></li>
<li><p>Prefabs: An issue is fixed where changes to hidden components like ParticleSystemRenderer and VFXRenderer were not handled correctly in all cases when applying or reverting component modifications, added component overrides, or removed component overrides on Prefab instances. (<a href="https://issuetracker.unity3d.com/issues/vfx-improved-prefab-changes-do-not-apply-to-the-prefab-if-saving-it-from-modified-component-from-the-burger-button">1263007</a>)</p></li>
<li><p>Prefabs: Fixed a  crash when loading a scene with a legacy disconnected prefab. (<a href="https://issuetracker.unity3d.com/issues/attempt-to-open-a-specific-scene-crahes-editor">1270456</a>)</p></li>
<li><p>Prefabs: Fixed a test instability. (1101428)</p></li>
<li><p>Prefabs: Fixed an editor crash caused by adding objects on prefab instance in combination with required components. (<a href="https://issuetracker.unity3d.com/issues/crash-on-iscomponentsubclassofmonoclass-when-reimporting-a-prefab">1226180</a>)</p></li>
<li><p>Prefabs: Fixed an exception that was thrown on Reimporting a Project in which the Tile Palette window was docked and New Palette was created. (<a href="https://issuetracker.unity3d.com/issues/2d-exception-is-thrown-on-reimporting-the-project-in-which-the-tile-palette-window-was-docked-and-new-palette-was-created">1275071</a>)</p></li>
<li><p>Prefabs: Fixed an issue when opening Prefab from the prompt displayed when deleting 2nd level nested Prefab shows double rendering in Prefab Mode. (<a href="https://issuetracker.unity3d.com/issues/opening-prefab-from-the-prompt-displayed-when-deleting-2nd-level-nested-prefab-shows-double-rendering-in-prefab-mode">1277627</a>)</p></li>
<li><p>Prefabs: Fixed an issue where a parent prefab might fail to correctly override changes to its nested children. (<a href="https://issuetracker.unity3d.com/issues/parent-prefab-fails-to-correctly-override-changes-to-its-children-prefabs-when-trying-to-override-the-parent-in-the-scene-view">1195496</a>)</p></li>
<li><p>Prefabs: Fixed Applying component or property takes current Animation Mode Preview or Recording values. (<a href="https://issuetracker.unity3d.com/issues/applying-component-or-property-takes-current-animation-mode-preview-or-recording-values">1077718</a>)</p></li>
<li><p>Prefabs: Fixed baked Occlusion Culling data affects Prefab Mode. (<a href="https://issuetracker.unity3d.com/issues/prefab-mode-gets-affected-by-the-scenes-baked-occlusion-culling-data">1136698</a>)</p></li>
<li><p>Prefabs: Fixed Crash when calling PrefabUtility.SaveAsPrefabAsset with absolute path outside of project's Assets folder. (<a href="https://issuetracker.unity3d.com/issues/crash-in-persistentmanager-writefile-when-calling-prefabutility-dot-saveasprefabasset-with-a-path-that-is-outside-of-projects-root">1210526</a>)</p></li>
<li><p>Prefabs: Fixed Inspector window flickers when Tag or Layer of a Prefab Asset is changed. (<a href="https://issuetracker.unity3d.com/issues/imgui-inspector-window-flickers-when-tag-or-layer-of-a-prefab-is-changed">1240896</a>)</p></li>
<li><p>Prefabs: Fixed Overrides dropdown comparison view remaining open if last override has been applied or reverted via context menu. (1071433)</p></li>
<li><p>Prefabs: Fixed placement of Prefab override margin lines for controls that are inside GUI clipping groups. (<a href="https://issuetracker.unity3d.com/issues/improved-prefab-override-indicator-blue-line-is-misaligned-for-size-field-of-line-renderer">1197808</a>)</p></li>
<li><p>Prefabs: Fixed PrefabUtility.SaveAsPrefabAsset() freezes the editor when called from OnValidate() method. (<a href="https://issuetracker.unity3d.com/issues/prefabutility-dot-saveasprefabasset-freezes-the-editor-when-called-from-onvalidate-method">1127313</a>)</p></li>
<li><p>Prefabs: Fixed preview material getting permanently set when dragging over Prefab instance with missing Asset. (<a href="https://issuetracker.unity3d.com/issues/material-gets-applied-to-a-broken-prefab-instance-when-dragging-it-over-the-broken-prefab-instance-in-the-scene-view">1124308</a>)</p></li>
<li><p>Prefabs: Fixed removing MonoBehaviours with missing scripts on prefab assets.</p></li>
<li><p>Prefabs: Fixed SerializableObject.GetIterator() throws ArgumentNullException when UnpackPrefabInstance() is called on an instantiated Prefab in Inspector logic. (<a href="https://issuetracker.unity3d.com/issues/serializableobject-dot-getiterator-throws-argumentnullexception-when-unpackprefabinstance-is-called-on-an-instantiated-prefab">1164099</a>)</p></li>
<li><p>Prefabs: Fixed suppressed components on Prefab instances incorrectly appearing as if they're removed components. For example if a Prefab instance has an added Rigidbody component and a Rigidbody is later added to the Prefab Asset as well, the one from the Asset will be suppressed (not be created) on the instance so avoid there being two Rigidbodies on the same GameObject. The suppressed one would previously appear as if it was a removed component override, even though it wasn't. (<a href="https://issuetracker.unity3d.com/issues/adding-multiple-single-type-components-to-the-prefab-prevents-reverting-a-removed-component-of-the-same-type-1">1240146</a>)</p></li>
<li><p>Prefabs: Fixed that the Inspector preview window displays all LODs on a prefab simultaneously, stacked on top of one another. (<a href="https://issuetracker.unity3d.com/issues/the-inspector-preview-window-displays-all-lods-on-a-prefab-simultaneously-stacked-on-top-of-one-another">1089143</a>)</p></li>
<li><p>Prefabs: If the user destroys the root game object of a prefab, Unity editor would crash. Now an error message is printed instead. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-in-getprefabhandle-when-deselecting-a-prefab-without-a-prefab-contents-root">1218129</a>)</p></li>
<li><p>Prefabs: Overrides Window: Fix overrides in nested instances are collapsed when one override is applied. (<a href="https://issuetracker.unity3d.com/issues/overridies-in-nested-instances-are-collapsed-when-one-override-is-applied">1112995</a>)</p></li>
<li><p>Profiler: Fixed a crash on load of corrupted profiler data captures. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-memorystats-deserialize-when-loading-specific-raw-profiler-file">1119369</a>)</p></li>
<li><p>Profiler: Fixed an issue that caused Profiler Counters of type TimeNanoseconds or FrequencyHz to be displayed as counts. (1278281)</p></li>
<li><p>Profiler: Fixed an issue where a recursive call in ProfilerUnsafeUtility.CreateMarker caused il2cpp builds to fail.</p></li>
<li><p>Profiler: Fixed an issue where Audio and Video memory stats were incorrectly reporting values which belong to other shared allocators.</p></li>
<li><p>Profiler: Fixed an issue where CPU Recorder sampleBlockCount was unstable depending of thread scheduling. (1201319)</p></li>
<li><p>Profiler: Fixed an issue where Profiler Timeline view displayed overlapping samples if their start time was in sub microseconds range. (1274134)</p></li>
<li><p>Profiler: Fixed an issue where Profiler UI Details module was not showing outdated markers. (<a href="https://issuetracker.unity3d.com/issues/profiler-ui-details-data-is-being-carried-over-when-loading-data-in-different-data">1240928</a>)</p></li>
<li><p>Profiler: Fixed an issue where Profiler was showing metadata for sliced samples only in the first frame. (1133819)</p></li>
<li><p>Profiler: Fixed an issue where Profiler.enabled getter and Profiler.EmitFrameMetaData were not thread safe. (1276709)</p></li>
<li><p>Profiler: Fixed an issue where the System Used Memory was reporting useless system memory and not app memory usage. (<a href="https://issuetracker.unity3d.com/issues/total-system-memory-usage-in-the-profiler-is-very-different-with-different-devices-with-the-same-build">1267773</a>)</p></li>
<li><p>Profiler: Fixed an issue where there were duplicate AsyncReadManager.ReadFile markers. (1258822)</p></li>
<li><p>Profiler: Fixed an issuw where warnings in package that were causing users with warnings as errors enabled to fail. (<a href="https://issuetracker.unity3d.com/issues/profile-analyzer-generates-compiler-warnings-on-2018-dot-4">1266375</a>)</p></li>
<li><p>Profiler: Fixed gc allocation in unsafe version of Profiler.EmitFrameMetaData. (1281405)</p></li>
<li><p>Profiler: Fixed GC Allocations not displaying values less than 1024 bytes in Memory chart of ProfilerWindow.</p></li>
<li><p>Profiler: Module Editor - Fixed an issue where restore defaults when the Module Editor is open would not refresh the UI with the latest list of modules. (1256874)</p></li>
<li><p>Profiler: Profile Analyzer (com.unity.performance.profile-analyzer) updated to version 1.0.2, fixing a bug where 2 versions of the profiler could appear. (<a href="https://issuetracker.unity3d.com/issues/profiler-duplicate-profilers-appearing-after-starting-slash-stopping-editor-playback">1244366</a>, 1250860, <a href="https://issuetracker.unity3d.com/issues/profile-analyzer-pull-data-button-is-inactive-when-profiler-recording-is-enabled">1257547</a>)</p></li>
<li><p>SceneManager: Fixed an issue where the editor would freezes for couple of seconds when using SceneManager.LoadSceneAsync while the Hierarchy was open. (<a href="https://issuetracker.unity3d.com/issues/editor-freezes-for-couple-of-seconds-when-using-loadsceneasync">1093359</a>)</p></li>
<li><p>Scripting: - Fix Burst SharedStatic&lt;T&gt; to be initialized to zero after a domain reload.</p></li>
<li><p>Scripting: Added dll verification to loading routine to prevent the editor from loading corrupt dlls. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-when-opening-the-project">1231038</a>)</p></li>
<li><p>Scripting: Added missing tooltips for some scripting related settings in the Build Player Window. (<a href="https://issuetracker.unity3d.com/issues/editor-tooltips-are-not-available-for-script-debugging-and-crete-visual-studio-solution-in-build-setting-window">1264507</a>)</p></li>
<li><p>Scripting: Allow duplicate enum members to refer to same underlying value as long as one is non-obsolete. (<a href="https://issuetracker.unity3d.com/issues/not-a-valid-textureformat-error-is-thrown-when-creating-astc-format-texture-arrays">1218124</a>)</p></li>
<li><p>Scripting: Ensure Roslyn server (VBCSCompiler.exe) is terminated when Editor is closed to prevent locked files. (1183240)</p></li>
<li><p>Scripting: Fixed a modifying Assembly Definitions results issue in recompile all.  Adding/Removing/Moving  still results in a recompile all. (<a href="https://issuetracker.unity3d.com/issues/asmdef-compilationpipeline-reimporting-asmdef-file-without-changes-does-not-respect-compilation-dependencies">1268925</a>)</p></li>
<li><p>Scripting: Fixed a player build and Disabled Domain Reload issue where the next enter playmode would trigger a domain reload. (<a href="https://issuetracker.unity3d.com/issues/a2-unexpected-assembly-reload-after-building-standalone-player-with-playmode-settings-set-to-not-reload-assemblies">1241086</a>)</p></li>
<li><p>Scripting: Fixed an Infinite project load when PrecompiledAssemblyException was encountered with clean project. (<a href="https://issuetracker.unity3d.com/issues/infinite-project-load-when-precompiledassemblyexception-is-encountered-with-clean-project">1277885</a>)</p></li>
<li><p>Scripting: Fixed an issue wher GarbaageCollector.Collectincremental was not always triggering a new incremental collection.</p></li>
<li><p>Scripting: Fixed an issue where ObjectChangeEventStream was no contained in a SceneChangeEvent when a scene was reloaded. (1278201)</p></li>
<li><p>Scripting: Fixed an issue where project files were generated incorrectly with Safe Mode in regards to Precompiled assembly references. (1288026)</p></li>
<li><p>Scripting: Fixed an issue where scripts containing attributes with explicit namespaces were not correctly imported. (1243839)</p></li>
<li><p>Scripting: Fixed an issue where scripts containing preprocessing directive in the last line were not correctly imported. (<a href="https://issuetracker.unity3d.com/issues/pragma-warning-restore-causes-scriptable-object-to-not-be-valid-and-unable-to-compile-when-new-line-after-is-not-present">1261028</a>)</p></li>
<li><p>Scripting: Fixed an issue where setting the parent of the child of a disabled game object to null moved the child to the active scene if it was not already there. (<a href="https://issuetracker.unity3d.com/issues/child-gameobject-is-moved-to-an-active-scene-when-the-child-gameobjects-parent-is-set-to-null">1275898</a>)</p></li>
<li><p>Scripting: Fixed an issue where WebCamTexture.updateCount was not automatically incrementing when streaming video. (<a href="https://issuetracker.unity3d.com/issues/scripting-webcamtexture-dot-updatecount-is-not-updating">1247198</a>)</p></li>
<li><p>Scripting: Fixed an issue where X509Chain.ChainStatus would throw a NotImplementedException.</p></li>
<li><p>Scripting: Fixed an issue with dynamic methods not being cleaned up on domain reload which would lead to corrupted data that would then cause this crash. (<a href="https://issuetracker.unity3d.com/issues/random-editor-crashes-on-mono-metadata-class-equal-when-entering-play-mode">1273662</a>)</p></li>
<li><p>Scripting: Fixed Assembly Overrides in connection to Safe Mode and script compilation. (1278580)</p></li>
<li><p>Scripting: Fixed crash when large amount of dynamic code is generated, potentially for XML serialization. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-on-gc-grow-table-when-trying-to-deserialize-an-xml-file">1191533</a>)</p></li>
<li><p>Scripting: Fixed Debug.Log* printing Debug.Filename.h after the stacktrace in IL2CPP/Mono with no PDB. (<a href="https://issuetracker.unity3d.com/issues/debug-dot-log-outputs-unnecesarry-lines-in-editor-log">1099724</a>)</p></li>
<li><p>Scripting: Fixed job reflection data creation could sometimes crash the editor.</p></li>
<li><p>Scripting: Fixed many UnityEngine.Random documentation issues. Aaddressed feedback from public comments, documented performance and detailed behavior of properties and methods, and improved code sample quality.</p></li>
<li><p>Scripting: Fixed possible crash caused by race condition during startup when the script debugger and profiler systems are enabled.</p></li>
<li><p>Scripting: Fixed several hangs and crashes in the Mono debugger when generating the callstack for the user interface.</p></li>
<li><p>Scripting: Fixed VT cache not being editable after enabling the Virtual Texture in Player Settings in OSX. (<a href="https://issuetracker.unity3d.com/issues/virtual-texturing-hdrp-vt-cache-settings-cannot-be-edited-in-hdrp-asset">1274526</a>)</p></li>
<li><p>Scripting: Improved error messages for errors in generated code coming from the jobs debugger and safety system.</p></li>
<li><p>Scripting: NativeArray.ReadOnly indexer now correctly validates its index.</p></li>
<li><p>Scripting: NativeArrayUnsafeUtility.ConvertExistingDataToNativeArray documentation now correctly states the its length parameter is in number of elements, not bytes.</p></li>
<li><p>Scripting: Unable to delete NewAssembly from Assembly Definition References list in Test Import Setting. (<a href="https://issuetracker.unity3d.com/issues/testrunner-unable-to-delete-newassembly-from-assembly-definition-references-list-in-test-import-setting">1217184</a>)</p></li>
<li><p>Scripting Upgrade: Fixed an issue where compiler error verification check would prolong compilation by 10-20 minutes when handling multiple errors. (<a href="https://issuetracker.unity3d.com/issues/compiler-error-verification-check-prolongs-compilation-by-10-20-minutes-when-handling-multiple-errors">1238888</a>)</p></li>
<li><p>Scripting Upgrade: Fixed an issue which might have prevented ApiUpdater from running when C# syntax (&gt;= 5.0) was used. (1046329)</p></li>
<li><p>Security: Fixed a security vulnerability. (CVE-2017-12939).</p></li>
<li><p>Security: Fixed a security vulnerability. (CVE-2019-9197).</p></li>
<li><p>Serialization: Fixed an issue where assigning a null managed reference and to an object did not apply. (1256341)</p></li>
<li><p>Serialization: Fixed an issue where instance deserialization was stopped when there was an exception during the managed ref deserialization process and still had a valid instance created. (1256991)</p></li>
<li><p>Serialization: Make sure that managed instances stored in array are not reinflated or reset to null when applying through a SerializedProperty. (1254060)</p></li>
<li><p>Serialization: Make sure to support resolution loops and empty messages in System.Obsolete for the API upgrading path. (<a href="https://issuetracker.unity3d.com/issues/editor-freezes-and-silently-crashes-when-an-object-with-serializereference-is-assigned-an-object-with-system-dot-obsolete-attribute">1222795</a>)</p></li>
<li><p>Services: Display of newer version of In-App Purchasing Package now correctly displays newest pre-migration version (prior to 3.X) if still on version 2.X or older. Verstion installed when selecting Update and Migrate also now function as intended.</p></li>
<li><p>Services: Fixed the parameter supplied to the request to enable analytics.</p></li>
<li><p>Shaders: Added precise keyword support on generated GLSL. (1227113)</p></li>
<li><p>Shaders: Fixed a build missing vertex data issue where on certain circumstances when "Optimize Mesh Data" is selected and Editor graphics API differs from the target platform API. (1275368)</p></li>
<li><p>Shaders: Fixed an issue to use the error shader when a variant failed to compile, thus not rendering anything. (<a href="https://issuetracker.unity3d.com/issues/shaders-livelink-when-a-variant-has-an-error-nothing-is-rendered-in-the-player">1253968</a>)</p></li>
<li><p>Shaders: Fixed an issue where shader compiler emited code for precise keyword when the target GLSL version was not support it. (<a href="https://issuetracker.unity3d.com/issues/bug-hlslcc-bad-codegen-on-gles2-slash-3-when-using-precise-keyword">1274141</a>)</p></li>
<li><p>Shaders: Fixed an issue where the keyword popup window would not have a proper minimum size. (<a href="https://issuetracker.unity3d.com/issues/shader-graph-directional-arrow-buttons-are-overlapping-on-scrollbar-handle-in-the-keyword-section-of-custome-fullscreen-pass">1254010</a>)</p></li>
<li><p>Shaders: Fixed an issue where the Loading shader wasn't used in the player while waiting for a variant to compiled. (<a href="https://issuetracker.unity3d.com/issues/shader-livelink-shader-livelink-uses-the-error-shader-while-the-variant-is-being-compiled-instead-of-loading-shader">1254843</a>)</p></li>
<li><p>Shaders: Fixed an issue where the RenderTexture was not created when ComputeShader.Dispatch is called when setting texture parameter to a compute shade. (<a href="https://issuetracker.unity3d.com/issues/rendertexture-is-not-automatically-created-when-used-as-a-compute-shader-output-calling-computeshader-dot-dispatch">1261303</a>)</p></li>
<li><p>Shaders: Fixed an issue which would causes shader requirements not to be serialised correctly.</p></li>
<li><p>Shaders: Fixed rendering on DX when using "Use full Sampler precision by default" option in the player settings. (<a href="https://issuetracker.unity3d.com/issues/shader-editor-gets-blank-on-selecting-use-full-sampler-precision-by-default-option-in-shader-precision-model">1293568</a>)</p></li>
<li><p>Shaders: Fixed static analysis issues ShaderCompiler Preprocessr code. (1217178)</p></li>
<li><p>Terrain: Added NavMesh Lod index in TreePrototype. The index is used to select LOD Level in LODGroup for NavMesh generation. (1193073)</p></li>
<li><p>Terrain: Export raw terrain now shows up immediately in Project Folder view. (<a href="https://issuetracker.unity3d.com/issues/terrain-exporting-raw-of-terrain-in-project-browser-doesnt-show-up-until-unity-is-refocused">1178342</a>)</p></li>
<li><p>Terrain: Fixed a memory OOB crash when painting detail objects on patches containing holes. (1293366)</p></li>
<li><p>Terrain: Fixed a null exception thrown from the Paint Texture terrain tool. (<a href="https://issuetracker.unity3d.com/issues/terrain-nullreference-exception-thrown-on-assigning-terrain-data-asset-to-the-terrain-component-when-paint-texture-is-selected">1268578</a>)</p></li>
<li><p>Terrain: Fixed an assertion error that occured when painting speed trees in prefab editor when the light is being baked. (<a href="https://issuetracker.unity3d.com/issues/terriain-assertion-failed-errors-occur-when-painting-speed-trees-in-prefab-editor-when-the-light-is-being-baked">1081131</a>)</p></li>
<li><p>Terrain: Fixed an issue where painted terrain details were not culled precisely against hole edges. (1270061)</p></li>
<li><p>Terrain: Fixed an issue where there was no warning message showing up on UI if a user uses LOD Group component on the detail prototype prefab. (<a href="https://issuetracker.unity3d.com/issues/detail-mesh-is-not-painted-on-the-terrain-when-the-object-is-using-lod-group">1209026</a>)</p></li>
<li><p>Terrain: Fixed baked shadow masks for terrain with more than 4 materials. (1148970)</p></li>
<li><p>Terrain: Fixed preview when multiple TerrainLayers are selected. (<a href="https://issuetracker.unity3d.com/issues/preview-window-in-the-inspector-shows-the-same-preview-image-when-multiple-terrain-layers-are-selected">1148952</a>)</p></li>
<li><p>Terrain: Fixed Terrain Brush list to update when brushes are modified, and adding tooltips to the Brush properties. (<a href="https://issuetracker.unity3d.com/issues/resetting-a-custom-brush-resets-the-falloff-curve-to-nothing">1170563</a>, <a href="https://issuetracker.unity3d.com/issues/custom-brush-settings-have-no-tooltips">1170565</a>, <a href="https://issuetracker.unity3d.com/issues/custom-brush-list-preview-in-terrain-paint-menu-doesnt-update-when-custom-brush-settings-are-changed">1170567</a>)</p></li>
<li><p>Terrain: Fixed Terrain to properly switch from base map to splat map rendering when splats are in a dirty modified state. (1178928)</p></li>
<li><p>Terrain: Fixed undo tracking for Terrain to be correctly record multiple different Paint operations in the same Undo operation, and properly Undo adding Terrain Layers. (1138273)</p></li>
<li><p>Terrain: Increased the Undo buffer size to better handle Terrain modifications. (1067258)</p></li>
<li><p>TextCore: - Updated FontEngine to improve performance as well as reduce memory allocations.<br></p> 
<ul>
<li>Fixed Font Asset Creation process not using Multi-Threading in the Editor when using SDF8, SDF16 and SDF32 modes.<br></li>
<li>Fixed memory allocation issue when retrieving glyph adjustment pairs.<br></li>
<li>Fixed PairAdjustmentRecords returning a value of infinity with certain font files.<br></li>
<li>Fixed incorrect PairAdjustmentValues when using SDF8, SDF16 and SDF32 modes.<br></li>
<li>SDF, SDF8, SDF16 and SDF32 modes no longer use hinting to improve glyph sampling at low point size.</li>
</ul></li>
<li><p>TextCore: Added Multi-Threading to Font Asset Creation process in the Editor.</p></li>
<li><p>Timeline: Fixed an issue where changes in the PlayableDirector Inspector would not allow the user to view and delete unused bindings. (<a href="https://issuetracker.unity3d.com/issues/invalid-scenebindings-of-playabledirector-do-not-get-cleaned-up">1234687</a>)</p></li>
<li><p>Timeline: Fixed warning in Timeline caused by assigning bindings in prefab editor. (<a href="https://issuetracker.unity3d.com/issues/prefab-asset-with-a-playable-director-throws-a-unnecessary-warning-when-using-an-instance-of-a-prefab-for-timeline-track-output">1235781</a>)</p></li>
<li><p>UI: Added ability to use Ctrl + Insert to copy text and shift + instert to paste text. (<a href="https://issuetracker.unity3d.com/issues/ctrl-plus-insert-copy-and-shift-plus-insert-paste-shortcuts-do-not-work-with-the-ui-input-field-component">1226349</a>)</p></li>
<li><p>UI: Added dirty call when setting pixelsPerUnitMultiplier so the verts are rebuilt. (<a href="https://issuetracker.unity3d.com/issues/changes-made-to-images-pixelsperunitmultiplier-property-are-not-applied-when-changing-it-in-script-during-runtime">1245967</a>)</p></li>
<li><p>UI: Fixed a memory error message. (<a href="https://issuetracker.unity3d.com/issues/ugui-causes-internal-jobtempalloc-has-allocations-that-are-more-than-4-frames-old-this-is-not-allowed-and-likely-a-leak">1275239</a>)</p></li>
<li><p>UI: Fixed an issue where AspectRatio was not able to be set when the mode was none in the editor. (<a href="https://issuetracker.unity3d.com/issues/imgui-unable-to-change-the-aspect-ratio-value-under-aspect-ratio-fitter-component-in-the-inspector">1264569</a>)</p></li>
<li><p>UI: Fixed an issue where new windows always loaded on the first connected monitor instead of the current monitor that the main window is in. (<a href="https://issuetracker.unity3d.com/issues/new-editor-windows-have-wrong-position-when-working-with-several-monitors">1148729</a>)</p></li>
<li><p>UI: Fixed an issue where scene needs to be saved twice when creating an instance of a Prefab having a Layout Group component and a child UI GameObject. (<a href="https://issuetracker.unity3d.com/issues/scene-needs-to-be-saved-twice-when-creating-an-instance-of-a-prefab-having-a-layout-group-component-and-a-child-ui-gameobject">1195283</a>)</p></li>
<li><p>UI: Fixed an issue where the update button onclick link would point to an inproper proper file.</p></li>
<li><p>UI: Fixed issue where GetModifiedMaterial would get root canvas even if not maskable causing performance spikes.</p></li>
<li><p>UI: Fixed issue where if a dropdown was part of a nested overrideSorting canvas it would grab the very root canvas which could have the wrong sorting layer data.</p></li>
<li><p>UI: Fixed issue where Text Mesh color was not reset properly upon calling "Reset". (<a href="https://issuetracker.unity3d.com/issues/imgui-color-property-from-text-mesh-component-is-not-resetting-on-selecting-reset">1223055</a>)</p></li>
<li><p>UI: Fixed issue where UIZTestMode was not initially set which could cause first frame render issues or issues if the GameView wasn't visible. (<a href="https://issuetracker.unity3d.com/issues/canvas-is-rendered-on-top-of-other-gameobjects-in-every-viewing-angle-in-the-scene-view-when-render-mode-is-set-to-world-space">1235078</a>)</p></li>
<li><p>UI: Fixed issue with indexedSet array access.</p></li>
<li><p>UI: Fixed issue with Selectable OnDrag not resetting to proper position as it used localPosition instead of anchoredPosition.</p></li>
<li><p>UI: Updated uGUI package documentation to include EventSystem.</p></li>
<li><p>UI Elements: Enabled MSAA on inspector windows to provide antialiased UIElements content. (1215973)</p></li>
<li><p>UI Elements: Fixed an isue where the slider value stayed unaffected when trying to change it using arrow keys. (<a href="https://issuetracker.unity3d.com/issues/uielements-slider-value-stays-unaffected-when-trying-to-change-it-using-arrow-keys">1244539</a>)</p></li>
<li><p>UI Elements: Fixed Editor memory leak on EditorWindow docking/undocking.</p></li>
<li><p>UI Elements: Fixed event currentTarget being null when event is sent only to target.</p></li>
<li><p>UI Elements: Fixed issue with right-click passing through the inspector preview if it's drawn over other inspector components. (<a href="https://issuetracker.unity3d.com/issues/imgui-right-click-carries-through-the-model-preview-window-and-interacts-with-the-inspector-window-when-docked">1226328</a>)</p></li>
<li><p>UI Elements: Fixed padding that caused truncated text in UIElements debugger search bar. (<a href="https://issuetracker.unity3d.com/issues/imgui-while-searching-type-name-or-class-text-letters-are-overlapped-or-clipped-in-the-search-bar">1233009</a>)</p></li>
<li><p>UI Elements: Fixed radial gradients on metal. (1225848)</p></li>
<li><p>UI Elements: Fixed right-click on titlebar outside of open or failed-to-load tabs not supposed to show context window. (<a href="https://issuetracker.unity3d.com/issues/ui-elements-the-entire-title-bar-of-a-window-is-interactable-and-its-close-tab-functionality-does-not-work">1228991</a>)</p></li>
<li><p>UI Elements: Fixed the SubUpdatesDoesntBreakNextElements test to work on OpenGL and Vulkan on Windows. (1222743)</p></li>
<li><p>UI Elements: Item height is now excluded from the ListView view data. (<a href="https://issuetracker.unity3d.com/issues/uielements-the-value-of-the-property-listview-dot-itemheight-cannot-be-changed-from-script-when-listview-dot-viewdatakey-is-set">1225888</a>)</p></li>
<li><p>UI Elements: Limiting the relative mouse position to account for the max size as well.<br> Added automated tests for the Visual Splitter.
(<a href="https://issuetracker.unity3d.com/issues/setting-max-width-on-left-column-content-of-uielements-visualsplitter-breaks-resizing">1215097</a>)</p></li>
<li><p>UI Elements: Limiting the relative position of the splitter to always be between 0f and 0.999f.<br> Added automated test to make sure the bug can never be reproduced.
(1227342)</p></li>
<li><p>UI Elements: Now the UIElements Debugger no longer sends a ChangeEvent when updating the VisualElement's Text field. (1185718)</p></li>
<li><p>UI Elements: Optimized StyleVariablesContext hash computation.</p></li>
<li><p>UI Elements: Setting twice a TextValueField (without notify) would sometimes skip display updates and result in displaying the wrong values (the field's value itself is ok, but not the text that represents the value). (1202400)</p></li>
<li><p>UI Elements: The Scrollbar is one item behind when using ScrollToItem method. (<a href="https://issuetracker.unity3d.com/issues/uielements-selected-item-in-resized-listview-uielement-with-scrollbar-is-not-shown-when-using-down-arrow-key-to-navigate">1219416</a>)</p></li>
<li><p>UI Toolkit: Changed the blending equation to allow blending of the resulting RenderTexture.</p></li>
<li><p>UI Toolkit: Fixed a wrong order of Attach/Detach events issue. (1269758)</p></li>
<li><p>UI Toolkit: Fixed an exception that was thrown when the Sprite Editor window was opened after transiting to play mode. (<a href="https://issuetracker.unity3d.com/issues/2d-exception-thrown-on-applying-changes-of-sprite-import-settings-in-play-mode-with-sprite-editor-window-is-opened">1249369</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue where .isPasswordField was not updating. (<a href="https://issuetracker.unity3d.com/issues/changes-to-textinputbasefield-dot-ispasswordfield-only-apply-when-textfield-is-focused-slash-hovered">1251000</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue where changing the cursor logged a warning. (1183813)</p></li>
<li><p>UI Toolkit: Fixed an issue where click events behaved inconsistent in Scene View. (1210649)</p></li>
<li><p>UI Toolkit: Fixed an issue where declaring an AssetImporterEditor extension with showImportedObject set to false would make its inspector repaint over and over again. (<a href="https://issuetracker.unity3d.com/issues/custom-inspector-window-continually-refreshes-when-assetimportereditor-dot-showimportedobject-is-set-to-false">1264833</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue where hover selector was not working during DragEvents. (1180282)</p></li>
<li><p>UI Toolkit: Fixed an issue where IMGUI container did not capture events when atop of the Scene window. (1220685)</p></li>
<li><p>UI Toolkit: Fixed an issue where PropertyField's label width calculation did not match IMGUI. (1230326)</p></li>
<li><p>UI Toolkit: Fixed an issue where TextField focus was not selecting text. (<a href="https://issuetracker.unity3d.com/issues/shadergraph-text-selection-for-properties-does-not-select-the-whole-text-on-the-first-click">1262318</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue where TextField was ignoring AltGr character combinations. (1238207, <a href="https://issuetracker.unity3d.com/issues/uitoolkit-textfield-doesnt-resigter-altgr-symbol-combinations">1261739</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue where the dropdown menu from toolbar of windows are glued to the left side of the screen on Mac. (1221212)</p></li>
<li><p>UI Toolkit: Fixed an issue where the GraphView edges disappeared when resizing the visual element container height smaller than a certain threshold. (1240884)</p></li>
<li><p>UI Toolkit: Fixed an issue where the TextField text editing cursor did not appear where it was clicked when WhiteSpace was set to Normal in Ed. (<a href="https://issuetracker.unity3d.com/issues/textfield-text-editing-cursor-doesnt-appear-where-it-was-clicked-when-whitespace-is-set-to-normal">1176895</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue where the use of "Random" was affecting the state. (<a href="https://issuetracker.unity3d.com/issues/ui-elements-alters-the-state-of-random">1188214</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue where [Scene Template] "Layout update is struggling" was throwing an error continuously when creating a "Scene Template" in the Project. (<a href="https://issuetracker.unity3d.com/issues/scene-template-layout-update-is-struggling-error-thrown-continuously-on-creating-scene-template-in-the-project-window">1275253</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue whwewre UXML preview rendered outside the preview zone. (<a href="https://issuetracker.unity3d.com/issues/ui-elements-preview-of-a-uxml-file-in-inspector-is-rendered-with-glitches-and-overflows-out-of-the-preview-window">1227277</a>)</p></li>
<li><p>UI Toolkit: Fixed an issue with ScrollView / ScrollTo. (1205850)</p></li>
<li><p>UI Toolkit: Fixed an issuw where ListView mouse events weren't replaced with pointer events. (<a href="https://issuetracker.unity3d.com/issues/listview-element-selection-does-not-change-when-clicking-on-a-textfield-slash-checkbox-element">1231301</a>)</p></li>
<li><p>UI Toolkit: Fixed MissingMethodException issue with Shortcut Manager window when UI Toolkit package is installed. (<a href="https://issuetracker.unity3d.com/issues/shortcut-windows-throws-errors-when-ui-toolkit-is-in-use">1276678</a>)</p></li>
<li><p>UI Toolkit: Fixed WebGL rendering glitches caused by sub-range buffer updates.</p></li>
<li><p>UI Toolkit: Removed cyclic dependency with Input System package. (<a href="https://issuetracker.unity3d.com/issues/assembly-with-cyclic-references-detected-errors-occur-when-input-system-and-ui-toolkit-packages-are-imported">1262723</a>)</p></li>
<li><p>UI Toolkit: Renamed "Update UIElements Schema" menu item to "Update UXML Schema".</p></li>
<li><p>UI Toolkit: Reverting a Toggle's text to null won't throw an exception. (1238606)</p></li>
<li><p>UI Toolkit: Slider's text field displayed value is not properly updated when value is set through code. (1263147)</p></li>
<li><p>UI Toolkit: The text value of TextValue based fields is now updated as soon as new formatString rule is set. (<a href="https://issuetracker.unity3d.com/issues/uielements-floatfield-dot-formatstring-is-not-applied-to-initial-field-values">1244514</a>)</p></li>
<li><p>UI Toolkit: Unhandled CommandEvents are now propagated to the EditorWindow's OnGUI(). (<a href="https://issuetracker.unity3d.com/issues/uielements-object-selector-stops-working-after-textfield-edit">1231271</a>)</p></li>
<li><p>Universal Windows Platform: Expose EnableFrameTimings in Player Settings for Universal Windows Platform. (1163531)</p></li>
<li><p>Universal Windows Platform: Fixed a Player crash when calling WebcamTexture.devices during Update. (1251067)</p></li>
<li><p>Universal Windows Platform: Fixed an incorrect error generated by Reference Rewriter tool for certain array types. (<a href="https://issuetracker.unity3d.com/issues/windows-dot-perception-dot-spatial-dot-spatialstageframeofreference-rewriter-error-when-building-to-uwp">1254820</a>)</p></li>
<li><p>Universal Windows Platform: Fixed an issue in D3D12 where disabling VSync didn't allow running at unlocked frame rate. (<a href="https://issuetracker.unity3d.com/issues/disabling-vsync-doesnt-work-on-uwp-when-using-d3d12">1289170</a>)</p></li>
<li><p>Universal Windows Platform: Fixed an issue where file types [array] preset were incompatibility in Player Settings (UWP). (1267108)</p></li>
<li><p>Universal Windows Platform: Fixed Preset incompatibilities in Player Settings (UWP). (1232071, 1232087)</p></li>
<li><p>Version Control: Fixed not being able to set VCS mode when running editor session with -vcsModeSession argument.</p></li>
<li><p>Version Control: Provider.CheckoutIsValid correctly returns false for exclusively locked files by remote user.</p></li>
<li><p>Version Control: Removed the VCS "Lock" and "Unlock" buttons in various menus when the enabled VCS system does not support those operations. (<a href="https://issuetracker.unity3d.com/issues/plastic-scm-trying-to-lock-a-file-through-its-inspector-throws-an-error-and-disconnects-vcs">1174664</a>)</p></li>
<li><p>Video: Added an instability in video playmode tests (VideoPlaybackCanPlayAudio).</p></li>
<li><p>Video: Fixed an issue where a requested custom gfx device callbacks would not occur on the "main" rendering thread. (1255849)</p></li>
<li><p>Video: Fixed VideoPlayerTimeReference playmode test instability.</p></li>
<li><p>Virtual Texturing: Fixed an issue where VT with hybrid v2 renderer gave "A Hybrid Renderer V2 batch is using a pass from the shader, which is not SRP batcher compatible" error. (1252572)</p></li>
<li><p>Web: Fixed rare cases where request would fail when using File download or upload handler.</p></li>
<li><p>WebGL: Added check for Linux to use the correct version of the Brotli compression library. (1241347)</p></li>
<li><p>WebGL: Fixed a crash with Unity web loader on new macOS Big Sur.</p></li>
<li><p>WebGL: Fixed an issue where the video started playback before the mute property was set, which resulted in an error and the video not to play. (<a href="https://issuetracker.unity3d.com/issues/webgl-videoplayer-autoplay-of-muted-video-is-blocked-when-wait-for-first-frame-option-is-disabled-in-the-videoplayer">1241584</a>)</p></li>
<li><p>WebGL: Fixed an issue where Transform.position of an element on a canvas could return incorrect value in Start method in WebGL. (<a href="https://issuetracker.unity3d.com/issues/transform-dot-position-is-different-in-start-and-update-methods-on-webgl-builds-when-canvas-scaler-is-set-to-scale-with-screen-size">1234614</a>)</p></li>
<li><p>WebGL: Fixed an issue with PlaySchedule. (<a href="https://issuetracker.unity3d.com/issues/playschedule-does-not-loop-audio-in-webgl-build">912244</a>)</p></li>
<li><p>WebGL: Fixed issue with gzip compression being broken for CentOS7. (<a href="https://issuetracker.unity3d.com/issues/linux-errors-regarding-unrecognized-option-keep-for-gzip-when-trying-to-build-for-webgl">1168715</a>)</p></li>
<li><p>WebGL: Fixed the issue which prevented usage of ES6 in user jspre plugins in WebGL. (1211536)</p></li>
<li><p>WebGL: Fixed WebAssembly streaming for compressed WebGL builds when naming files as hashes. (<a href="https://issuetracker.unity3d.com/issues/webassembly-streaming-and-multi-threading-not-working-for-builds-compiled-with-name-files-as-hashes-option-enabled">1223772</a>)</p></li>
<li><p>WebGL: Fixed WebGL builds for projects with utf-8 symbols. (<a href="https://issuetracker.unity3d.com/issues/a-project-fails-to-build-for-webgl-if-the-project-name-contains-utf-8-symbols">1179135</a>)</p></li>
<li><p>Windows: Added support for VideoCapture API to Windows Standalone Player and Editor. (<a href="https://issuetracker.unity3d.com/issues/onvideocaptureresourcecreatedcallback-does-not-get-called-when-passing-it-as-a-videocapture-dot-createasync-parameter">1195027</a>)</p></li>
<li><p>Windows: Fixed a built project crash when Screen.SetResolution() method was used with height or width set to 0. (<a href="https://issuetracker.unity3d.com/issues/built-project-crashes-when-screen-dot-setresolution-method-is-used-with-height-or-width-set-to-0">1242757</a>)</p></li>
<li><p>Windows: Fixed a couple of crashes when closing custom modal dialogs. (<a href="https://issuetracker.unity3d.com/issues/closing-a-modal-window-hits-a-debugassert-and-crashes-unity">1235986</a>)</p></li>
<li><p>Windows: Fixed an issue when running player when not monitor is connected to the system. (1228505)</p></li>
<li><p>Windows: Fixed an issue where audio would not pause when the Editor was minimized by clicking the taskbar. (<a href="https://issuetracker.unity3d.com/issues/timeline-audio-is-not-paused-when-unity-is-minimized-through-the-taskbar-in-play-mode">1208758</a>)</p></li>
<li><p>Windows: Fixed an issue where the cursor was not updating in the Player when using NewInput. (<a href="https://issuetracker.unity3d.com/issues/cursor-displays-loading-icon-until-game-window-loses-and-regains-focus-when-building-without-splash-screen">1238158</a>)</p></li>
<li><p>Windows: Fixed an issue where the popover window in Frame debugger would not close when pressing up or down on the keyboard in the tree view.</p></li>
<li><p>Windows: Fixed an UWP certificate generation issue where key container was unusable. (1235410)</p></li>
<li><p>Windows: Fixed issue where the wrong window would sometimes get mouse click events if they were overlapped. (1242368)</p></li>
<li><p>Windows: Fixed Time.deltaTime calculations on D3D11 and D3D12 when running on a secondary monitor that has a refresh rate that is not a divisor of the primary monitor refresh rate (like 60 Hz and 144 Hz). (<a href="https://issuetracker.unity3d.com/issues/time-dot-deltatime-issues-on-secondary-monitor-in-windowed-mode">1285420</a>)</p></li>
<li><p>Windows: Fixed Time.deltaTime calculations on D3D11 and D3D12 when VSync is force disabled from the driver software (like Nvidia Control Panel, Radeon Settings or Intel Graphics Command Center).</p></li>
<li><p>XR: Added missing Vulkan device flush from XRDisplay.</p></li>
<li><p>XR: Disabled watermarks when rendering to VR device with XR SDK.</p></li>
<li><p>XR: Fixed a case where the camera does not respect near/far clipping plane settings.</p></li>
<li><p>XR: Fixed a crash by preventing B10G11R11 texture format usage on Oculus Quest.</p></li>
<li><p>XR: Fixed a crash with MockHMD (multipass) when a terrain was present. (<a href="https://issuetracker.unity3d.com/issues/xr-sdk-mockhmd-editor-crashes-after-switching-rendering-modes-and-entering-play-mode-when-scene-has-terrain-game-object">1228228</a>)</p></li>
<li><p>XR: Fixed a Quest app crash with URP 10 package due to the memory leak. (<a href="https://issuetracker.unity3d.com/issues/xr-quest-crash-with-urp-10-preview-and-opengles">1269108</a>)</p></li>
<li><p>XR: Fixed a Vulkan framebuffer layer count logic issue when using multiview. (1256388)</p></li>
<li><p>XR: Fixed an issue where partial viewport clear on texture arrays on platforms that can't clear non-fullscreen.</p></li>
<li><p>XR: Fixed an issue where XRDevice, XRSettings, and XRStats were not providing valid data with scriptable render pipelines.</p></li>
<li><p>XR: Fixed an issue with Texture2DMSArray shader compilation with OpenGL.</p></li>
<li><p>XR: Fixed an URP XR crash when "Optimized Frame Pacing" was selected. (<a href="https://issuetracker.unity3d.com/issues/xr-quest-urp-universal-rp-xr-apps-built-from-recent-graphics-master-crash-on-quest-upon-launch">1264046</a>)</p></li>
<li><p>XR: Fixed application of MSAA in Vulkan Multiview.</p></li>
<li><p>XR: Fixed automatic upgrading for URP and HDRP projects.</p></li>
<li><p>XR: Fixed MirrorView BlitMode C# out of sync with XR display header.</p></li>
<li><p>XR: Fixed multipass color resolve to right eye in certain circumstances.</p></li>
<li><p>XR: Fixed regression introduced in render pass fix. (<a href="https://issuetracker.unity3d.com/issues/xr-urp-multipass-not-rendering-right-eye">1225548</a>)</p></li>
<li><p>XR: Fixed Sprite Mask not working in URP XR. (<a href="https://issuetracker.unity3d.com/issues/urp-oculus-xr-sdk-right-eye-does-not-display-sprite-masks-correctly-in-instanced-rendering">1195098</a>)</p></li>
<li><p>XR: Fixed zero-initialization for ScriptableCullingParameters.</p></li>
<li><p>XR: Make sure GetInstanceCountMultiplier() is used correctly in DrawNullGeometry() and DrawIndexedNullGeometry() with OpenGL.</p></li>
<li><p>XR: Modified scripts in play mode nolonger causes Subsystems to unload.</p></li>
<li><p>XR: No longer emitting deprecation warnings for subsystem infrastructure. (1238848)</p></li>
<li><p>XR: Set the appropriate Vulkan usage flag for the fragment density map.</p></li>
<li><p>XR: Updated XR Plugin Management for improved user workflow.</p></li>
<li><p>XR: UWP: Fix erroneous assert when running in XR mode: WaitForLastPresentationAndGetTimestamp() was called multiple times in a row... (1287953)</p></li>
</ul>

### Known Issues in 2020.2.0f1
<ul>
<li><p>Asset Import Pipeline: Prefabs are reimporting every time a code change is made (<a href="https://issuetracker.unity3d.com/issues/prefabs-are-reimporting-every-time-a-code-change-is-made">1294785</a>)</p></li>
<li><p>Asset Importers: [Performance Regression] Importing an fbx model is noticeably slower when the model contains Animations (<a href="https://issuetracker.unity3d.com/issues/performance-regression-importing-an-fbx-model-is-noticeably-slower-when-the-model-contains-animations">1265275</a>)</p></li>
<li><p>Audio: [editor][fmod][macOS] Editor is preventing Mac OS from entering sleep mode automatically (<a href="https://issuetracker.unity3d.com/issues/editor-is-preventing-mac-os-from-entering-sleep-mode-automatically">995866</a>)</p></li>
<li><p>Cloth: Skinned Mesh Renderer's Bounds Extent is set to half of the Transform's Scale when using a Cloth Component (<a href="https://issuetracker.unity3d.com/issues/skinned-mesh-renderers-bounds-extent-is-set-to-half-of-the-transforms-scale-when-using-a-cloth-component">1209765</a>)</p></li>
<li><p>Global Illumination: [macOS] BugReporter doesn't get invoked when the project crashes (<a href="https://issuetracker.unity3d.com/issues/macos-bugreporter-doesnt-get-invoked-when-the-project-crashes">1219458</a>)</p></li>
<li><p>Installer: WindowsInstallerSet builder calculates compressed install sizes (<a href="https://issuetracker.unity3d.com/issues/windowsinstallerset-builder-calculates-compressed-install-sizes">1297868</a>)</p></li>
<li><p>Linux:  InputSystem's Mouse delta values do not change when the Cursor lockState is set to Locked (<a href="https://issuetracker.unity3d.com/issues/linux-inputsystems-mouse-delta-values-do-not-change-when-the-cursor-lockstate-is-set-to-locked">1248389</a>)</p></li>
<li><p>Linux: Linux Editor crashes at "gtk_fixed_put" when opening a project (<a href="https://issuetracker.unity3d.com/issues/linux-editor-crashes-at-burst-signal-handler-when-opening-a-project">1288797</a>)</p></li>
<li><p>Linux: Linux Editor tooltip shows up in the window switcher as a separate window (<a href="https://issuetracker.unity3d.com/issues/linux-editor-tooltip-shows-up-in-the-window-switcher-as-a-separate-window">1287440</a>)</p></li>
<li><p>Physics: Editor crashes when Raycasting a Mesh with a lot of triangles located very close to each other or opening the Physics Debugger (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-raycasting-a-mesh-with-a-lot-of-triangles-located-very-close-to-each-other-or-opening-the-physics-debugger">1297721</a>)</p></li>
<li><p>Profiling: Once paused, the Profiler does not resume recording when profiling WebGL player (<a href="https://issuetracker.unity3d.com/issues/once-paused-the-profiler-does-not-resume-recording-when-profiling-webgl-player">1271012</a>)</p></li>
<li><p>Profiling: [Profiler] Hierarchy randomly hides parts of the sample hierarchy if Editor Only Samples are present and set to be Collapsed (<a href="https://issuetracker.unity3d.com/issues/profiler-hierarchy-randomly-hides-parts-of-the-sample-hierarchy-if-editor-only-samples-are-present-and-set-to-be-collapsed">1297955</a>)</p></li>
<li><p>Project Browser: Icon size slider is missing in Project Browser in One Column Layout (<a href="https://issuetracker.unity3d.com/issues/icon-size-slider-is-missing-in-project-browser-in-one-column-layout">1295227</a>)</p></li>
<li><p>Scene Management: Crash on EditorUserSettings::UpdateRecentSceneConfigValues when opening multiple Scenes several times one by one through Script (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-after-opening-multiple-scenes-several-times">1294937</a>)</p></li>
<li><p>Shader System: Freeze or crash with various stack traces when opening a project while connected to a VPN service (<a href="https://issuetracker.unity3d.com/issues/editor-freezes-slash-crashes-when-connected-to-nordvpn">1025558</a>)</p></li>
<li><p>Shader System: [Shaders] 'TLS Allocator' errors and Allocation logs are continuously thrown after cancelling a build in progress (<a href="https://issuetracker.unity3d.com/issues/shaders-tls-allocator-errors-are-thrown-when-cancelling-build-during-compiling-shader-variants-step">1224325</a>)</p></li>
<li><p>Shadows/Lights: Skybox lighting is not rendered after creating gameobjects in the new scene until the lighting is rebaked (<a href="https://issuetracker.unity3d.com/issues/skybox-lighting-is-not-shown-after-creating-new-gameobjects-in-the-new-scene">1250293</a>)</p></li>
<li><p>WebGL: [Linux] WebGL build always fails and throws a FileNotFoundException (<a href="https://issuetracker.unity3d.com/issues/linux-webgl-build-always-fails-and-throws-a-filenotfoundexception">1268262</a>)</p></li>
<li><p>Window Management: Pop-up windows like Color Picker close upon clicking them when they are hovered on immediately after opening (<a href="https://issuetracker.unity3d.com/issues/pop-up-windows-like-color-picker-get-closed-when-clicked-immediately-after-opening-it">1239613</a>)</p></li>
<li><p>XR: [XR SDK][Oculus] EarlyUpdate.XRUpdate spikes inconsistently (<a href="https://issuetracker.unity3d.com/issues/xr-sdk-oculus-earlyupdate-dot-xrupdate-spikes-inconsistently">1262597</a>)</p></li>
</ul>

### New 2020.2.0f1 Entries since 2020.2.0b14
