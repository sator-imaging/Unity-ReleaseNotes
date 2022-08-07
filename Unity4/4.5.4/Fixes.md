# Unity 4.5.4
https://unity3d.com/unity/whats-new/unity-4.5.4

## Fixes

<ul>
<li>2D: Fixed sprite importing regression which caused sprite references to be lost on texture rename.</li>
<li>Android: Fixed application hanging and crashing when trying to close the IME with the back button.</li>
<li>Android: Fixed game starting not full screen if the orientation is not set to Auto Rotation.</li>
<li>Android: Fixed mouse input for interacting with standard GUI.</li>
<li>Asset Import: Fixed crash when plugin DLL calls AssetDatabase.Refresh in type initializer.</li>
<li>Editor &amp; Webplayer: Fixed crash when loading some meshes imported with Unity 3.5.</li>
<li>Editor: Fixed "ArgumentException: Invalid path" error that might occur with some custom windows.</li>
<li>Editor: Fixed an issue whereby text went out of the TextArea in custom editor when return was pressed or multi line text was pasted.</li>
<li>Editor: Fixed Asset Store window showing up blank in DirectX 11 mode on some Intel graphics cards.</li>
<li>Editor: Fixed Hierarchy NullReferenceException happening when dragging an item over another item that is not a parent.</li>
<li>Editor: Fixed inspector rendering when having more than one missing script on a GameObject.</li>
<li>Editor: Fixed launch of Visual Studio for script editing, added additional logging to the editor log to troubleshoot future problems.</li>
<li>Editor: Fixed that a hidden Hierarchy window did not refresh when changing scenes.</li>
<li>Editor: Fixed that the icon for Alphabetical Sorting in the Hierarchy toolbar did not show when selected.</li>
<li>Editor: Fixed that when searching in the Hierarchy clicking on a search result item and then on "x" button did not reveal it.</li>
<li>Editor: Multiple events in the animation window can be dragged.</li>
<li>Editor: SpritePacker will not crash packing sprites generated from textures with certain OnPostprocessTexture scripts.</li>
<li>Editor/iOS: Large memory samples in profiler now work. Fix for the error "Buffer is not large enough for the message."</li>
<li>Graphics: Fixed Shader Material Keyword changes not applying to Materials on objects in the scene.</li>
<li>Graphics: Fixed skinned meshes sometimes not rendering in player builds when Read/Write Enabled import option is disabled.</li>
<li>Graphics: Fixed stencil modes only affecting front facing geometry when shader has Cull Off.</li>
<li>Graphics: Fixed textures in material property blocks (e.g. sprites) sometimes messing up other textures in the material on OpenGL.</li>
<li>Graphics: Fixed "allocation 0x00000000 already registered" error messages.</li>
<li>Graphics: Work around crash when trying to read invalid shader properties.</li>
<li>IMGUI: OnMouseExit not called when mouse is moved from a collider to IMGUI element that is occluding it.</li>
<li>iOS: Fixed crash occurring when using webcam texture whilst privacy settings deny access to the camera.</li>
<li>iOS: Fixed handling of resolution preset in Player Settings.</li>
<li>iOS: Fixed startup orientation handling on iOS 8.</li>
<li>iOS: Support files with multiple fonts when building font metadata.</li>
<li>iOS: Update and render additional frame after app suspension. Allows customising paused app's thumbnail.</li>
<li>Linux: Fixed text entry when pressing enter/return.</li>
<li>Mac OS X: Fixed a bug where certain third party mice would cause the editor or players to take a very long time to start up.</li>
<li>Mac OS X: Fixed full screen rendering at less than native resolution.</li>
<li>Mac OS X: Fixed duplicate input events being sent in OS X standalone player.</li>
<li>Mecanim: Fixed crash when opening a project with Free License where Animator Layer Sync has been turned on by a Pro License user.</li>
<li>Mecanim: Fixed bug where Animator.StartRecording would prevent Animator.Play from playing animations.</li>
<li>OpenGL ES2: Fixed shader depth state handling.</li>
<li>Physics 2D: 2D colliders marked as triggers now don't affect center of mass or inertia calculations.</li>
<li>Physics 2D: Allow the change of Z transform position only, without disturbing Rigidbody2D interpolation.</li>
<li>Physics 2D: Rigidbody2D without colliders now has default inertia and center of gravity.</li>
<li>Physics 2D: Stop memory leak when assigning vertex array to PolygonCollider2D.points with invalid geometry.</li>
<li>Scripting: Fixed ARM thunk creation in dynamic methods on AOT platforms.</li>
<li>Scripting: Fixed occasional crash when switching between scenes.</li>
<li>Scripting: Fixed potential crashes during breakpoint and single stepping in debugger.</li>
<li>Scripting: Fixed the debugger causing waits to be interrupted.</li>
<li>Shaders: VFACE pixel shader input semantic works now. Previously was not quite working on D3D9.</li>
<li>Substance: Fixed crash when loading a scene with an object that has a script with a ProceduralMaterial assigned to a Material property.</li>
<li>Windows Phone 8.0: Fixed an issue which caused shader depth bias being applied to the wrong direction on old WP 8.0 OS builds.</li>
<li>Windows Phone 8.0: Unity no longer prevents build even if it finds code that will potentially crash during runtime.</li>
<li>Windows Phone 8.1: Fixed Unity player not pausing when a phone call is incoming.</li>
<li>Windows Phone 8.1: Input.inputString now works properly.</li>
<li>Windows Phone: Fixed crash on application exit when location was enabled.</li>
<li>Windows Phone: Unity no longer generates empty files that cause XAP deployment failures.</li>
<li>Windows Store / Phone: Fixed an issue which caused Unity player to crash sometimes when loading a DLL not built for WinRT.</li>
<li>Windows Store / Phone: Unity will produce full PDB files for scripts even in non-development builds.</li>
<li>Windows Store Apps: Fixed exceptions which occur when trying to use reflection.</li>
</ul>
