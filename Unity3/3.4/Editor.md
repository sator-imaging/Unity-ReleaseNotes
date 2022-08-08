# Unity 3.4

https://unity3d.com/unity/whats-new/unity-3.4

## Editor

- [Improvements](#improvements)
- [Fixes](#fixes)


### Improvements

*   You can now drag any GameObject into the project view to create a prefab with minimal hassle.
*   Faster Play/Stop times on scenes with many prefabs.
*   The Object Picker can now show individual previews for sub-assets, such as the individual meshes in a model asset.
*   MonoDevelop is now the default script editor.
*   Optimized PVRTC decompressor; scenes/textures will load much faster when in iOS mode.
*   Launch VS using the C#-only solution by default.
*   Primitive Collider handles are now only shown when pressing Shift.
*   Show recommended shader help text in Material Inspector.
*   Implemented field for editing Bounds in the inspector.
*   Implemented editing of Bounds for Animation and SkinnedMeshRenderer components in the Inspector and Scene view.
*   Improved VisualStudio/MonoDevelop solution synchronization performance.
*   Added depth buffer bits field to RenderTexture inspector.
*   GenericMenu has been documented and should be used for custom context menus.
*   Tools class have been exposed so you can better make custom editors.

### Fixes

*   Moving and deleting keyframes from the timeline now works with undo.
*   Trail Renderers now always have the handle placed at the origin so they don't jump around as the game object is dragged in the scene view.
*   Surface snapping now correctly ignores colliders that are set to triggers.
*   Vertex snapping of objects dragged into sceneview now works.
*   Vertex snapping of sub-objects fixed.
*   Painting terrain heights and dragging outside the sceneview no longer leaves the terrain in a weird state.
*   Light inspector now correctly hides soft shadow options when they don't apply to the light.
*   Camera gizmo and preview is now based on Game View aspect ratio instead of Scene View aspect ratio.
*   On Windows right mouse clicking the Game View tab now shows the context menu.
*   Closing tabs with middle mouse button is now closes the correct tab.
*   Cursor is no longer allowed to be locked when pausing before pressing play i.e. the cursor is forced visible (same behavior as when pressing pause during play).
*   Maximize on Play no longer cancels Screen.lockCursor.
*   When loading a project the directory structure is now validated.
*   Improved progress indication during building to other platforms.
*   Uninstalling editor will now clean up the install folder correctly.
*   Toggling pro skin no longer resets the script editor.
*   Lightcookie textures are no longer marked as dirty during rendering (case 389444).
*   The material preview pane now updates when the shader used by the material is recompiled.
*   Animation View: Fix issue with different properties sometimes inappropriately sharing the same curve state.
*   Fixed crash when importing an empty shader file.
*   Pass the solution file and line numbers to the default MonoDevelop installation.
*   Fixed problem executing the PostprocessBuildPlayer script on Macs when executable bit was not set.
*   Fixed crash when dragging a Prefab into Scene View.
*   Fixed Input.mousePosition reporting wrong coordinates after a pause and lost focus of Unity Editor.
*   Asset Server now detects changes to script icons.
*   Removed .asset extension from AnnotationManager.asset in the Library folder.
*   Fix cropping of TextAsset.bytes when data contains leading null values
*   Fixed a crash bug when deleting keyframes in the Animation view.
*   Improved synchronisation of Visual Studio projects.
*   Fixed Material Inspector sometimes displaying a wrong name for a shader.
*   Yield on WaitForEndOfFrame works in batch mode.
*   Fixed NullRef in AudioSource/LPF Curve inspector.
*   Mac Editor: fixed memory error message in console when using the color picker.
*   Mac Editor: fixed crash on Mac OS X 10.7 Lion when using the color picker.
*   Fixed indentation issues in Vector3, Vector4 and Rect fields.
*   Project/Hierarchy search field no longer eats first character if it had all text selected in some cases.
*   Fixed debug logs not getting cleared with Clear On Play enabled when logs were created in edit mode.
*   Fixed some fixed function shaders not displaying correctly in OpenGL ES 1.1 emulation (on Windows).
*   Disabled colliders now use a dimmed color for their gizmos.
*   It is now possible to close a maximized EditorWindow from script.
*   Do not allow to select target iOS version lower than 3.1.3 if iPad or iPad + iPhone device target is selected in player settings.
*   Texture2D.PackTextures force padding on right and tops of each texture element.
*   Do not upgrade a 2.6 project twice in cases when scripts would have to be patched during the upgrade.
*   When generating unique asset paths, don't add a space before the number if the asset is a script.
*   When a corrupted scene with invalid prefabs is detected they will now be cleaned up when saving the scene.
*   Fixed various issues with Image Effects when switching platforms or graphics emulation settings.
*   Fixed regression when renaming assets causing them to be reimported when quiting. Assets are now reimported immediately after renaming (case 409155).
*   Fixed a rare bug where complex chains of shaders with fallbacks are treated as unsupported when switching platforms in the editor.
*   Added Tooltip to the GameObject class.
*   Fix crash when switching target to Wii or Xbox in the Build Settings menu.
*   Fix crash when debugging and evaluating an expression that triggers a null reference exception.
*   Fix intermittent exceptions when launching Visual Studio.
*   Scene view icons are no longer affected by editor quality settings (blurred at low quality).