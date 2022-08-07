# Unity 3.4
https://unity3d.com/unity/whats-new/unity-3.4

## Editor


### Improvements
<ul>
<li>You can now drag any GameObject into the project view to create a prefab with minimal hassle.</li>
<li>Faster Play/Stop times on scenes with many prefabs.</li>
<li>The Object Picker can now show individual previews for sub-assets, such as the individual meshes in a model asset.</li>
<li>MonoDevelop is now the default script editor.</li>
<li>Optimized PVRTC decompressor; scenes/textures will load much faster when in iOS mode.</li>
<li>Launch VS using the C#-only solution by default.</li>
<li>Primitive Collider handles are now only shown when pressing Shift.</li>
<li>Show recommended shader help text in Material Inspector.</li>
<li>Implemented field for editing Bounds in the inspector.</li>
<li>Implemented editing of Bounds for Animation and SkinnedMeshRenderer components in the Inspector and Scene view.</li>
<li>Improved VisualStudio/MonoDevelop solution synchronization performance.</li>
<li>Added depth buffer bits field to RenderTexture inspector.</li>
<li>GenericMenu has been documented and should be used for custom context menus.</li>
<li>Tools class have been exposed so you can better make custom editors.</li>
</ul>

### Fixes
<ul>
<li>Moving and deleting keyframes from the timeline now works with undo.</li>
<li>Trail Renderers now always have the handle placed at the origin so they don't jump around as the game object is dragged in the scene view.</li>
<li>Surface snapping now correctly ignores colliders that are set to triggers.</li>
<li>Vertex snapping of objects dragged into sceneview now works.</li>
<li>Vertex snapping of sub-objects fixed.</li>
<li>Painting terrain heights and dragging outside the sceneview no longer leaves the terrain in a weird state.</li>
<li>Light inspector now correctly hides soft shadow options when they don't apply to the light.</li>
<li>Camera gizmo and preview is now based on Game View aspect ratio instead of Scene View aspect ratio.</li>
<li>On Windows right mouse clicking the Game View tab now shows the context menu.</li>
<li>Closing tabs with middle mouse button is now closes the correct tab.</li>
<li>Cursor is no longer allowed to be locked when pausing before pressing play i.e. the cursor is forced visible (same behavior as when pressing pause during play).</li>
<li>Maximize on Play no longer cancels Screen.lockCursor.</li>
<li>When loading a project the directory structure is now validated.</li>
<li>Improved progress indication during building to other platforms.</li>
<li>Uninstalling editor will now clean up the install folder correctly.</li>
<li>Toggling pro skin no longer resets the script editor.</li>
<li>Lightcookie textures are no longer marked as dirty during rendering (case 389444).</li>
<li>The material preview pane now updates when the shader used by the material is recompiled.</li>
<li>Animation View: Fix issue with different properties sometimes inappropriately sharing the same curve state.</li>
<li>Fixed crash when importing an empty shader file.</li>
<li>Pass the solution file and line numbers to the default MonoDevelop installation.</li>
<li>Fixed problem executing the PostprocessBuildPlayer script on Macs when executable bit was not set.</li>
<li>Fixed crash when dragging a Prefab into Scene View.</li>
<li>Fixed Input.mousePosition reporting wrong coordinates after a pause and lost focus of Unity Editor.</li>
<li>Asset Server now detects changes to script icons.</li>
<li>Removed .asset extension from AnnotationManager.asset in the Library folder.</li>
<li>Fix cropping of TextAsset.bytes when data contains leading null values</li>
<li>Fixed a crash bug when deleting keyframes in the Animation view.</li>
<li>Improved synchronisation of Visual Studio projects.</li>
<li>Fixed Material Inspector sometimes displaying a wrong name for a shader.</li>
<li>Yield on WaitForEndOfFrame works in batch mode.</li>
<li>Fixed NullRef in AudioSource/LPF Curve inspector.</li>
<li>Mac Editor: fixed memory error message in console when using the color picker.</li>
<li>Mac Editor: fixed crash on Mac OS X 10.7 Lion when using the color picker.</li>
<li>Fixed indentation issues in Vector3, Vector4 and Rect fields.</li>
<li>Project/Hierarchy search field no longer eats first character if it had all text selected in some cases.</li>
<li>Fixed debug logs not getting cleared with Clear On Play enabled when logs were created in edit mode.</li>
<li>Fixed some fixed function shaders not displaying correctly in OpenGL ES 1.1 emulation (on Windows).</li>
<li>Disabled colliders now use a dimmed color for their gizmos.</li>
<li>It is now possible to close a maximized EditorWindow from script.</li>
<li>Do not allow to select target iOS version lower than 3.1.3 if iPad or iPad + iPhone device target is selected in player settings.</li>
<li>Texture2D.PackTextures force padding on right and tops of each texture element.</li>
<li>Do not upgrade a 2.6 project twice in cases when scripts would have to be patched during the upgrade.</li>
<li>When generating unique asset paths, don't add a space before the number if the asset is a script.</li>
<li>When a corrupted scene with invalid prefabs is detected they will now be cleaned up when saving the scene.</li>
<li>Fixed various issues with Image Effects when switching platforms or graphics emulation settings.</li>
<li>Fixed regression when renaming assets causing them to be reimported when quiting. Assets are now reimported immediately after renaming (case 409155).</li>
<li>Fixed a rare bug where complex chains of shaders with fallbacks are treated as unsupported when switching platforms in the editor.</li>
<li>Added Tooltip to the GameObject class.</li>
<li>Fix crash when switching target to Wii or Xbox in the Build Settings menu.</li>
<li>Fix crash when debugging and evaluating an expression that triggers a null reference exception.</li>
<li>Fix intermittent exceptions when launching Visual Studio.</li>
<li>Scene view icons are no longer affected by editor quality settings (blurred at low quality).</li>
</ul>
