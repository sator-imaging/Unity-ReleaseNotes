# Unity 3.5

https://unity3d.com/unity/whats-new/unity-3.5

## Improvments

- [Android](#android)
- [Audio](#audio)
- [Documentation](#documentation)
- [Editor](#editor)
- [Graphics](#graphics)
- [Lightmapping](#lightmapping)
- [iOs](#ios)
- [Scripting](#scripting)
- [Miscellaneous](#miscellaneous)


### Android

*   Added AndroidJavaRunnable to automatically marshal script delegates to Java code.
*   Introduced automatic unlocking of the device when running development builds.
*   Introduced passing touch and key events directly to native code when using NativeActivity.
*   Removed delay when returning to an application, stemming from an unnecessary recreation of the GL context.
*   Stored the keystore file relative to the project path.

### Audio

*   Changing mixer's sample rate and buffer sizes from script now possible.
*   Cross domain security check for AudioClip::GetData() in webplayers.
*   Custom DSPs (OnAudioFilterRead) now respect the settings of the attached AudioSource (mute, attenuation curves etc.)
*   Microphone frequency capabilities now accessible from script and can be used in Record().
*   Multichannel (>2) OGG files are now encoded and mapped correctly.
*   Introduced non-blocking waveform renderer (higher resolution and nicer-looking)

### Documentation

*   Added extensive sections on new features in the Manual (Shuriken, Navigation Mesh, Level of Detail).
*   Fixed formatting issues for code snippets on IE
*   Fixed up many code examples.

### Editor

*   Fixed the "Generate Lightmap UVs" reducing the difference between mac/win. Not there yet, but should be fixed for the most part. Please reimport meshes and rebake lightmaps.
*   A LOD group that was created on import can now be updated in the scene and send these settings back to the importer.
*   Added "All" and "None" items for active Layer selection menu.
*   API: Added optional parameter includeChildren to PropertyField to allow creating entire class or array controls with a single function call.
*   API: Exposed GetIconSize and SetIconSize.
*   API: Made DrawDefaultInspector work with both LooksLikeInspector and LooksLikeControls.
*   API: Made PropertyField respect indent level instead of overwriting it with property depth.
*   Asset Import performance optimizations for large project folder. For example detecting assets to be refreshed is around 10x faster now. Opening an already imported project is around 50x faster.
*   Audio clips now use the static preview system. This means that audio clips now have a preview in the object picker/browser.
*   Break prefab menu item added to Game Object menu (Break button was removed from gameobject inspector).
*   Curve Editor key selection improvement: Always select the topmost key if keys of multiple curves are overlapping.
*   Debug.DrawLine and Debug.DrawRay now take an optional bool that can disable depth testing.
*   Ensure terrain brush settings are not reset when selecting a different object or when entering or exiting Play mode.
*   EnumPopup element strings are now "nicified".
*   Even more fixes to "Generate Lightmap UVs" to make it generate same UVs across Mac/Win.
*   Fixed various project import issues where a crash of Unity could lead to a full project reimport in some cases.
*   Implement EditorGUI functions BeginChangeCheck, EndChangeCheck, BeginDisabledGroup, EndDisabledGroup as more high-level alternative to setting GUI.changed and GUI.enabled directly.
*   Import settings are now shown at the top in the Inspector and the imported result below (when relevant).
*   Improve feedback to the UI about which color space is active.
*   Lightmapping Window, Occlusion Window, and Navigation Window now have type based scene filters for quick picking of relevant objects.
*   Made intValue property in SerializedProperty API work for LayerMask type.
*   Made inspector display large Asian fonts with kerning information quickly, and show progress bar for import.
*   Miscellaneous LOD group editor improvements.
*   Made rectangle selection of meshes more precise.
*   Introduced the property EditorGUIUtility.isProSkin.
*   Objects can now be tagged separately as occluders and occludees.
*   Optimized performance of changing parenting in the hierarchy window.
*   Polished Import/Export package dialogs a bit.
*   Scene View FPS motion is a bit slower by default, and has acceleration for when you want to go far.
*   Show warning about precision errors in Transform inspector if world position exceeds 100.000 in any axis.
*   The Navigation window now lets you change the Navigation Static flag of selected game objects.
*   Transform gizmo now has planar sliders.
*   Undo / Redo now works as expected when enabling and disabling components.
*   Unity can import meshes with vertex count larger than 65000. Instead of aborting import it will split the mesh into parts each containing less than 65000 vertices.
*   Upgraded FBX SDK to 2012.2.
*   When changing numbers using sliders, do context sensitive rounding. The rounding will leave exactly enough decimals to represent the change resulting from moving the slider one pixel. If more decimals are typed in manually, they will not be lost (within the limitations of floating point numbers).
*   When selecting objects of different types, the Inspector will now help narrowing down the selection to objects of only one type.
*   You can now set a default font color via the font importer.

### Graphics

*   Extended the maximum number of shader keywords from 32 to 64.
*   For each shader compilation error show the keywords that were used.
*   MaterialPropertyBlock can now have an unlimited number of properties.
*   OnWillRenderObject lets you rotate or slightly move an object before rendering. The updated transform will be used during the render pass. This makes it possible to for example align a billboard only when it is visible using OnWillRenderObject.

### Lightmapping

*   Exposed the padding property that controls texel spacing between bake instances.
*   Improved mipmap generation for lightmaps - the space between bake instances is filled with colors coming from those bake instances when going down and up the mip chain. The lighting in smaller mip levels is more accurate and preserves the overall feel of the lightmap better. Please rebake the lightmaps to get the benefit.
*   Made fetching lightmaps use much less temporary memory.

### iOs

*   Added Caching.SetNoBackupFlag and Caching.ResetNoBackupFlag to set "No Backup" flag on cache.
*   Added iPhone.SetNoBackupFlag and iPhone.ResetNoBackupFlag to set "No Backup" flag.
*   Caching now set no-backup flag by default on newly added objects.

### Scripting

*   JavaScript: Creating a new script automatically adds “#pragma strict” by default.
*   JavaScript: Warn when bitwise operators are used with boolean operands to suggest the shortcircuiting boolean operators.
*   JavaScript: @script attribute declarations can now appear before 'import'.
*   JavaScript: Files containing interface and/or enum definitions named after them are now supported (e.g. interface IFoo in file IFoo.js) as the compiler will no longer generate a conflicting MonoBehaviour definition.
*   Boo: Pattern matching for lists.
*   Boo: Selective import support.
*   Boo: Better linq (and extension method support) in general: 'import System.Linq;' is enough now.
*   Boo: Optimized multidimensional array operations (up to 100X in some cases).

### Miscellaneous

*   Asset Import: Texture importing now uses a lot less temporary memory.
*   Asset Server: Projects can now be copied in the admin view.
*   Mac OS X Standalone: Added a "close" button to the player window.
*   ModelImport: Warnings about quaternions now contains the name of the model and can in most cases be clicked to highlight the model in the project view.
*   MonoDevelop (JavaScript/Boo): Added limited jump to definition support.
*   Occlusion culling baking now doesn't run out of memory.
*   Occlusion culling now works correctly with shadows and is much faster. All occlusion culling modes should work as expected now across all platforms.
*   Player: Pre-load asset dependencies when doing Resources.Load/LoadAll to avoid hiccups during runtime.
*   Profiler: Added API to enable binary filedump of profiling data, and API to read it back in the Editor.
*   Reduced memory usage when importing large project folders.
*   Scripting: Added Handheld.use32bitDisplayBuffer to change Display buffer bit-depth at runtime.
*   Scripting: Added WWW.textureNonReadable to mark as non-readable after download.
*   SkinnedMeshes can now be marked as occluders and occludees.
*   Substance import issues with input textures were fixed.
*   Static batch mesh generation (Part of the build process and editor play mode) is now a lot faster.
*   Support copying files from Assets/StreamingAssets for Win/Mac standalone players.
*   Unwrap: All known cases of mac/win uv generation were fixed. Please reimport your meshes.
*   Web Player: If the embedding page or unity3d file is hosted on https, the web player will use https for all connections (update checks and downloads), so the browser will not show warnings about insecure connections.
*   When baking occlusion culling with transparent objects marked as occluders a warning is now given telling you which objects are marked static incorrectly.
*   When imported assets are dirtied because a script modifies the imported asset it will no longer cause the asset to be reimported. Instead it will unload the asset and reload from disk as soon as nothing is referencing the asset anymore. This fixes an issue where a lot of assets would get reimported when shutting down Unity after entering playmode depending on what the scripts did.
*   Windows: Connected joysticks are detected at runtime.