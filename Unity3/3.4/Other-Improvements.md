# Unity 3.4

https://unity3d.com/unity/whats-new/unity-3.4

## Other Improvements



*   Mac App Store:
    *   Added a feature to perform receipt validation for the Mac App Store.
*   Scripting:
    *   Ability to control the order that scripts are executed in. Use Edit->Project Settings->Script Execution Order.
    *   Texture2D.SetPixels32/GetPixels32 for much faster pixel operations.
    *   Added Caching.MarkAsUsed function. This is used to ensure that some files are not thrown out of the least-recently-used cache if you know that they will be used in the future.
*   Input:
    *   Win7 touchscreen input now fully supported.
    *   Input.eatKeyPressOnTextFieldFocus added to be able to control input behavior during textfield focus. This is default true from 3.4 and forth. Set this to false to achieve pre 3.4 behavior.
    *   Key input (i.e. Input.GetKeyDown) is now suppressed when a textfield is active. This is enabled only content built with 3.4 and later. To query key input during an active textfield, use Event.current in OnGUI.
    *   Fixed support for mouse deltas from Apple's Magic Trackpad.
*   MonoDevelop:
    *   Scripting projects are now built the same way that Unity builds them.
    *   Now compiles Boo and UnityScript.
*   Profiling:
    *   Intel GPA 4.0 Platform Analyzer profiler is supported for Windows Standalone Players.
*   Javascript improvements:
    *   Allow characters in #pragma lines.
    *   Array.slice(startIndex) must return all elements starting from startIndex.
    *   Array.slice accepts negative indexes counting from the end of the array: \[1, 2, 3, 4\].slice(-2) // => \[3, 4\]
    *   Proper support for do-while loops
    *   Proper support for generic dictionaries of functions:
        *   var dict = new Dictionary.();
        *   dict\["foo"\] = function() print("foo");
        *   dict\["foo"\] (); // prints foo
*   Importers:
    *   Implemented 3 minute timeout for 3DStudio Max FBX conversion.
    *   Only show import settings on root asset. Showing them on every sub-asset could lead to the false impression that every sub-asset can have individual import settings.
*   Other improvements:
    *   Removed tray icon for Windows Standalones when in batchmode allowing apps to run as a service.
    *   Removed option 'Always Show Watermark' from the Player Settings.