# Unity 3.5
https://unity3d.com/unity/whats-new/unity-3.5

## Fixes


### Android
<ul>
<li>Texture2D.EncodeToPNG() / Application.CaptureScreenshot() produced broken images.</li>
<li>Calling Application.Quit from OnApplicationPause() had unexpected consequences.</li>
<li>Calling Network.TestConnection() caused the application to crash.</li>
<li>Calling Time. from OnApplicationPause() could cause application to hang.</li>
<li>Calling game scripts from the Java UI thread could cause a crash on rare occasions.</li>
<li>Fixed a GLES 2.0 rendering problem specific to Broadcom chipsets.</li>
<li>Fixed crash on Honeycomb/IceCreamSandwich devices triggered by 'auto-rotation' or any kind of screen rotation.</li>
<li>Fixed incorrect handling of Debug.Log in non-development builds - Message is now printed, but callstack parsing is disabled to keep performance up.</li>
<li>Fixed video playback when using a local (file://) source.</li>
<li>Graphical artifacts in decompressed ETC1 textures have been corrected.</li>
<li>In the editor resolution/aspect ratio settings, the HTC Legend dimensions were swapped.</li>
<li>JDK 7 can now be used without getting a INSTALL_PARSE_FAILED_NO_CERTIFICATES error with signed applications.</li>
<li>JNI marshaling null-strings from Java would cause the VM to abort.</li>
<li>The basic/pro license was not honored correctly in some places.</li>
<li>The saved instance state bundle passed to Activity.onCreate was not forwarded from the Proxy activity.</li>
<li>Update AndroidManifest.xml permissions when Application.internetReachability is used - adding ACCESS_NETWORK_STATE fixes the problem with incorrect return value.</li>
<li>Using a custom splash during an advanced license trial period could lead to runtime crashes when trial expired.</li>
<li>Using a Linux 3.x kernel would cause Unity to hang/crash on multi-core CPUs.</li>
<li>WWW calls to a server that redirects from HTTPS to HTTP were failing.</li>
<li>Nvidia's PerfHUD for Tegra reported increasing frame times when the application was paused.</li>
<li>A few hardware keys were missing, like (forward) DELETE and left/right CTRL - these have now been added.</li>
<li>Callbacks to MonoBehaviour.OnApplicationFocus is now supported.</li>
<li>Added support for Galaxy Note Stylus Pen (through KeyCode.LeftControl and KeyCode.Delete).</li>
<li>Fixed annoying but harmless error about missing directory when building.</li>
<li>Android Remote: fixed occasional stale touches.</li>
<li>Android Remote: fixed flickering and improved stability on tablets.</li>
</ul>

### Audio
<ul>
<li>'Decompress On Load'/'Compressed in memory' option not shown for uncompressed audio.</li>
<li>Don't show BPS for MPEG files.</li>
<li>Audio/Video: Pause audio when video is done in the inspector.</li>
<li>Fixed custom rolloff curves.</li>
<li>Fixed 32 bit filtering.</li>
<li>libVorbis updated to the latest version.</li>
<li>Lowpass filter inspector fixed.</li>
<li>Reset on filters and reverb zones now works.</li>
<li>Size in inspector now correct for all platforms and audio types.</li>
<li>Support for compression of 32bit input files.</li>
</ul>

### Debugger
<ul>
<li>Fixed abort with reentrant evaluation.</li>
<li>Fixed crash with nullable evaluation.</li>
<li>Fixed debugger crash when debugging in the editor.</li>
</ul>

### Editor
<ul>
<li>After moving or renaming the current open scene, saving will now save into the new location rather than the old.</li>
<li>Editor: Curve Editor now correctly reverts and resets any change when dragging and Esc is pressed.</li>
<li>Editor: Dark skin component checkboxes no longer twitch.</li>
<li>Editor: Dark skin's object picker tweaks.</li>
<li>ESC to cancel searching is more robust.</li>
<li>Editor: Fixed animated GUI groups breaking and giving errors after a window has been re-docked.</li>
<li>Fixed color picker incorrectly initializing alpha to 255 if original color is (0,0,0,0).</li>
<li>Editor: Fixed dragging textures to apply in Scene View sometimes showing errors and displaying progress bar that never closes.</li>
<li>Fixed Esc not clearing search field on Mac in Object Picker.</li>
<li>Fixed GameObject static dropdown not marking "Nothing" as selected when no flags were selected.</li>
<li>Fixed handling of unicode characters in scripts. Scripts should have utf-8 encoding.</li>
<li>Fixed many Handle controls not respecting Handles.matrix.</li>
<li>Fixed mouse cursor sometimes flickering garbage on Windows.</li>
<li>Fixed not being able to assign characters like ' , . / ` ] [ = as editor shortcuts on Windows.</li>
<li>Fixed null reference exception in project pane when displaying filtered results that return no hits and pressing up arrow key.</li>
<li>Fixed null reference exception when dragging sub-asset to the root of Project View.</li>
<li>Fixed Object Picker not focusing search field when being opened.</li>
<li>Fixed opening editor preferences when no inspector is open.</li>
<li>Fixed precision loss when viewing or editing large integers in the GUI.</li>
<li>Fixed repaint issue that made the Editor on Windows seem to have poor performance when mouse dragging gui components or scene view handles.</li>
<li>Fixed SceneView not resetting Handles.matrix if it was changed in an OnSceneGUI callback.</li>
<li>Fixed a bug where lists of enums were not editable in the inspector.</li>
<li>Fixed Animation View leaking materials when saving, while animation edit mode is active.</li>
<li>Editor: Fixed assert "vertexCount &gt; 60000" when using colliders with polygon count over 10000.</li>
<li>Fixed crash when resizing arrays in the inspector.</li>
<li>Fixed crash when trying to import mesh, which contains polygons, which have less than 3 vertices.</li>
<li>Fixed drop-down menus on Windows so they no longer overlap with the GUI control.</li>
<li>Fixed material import from COLLADA files.</li>
<li>Fixed memory problem when committing a lot of assets in the Asset Server window.</li>
<li>Fixed null ref when exporting a package.</li>
<li>Fixed out of memory crash when importing huge cube maps.</li>
<li>Fixed problem setting custom fields in webtemplates (they'd disappear as soon as focus left the field).</li>
<li>Fixed regression where import mode for normals and tangents on models where ignored, when upgrading from 3.4 to 3.5</li>
<li>Editor: Fixed reversing of triangle culling in some imported models (that used to happen in some very special cases).</li>
<li>Fixed some situations where the scene view mode could get stuck.</li>
<li>Fixed texture detection for imported materials when FBX contains mixed slashes in texture file paths.</li>
<li>Fixed Warning when saving a scene to a new folder created from the Save dialog.</li>
<li>Fixed terrain trees permanently being hidden when right clicking while left-dragging to paint height.</li>
<li>Fixed crash when closing Editor Window in OnFocus.</li>
<li>Fixed that Unity sometimes fails to recompile changed scripts or notice changed assets when leaving Unity while its unresponsive (Windows).</li>
<li>Focusing on a particle system will now respect the bounds of the system properly.</li>
<li>GetMiniThumbnail returns proper icons for DefaultAssets.</li>
<li>Icons for unknown asset types are now cached, prevents out-of-memory crash if there are a lot of unknown assets in a project.</li>
<li>Improved interaction with Visual Studio 2010.</li>
<li>Installer on Windows now has a large icon.</li>
<li>Made 3DS file loader more robust - Unity handles invalid files better now.</li>
<li>Make ProceduralTextureInspector and ProceduralMaterialInspector partially support multi-object editing (multi-editing procedural properties is not supported).</li>
<li>Make ProceduralTextureInspector repaint until not regenerating anymore.</li>
<li>Made sure EditorGUI controls respect indent level consistently and fixed some rarely used overloads that ignored some of the given parameters.</li>
<li>Multiple project windows don't share search string.</li>
<li>Got rid of white 1-px outlines on OSX Lion.</li>
<li>On OSX don't allow saving files with special characters in save file dialogs.</li>
<li>On OSX don't make "error" sounds when navigating object browser using keyboard.</li>
<li>On Windows, don't open new explorer window every time the player is build.</li>
<li>Resolve intermittent hangs.</li>
<li>Scene View controls no longer freezes when using left mouse button on scene view handles while right mouse button is pressed down.</li>
<li>Setting TextureImporter.textureType now sets all the required properties.</li>
<li>Use significantly less memory in most cases when generating a cubemap from a very high-resolution source image to make out-of-memory crashes less likely.</li>
<li>Windows Editor menus support Unicode characters.</li>
<li>You can now slide values with sliders by dragging the label (same as float fields).</li>
<li>(Windows) Build Settings will not open after Cancel.</li>
<li>(Windows) Asset progress bar &amp; build progress steals focus from other applications on windows.</li>
<li>Will now give a proper error when trying to import a movie with unsupported codecs.</li>
<li>Checked for scene camera rotation of NaN and fixed it.</li>
<li>Drastically reduce Scene View grid artifacts that caused it to be imprecise.</li>
<li>Fixed issue where editor would hang if left in background.</li>
<li>Child's scale is updated correctly when rotating with Inspector or Rotation Tool (when parent is non-uniformly scaled).</li>
<li>Deleting the root game object in OnPostProcessModel will no longer crash Unity.</li>
<li>Importing FBX models with bad texture references like "." and ".." no longer crashes Unity.</li>
<li>Upgrading a 3.4.x projects with Modo files will now retain ids for meshes, meaning that references to meshes are not lost. References to subgameobjects will still be lost.</li>
<li>(Windows) Fixed common random crash.</li>
<li>Fixed crash when calling SetActiveRecursively within Awake.</li>
<li>Fixed intermittent "Moving file failed" error when building player.</li>
<li>Fixed error when attempting to edit deleted terrain.</li>
<li>Advanced texture importer now correctly reflects internal texture import modes (For example no linear option for normal map textures).</li>
<li>Setting color preferences now has an instant effect on the editor.</li>
<li>Fixed that Unity does not refresh scripts when giving Unity focus by clicking on child windows.</li>
</ul>

### Graphics
<ul>
<li>Beast will no longer fail bakes on OSX if Unity installation path contains non-alphanumerical symbols.</li>
<li>Beast will no longer fail bakes on degenerate meshes, like bushes composed completely of billboarded leaves.</li>
<li>Compute correct tangents for non-uniformly scaled static meshes.</li>
<li>Enforce linear lighting status on hardware that does not support it.</li>
<li>Fixed broken values for builtin arrays when only 0th element was used (e.g. unity_LightPosition[0]).</li>
<li>Fixed issue related to deferred rendering when no lights are present and you are using HDR.</li>
<li>Fixed Particles/Alpha Blend shader turning black when in Fog.</li>
<li>Fixed pow() sometimes being mis-compiled for Direct3D 9.</li>
<li>Fixed Preview lighting on uniformly scaled meshes in GameObjects.</li>
<li>Fixed shadow caster culling for asymmetric view frustums.</li>
<li>Fixes and improvements to HLSL-&gt;GLSL translator and GLSL Optimizer.</li>
<li>Flares without a texture assigned don't crash the editor anymore.</li>
<li>Texture2D.Compress prints proper error message when texture is not marked as readable (previously was silently filling texture with garbage when not in editor).</li>
<li>Fixed incorrect rendering order when using transparent shader with ParticleRenderer and MeshRenderer.</li>
<li>Fixed error message when setting null texture on a GUITexture.</li>
<li>Fixed more than one directional light shadow (via "fullfowardshadows") not working in Forward rendering if Image Effects are used.</li>
<li>Tweaked RGBM lightmap encoding, so that there are no brighter lines appearing in dark areas when bilinear filtering is used. Makes a huge difference in linear lighting mode, since dark values get relatively much brighter.</li>
<li>Lightmapping: "Use in forward rend." is only respected in Dual Lightmaps mode as the GUI suggests.</li>
<li>Lightmapping: Fixed clearing lightmaps -- it resets lightmap index, tiling and offset on all renderers.</li>
<li>Lightmapping: Made light be culled below horizon for specular bounces when shadows are disabled. Fixes a case where a face pointing away from light would bounce light in that direction.</li>
<li>Lightmapping: Use alpha from the base texture (_MainTex) as the gloss map.</li>
<li>Lightmapping: Got rid of self-shadowing artifacts in small scenes placed far away from the origin (0,0,0).</li>
</ul>
