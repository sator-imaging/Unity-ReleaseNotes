# Unity 2019.3.0

https://unity3d.com/unity/whats-new/2019.3.0

## Changes



*   Android: Android: When "Installed with Unity (recommended)" is selected in Editor Tools Preferences window and the expected path is not available, don't look for alternative paths.
    
*   Android: Improved error messages for cases where an Android application fails to load libmain.so. Unity now prints "Failed to load 'libmain.so', the application will terminate.", and an exception from System.loadLibrary with detailed information about where the application was looking for libmain.so.
    
*   Android: Minimum supported Android version is now Android 4.4 KitKat (API 19)
    
*   Android: The option to target x86 for Android has now been removed.
    
*   Android: Updated Android NDK used to version r19.
    
*   Apple TV: Removed support for Universal Harmony Remote, currently there's no way to properly support Universal Harmony Remote without breaking Siri Remote.
    
*   Asset Import: Added a warning when Unity imports multiple sub-Assets with the same name or type. This often happens when importing Models with multiple Meshes or Materials that have the same name in the .fbx file. Their resulting fileID (and thus references to them) may break or change if Unity finds a new sub-Asset with the same name before the existing one after re-importing.
    
*   Editor: The Preset Manager now supports a list of default Presets for each Preset type instead of a single Preset. The default Preset contains a filter that is tested against the new default Object to determine whether or not to apply the Preset to the Object. Every matching Preset is applied, in order, to the new default Object, regardless of whether it was created using the ObjectFactory API or an importer.
    
*   GI: Deprecated Enlighten, and hid it from new Projects in Scriptable Render Pipelnes. Upgraded Projects will still show it.
    
*   Graphics: Adding explicit depth resolve to RenderPass Metal
    
*   Graphics: Graphics Jobs is now enabled by default in the 3D Template
    
*   Scripting: Incremental GC is now no longer marked as "Experimental"
    
*   Timeline: Enabled rectangle tool for inline curves.
    
*   Universal Windows Platform: Removed icons that were only used on Windows 8.1 apps from Player Settings ([1139095](https://issuetracker.unity3d.com/issues/uwp-legacy-store-icons-arent-removed-from-player-settings))
    
*   Version Control: Assets menu Version Control submenu got moved near top of the menu, into the same place where Collaborate menu is.
    
*   Version Control: Paths outside of the unity project are considered to never be part of version control, e.g. AssetDatabase.IsOpenForEdit will return true for them
    
*   Video: Legacy MovieTexture (Theora-based video playback system) has been removed. Use VideoPlayer instead.
    
*   Windows: Command line arguments '-gpu' and '-adapter' replaced with '-force-device-index' and '-monitor' respectively to be consistent with MacOS and Linux.
    
*   XR: Removed Vuforia built-in functionality from the Editor. Moved to package.