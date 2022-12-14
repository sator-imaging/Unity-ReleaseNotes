# Unity 4.5.3

https://unity3d.com/unity/whats-new/unity-4.5.3

## Fixes



*   2D: Reduced Sprite Packer memory requirements.
*   2D: Sprite Packer will write atlases to cache earlier in the packing process. Now they can be recovered after cancelling packing or in case of a crash.
*   2D: Sprite.packed will return the correct value if a packed sprite is loaded from an asset bundle in the editor.
*   2D: Fixed vertex snapping of sprites with non-default pivots.
*   2D: SpriteEditor will not throw exceptions when a cubemap/reflection texture is selected.
*   Android: Fixed ANR when the application is paused with an active touch.
*   Android: Fixed OnApplicationFocus event.
*   Android: Fixed possible crash when calling Application.Quit in OnApplicationPause().
*   Animation: Fixed an issue whereby playing a full-body additive animation caused the character to slide around the scene wildly.
*   Animation: Fixed crash when previewing a transition.
*   Animation: Fixed getting invalid rotation when animating some specific transform hierarchy.
*   Audio: Fix for audio streaming from WWW objects.
*   Editor: Fixed freeze on printing long strings to console log (limited single entry length to 16k characters).
*   Editor: Pressing the down arrow in the hierarchy window's search box now immediately jumps to first result.
*   Editor: Fixed regression of importing scripts when running editor in batch mode.
*   Editor: Spawned child processes will no longer inherit files opened by the Editor on Windows. Fixes issues with VCS or shader compiler processes holding locks to files.
*   iOS: Correctly receive input events when VoiceOver is enabled.
*   iOS: Enabled 1080p WebCamTexture.
*   iOS: Fixed script AOT compiler memory leak while compiling generic classes.
*   iOS: Fixed script AOT compiler out of memory crash.
*   iOS: Fixed Handheld.PlayFullScreenMovie on iOS8.
*   iOS: Fixed touch coordinates being wrong under interface rotation.
*   iOS: Warn Pro users about missing splash screen images in release builds.
*   iOS: Fixed app home directory that now points to the permitted path of Documents.
*   iOS: Added support for files with multiple fonts when building dynamic font metadata cache.
*   iOS: Combined splash screen warnings into one.
*   iOS: Added Xcode 6 "Build and Run" support.
*   iOS: Made non-readable meshes to take less memory.
*   iOS: Fixed Video Playback issues in case of plugging/unplugging headphones.
*   Mobile Rendering: Fixed multi-threaded rendering issues with picking wrong format for RenderTextures used in Image Effects.
*   Mobile Rendering: Fixed native rendering plugins in OnPreRender breaking rendering.
*   Mobile Rendering: Fixed multi-threaded rendering issues with dynamic meshes on OpenGL ES 2.0.
*   Mobile Rendering: Fixed image effects in case of MSAA on OpenGL ES 3.0.
*   Networking: Fixed a leak of 256k per WWW instance, when loading uncompressed AssetBundles from disk.
*   Physics 2D: Added ability to select whether deleting a 2D collider or rigid body during a collision callback stops remaining callbacks or not.
*   Physics 2D: Fixed regression where 2D colliders didn't update when animated.
*   Physics 2D: Fixed crash when Rigidbody2D component is destroyed during contact callback.
*   Physics 2D: Ensure that the lower/upper translation limits on JointTranslationLimit2D are correct with respect to each other (used on SliderJoint2D).
*   Physics 2D: Stop interpolation/extrapolation from being halted during next physics update when a new Rigidbody2D is added.
*   Shaders: Fixed more cases of errors in shaders not being reported on correct line numbers (for GLSL platforms).
*   Shaders: Fixed wrong HLSL-to-GLSL translation of clip() with a vector argument.
*   Shuriken: Fix for re-enabled particle system which was disabled before it has finished.
*   Substance: Normal maps are correctly displayed now in the Editor when targeting GL platforms.
*   Substance: Thumbnails for normal maps are now generated correctly instead of being displayed in grayscale.
*   Substance: Fixed crash when baking a ProceduralTexture without mipmaps to a compressed format.
*   Substance: Fixed ProceduralMaterials looking black after disabling the ProceduralMaterialInspector.
*   Version Control: Adding files in perforce would escape special characters such as '@' into '%40'. This issue has been fixed.
*   Windows Phone: Fixed an issue which caused serialization weaver to crash sometimes when processing methods that return IEnumerable.
*   Windows Phone: Winmd plugins are now correctly handled.
*   Windows Phone: Editor reports if arrays with generic element types that can cause crash at runtime are used.
*   Windows Phone / Store: Enum.ToObject now works with all primitive types.
*   Windows Phone / Store: Methods returning boolean values are now correctly handled.
*   Windows Phone / Store: Plugins that are signed with strong name now work properly.
*   Windows Phone / Store: When compiling JS/Boo files, debugging information will be added only when Development checkbox is on, previous behavior was debugging information was always being added.
*   Windows Phone / Store: Fixed an issue which caused private members are not initialized in serializable class.
*   Windows Phone / Store: Structs are always serialized correctly.
*   Windows Player: Fixed Alt-Tab in DirectX 11 full-screen mode freezing the application.
*   Windows Player: Run in Background now works properly in DirectX 9 fullscreen mode.
*   Windows Player: Performance improvements including lower latency in DirectX 11 mode.
*   Windows Player: The default full-screen mode no longer changes the desktop resolution, so things like IME text input work.
*   Windows Player: Hint to NVIDIA driver that it should use the discrete GPU in Optimus chipsets.
*   Windows Store Apps: Added support for TouchScreenKeyboard.text property.
*   Windows Store Apps: Portable class libraries can now successful use methods like Type.GetFields or Type.GetProperties.
*   Windows Store Apps: Show keyboard when TouchScreenKeyboard.Open() is called, no need to manually set active to true.
*   Windows Store Apps: Added support for key modifiers in GUI events.
*   Windows Store Apps: Fixed the return value of SystemInfo.supportsLocationService.