# Unity 3.4.1

https://unity3d.com/unity/whats-new/unity-3.4.1

## Fixes

- [Editor](#editor)
- [Runtime](#runtime)
- [Standard assets](#standard-assets)
- [Javascript](#javascript)
- [MonoDevelop](#monodevelop)


### Editor

*   Icons on newly created Prefabs no longer stay after the Prefab is deleted from the scene.
*   Fixed crash on Windows related to AssetStore server side errors.
*   Fixed right click menu for keys on curves in the AudioSource Component not working when a AudioLowPassFilter component was also attached.
*   Fixed crash when changing .meta files and the .meta data file is disagreeing with the changes.
*   Only display progress bar when it changes at least one percentage point, fixes crash due to out of memory and faster asset scan speed.
*   Fixed texture importer rescan memory leak, which caused out of memory crashes.
*   Clear log callback when unloading domains, fixes crash when hitting Play button.
*   Fixed auto release leaks in progress bars on Mac OS X.
*   Fixed potential crash in curve editing for audio sources.
*   Fixed render texture creation error when searching in the project view.

### Runtime

*   Fix intermittent crash-on-reload on Windows.
*   Fixed crash on exit when "Exit on Suspend" was checked on iOS.
*   Fixed crash on exit in forced OpenGL mode on Windows.
*   Fixed webplayer graphical glitches existing in Safari on Mac OS X Lion for some AMD graphics cards.
*   Fixed crash in skinning meshes with invalid bone indices or when mesh has just been updated.
*   Fixed crash in SSE2 skinning code when reading out of bounds.
*   Fixed regression against Unity 3.3 when using RenderTexture.GetTemporary with cubemaps.

### Standard assets

*   Added missing Pro Water shaders.

### Javascript

*   Implicit downcasts (for example, assignment from a variable of type Object to a variable of type String) will now be reported as warnings instead of errors in strict mode.

### MonoDevelop

*   Fixed US International input method to allow input of ' and ".
*   Better window resizing on Mac OS X Lion.