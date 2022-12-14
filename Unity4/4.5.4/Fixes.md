# Unity 4.5.4

https://unity3d.com/unity/whats-new/unity-4.5.4

## Fixes



*   2D: Fixed sprite importing regression which caused sprite references to be lost on texture rename.
*   Android: Fixed application hanging and crashing when trying to close the IME with the back button.
*   Android: Fixed game starting not full screen if the orientation is not set to Auto Rotation.
*   Android: Fixed mouse input for interacting with standard GUI.
*   Asset Import: Fixed crash when plugin DLL calls AssetDatabase.Refresh in type initializer.
*   Editor & Webplayer: Fixed crash when loading some meshes imported with Unity 3.5.
*   Editor: Fixed "ArgumentException: Invalid path" error that might occur with some custom windows.
*   Editor: Fixed an issue whereby text went out of the TextArea in custom editor when return was pressed or multi line text was pasted.
*   Editor: Fixed Asset Store window showing up blank in DirectX 11 mode on some Intel graphics cards.
*   Editor: Fixed Hierarchy NullReferenceException happening when dragging an item over another item that is not a parent.
*   Editor: Fixed inspector rendering when having more than one missing script on a GameObject.
*   Editor: Fixed launch of Visual Studio for script editing, added additional logging to the editor log to troubleshoot future problems.
*   Editor: Fixed that a hidden Hierarchy window did not refresh when changing scenes.
*   Editor: Fixed that the icon for Alphabetical Sorting in the Hierarchy toolbar did not show when selected.
*   Editor: Fixed that when searching in the Hierarchy clicking on a search result item and then on "x" button did not reveal it.
*   Editor: Multiple events in the animation window can be dragged.
*   Editor: SpritePacker will not crash packing sprites generated from textures with certain OnPostprocessTexture scripts.
*   Editor/iOS: Large memory samples in profiler now work. Fix for the error "Buffer is not large enough for the message."
*   Graphics: Fixed Shader Material Keyword changes not applying to Materials on objects in the scene.
*   Graphics: Fixed skinned meshes sometimes not rendering in player builds when Read/Write Enabled import option is disabled.
*   Graphics: Fixed stencil modes only affecting front facing geometry when shader has Cull Off.
*   Graphics: Fixed textures in material property blocks (e.g. sprites) sometimes messing up other textures in the material on OpenGL.
*   Graphics: Fixed "allocation 0x00000000 already registered" error messages.
*   Graphics: Work around crash when trying to read invalid shader properties.
*   IMGUI: OnMouseExit not called when mouse is moved from a collider to IMGUI element that is occluding it.
*   iOS: Fixed crash occurring when using webcam texture whilst privacy settings deny access to the camera.
*   iOS: Fixed handling of resolution preset in Player Settings.
*   iOS: Fixed startup orientation handling on iOS 8.
*   iOS: Support files with multiple fonts when building font metadata.
*   iOS: Update and render additional frame after app suspension. Allows customising paused app's thumbnail.
*   Linux: Fixed text entry when pressing enter/return.
*   Mac OS X: Fixed a bug where certain third party mice would cause the editor or players to take a very long time to start up.
*   Mac OS X: Fixed full screen rendering at less than native resolution.
*   Mac OS X: Fixed duplicate input events being sent in OS X standalone player.
*   Mecanim: Fixed crash when opening a project with Free License where Animator Layer Sync has been turned on by a Pro License user.
*   Mecanim: Fixed bug where Animator.StartRecording would prevent Animator.Play from playing animations.
*   OpenGL ES2: Fixed shader depth state handling.
*   Physics 2D: 2D colliders marked as triggers now don't affect center of mass or inertia calculations.
*   Physics 2D: Allow the change of Z transform position only, without disturbing Rigidbody2D interpolation.
*   Physics 2D: Rigidbody2D without colliders now has default inertia and center of gravity.
*   Physics 2D: Stop memory leak when assigning vertex array to PolygonCollider2D.points with invalid geometry.
*   Scripting: Fixed ARM thunk creation in dynamic methods on AOT platforms.
*   Scripting: Fixed occasional crash when switching between scenes.
*   Scripting: Fixed potential crashes during breakpoint and single stepping in debugger.
*   Scripting: Fixed the debugger causing waits to be interrupted.
*   Shaders: VFACE pixel shader input semantic works now. Previously was not quite working on D3D9.
*   Substance: Fixed crash when loading a scene with an object that has a script with a ProceduralMaterial assigned to a Material property.
*   Windows Phone 8.0: Fixed an issue which caused shader depth bias being applied to the wrong direction on old WP 8.0 OS builds.
*   Windows Phone 8.0: Unity no longer prevents build even if it finds code that will potentially crash during runtime.
*   Windows Phone 8.1: Fixed Unity player not pausing when a phone call is incoming.
*   Windows Phone 8.1: Input.inputString now works properly.
*   Windows Phone: Fixed crash on application exit when location was enabled.
*   Windows Phone: Unity no longer generates empty files that cause XAP deployment failures.
*   Windows Store / Phone: Fixed an issue which caused Unity player to crash sometimes when loading a DLL not built for WinRT.
*   Windows Store / Phone: Unity will produce full PDB files for scripts even in non-development builds.
*   Windows Store Apps: Fixed exceptions which occur when trying to use reflection.