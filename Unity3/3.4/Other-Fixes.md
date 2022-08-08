# Unity 3.4

https://unity3d.com/unity/whats-new/unity-3.4

## Other Fixes



*   Web player:
    *   Fix several cases that caused crash in rare occasions and improve error handling in general.
    *   Fix issue that prevented Web Player from working in closed networks.
    *   Fix issue that prevented auto update from working for non-administartor users on Mac OS X.
    *   Prevent cursor from vanishing in fullscreen mode when cursor trail is enabled.
    *   Prevent cursor from vanishing when another game is running on a different browser tab.
    *   Stabilized web player framerates.
    *   Web player now behaves correctly when resizing window in Firefox4.
    *   Removed 16 kilobyte limit for Application.ExternalCall() and ExternalEval().
    *   Chrome, Safari and FF4 on Mac OS X now registers keypresses on input string.
    *   Input.GetAxis() returns correct value when focus is restored.
    *   Fixed an occasional crash when switching to fullscreen on Mac OS X.
    *   Fixed audio pausing in the background in Dashboard on Mac OS X.
*   Networking:
    *   Fixed error when reading 32bit Network View IDs, huge amounts of views can properly be instantiated.
*   MonoDevelop:
    *   Fixed bug where seemingly random parts of the Unity API would fail to show up in autocomplete lists.
    *   Fixed update expandability of items in the Locals pad when debugging over a slow network.
*   Asset pipeline:
    *   Made clearer error message when importing .dds file with missing mipmap levels in texture importer.
    *   3DStudio Max importer no longer crashes when trying to parse a broken .3ds file.
    *   Changing "Pack Margin" and other settings in the advanced Model import setting is now recognized as a change.
*   Input:
    *   Shift keys now recognized in fullsceen on Mac OS X web players.
    *   Mouse position now reported correctly for Windows 7 touchscreens (only works in full screen for now – see known issues).
*   Physics:
    *   ConfigurableJoint.configuredInWorldSpace will no longer result in a wrong coordinate space. Projects using this setting need to be readjusted!
    *   Better Skinned Cloth behaviour when the mesh does not have normals, or is rendered with a shader that does not use normals.
*   Other fixes:
    *   Fixed a bunch of minor mistakes in the documentation.
    *   Cleaned up the use of non-public APIs that caused Mac OS X standalone builds to be rejected for the Mac App Store.
    *   Fixed crash when doing raycasts on 64 bit standalone players.
    *   AssetBundle.Load() now preloads all dependent assets like AssetBundle.LoadAsync() does.
    *   Fixed regression introduced in Unity 3.3 where preload data was not written correctly leading to some hiccups during gameplay when first accessing a referenced asset.
    *   Fixed crash when loading Asset Bundles to big to fit in memory.
    *   Fix bug preventing standalone player & web player from using more than 2GB of ram on Windows.
    *   Fixed crash when deleting the last slot of a builtin array.
    *   Fix bug where enums were sometimes not displayed correctly for embedded classes in arrays.
    *   Fixed creation of empty cache folders for each new project.
    *   Workaround for crash in Apple's Font unloading code in Mac OS X 10.7.