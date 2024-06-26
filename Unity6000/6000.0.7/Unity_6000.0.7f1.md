# Unity 6000.0.7f1
Thu, 20 Jun 2024 16:04:46 GMT  
https://unity.com/releases/editor/whats-new/6000.0.7

# Known Issues in 6000.0.7f1

- Asset - Database: OnAfterDeserialize is not called when Prefabs are instantiated using InstantiateAsync
    ([UUM-71810](https://issuetracker.unity3d.com/issues/onafterdeserialize-is-not-called-when-prefabs-are-instantiated-using-instantiateasync))

- Editor Platform: Building freezes when building Universal 3D Sample/Cinematic Studio Project
    ([UUM-73997](https://issuetracker.unity3d.com/issues/building-freezes-when-building-universal-3d-sample-slash-cinematic-studio-project))

- Kernel: Profiler does not profile after building the Project with Autoconnect Profiler Option enabled
    ([UUM-71750](https://issuetracker.unity3d.com/issues/profiler-does-not-profile-after-building-the-project-with-autoconnect-profiler-option-enabled))

- Kernel: VirtualFileSystem crash because of data races.
    ([UUM-72557](https://issuetracker.unity3d.com/issues/virtualfilesystem-crash-because-of-data-races))

- Mono: [TypeCache] Crash on RaiseException when opening a specific project
    ([UUM-66498](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-opening-a-specific-project))

- PhysX Integration: A 1000 times heavier GameObject will stutter when colliding with a lighter GameObject
    ([UUM-65366](https://issuetracker.unity3d.com/issues/a-1000-times-heavier-gameobject-will-stutter-when-colliding-with-a-lighter-gameobject))

- PhysX Integration: Jerky initialization of Joints occurs when Configurable Joint Limits are used
    ([UUM-72854](https://issuetracker.unity3d.com/issues/jerky-initialization-of-joints-occurs-when-configurable-joint-limits-are-used))

- Serialization: Crash on TypeTreeQueries::GetFullTypeNameFromReferencedType when an xoJunction GameObject is selected in the Hierarchy Window
    ([UUM-74373](https://issuetracker.unity3d.com/issues/crash-on-typetreequeries-getfulltypenamefromreferencedtype-when-an-xojunction-gameobject-is-selected-in-the-hierarchy-window))

- Texture: [AsyncLoadInEditor] Crash on memcpy when opening a project that loads TSS files
    ([UUM-71323](https://issuetracker.unity3d.com/issues/crash-on-memcpy-when-opening-a-project-that-loads-tss-files))

- UI Toolkit Framework: "TextureImporterInspector.OnInspectorGUI must call ApplyRevertGUI to avoid unexpected behaviour." thrown when selecting Asset then selecting and deselecting Texture 2D
    ([UUM-35998](https://issuetracker.unity3d.com/issues/textureimporterinspector-dot-oninspectorgui-must-call-applyrevertgui-to-avoid-unexpected-behaviour-dot-thrown-when-selecting-asset-then-selecting-and-deselecting-texture-2d))

- UI Toolkit Framework: The "StackOverflowException" error is thrown in the console and the Editor freezes when Spacebar is pressed after selecting the last element of a list
    ([UUM-69616](https://issuetracker.unity3d.com/issues/the-stackoverflowexception-error-is-thrown-in-the-console-and-the-editor-freezes-when-spacebar-is-pressed-after-selecting-the-last-element-of-a-list))

- Vulkan:  Editor crash when changing Vulkan Number of Swapchain Buffers
    ([UUM-60016](https://issuetracker.unity3d.com/issues/vulkan-editor-crash-when-changing-vulkan-number-of-swapchain-buffers))

- Vulkan: [Linux][Vulkan] Crash when using Nvidia drivers >545 and graphics API set to Vulkan
    ([UUM-73447](https://issuetracker.unity3d.com/issues/linux-vulkan-crash-when-using-nvidia-drivers-545-and-graphics-api-set-to-vulkan))



# 6000.0.7f1 Release Notes

## Features

- Package Manager: Added a new Editor `-upmLogFile` command line argument that specifies a custom file path for UPM log output.

- Shaders: Added support for the `#push_line 1234 filename` and `#pop_line` directives to the Shader Pre-processor.



## Improvements

- 2D: Add toggle to allow users to generate an outline for all Sprites in a Texture, even if the Sprites already had an outline defined.

- 2D: In the Sprite Editor, users now can:<br>
    - Copy an outline from a module and persist the outline to the other module<br>
    - Copy and paste the outline from the alternate module \(Outline to Physics Shape and Physics Shape to Outline\)<br>
    - Copy and paste all outlines from the alternate module

- Documentation: Added a new workflow to the Timeline Workflows documentation: The Create a custom Notes marker workflow, which demonstrates how to create a custom marker for adding notes to Timeline instances. This workflow also demonstrates how to change the default appearance of a custom marker with scripting and a Unity Style Sheet \(USS\).

- Editor: Added a warning for lights baked in shadow mask mode falling back to fully baked.

- Editor: Added Prefab Variant to the Shortcut area of the Create Menu.
    ([UUM-73105](https://issuetracker.unity3d.com/issues/prefab-variant-creation-is-too-hidden-when-creating-via-context-menu))

- Graphics: Improved vertex data copy for Dynamic Batching.

- HDRP: Added SG custom refraction example to Transparency sample.

- HDRP: Adding environment samples showcasing environment effects together.

- iOS: Print a warning if there are symlinks in a framework when building on Windows.

- iOS: Validate that frameworks contain Info.plist file.

- macOS: Added a better error message for duplicate source file plugins.

- Package Manager: Package icons positions are now consistent with the type of information they pass on to the users.

- Physics: Improved the behavior of MeshCollider mesh cooking by allowing again the use of meshes where the distance between two vertices of a triangle is greater than 500 units. Using meshes as such can break simulation \(especially character controller\) and query stability in PhysX. This issue would only occur when MeshColliderCookingOptions.WeldColocatedVertices or MeshColliderCookingOptions.EnableMeshCleaning would be enabled when baking a triangle mesh.

- Physics: Improved the label for the physics integration dropdown in order to clarify what the property does.

- Physics: Improved the message provided when using a mesh that contains triangles where the distance between any two vertices is greater than 500 units. The message now effectively reflects the guidance within the PhysX SDK documentation.

- Scene/Game View: EditorTool buttons now automatically refresh state if respective tool's availability changes and unavailable tools are shown as disabled instead of hidden.

- UI Elements: Improved performance of MultiColumnListView and MultiColumnTreeView when changing the visibility status of columns.<br>
    A rebuild will now be scheduled instead of performed after each status change.
    ([UUM-72241](https://issuetracker.unity3d.com/issues/multicolumnlistview-causes-a-memory-leak-when-repeatedly-shown-and-hidden))

- VisionOS: Plugin path "Assets/Plugins/VisionOS/" is now recognized and auto-selects VisionOS as compatible platform.

- VisionOS: Soft Particle effects now account for foveation when sampling the depth buffer.



## API Changes

- Android: Added: Added AndroidConfiguration class which contains properties for many aspects of Android application, see https://developer.android.com/reference/android/content/res/Configuration for more information.

- Android: Added: Added AndroidJNI.InvokeAttached which you can you use from threads to invoke java methods without the worry of calling AttachCurrentThread/DetachCurrentThread.

- Android: Added: Added UnityEngine.AndroidApplication class which you can use to get current activity instance, invoke on UI or Main thread, and subscribe to configuration changes.

- UI Toolkit: Added: Added EnumButtonsAttribute. This can be used to display an enum field with a ToggleButtonGroup instead of a popup field.



## Changes

- Editor: Update 7-Zip to 24.06.

- Physics 2D: Change the default value of contact-threshold to zero \(off\) by default for new projects and improve its tooltip.

- Serialization: Changed alignment in SerializedFile from 8 to 16 bytes, and added 16 bytes alignment into ResourceFileBuilder to improve patching results on some platforms.



## Fixes

- 2D: Fixed blend issues in rendergraph 2d pipeline.
    (UUM-72414)

- 2D: Fixed issue where the outline detail is reset to 0 for a Sprite Rect in the Sprite Editor when an outline is pasted onto a Sprite Rect.
    ([UUM-72965](https://issuetracker.unity3d.com/issues/sprite-editor-reverts-the-outline-detail-parameter-to-0-when-a-copied-outline-is-pasted))

- 2D: Fixed null exception error when the user clicks on the Tile Palette Clipboard when there are no Tile Palettes available in the project.
    ([UUM-72843](https://issuetracker.unity3d.com/issues/nullreferenceexception-erorr-is-thrown-when-left-or-right-clicking-the-blank-preview-section-in-the-tile-palette-window))

- 2D: Fixed Sprite Mask issue with target sorting layers.
    ([UUM-72180](https://issuetracker.unity3d.com/issues/sprite-masks-affect-sprite-renderers-outside-their-range-when-a-light2d-is-present-with-specific-target-sorting-layers-selected))

- Android: Fixed crash on Xclipse GPU based devices when setting Buffer Debug name on OpenGLES3 and Development build settings.
    ([UUM-65666](https://issuetracker.unity3d.com/issues/android-graphics-the-player-crashes-with-gfxdeviceworker-runcommand-error-when-both-opengles3-and-development-build-are-selected))

- Android: Fixed problem with black screen when app is put to split mode.
    ([UUM-67558](https://issuetracker.unity3d.com/issues/android-an-issue-that-an-app-show-black-screen-when-it-is-put-into-multi-window-mode))

- Android: To add activity null handling in isInMultiWindowMode API
    ([UUM-71574](https://issuetracker.unity3d.com/issues/android-the-player-crashes-at-isinmultiwindowmode-when-using-lifecycle-methods))

- Asset Bundles: Only call CollectAllSpriteAtlasesAndPack once when building AssetBundles
    (UUM-73147)

- Asset Pipeline: Fixed issue with userData field in meta files not being read for script assets
    ([UUM-64694](https://issuetracker.unity3d.com/issues/empty-string-is-returned-when-using-assetimporter-dot-userdata))

- Audio: Fixed exception thrown while pausing when ARC window is empty.
    ([UUM-54894](https://issuetracker.unity3d.com/issues/error-pressing-the-editor-pause-button-throws-a-null-reference-error-if-arc-window-is-empty))

- Audio: Made the AudioRandomContainer more robust against rapid pitch changes from doppler.
    ([UUM-54951](https://issuetracker.unity3d.com/issues/arc-playback-stops-due-to-doppler-pitch-scheduling))

- Build Pipeline: Fixed an issue where if vswhere.exe failed to detect Visual Studio installations.  Now a warning is emitted to the editor console.
    (UUM-71000)

- Core: Fixed bake buttons that could still be clicked when baking is in progress.
    ([UUM-71747](https://issuetracker.unity3d.com/issues/nullreferenceexception-floods-the-console-when-previewing-probe-adjustments-before-probe-volume-baking-is-finished-prove-volume-baking-hangs))

- Core: Fixed baking reflection probes.
    ([UUM-73160](https://issuetracker.unity3d.com/issues/bake-reflection-probes-button-no-longer-works-and-produces-a-nullref-error))

- Core: Fixed brick placement when using probe offset and max possible probe spacing.
    (UUM-70739)

- Core: Fixed cloning of baking sets when opening a new scene in 'Single Scene' mode.
    (UUM-73037)

- Core: Fixed holes when placing APV probes on terrains.
    (UUM-73036)

- Core: Improved error reporting when baking APV with an incorrect setup.
    (UUM-72047)

- Documentation: Added the Enable constrained proportions option to the Transforms page.

- Documentation: Fixed URP and HDRP documentation for APV Rendering Layers.

- Documentation: Updated directions to the Project Settings window in our Settings page.

- DX12: .Fixed an out-of-memory crash on XBox.
    (UUM-69790)

- DX12: Fixed an issue by binding the color attachments in the correct order.
    (UUM-53003)

- Editor: A new setting has been included to skip local package scanning during version control initialization.
    ([UUM-70391](https://issuetracker.unity3d.com/issues/the-editor-hangs-when-opening-a-project-that-uses-local-packages-and-version-control))

- Editor: Build Profile -  Fixed for 'Recursive serialization is not allowed for threaded serialization' when the build profile context instance is created in a serialization callback.
    ([UUM-73206](https://issuetracker.unity3d.com/issues/build-profile-context-recursive-serialization-is-not-allowed-for-threaded-serialization-error))

- Editor: Build Profile - Redirecting the old build settings window to open the build profile window.
    (UUM-61498)

- Editor: Drag and drop operations performed on files within the currently open projects' folder should now succeed on Windows.
    ([UUM-54537](https://issuetracker.unity3d.com/issues/dragperformevent-is-not-called-when-files-from-the-project-folder-are-used))

- Editor: Ensure the editor uses ADB to compute a preview only for .prefab asset file.
    ([UUM-72567](https://issuetracker.unity3d.com/issues/could-not-open-file-for-read-error-logged-in-urp-sample-template-when-searching-for-assets))

- Editor: Fixed an issue where Texture.SetTextureSetting would take invalid values.
    ([UUM-63703](https://issuetracker.unity3d.com/issues/sprite-is-not-generated-when-its-texture-settings-are-changed-via-textureimportersettings))

- Editor: Fixed an issue where web proxy credentials would not be found when added through a dialog triggered by macOS/Safari after web proxy auto-discovery was enabled.

- Editor: Fixed an issue where, an Infinite loop within editor launch screen causes it to hang on exit.
    (UUM-60981)

- Editor: Fixed an issue with ordering of processing newly created ScriptableObjects. Awake\(\) is now the last step as expected and is no longer called twice.
    ([UUM-54568](https://issuetracker.unity3d.com/issues/assetpostprocessor-dot-onpostprocessallassets-is-called-twice-when-creating-an-asset-and-any-changes-to-serialized-fields-performed-in-the-first-call-are-not-saved))

- Editor: Fixed bug where polygons are created on the opposite side of the sprite for uGUI images.
    ([UUM-71372](https://issuetracker.unity3d.com/issues/polygons-are-created-on-the-opposite-side-of-the-sprite-when-the-sprite-boundaries-are-above-the-edge-of-the-texture))

- Editor: Fixed Copy/Paste for IMGUI ColorField so it only works when the field is selected.
    ([UUM-69791](https://issuetracker.unity3d.com/issues/lighting-components-and-lighting-settings-numerical-fields-are-stored-as-hex-expressions-and-cannot-be-saved-to-clipboard-as-numerical-values-when-using-keyboard-shortcuts))

- Editor: Fixed issue where clicking the "Fix" button in an XR project validation page can cause the Editor to crash.
    ([UUM-72376](https://issuetracker.unity3d.com/issues/crash-on-progressbadge-progressbadgeofsize-when-pressing-the-fix-button-for-camera-usage))

- Editor: Fixed issue with text shader not updating correctly after a transform change.
    ([UUM-73738](https://issuetracker.unity3d.com/issues/changing-button-transform-via-script-makes-text-appear-as-blurry-rectangles))

- Editor: Fixed LinuxEditor crash calling WarpCursorPosition outside of PlayMode.
    ([UUM-71828](https://issuetracker.unity3d.com/issues/linux-crash-on-newinput-mousecallbacks-ioctl-when-warpcursorposition-function-is-called))

- Editor: Fixed null ref when using TMP without essential resources imported.
    (UUM-73546)

- Editor: Fixed random flickering in some scene with dx12+graphics jobs.
    ([UUM-69987](https://issuetracker.unity3d.com/issues/material-on-a-gameobject-flickers-when-the-parent-of-the-gameobject-is-selected-and-the-mouse-is-dragged-over-the-scene-view-toolbar-buttons))

- Editor: Fixed Ray tracing quality keyword not having a pathtracing input.
    (UUM-48348)

- Editor: Fixed removing a scene from a baking set when it has just been added.
    ([UUM-72471](https://issuetracker.unity3d.com/issues/cant-add-a-scene-to-a-baking-set-when-it-has-just-been-deleted-from-the-set))

- Editor: Fixed splash screen logo and background sprites being unloaded after preview. This would also unload them if they were being used in the scene.
    ([UUM-72535](https://issuetracker.unity3d.com/issues/all-instances-of-the-splash-screen-sprite-are-not-rendered-after-the-splash-screen-ends-when-it-is-previewed-in-the-editor))

- Editor: Fixed subsection of HDRP Asset not opening when using same index as its parent section.
    (UUM-62809)

- Editor: Fixed the serialized property becoming invalid whilst changing prefab fields via dropdown.
    ([UUM-72761](https://issuetracker.unity3d.com/issues/nulleferenceexception-serializedobject-of-serializedproperty-has-been-disposed-dot-is-thrown-when-changing-layermask-in-the-inspector))

- Editor: Fixed transient resources in NRP RenderGraph.
    (UUM-70422)

- Editor: Fixed URP render pass names. They now match the profiler sampler names, are more consistent and descriptive. Also solving issues with the profiler scopes for certain passes.
    (UUM-73451)

- Editor: Fixed wireframe not rendering when using Vulkan.
    ([UUM-36914](https://issuetracker.unity3d.com/issues/objects-are-invisible-in-scene-view-when-using-wireframe-shading-mode))

- Editor: Fixed YAML parsing error when property containing GUID is not defined in a single line
    ([UUM-72596](https://issuetracker.unity3d.com/issues/player-settings-common-optimization-setting-preload-assets-throws-parser-error))

- Editor: Improve setlocale LC_NUMERIC guards.
    (UUM-58980)

- Editor: Minor update of the Unity theme.

- Editor: NativeRenderPass in URP can reach a hard-coded limit that breaks the rendering when using Compatibility Mode.
    (UUM-69909)

- Editor: NullReference exception gathering GlobalSettings while having the GraphicsSettings inspector opened.
    (UUM-72335)

- Editor: Property attribute with `applyToCollection` set to true should not affect non-collection fields.
    ([UUM-67390](https://issuetracker.unity3d.com/issues/property-attributes-dont-affect-regular-fields-when-applytocollection-is-set-to-true))

- Editor: Switch to Custom GetHashCode for Delegates in RenderGraphPass.
    (UUM-71876)

- GI: Fixed a crash when cancelling during a lightmap bake.
    ([UUM-71709](https://issuetracker.unity3d.com/issues/crash-on-convertbuffertoexrbuffer-when-lighting-generation-is-cancelled))

- GI: Fixed a crash when the Enlighten precompute data is too large. Report an error instead.
    ([UUM-70217](https://issuetracker.unity3d.com/issues/crash-on-memcpy-when-importing-lightmaps-after-gi-bake))

- Graphics: Fixed a crash when unsupported Vulkan debug tools were used accidentally.
    ([UUM-72790](https://issuetracker.unity3d.com/issues/android-vk-crash-on-vk-debugtoolsutils-setvkdebugobjectname-vkdevice-t-star-vkobjecttype-unsigned-long-char-const-star-const-plus-when-vulkan-graphics-api-is-in-use-on-a-specific-device))

- Graphics: Fixed blending artifacts on some old Adreno GPUs.
    ([UUM-72350](https://issuetracker.unity3d.com/issues/vulkan-android-visual-corruption-is-visible-on-some-android-devices-in-the-player-when-depth-of-field-is-enabled-in-global-volume-and-the-vulkan-graphics-api-is-selected))

- Graphics: Fixed by issuing an error and doing an early return instead of crashing.
    ([UUM-72801](https://issuetracker.unity3d.com/issues/crash-on-renderbuffermanager-textures-gettempbuffer-when-rendering-a-specific-scene))

- Graphics: Fixed several crashes when assigning indices to a mesh that has overlapping sub-meshes.
    (UUM-12003)

- Graphics: Preventing vertex input dynamic state optimization from being used on Adreno 740 because of driver bug.
    ([UUM-41282](https://issuetracker.unity3d.com/issues/ui-toolkit-draws-black-screen-on-adreno-740))

- Graphics: Warning about missing Depth for a RenderTexture needs to be improved.
    (UUM-72935)

- Graphics Tests: Error is no longer thrown if reference image is not present on Android and WebGL
    ([UUM-73039](https://issuetracker.unity3d.com/issues/error-is-thrown-if-reference-image-is-not-present-on-android-and-webgl))

- HDRP: Fixed an issue where Terrains with 4 layers or less displayed a checker texture when using debug views.
    ([UUM-65807](https://issuetracker.unity3d.com/issues/hdrp-terrain-displays-the-checker-texture-in-unlit-draw-mode-despite-a-base-texture-layer-being-set))

- IL2CPP: Changes to ensure unique field names in C++.
    ([UUM-65459](https://issuetracker.unity3d.com/issues/build-failure-occurs-due-to-a-duplicate-member-error-when-a-callback-with-two-unnamed-arguments-is-defined-in-the-il2cpp-scripting-backend-in-the-development-build))

- IL2CPP: Fixed a memory leak related to thread static data.
    ([UUM-69774](https://issuetracker.unity3d.com/issues/android-memory-increases-continuously-after-calling-java-code-via-jni-bridge))

- IL2CPP: Fixed custom linker setup with --linker-flags-file.
    (UUM-71341)

- IL2CPP: Fixed slow performance when loading an XML document with DTD.
    ([UUM-66880](https://issuetracker.unity3d.com/issues/headers-of-xhtml-documents-are-rewritten-when-building-with-il2cpp))

- IL2CPP: Fixed sporadic crashes on ARM based platforms.
    ([UUM-68221](https://issuetracker.unity3d.com/issues/android-il2cpp-player-crashes-on-memcpy-aarch64-simd-plus-276-when-invoking-native-code-via-a-plugin-on-some-arm64-android-devices))

- Input: Improved the performance of the Gamepad.SetMotorSpeeds\(\) script API.
    ([UUM-72692](https://issuetracker.unity3d.com/issues/gamepad-dot-setmotorspeeds-cpu-usage-is-3-times-higher-when-the-controller-is-connected-via-bluetooth))

- iOS: Don't symlink .xcprivacy files when "Symlink Sources" build option is selected.
    (UUM-72375)

- iOS: Fixed a small memory leak in UnityWebRequest \(custom HTTP headers\).
    ([UUM-73104](https://issuetracker.unity3d.com/issues/ios-memory-leaks-occur-when-unitywebrequest-dot-get-is-called))

- Kernel: Reduced job system overhead when many jobs finished executing simultaneously.
    ([UUM-73194](https://issuetracker.unity3d.com/issues/job-allocator-contention-causes-slow-job-execution))

- Package Manager: Disabled uneditable package manager values in inspector for selected packages.
    ([UUM-42560](https://issuetracker.unity3d.com/issues/package-manager-values-in-the-inspector-are-displayed-in-uneditable-text-boxes))

- Package Manager: Displaying a console warning when the user attempts to install a git package while another installation is in progress, explaining the reason for the operation's failure.
    ([UUM-63744](https://issuetracker.unity3d.com/issues/just-the-first-package-is-being-installed-and-no-error-slash-warning-message-is-logged-when-installing-two-packages-using-add-package-from-git-url))

- Package Manager: Enable/Disabling 'All' and 'None' buttons in package Import/Export window based on the checked files.
    ([UUM-42266](https://issuetracker.unity3d.com/issues/packman-all-button-is-displayed-as-active-in-the-import-window-even-there-are-no-other-items-which-could-be-selected))

- Package Manager: Fixed an issue where Web proxy credentials added by macOS during a system request through a WPAD web proxy were not found.

- Package Manager: Fixed the issue where All and None buttons in asset remove window are active all the time.
    (UUM-72076)

- Package Manager: Fixed the issue where the git tag show up as ellipsis in the Package list.
    (UUM-70418)

- Package Manager: Fixed the issue where tooltip on actions dropdown menu for Asset Store packages doesn't appear anymore.
    (UUM-73315)

- Package Manager: Import and Export buttons are now disabled if there is nothing to import or export.
    ([UUM-41782](https://issuetracker.unity3d.com/issues/import-button-is-active-in-the-import-unity-packages-window-even-if-there-are-no-items-selected-for-import))

- Physics: Fixed an issue where ignorance lists would not persist if the involved colliders get disabled and re-enabled.
    ([UUM-72127](https://issuetracker.unity3d.com/issues/physics-dot-ignorecollision-function-is-not-applied-when-toggling-the-gameobject-dot-setactive))

- Physics: Fixed an issue where the physics integration dropdown would always be disabled.

- Physics: Fixed an issue where the Physics settings uxml files defined the window title labels without a proper padding. Resulting in the titles being slightly misaligned.

- Physics: Fixed raycast not hitting a collider when part of a ignore collision pair.
    (UUM-71659)

- Physics 2D: A PolygonCollider2D associated with a SpriteRenderer using "Sliced" Draw Mode should not crash when empty paths are added.
    ([UUM-71177](https://issuetracker.unity3d.com/issues/crash-on-schedulegeneratetilingshape-when-modifying-polygoncollider2d-path-count-and-setting-path-vertices))

- Player: Fixed as issue in URP Forward+ where screen space decals would not render in builds if using rendering layers.
    ([UUM-72315](https://issuetracker.unity3d.com/issues/mobile-the-material-is-not-visible-when-using-the-decal-renderer-feature))

- Player: Fixed possible crash on shut down when custom player loop is set.
    ([UUM-72551](https://issuetracker.unity3d.com/issues/ios-crash-on-il2cpp-gc-gchandle-free-when-app-returns-to-foreground))

- Prefabs: Added checks for TransformHierarchy initialization in SetParent.
    ([UUM-73287](https://issuetracker.unity3d.com/issues/crash-on-transform-setparent-when-duplicating-a-prefab-in-the-hierarchy))

- Scene/Game View: Fixed the direction label that was not updating anymore since moving the orientation gizmo to an overlay.
    ([UUM-72103](https://issuetracker.unity3d.com/issues/the-text-below-orientation-gizmo-does-not-change-when-the-scene-viewing-direction-changes))

- Scripting: Fixed crashes and hangs in multithreaded code that uses `Awaitable`.
    (UUM-73652)

- Scripting: Fixed issue with an InstantiateAsync overload that took a parent as parameter but did not apply it.
    ([UUM-67809](https://issuetracker.unity3d.com/issues/instantiated-prefabs-recttransform-values-are-incorrect-when-object-dot-instantiateasync-is-used))

- Scripting: Fixed issue with SkinnedMeshRenderer using the original object's bones after being cloned with InstantateAsync.
    ([UUM-67809](https://issuetracker.unity3d.com/issues/instantiated-prefabs-recttransform-values-are-incorrect-when-object-dot-instantiateasync-is-used))

- Scripting: Fixed issue with values in RectTransform not being copied with InstantiateAsync.
    ([UUM-67809](https://issuetracker.unity3d.com/issues/instantiated-prefabs-recttransform-values-are-incorrect-when-object-dot-instantiateasync-is-used))

- Serialization: Ensure m_Reader destructor is not called after its dependencies are destroyed.
    (UUM-69875)

- Shadergraph: Add support for perceptual color mode for gradients in shader graph.
    ([UUM-72278](https://issuetracker.unity3d.com/issues/the-gradient-shader-is-inverted-when-using-the-perceptual-blend-mode))

- Shaders: Fixed "incompatible keyword state" assertions being generated by shaders whose `UsePass` command resolved to a pass from the target shader's fallback
    ([UUM-71342](https://issuetracker.unity3d.com/issues/resolveusepasses-now-extracts-passes-from-all-subshaders-including-fallbacks-in-contrast-to-documented-behaviour))

- Shaders: Fixed reversebits implementation on metal.
    (UUM-73255)

- Shaders: Fixed ShaderLab's `UsePass` command finding passes from multiple subshaders.
    ([UUM-71342](https://issuetracker.unity3d.com/issues/resolveusepasses-now-extracts-passes-from-all-subshaders-including-fallbacks-in-contrast-to-documented-behaviour))

- SRP Core: Fixed an exception thrown when Render Graph pass was missing its renderFunc but tried to compute its hash value.
    (UUM-72067)

- SRP Core: Fixed light.useViewFrustumForShadowCasterCull previously being ignored for shadow cascades. light.useViewFrustumForShadowCasterCull now works as expected.
    ([UUM-56026](https://issuetracker.unity3d.com/issues/light-dot-useviewfrustumforshadowcastercull-not-working-properly-for-shadow-cascades))

- SRP Core: Fixed Render Graph Compiler logic bug where UnsafePass using MSAA texture could result in missing resolve surface errors.
    ([UUM-73154](https://issuetracker.unity3d.com/issues/draw-objects-pass-and-endrenderpass-errors-are-thrown-when-anti-aliasing-msaa-is-enabled-and-beautify-asset-is-added-as-a-renderer-feature))

- Text: Fixed rounding issue in text measurement.
    (UUM-70819)

- TextCore: Address issue with CRLF line-endings breaking the text measurement.
    (UUM-70040)

- Timeline: Fixed an issue where using , and . \(&lt;&gt;\) to step frames in the Animation Window while the Timeline Window was linked would sometimes not work.

- Timeline: When the Timeline and Animation windows are linked and the Timeline Window is active, moving the playhead in the Timeline Window will cause the animation window to repaint immediately.

- UI Elements: Clicking to the left/right of the MinMaxSlider will now adjust the min/max bound value instead of moving the slider.
    ([UUM-54703](https://issuetracker.unity3d.com/issues/interacting-with-a-randomization-slider-by-clicks-changes-the-other-end))

- UI Toolkit: Correctly implement background repeat rounded corner.
    (UUM-72717)

- UI Toolkit: Fixed an issue in the runtime bindings system where classes having a dynamic hash code would throw an exception.
    ([UUM-69322](https://issuetracker.unity3d.com/issues/invalidoperationexception-errors-are-thrown-when-changing-property-elements-and-attempting-to-access-them-during-runtime))

- UI Toolkit: Fixed attributes overrides not being applied when having some unnamed templates.
    ([UUM-72983](https://issuetracker.unity3d.com/issues/properties-of-custom-visual-elements-fail-to-initialize-when-inside-of-template-that-has-been-renamed))

- UI Toolkit: Fixed builtin resources being added as dependencies to UXML files.
    (UUM-69932)

- UI Toolkit: Fixed colliding ids for uxml objects.
    ([UUM-73046](https://issuetracker.unity3d.com/issues/invalid-uxml-or-uss-system-dot-invalidcastexception-and-argumentexception-invalid-path-errors-are-thrown-and-ui-documents-become-unusable-when-they-are-saved-with-invalid-attributes))

- UI Toolkit: Fixed exception when adding a UxmlObject that had no attributes to a list in the UI Builder.
    ([UUM-71735](https://issuetracker.unity3d.com/issues/invalidoperationexception-is-thrown-and-list-elements-cant-be-added-when-a-uxmlobject-in-a-list-has-no-attributes))

- UI Toolkit: Fixed renaming field focused after entering an invalid name in UI Builder.
    (UUM-73106)

- UI Toolkit: Fixed UI Builder flex-grow tooltip information.
    ([UUM-73486](https://issuetracker.unity3d.com/issues/incorrect-description-is-shown-when-viewing-the-tooltip-of-uss-property-flex-grow-in-ui-builder))

- Universal RP: Added warning box in the camera inspector when both TAA and MSAA is enabled to notify the user that TAA will be skiped with current settings.
    ([UUM-62984](https://issuetracker.unity3d.com/issues/taa-urp-setting-missing-info-slash-warning-box-to-inform-action-needed))

- Universal RP: Fixed a render graph bug where a pass-break between GBuffer and deferred lighting would cause an error.
    ([UUM-63928](https://issuetracker.unity3d.com/issues/errors-are-thrown-and-the-scene-view-is-not-rendered-when-rendering-path-is-set-to-deferred))

- Universal RP: Fixed render graph scheduling logic for CopyDepth pass when custom passes that read depth are present.
    (UUM-73174)

- URP: Fixed render graph allocated textures not respecting dynamic scaling settings in some cases.
    ([UUM-65350](https://issuetracker.unity3d.com/issues/copydepthpass-rthandle-ignores-dynamic-scaling-and-breaks-depth-based-post-processing-when-changing-the-scale-factor-value))

- URP: Made the gBuffer components non-global.
    (UUM-69940)

- VFX Graph: Fixed "int" type could not be parsed when the access modifier is not specified
    ([UUM-71490](https://issuetracker.unity3d.com/issues/vfx-custom-hlsl-with-int-parameter-without-the-in-slash-out-slash-inout-access-modifier-is-not-supported))

- VFX Graph: Fixed a leak while spamming ReInit.
    ([UUM-71455](https://issuetracker.unity3d.com/issues/vfx-graph-memory-leak-when-calling-the-clearpropertybinders-and-addremovevfxproperty))

- VFX Graph: Fixed compilation error when using the Six-way Lit Output with Adaptive Probe Volumes.
    (UUM-72781)

- VFX Graph: Fixed output properties in subgraphs had misplaced wire connector.
    (UUM-72960)

- VFX Graph: Fixed potential crash when using the Noise Module in a particle system.
    ([UUM-72971](https://issuetracker.unity3d.com/issues/crash-on-block-merge-next-when-moving-a-gameobject-with-a-specific-particle-system-component-and-rate-over-distance-is-set-to-above-0-in-the-emission-tab))

- VFX Graph: Fixed potential exception message in the console when opening any VFX Graph.
    ([UUM-71918](https://issuetracker.unity3d.com/issues/windows-error-argumentexception-illegal-characters-in-path-logged-when-creating-a-vfx-graph))

- VFX Graph: Fixed some UI elements could overflow their reserved space.
    ([UUM-70602](https://issuetracker.unity3d.com/issues/vfxg-the-input-fields-have-overflowed-their-container-due-changing-label-size))

- VFX Graph: Fixed unexpected CustomHLSL includes in neighbors contexts.
    (UUM-66620)

- Video: Editor freezes when playing videos with playback speed value &lt;1 and setting time via started callback
    ([UUM-73115](https://issuetracker.unity3d.com/issues/editor-freezes-when-playing-videos-from-url-with-playback-speed-value-1-and-setting-time-via-started-callback))

- Video: \[Android\] Player with the specific Video clip crashes on "/apex/com.android.runtime/lib/bionic/libc.so \(__memcpy_a53+96\)" when the video is bundled with other video clips and Codec is set to VP8.
    ([UUM-73032](https://issuetracker.unity3d.com/issues/android-player-with-the-specific-video-clip-crashes-on-slash-apex-slash-com-dot-android-dot-runtime-slash-lib-slash-bionic-slash-libc-dot-so-memcpy-a53-plus-96-when-the-video-is-bundled-with-other-video-clips-and-codec-is-set-to-vp8))

- VisionOS: Consider plugins compatibility even if their .meta files are empty \(default import settings\).
    (UUM-72377)

- WebGL: Fixed a bug that prevented users from copying and pasting between other html elements.
    ([UUM-72388](https://issuetracker.unity3d.com/issues/event-handlers-are-preventing-operations-when-trying-to-copy-or-paste-html-text-in-the-webgl-player))

- WebGL: \[WebGPU\] Fixed an error about null texture data.

- WebGL: \[WebGPU\] Fixed error about commands being executed while a render pass is still active.

- WebGL: \[WebGPU\] Fixed for compute shader write-only storage textures.

- WebGL: \[WebGPU\] Fixed native texture creation.

- WebGL: \[WebGPU\] Fixed webgpu shader compilation compute shaders for false errors about non-uniform barrier calls.




## Package changes in 6000.0.7f1

## Packages updated

- com.unity.2d.spriteshape: [10.0.5](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@10.0//changelog/CHANGELOG.html) to [10.0.6](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@10.0//changelog/CHANGELOG.html)

- com.unity.purchasing: [4.11.0](https://docs.unity3d.com/Packages/com.unity.purchasing@4.11//changelog/CHANGELOG.html) to [4.12.0](https://docs.unity3d.com/Packages/com.unity.purchasing@4.12//changelog/CHANGELOG.html)

- com.unity.recorder: [5.1.0](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) to [5.1.1](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html)

- com.unity.timeline: [1.8.6](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) to [1.8.7](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)

- com.unity.xr.arcore: [6.0.1](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.0//changelog/CHANGELOG.html) to [6.0.2](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.0//changelog/CHANGELOG.html)

- com.unity.xr.arfoundation: [6.0.1](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.0//changelog/CHANGELOG.html) to [6.0.2](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.0//changelog/CHANGELOG.html)

- com.unity.xr.arkit: [6.0.1](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.0//changelog/CHANGELOG.html) to [6.0.2](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.0//changelog/CHANGELOG.html)

- com.unity.xr.hands: [1.4.0](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.4//changelog/CHANGELOG.html) to [1.4.1](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.4//changelog/CHANGELOG.html)

- com.unity.multiplayer.playmode: [1.1.0](https://docs.unity3d.com/Packages/com.unity.multiplayer.playmode@1.1//changelog/CHANGELOG.html) to [1.2.0](https://docs.unity3d.com/Packages/com.unity.multiplayer.playmode@1.2//changelog/CHANGELOG.html)

- com.unity.dedicated-server: [1.1.0](https://docs.unity3d.com/Packages/com.unity.dedicated-server@1.1//changelog/CHANGELOG.html) to [1.2.0](https://docs.unity3d.com/Packages/com.unity.dedicated-server@1.2//changelog/CHANGELOG.html)

**Pre-release packages added**

- [com.unity.purchasing@4.12.1-pre.1](https://docs.unity3d.com/Packages/com.unity.purchasing@4.12//changelog/CHANGELOG.html)

- [com.unity.xr.hands@1.5.0-pre.3](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.5//changelog/CHANGELOG.html)