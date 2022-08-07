# Unity 3.5
https://unity3d.com/unity/whats-new/unity-3.5

## Changes

<ul>
<li>Added KeyCode enum values for Joystick 4.</li>
<li>Android/iOS: The Android Target Graphics setting is not linked to the iOS Target Platform setting anymore.</li>
</ul>

### Android
<ul>
<li>Attached names to the native threads for easier debugging.</li>
<li>Changed labeling of Force Internet Permission to Internet Access (Auto / Require).</li>
<li>Changed labeling of Force SD-Card Permission to Write Access (Internal Only / External (SDCard)).</li>
<li>Development builds now have extended logging also from the Java side.</li>
<li>Editor requires at least API level 14 to build Android applications. It is still possible to target earlier platforms.</li>
<li>Force debug.checkjni property when launching development builds (to prevent incorrect JNI calls from plugins).</li>
<li>Keep the LVL code from outputting errors if it's not used anyway.</li>
<li>Restructured parts of the Java code found in classes.jar.</li>
<li>The Emulator device filter was removed, as the Android Virtual Device (with SDK-r14) now supports ARMv6/ARMv7 binaries.</li>
<li>The splash image is now decoded as 32bit texture (rather than 16bit).</li>
<li>The Texture Compression Override option in the Build Settings menu has been changed to affect all textures using a compressed texture format.</li>
<li>To save memory when streaming AssetBundles, the number of compressed buffers in flight has been reduced.</li>
<li>Traded some temporary memory (240KB, in the scene loader) for an on-average massive load speedup with projects having really bad load times.</li>
</ul>

### Editor
<ul>
<li>Added optional saveAsCopy parameter to EditorApplication.SaveScene to allow saving the scene without changing what is the current scene.</li>
<li>Asset Path names starting with a space character are now no longer allowed.</li>
<li>Migrated direct Blender to Unity import from Blender 2.56 to Blender 2.58. Implemented support for Blender 2.59 as well.</li>
<li>OnSceneGUI is now called on all selected objects with custom editors, not only editors visible in the inspector.</li>
<li>The Editor will no longer allow creation or import of Assets with file names which are not legal on either Windows or OS X.</li>
<li>Undo while dragging never worked correctly and is now disabled. Note: Most dragging operations allow you to press Esc to cancel, which can be used instead.</li>
</ul>

### iOS
<ul>
<li>Added 5.0 SDK selection in PlayerSettings.</li>
<li>Added iPhone4S generation for iPhone.generation.</li>
<li>Added warning when compressed texture is used as icon or splash screen.</li>
<li>Changing target devices does not require to overwrite Xcode project anymore.</li>
<li>Screen.dpi implemented.</li>
</ul>

### Miscellaneous
<ul>
<li>Mac OS X Standalone: Moved Cache file location to ~/Library/Caches/bundleID for Mac App Store compliance.</li>
<li>Mac OS X: Use OS events for more reliable mouse wheel input. Should now work with all devices which work with the OS, but only work when mouse cursor is over the window.</li>
<li>Removed support for OS X Dashboard builds.</li>
<li>Removed support for OS X PowerPC builds.</li>
<li>Removed support for Unitron and UniSciTE.</li>
<li>Stripping: Now 3rd party dlls aren't treated as managed code stripping roots. Improves build size, but might require extra care with libraries that use reflection and generics a lot.</li>
<li>Windows Web Player: If no graphics drivers are installed at all, Unity will not try to run the game using the really bad Windows' OpenGL 1.1 renderer; an error message will be displayed to the user instead.</li>
<li>WWW: charset property is now honored by the WWW.text attribute.</li>
<li>WWW: Made HTTP errors be reported in www.error string.</li>
<li>WWW: Made HTTP headers be set appropriately even when errors occur. Added the HTTP status code to the header list under the "STATUS" key.</li>
</ul>
