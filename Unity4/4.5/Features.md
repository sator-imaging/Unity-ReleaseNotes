# Unity 4.5

https://unity3d.com/unity/whats-new/unity-4.5

## Features

- [Graphics features:](#graphics-features)
- [Module Manager:](#module-manager)
- [Editor features:](#editor-features)
- [2D Physics features:](#2d-physics-features)
- [Unity Remote upgrade:](#unity-remote-upgrade)
- [Mecanim features:](#mecanim-features)
- [Windows Store apps features:](#windows-store-apps-features)
- [Other features:](#other-features)


### Graphics features:

*   Shader importing has been massively improved:
    *   Shaders are imported much faster, especially complex surface shaders. Instead of compiling all shader variants for all possible platforms at import time, now the needed shader variants for needed platforms are compiled on-demand. Shader compilation results are cached under Library folder, so identical compilations happen much faster.
    *   Error reporting was improved. Errors are reported on correct lines (imagine that!), and errors in .cginc files report the filename.
    *   Surface shader debugging was improved. No more "#pragma debug" nonsense; just click "Show generated code" in the inspector.
*   Added Sparse Texture support (also known as "mega textures" or "tiled textures"). This is a low-level API feature, see SparseTexture class. Implemented on DirectX 11.2 (via tiled resources) and desktop OpenGL (via ARB\_sparse\_texture).
*   Added stereoscopic rendering on DX 11.1 (requires Windows 8.1 and compatible hardware).
*   Introduced support for OpenGL ES 3.0 on iOS devices (starting with A7 devices).
*   Graphics: Support for 3D textures in OpenGL ES 3.0.

### Module Manager:

*   Introduced Module Manager with updatable platform support. iOS, Android, Windows Phone 8, Blackberry Unity add ons can be updated without downloading full editor installer. Accessed through Modules menu, next to Preferences menu.

### Editor features:

*   New Hierarchy Window sorting - sorting of elements is now based on transform order instead of name.
*   Introduced new editor API AssetDatabase.FindAssets (string filter, string\[\] folders). Search the Asset Database for assets by filename, type and asset label. See documentation for more information.
*   Added Selection.assetGUIDs for getting the current selected assets in the Project Browser. It also returns the folder selection in the first column in the Project Browser (in Two Column mode) which is not part of the main selection.

### 2D Physics features:

*   Added 2D Joint Gizmos.
*   Added new 2D physics component: WheelJoint2D.

### Unity Remote upgrade:

*   Unity Remote 4 is our play testing solution for iOS and Android. As of Unity 4.5, there’ll be no more Wifi latency when playtesting your games on iOS devices. Plus, we’ve added support for the full range of iOS device inputs including accelerometers, gyroscopes and camera images. Unity Remote 4 is available free of charge from Google Play and the App Store.

### Mecanim features:

*   Added CanTransitionToSelf option on AnyState Transitions.
*   Added new scripting function Animator.Rebind(). You can use this function to manually rebind the animator data set to unity when you change something in your GameObject hierarchy.
*   For humanoid rigs, in the importer, you can specify a transform node that will be used as root motion for an animation clip. The transform node will replace the automatically extracted root motion computed by Mecanim. (Pro Only).

### Windows Store apps features:

*   Added Compass API to check for compass accuracy.
*   AppCallbacks methods InvokeOnUIThread and InvokeOnAppThread will detect deadlock and throw exception. Added TryInvokeOnUIThread and TryInvokeOnAppThread, which return true or false instead.
*   Support for programmatically opening touch screen keyboard.
*   In Player Preferences added support for scaled resources: splash screen, medium and wide tile, store and small logos.
*   In Player Preferences added support for Windows 8.1 scaled resources and related settings.
*   New APIs for changing system cursor - AppCallbacks::SetCursor, AppCallbacks::SetCustomCursor, WSA.Cursor.SetCustomCursor.
*   Added support for changing screen resolution on Windows 8.1.

### Other features:

*   Scripting: Introduced DisallowMultipleComponentAttribute for disallowing multiple components of the same type being added to a single GameObject.
*   Scripting: Add UnityEngine.ISerializationCallbackReceiver interface, to get a callback right before serialisation and right after deserialization.
*   Scripting: Structs with System.Serializable attribute can now be serialized. Also, fields of AnimationCurve\[\] and double\[\] now get serialised.
*   WebPlugin: Added Enhanced Protected Mode support for Internet Explorer. Supports IE 64 bit.