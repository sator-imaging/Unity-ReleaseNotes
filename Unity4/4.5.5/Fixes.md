# Unity 4.5.5
https://unity3d.com/unity/whats-new/unity-4.5.5

## Fixes

<ul>
<li>Android: Android TV - Fixed uses-feature attribute in manifest that could require touchscreen.</li>
<li>Android: Fixed delay when resuming game from paused state.</li>
<li>Android: Fixed flickering screen on resume.</li>
<li>Android: Added missing implementation of UnityMemoryBarrier()</li>
<li>Android: Fixed crash on application resume on Adreno devices with Android 4.1.1 or 4.1.2.</li>
<li>Android: Preventing black frame to be displayed when on-screen keyboard appears/disappears.</li>
<li>Android: Export now works for projects that use UnityPlayerActivity or UnityPlayerProxyActivity.</li>
<li>Asset Import: Recompile scripts synchronously when the -buildTarget parameter is used.</li>
<li>Core: Fixed the "Failed to initialize unity graphics" error when using the -no-graphics flag in OS X</li>
<li>Direct3D 11: Unity will now correctly fall back to no MSAA depth textures if the GPU does not support ones with MSAA.</li>
<li>Documentation: Fixed rendering for richText.</li>
<li>Editor: Fixed word wrapping in the detail area of the console.</li>
<li>Editor: Handle an intermittent failure in CoCreateInstance during the Visual Studio launch process.</li>
<li>Editor: Open a script in the correct version of Visual Studio when the script is already open in a different version.</li>
<li>Editor: Fixed selected wireframe not rendered if object's shader has GrabPass as the first pass.</li>
<li>Editor: Use External Editor argument expansion in undocumented API.</li>
<li>Editor: Fixed an issue whereby dragging a prefab into hierarchy from project view was not selected automatically.</li>
<li>Editor: Don't pass out incorrect PropertyHandler on first call to GetHandler.</li>
<li>Flash : Empty project no longer has (harmless) errors in the log.</li>
<li>OpenGL ES 2: Fixed issues with native plugin called in OnPreRender .</li>
<li>Graphics: Send kGfxDeviceEventInitialize to native plugins if renderer changes.</li>
<li>Graphics: Fixed light culling with custom projection matrix.</li>
<li>Image Effects: Fixed Image filters targeting a render texture when a camera doesn't clear the color buffer.</li>
<li>Image Effects: Fixed Fast Bloom rendering upside down on Direct3D when anti-aliasing was used (reimport Image Effects package to get the fix).</li>
<li>iOS: Adaptively increase AOT build timeout to fix builds on large projects.</li>
<li>iOS: Do not run excessive number of mono AOT compiler instances.</li>
<li>iOS: Fixed Xcode 6 GM build &amp; run support.</li>
<li>iOS: Fixed Xcode 6 GM Simulator support.</li>
<li>License: Give permissions to Users group on Windows to modify/write the license .ulf file, after Unity was activated by an administrator.</li>
<li>Linux: When using "Default is fullscreen" and "Default is native resolution" on a multidisplay system, store the resolution pref from the actual window size instead of the full desktop resolution.</li>
<li>Manual: Update documentation for player command line arguments.</li>
<li>Mecanim: Fixed trigger parameter consumption when used by multiple layers.</li>
<li>OSX: Now GameKit is loaded dynamically, it should help with Mac App Store submissions for games, which are not using Game Center.</li>
<li>OSX: Application.persistentDataPath changed from ~/Library/Caches/ to ~/Library/Application Support/</li>
<li>Physics: 'OnMouseDown' and 'OnMouseUp' callbacks for 3D physics now don't take priority over 2D physics, they can run simultaneously.</li>
<li>Physics: 'OnMouseDown' and 'OnMouseUp' callbacks for both 2D and 3D colliders now correctly use camera near/far plane distance.</li>
<li>Scripting: Properly validate class constraint on generics with reference type constraint.</li>
<li>Shaders: Fixed #include processing that are nested in #ifdef blocks in surface shaders.</li>
<li>Shaders: Fixed faceforward() for OpenGL platforms.</li>
<li>Shaders: VFACE pixel shader semantic translates more properly to OpenGL platforms now (values of -1 or 1, not 0 or 1 like before).</li>
<li>Substance: Fixed regression where valid runtime cache data would not be used and ProceduralTextures would be needlessly recomputed.</li>
<li>Substance: ProceduralTextures are no longer corrupted when switching color space in the editor.</li>
<li>Substance: ProceduralTextures are no longer corrupted when switching the masterTextureLimit in the editor.</li>
<li>Substance: Textures generated from a cloned ProceduralMaterial now have the proper alpha channel.</li>
<li>Terrain: Now tree imposter image will render in correct color space.</li>
<li>Version Control: Disallowing moving/renaming version controlled files that are changed/checked out remote.</li>
<li>WebCamTexture: Uses the first webcam device by default on all platforms.</li>
<li>WebPlayer: Fixed WebPlayer Loading failure when UNITY_DISABLE_PLUGIN_UPDATES = yes.</li>
<li>Windows Phone 8.0: Fixed an issue which caused rendering from scripts not to work the same frame that back button was pressed on certain devices.</li>
<li>Windows Phone 8.0: Using image effects no longer distorts the image resolution.</li>
<li>Windows Phone 8.1: Fixed copying of 240% sized wide tile to final VS solution.</li>
<li>Windows Phone 8.1: TouchScreenKeyboard.visible no longer throws an exception if called before creating an actual keyboard.</li>
<li>Windows Phone 8.1: Unity no longer overrides 106x106 icon in final VS solution when a custom icon is placed there.</li>
<li>Windows Player: Fixed blank window appearing briefly before entering fullscreen mode.</li>
<li>Windows Store Apps: Fixed an issue which caused C# scripts to sometimes be included to wrong assemblies if "Debugging C# projects" checkbox was checked when building the project.</li>
<li>Windows Store Apps: C++ plugins are now correctly copied to output directory when using C++ project type.</li>
<li>Windows Store Apps: Unprocessed plugins are no longer included in Visual Studio pre-build event.</li>
<li>Windows Store Apps: Unity C# projects are referenced by project references instead of assembly references.</li>
<li>Windows Store Apps / Windows Phone: Fixed an issue which caused methods of WebHeaderCollection class throw exceptions</li>
<li>Windows Store Apps / Windows Phone 8.1: Fixed Screen.dpi to return physical screen DPI, instead of logical DPI.</li>
<li>Windows Store Apps / Windows Phone 8.1: Significantly reduces memory used by compressed audio.</li>
</ul>
