# Unity 4.5.3
https://unity3d.com/unity/whats-new/unity-4.5.3

## Fixes

<ul>
<li>2D: Reduced Sprite Packer memory requirements.</li>
<li>2D: Sprite Packer will write atlases to cache earlier in the packing process. Now they can be recovered after cancelling packing or in case of a crash.</li>
<li>2D: Sprite.packed will return the correct value if a packed sprite is loaded from an asset bundle in the editor.</li>
<li>2D: Fixed vertex snapping of sprites with non-default pivots.</li>
<li>2D: SpriteEditor will not throw exceptions when a cubemap/reflection texture is selected.</li>
<li>Android: Fixed ANR when the application is paused with an active touch.</li>
<li>Android: Fixed OnApplicationFocus event.</li>
<li>Android: Fixed possible crash when calling Application.Quit in OnApplicationPause().</li>
<li>Animation: Fixed an issue whereby playing a full-body additive animation caused the character to slide around the scene wildly.</li>
<li>Animation: Fixed crash when previewing a transition.</li>
<li>Animation: Fixed getting invalid rotation when animating some specific transform hierarchy.</li>
<li>Audio: Fix for audio streaming from WWW objects.</li>
<li>Editor: Fixed freeze on printing long strings to console log (limited single entry length to 16k characters).</li>
<li>Editor: Pressing the down arrow in the hierarchy window's search box now immediately jumps to first result.</li>
<li>Editor: Fixed regression of importing scripts when running editor in batch mode.</li>
<li>Editor: Spawned child processes will no longer inherit files opened by the Editor on Windows. Fixes issues with VCS or shader compiler processes holding locks to files.</li>
<li>iOS: Correctly receive input events when VoiceOver is enabled.</li>
<li>iOS: Enabled 1080p WebCamTexture.</li>
<li>iOS: Fixed script AOT compiler memory leak while compiling generic classes.</li>
<li>iOS: Fixed script AOT compiler out of memory crash.</li>
<li>iOS: Fixed Handheld.PlayFullScreenMovie on iOS8.</li>
<li>iOS: Fixed touch coordinates being wrong under interface rotation.</li>
<li>iOS: Warn Pro users about missing splash screen images in release builds.</li>
<li>iOS: Fixed app home directory that now points to the permitted path of Documents.</li>
<li>iOS: Added support for files with multiple fonts when building dynamic font metadata cache.</li>
<li>iOS: Combined splash screen warnings into one.</li>
<li>iOS: Added Xcode 6 "Build and Run" support.</li>
<li>iOS: Made non-readable meshes to take less memory.</li>
<li>iOS: Fixed Video Playback issues in case of plugging/unplugging headphones.</li>
<li>Mobile Rendering: Fixed multi-threaded rendering issues with picking wrong format for RenderTextures used in Image Effects.</li>
<li>Mobile Rendering: Fixed native rendering plugins in OnPreRender breaking rendering.</li>
<li>Mobile Rendering: Fixed multi-threaded rendering issues with dynamic meshes on OpenGL ES 2.0.</li>
<li>Mobile Rendering: Fixed image effects in case of MSAA on OpenGL ES 3.0.</li>
<li>Networking: Fixed a leak of 256k per WWW instance, when loading uncompressed AssetBundles from disk.</li>
<li>Physics 2D: Added ability to select whether deleting a 2D collider or rigid body during a collision callback stops remaining callbacks or not.</li>
<li>Physics 2D: Fixed regression where 2D colliders didn't update when animated.</li>
<li>Physics 2D: Fixed crash when Rigidbody2D component is destroyed during contact callback.</li>
<li>Physics 2D: Ensure that the lower/upper translation limits on JointTranslationLimit2D are correct with respect to each other (used on SliderJoint2D).</li>
<li>Physics 2D: Stop interpolation/extrapolation from being halted during next physics update when a new Rigidbody2D is added.</li>
<li>Shaders: Fixed more cases of errors in shaders not being reported on correct line numbers (for GLSL platforms).</li>
<li>Shaders: Fixed wrong HLSL-to-GLSL translation of clip() with a vector argument.</li>
<li>Shuriken: Fix for re-enabled particle system which was disabled before it has finished.</li>
<li>Substance: Normal maps are correctly displayed now in the Editor when targeting GL platforms.</li>
<li>Substance: Thumbnails for normal maps are now generated correctly instead of being displayed in grayscale.</li>
<li>Substance: Fixed crash when baking a ProceduralTexture without mipmaps to a compressed format.</li>
<li>Substance: Fixed ProceduralMaterials looking black after disabling the ProceduralMaterialInspector.</li>
<li>Version Control: Adding files in perforce would escape special characters such as '@' into '%40'. This issue has been fixed.</li>
<li>Windows Phone: Fixed an issue which caused serialization weaver to crash sometimes when processing methods that return IEnumerable.</li>
<li>Windows Phone: Winmd plugins are now correctly handled.</li>
<li>Windows Phone: Editor reports if arrays with generic element types that can cause crash at runtime are used.</li>
<li>Windows Phone / Store: Enum.ToObject now works with all primitive types.</li>
<li>Windows Phone / Store: Methods returning boolean values are now correctly handled.</li>
<li>Windows Phone / Store: Plugins that are signed with strong name now work properly.</li>
<li>Windows Phone / Store: When compiling JS/Boo files, debugging information will be added only when Development checkbox is on, previous behavior was debugging information was always being added.</li>
<li>Windows Phone / Store: Fixed an issue which caused private members are not initialized in serializable class.</li>
<li>Windows Phone / Store: Structs are always serialized correctly.</li>
<li>Windows Player: Fixed Alt-Tab in DirectX 11 full-screen mode freezing the application.</li>
<li>Windows Player: Run in Background now works properly in DirectX 9 fullscreen mode.</li>
<li>Windows Player: Performance improvements including lower latency in DirectX 11 mode.</li>
<li>Windows Player: The default full-screen mode no longer changes the desktop resolution, so things like IME text input work.</li>
<li>Windows Player: Hint to NVIDIA driver that it should use the discrete GPU in Optimus chipsets.</li>
<li>Windows Store Apps: Added support for TouchScreenKeyboard.text property.</li>
<li>Windows Store Apps: Portable class libraries can now successful use methods like Type.GetFields or Type.GetProperties.</li>
<li>Windows Store Apps: Show keyboard when TouchScreenKeyboard.Open() is called, no need to manually set active to true.</li>
<li>Windows Store Apps: Added support for key modifiers in GUI events.</li>
<li>Windows Store Apps: Fixed the return value of SystemInfo.supportsLocationService.</li>
</ul>
