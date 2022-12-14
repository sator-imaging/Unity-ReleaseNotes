# Unity 4.5.5

https://unity3d.com/unity/whats-new/unity-4.5.5

## Fixes



*   Android: Android TV - Fixed uses-feature attribute in manifest that could require touchscreen.
*   Android: Fixed delay when resuming game from paused state.
*   Android: Fixed flickering screen on resume.
*   Android: Added missing implementation of UnityMemoryBarrier()
*   Android: Fixed crash on application resume on Adreno devices with Android 4.1.1 or 4.1.2.
*   Android: Preventing black frame to be displayed when on-screen keyboard appears/disappears.
*   Android: Export now works for projects that use UnityPlayerActivity or UnityPlayerProxyActivity.
*   Asset Import: Recompile scripts synchronously when the -buildTarget parameter is used.
*   Core: Fixed the "Failed to initialize unity graphics" error when using the -no-graphics flag in OS X
*   Direct3D 11: Unity will now correctly fall back to no MSAA depth textures if the GPU does not support ones with MSAA.
*   Documentation: Fixed rendering for richText.
*   Editor: Fixed word wrapping in the detail area of the console.
*   Editor: Handle an intermittent failure in CoCreateInstance during the Visual Studio launch process.
*   Editor: Open a script in the correct version of Visual Studio when the script is already open in a different version.
*   Editor: Fixed selected wireframe not rendered if object's shader has GrabPass as the first pass.
*   Editor: Use External Editor argument expansion in undocumented API.
*   Editor: Fixed an issue whereby dragging a prefab into hierarchy from project view was not selected automatically.
*   Editor: Don't pass out incorrect PropertyHandler on first call to GetHandler.
*   Flash : Empty project no longer has (harmless) errors in the log.
*   OpenGL ES 2: Fixed issues with native plugin called in OnPreRender .
*   Graphics: Send kGfxDeviceEventInitialize to native plugins if renderer changes.
*   Graphics: Fixed light culling with custom projection matrix.
*   Image Effects: Fixed Image filters targeting a render texture when a camera doesn't clear the color buffer.
*   Image Effects: Fixed Fast Bloom rendering upside down on Direct3D when anti-aliasing was used (reimport Image Effects package to get the fix).
*   iOS: Adaptively increase AOT build timeout to fix builds on large projects.
*   iOS: Do not run excessive number of mono AOT compiler instances.
*   iOS: Fixed Xcode 6 GM build & run support.
*   iOS: Fixed Xcode 6 GM Simulator support.
*   License: Give permissions to Users group on Windows to modify/write the license .ulf file, after Unity was activated by an administrator.
*   Linux: When using "Default is fullscreen" and "Default is native resolution" on a multidisplay system, store the resolution pref from the actual window size instead of the full desktop resolution.
*   Manual: Update documentation for player command line arguments.
*   Mecanim: Fixed trigger parameter consumption when used by multiple layers.
*   OSX: Now GameKit is loaded dynamically, it should help with Mac App Store submissions for games, which are not using Game Center.
*   OSX: Application.persistentDataPath changed from ~/Library/Caches/ to ~/Library/Application Support/
*   Physics: 'OnMouseDown' and 'OnMouseUp' callbacks for 3D physics now don't take priority over 2D physics, they can run simultaneously.
*   Physics: 'OnMouseDown' and 'OnMouseUp' callbacks for both 2D and 3D colliders now correctly use camera near/far plane distance.
*   Scripting: Properly validate class constraint on generics with reference type constraint.
*   Shaders: Fixed #include processing that are nested in #ifdef blocks in surface shaders.
*   Shaders: Fixed faceforward() for OpenGL platforms.
*   Shaders: VFACE pixel shader semantic translates more properly to OpenGL platforms now (values of -1 or 1, not 0 or 1 like before).
*   Substance: Fixed regression where valid runtime cache data would not be used and ProceduralTextures would be needlessly recomputed.
*   Substance: ProceduralTextures are no longer corrupted when switching color space in the editor.
*   Substance: ProceduralTextures are no longer corrupted when switching the masterTextureLimit in the editor.
*   Substance: Textures generated from a cloned ProceduralMaterial now have the proper alpha channel.
*   Terrain: Now tree imposter image will render in correct color space.
*   Version Control: Disallowing moving/renaming version controlled files that are changed/checked out remote.
*   WebCamTexture: Uses the first webcam device by default on all platforms.
*   WebPlayer: Fixed WebPlayer Loading failure when UNITY\_DISABLE\_PLUGIN\_UPDATES = yes.
*   Windows Phone 8.0: Fixed an issue which caused rendering from scripts not to work the same frame that back button was pressed on certain devices.
*   Windows Phone 8.0: Using image effects no longer distorts the image resolution.
*   Windows Phone 8.1: Fixed copying of 240% sized wide tile to final VS solution.
*   Windows Phone 8.1: TouchScreenKeyboard.visible no longer throws an exception if called before creating an actual keyboard.
*   Windows Phone 8.1: Unity no longer overrides 106x106 icon in final VS solution when a custom icon is placed there.
*   Windows Player: Fixed blank window appearing briefly before entering fullscreen mode.
*   Windows Store Apps: Fixed an issue which caused C# scripts to sometimes be included to wrong assemblies if "Debugging C# projects" checkbox was checked when building the project.
*   Windows Store Apps: C++ plugins are now correctly copied to output directory when using C++ project type.
*   Windows Store Apps: Unprocessed plugins are no longer included in Visual Studio pre-build event.
*   Windows Store Apps: Unity C# projects are referenced by project references instead of assembly references.
*   Windows Store Apps / Windows Phone: Fixed an issue which caused methods of WebHeaderCollection class throw exceptions
*   Windows Store Apps / Windows Phone 8.1: Fixed Screen.dpi to return physical screen DPI, instead of logical DPI.
*   Windows Store Apps / Windows Phone 8.1: Significantly reduces memory used by compressed audio.