# Unity 3.5

https://unity3d.com/unity/whats-new/unity-3.5

## Changes

- [Android](#android)
- [Editor](#editor)
- [iOS](#ios)
- [Miscellaneous](#miscellaneous)


*   Added KeyCode enum values for Joystick 4.
*   Android/iOS: The Android Target Graphics setting is not linked to the iOS Target Platform setting anymore.

### Android

*   Attached names to the native threads for easier debugging.
*   Changed labeling of Force Internet Permission to Internet Access (Auto / Require).
*   Changed labeling of Force SD-Card Permission to Write Access (Internal Only / External (SDCard)).
*   Development builds now have extended logging also from the Java side.
*   Editor requires at least API level 14 to build Android applications. It is still possible to target earlier platforms.
*   Force debug.checkjni property when launching development builds (to prevent incorrect JNI calls from plugins).
*   Keep the LVL code from outputting errors if it's not used anyway.
*   Restructured parts of the Java code found in classes.jar.
*   The Emulator device filter was removed, as the Android Virtual Device (with SDK-r14) now supports ARMv6/ARMv7 binaries.
*   The splash image is now decoded as 32bit texture (rather than 16bit).
*   The Texture Compression Override option in the Build Settings menu has been changed to affect all textures using a compressed texture format.
*   To save memory when streaming AssetBundles, the number of compressed buffers in flight has been reduced.
*   Traded some temporary memory (240KB, in the scene loader) for an on-average massive load speedup with projects having really bad load times.

### Editor

*   Added optional saveAsCopy parameter to EditorApplication.SaveScene to allow saving the scene without changing what is the current scene.
*   Asset Path names starting with a space character are now no longer allowed.
*   Migrated direct Blender to Unity import from Blender 2.56 to Blender 2.58. Implemented support for Blender 2.59 as well.
*   OnSceneGUI is now called on all selected objects with custom editors, not only editors visible in the inspector.
*   The Editor will no longer allow creation or import of Assets with file names which are not legal on either Windows or OS X.
*   Undo while dragging never worked correctly and is now disabled. Note: Most dragging operations allow you to press Esc to cancel, which can be used instead.

### iOS

*   Added 5.0 SDK selection in PlayerSettings.
*   Added iPhone4S generation for iPhone.generation.
*   Added warning when compressed texture is used as icon or splash screen.
*   Changing target devices does not require to overwrite Xcode project anymore.
*   Screen.dpi implemented.

### Miscellaneous

*   Mac OS X Standalone: Moved Cache file location to ~/Library/Caches/bundleID for Mac App Store compliance.
*   Mac OS X: Use OS events for more reliable mouse wheel input. Should now work with all devices which work with the OS, but only work when mouse cursor is over the window.
*   Removed support for OS X Dashboard builds.
*   Removed support for OS X PowerPC builds.
*   Removed support for Unitron and UniSciTE.
*   Stripping: Now 3rd party dlls aren't treated as managed code stripping roots. Improves build size, but might require extra care with libraries that use reflection and generics a lot.
*   Windows Web Player: If no graphics drivers are installed at all, Unity will not try to run the game using the really bad Windows' OpenGL 1.1 renderer; an error message will be displayed to the user instead.
*   WWW: charset property is now honored by the WWW.text attribute.
*   WWW: Made HTTP errors be reported in www.error string.
*   WWW: Made HTTP headers be set appropriately even when errors occur. Added the HTTP status code to the header list under the "STATUS" key.