# Unity 3.5

https://unity3d.com/unity/whats-new/unity-3.5

## Fixes

- [Android](#android)
- [Audio](#audio)
- [Debugger](#debugger)
- [Editor](#editor)
- [Graphics](#graphics)


### Android

*   Texture2D.EncodeToPNG() / Application.CaptureScreenshot() produced broken images.
*   Calling Application.Quit from OnApplicationPause() had unexpected consequences.
*   Calling Network.TestConnection() caused the application to crash.
*   Calling Time. from OnApplicationPause() could cause application to hang.
*   Calling game scripts from the Java UI thread could cause a crash on rare occasions.
*   Fixed a GLES 2.0 rendering problem specific to Broadcom chipsets.
*   Fixed crash on Honeycomb/IceCreamSandwich devices triggered by 'auto-rotation' or any kind of screen rotation.
*   Fixed incorrect handling of Debug.Log in non-development builds - Message is now printed, but callstack parsing is disabled to keep performance up.
*   Fixed video playback when using a local (file://) source.
*   Graphical artifacts in decompressed ETC1 textures have been corrected.
*   In the editor resolution/aspect ratio settings, the HTC Legend dimensions were swapped.
*   JDK 7 can now be used without getting a INSTALL\_PARSE\_FAILED\_NO\_CERTIFICATES error with signed applications.
*   JNI marshaling null-strings from Java would cause the VM to abort.
*   The basic/pro license was not honored correctly in some places.
*   The saved instance state bundle passed to Activity.onCreate was not forwarded from the Proxy activity.
*   Update AndroidManifest.xml permissions when Application.internetReachability is used - adding ACCESS\_NETWORK\_STATE fixes the problem with incorrect return value.
*   Using a custom splash during an advanced license trial period could lead to runtime crashes when trial expired.
*   Using a Linux 3.x kernel would cause Unity to hang/crash on multi-core CPUs.
*   WWW calls to a server that redirects from HTTPS to HTTP were failing.
*   Nvidia's PerfHUD for Tegra reported increasing frame times when the application was paused.
*   A few hardware keys were missing, like (forward) DELETE and left/right CTRL - these have now been added.
*   Callbacks to MonoBehaviour.OnApplicationFocus is now supported.
*   Added support for Galaxy Note Stylus Pen (through KeyCode.LeftControl and KeyCode.Delete).
*   Fixed annoying but harmless error about missing directory when building.
*   Android Remote: fixed occasional stale touches.
*   Android Remote: fixed flickering and improved stability on tablets.

### Audio

*   'Decompress On Load'/'Compressed in memory' option not shown for uncompressed audio.
*   Don't show BPS for MPEG files.
*   Audio/Video: Pause audio when video is done in the inspector.
*   Fixed custom rolloff curves.
*   Fixed 32 bit filtering.
*   libVorbis updated to the latest version.
*   Lowpass filter inspector fixed.
*   Reset on filters and reverb zones now works.
*   Size in inspector now correct for all platforms and audio types.
*   Support for compression of 32bit input files.

### Debugger

*   Fixed abort with reentrant evaluation.
*   Fixed crash with nullable evaluation.
*   Fixed debugger crash when debugging in the editor.

### Editor

*   After moving or renaming the current open scene, saving will now save into the new location rather than the old.
*   Editor: Curve Editor now correctly reverts and resets any change when dragging and Esc is pressed.
*   Editor: Dark skin component checkboxes no longer twitch.
*   Editor: Dark skin's object picker tweaks.
*   ESC to cancel searching is more robust.
*   Editor: Fixed animated GUI groups breaking and giving errors after a window has been re-docked.
*   Fixed color picker incorrectly initializing alpha to 255 if original color is (0,0,0,0).
*   Editor: Fixed dragging textures to apply in Scene View sometimes showing errors and displaying progress bar that never closes.
*   Fixed Esc not clearing search field on Mac in Object Picker.
*   Fixed GameObject static dropdown not marking "Nothing" as selected when no flags were selected.
*   Fixed handling of unicode characters in scripts. Scripts should have utf-8 encoding.
*   Fixed many Handle controls not respecting Handles.matrix.
*   Fixed mouse cursor sometimes flickering garbage on Windows.
*   Fixed not being able to assign characters like ' , . / \` \] \[ = as editor shortcuts on Windows.
*   Fixed null reference exception in project pane when displaying filtered results that return no hits and pressing up arrow key.
*   Fixed null reference exception when dragging sub-asset to the root of Project View.
*   Fixed Object Picker not focusing search field when being opened.
*   Fixed opening editor preferences when no inspector is open.
*   Fixed precision loss when viewing or editing large integers in the GUI.
*   Fixed repaint issue that made the Editor on Windows seem to have poor performance when mouse dragging gui components or scene view handles.
*   Fixed SceneView not resetting Handles.matrix if it was changed in an OnSceneGUI callback.
*   Fixed a bug where lists of enums were not editable in the inspector.
*   Fixed Animation View leaking materials when saving, while animation edit mode is active.
*   Editor: Fixed assert "vertexCount > 60000" when using colliders with polygon count over 10000.
*   Fixed crash when resizing arrays in the inspector.
*   Fixed crash when trying to import mesh, which contains polygons, which have less than 3 vertices.
*   Fixed drop-down menus on Windows so they no longer overlap with the GUI control.
*   Fixed material import from COLLADA files.
*   Fixed memory problem when committing a lot of assets in the Asset Server window.
*   Fixed null ref when exporting a package.
*   Fixed out of memory crash when importing huge cube maps.
*   Fixed problem setting custom fields in webtemplates (they'd disappear as soon as focus left the field).
*   Fixed regression where import mode for normals and tangents on models where ignored, when upgrading from 3.4 to 3.5
*   Editor: Fixed reversing of triangle culling in some imported models (that used to happen in some very special cases).
*   Fixed some situations where the scene view mode could get stuck.
*   Fixed texture detection for imported materials when FBX contains mixed slashes in texture file paths.
*   Fixed Warning when saving a scene to a new folder created from the Save dialog.
*   Fixed terrain trees permanently being hidden when right clicking while left-dragging to paint height.
*   Fixed crash when closing Editor Window in OnFocus.
*   Fixed that Unity sometimes fails to recompile changed scripts or notice changed assets when leaving Unity while its unresponsive (Windows).
*   Focusing on a particle system will now respect the bounds of the system properly.
*   GetMiniThumbnail returns proper icons for DefaultAssets.
*   Icons for unknown asset types are now cached, prevents out-of-memory crash if there are a lot of unknown assets in a project.
*   Improved interaction with Visual Studio 2010.
*   Installer on Windows now has a large icon.
*   Made 3DS file loader more robust - Unity handles invalid files better now.
*   Make ProceduralTextureInspector and ProceduralMaterialInspector partially support multi-object editing (multi-editing procedural properties is not supported).
*   Make ProceduralTextureInspector repaint until not regenerating anymore.
*   Made sure EditorGUI controls respect indent level consistently and fixed some rarely used overloads that ignored some of the given parameters.
*   Multiple project windows don't share search string.
*   Got rid of white 1-px outlines on OSX Lion.
*   On OSX don't allow saving files with special characters in save file dialogs.
*   On OSX don't make "error" sounds when navigating object browser using keyboard.
*   On Windows, don't open new explorer window every time the player is build.
*   Resolve intermittent hangs.
*   Scene View controls no longer freezes when using left mouse button on scene view handles while right mouse button is pressed down.
*   Setting TextureImporter.textureType now sets all the required properties.
*   Use significantly less memory in most cases when generating a cubemap from a very high-resolution source image to make out-of-memory crashes less likely.
*   Windows Editor menus support Unicode characters.
*   You can now slide values with sliders by dragging the label (same as float fields).
*   (Windows) Build Settings will not open after Cancel.
*   (Windows) Asset progress bar & build progress steals focus from other applications on windows.
*   Will now give a proper error when trying to import a movie with unsupported codecs.
*   Checked for scene camera rotation of NaN and fixed it.
*   Drastically reduce Scene View grid artifacts that caused it to be imprecise.
*   Fixed issue where editor would hang if left in background.
*   Child's scale is updated correctly when rotating with Inspector or Rotation Tool (when parent is non-uniformly scaled).
*   Deleting the root game object in OnPostProcessModel will no longer crash Unity.
*   Importing FBX models with bad texture references like "." and ".." no longer crashes Unity.
*   Upgrading a 3.4.x projects with Modo files will now retain ids for meshes, meaning that references to meshes are not lost. References to subgameobjects will still be lost.
*   (Windows) Fixed common random crash.
*   Fixed crash when calling SetActiveRecursively within Awake.
*   Fixed intermittent "Moving file failed" error when building player.
*   Fixed error when attempting to edit deleted terrain.
*   Advanced texture importer now correctly reflects internal texture import modes (For example no linear option for normal map textures).
*   Setting color preferences now has an instant effect on the editor.
*   Fixed that Unity does not refresh scripts when giving Unity focus by clicking on child windows.

### Graphics

*   Beast will no longer fail bakes on OSX if Unity installation path contains non-alphanumerical symbols.
*   Beast will no longer fail bakes on degenerate meshes, like bushes composed completely of billboarded leaves.
*   Compute correct tangents for non-uniformly scaled static meshes.
*   Enforce linear lighting status on hardware that does not support it.
*   Fixed broken values for builtin arrays when only 0th element was used (e.g. unity\_LightPosition\[0\]).
*   Fixed issue related to deferred rendering when no lights are present and you are using HDR.
*   Fixed Particles/Alpha Blend shader turning black when in Fog.
*   Fixed pow() sometimes being mis-compiled for Direct3D 9.
*   Fixed Preview lighting on uniformly scaled meshes in GameObjects.
*   Fixed shadow caster culling for asymmetric view frustums.
*   Fixes and improvements to HLSL->GLSL translator and GLSL Optimizer.
*   Flares without a texture assigned don't crash the editor anymore.
*   Texture2D.Compress prints proper error message when texture is not marked as readable (previously was silently filling texture with garbage when not in editor).
*   Fixed incorrect rendering order when using transparent shader with ParticleRenderer and MeshRenderer.
*   Fixed error message when setting null texture on a GUITexture.
*   Fixed more than one directional light shadow (via "fullfowardshadows") not working in Forward rendering if Image Effects are used.
*   Tweaked RGBM lightmap encoding, so that there are no brighter lines appearing in dark areas when bilinear filtering is used. Makes a huge difference in linear lighting mode, since dark values get relatively much brighter.
*   Lightmapping: "Use in forward rend." is only respected in Dual Lightmaps mode as the GUI suggests.
*   Lightmapping: Fixed clearing lightmaps -- it resets lightmap index, tiling and offset on all renderers.
*   Lightmapping: Made light be culled below horizon for specular bounces when shadows are disabled. Fixes a case where a face pointing away from light would bounce light in that direction.
*   Lightmapping: Use alpha from the base texture (\_MainTex) as the gloss map.
*   Lightmapping: Got rid of self-shadowing artifacts in small scenes placed far away from the origin (0,0,0).