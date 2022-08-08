# Unity 2019.1

https://unity3d.com/unity/whats-new/2019.1.0

## Features



*   Android: Added Android notch/cut-out support to `Screen.safeArea`
    
*   Android: Added OpenGL ES 3.2 support
    
*   Android: Added Script Only Patching functionality, which sends only script-related changes to the device instead of repackaging the APK file.
    
*   Android: Added support for ASTC HDR texture formats
    
*   Android: Added `AndroidDevice.SetSustainedPerformanceMode` to the API to enable/disable sustained performance mode in runtime
    
*   Android: Enabled redistributing Android NDK and SDK components with Android Build Support
    
*   Editor: Added a new Scene view **Camera settings** menu to control field of view (FOV), Camera speed, and Camera easing while moving and zooming. In Flythrough mode, the mouse scroll wheel adjusts the Camera speed.
    
*   Editor: Added a new Shortcuts Manager window for managing keyboard shortcuts.
    
*   Editor: Added a search field to the Console for filtering output by keyword.
    
*   Editor: Added checkboxes to the Gizmos menu for selecting/deselecting all gizmos in a given section (**Built-in Components**, **Scripts**, and so on).
    
*   Editor: Added new **EditorTools** API for creating custom tools that behave like native tools. The **Available Custom Editor Tools** button in the Scene view toolbar opens a custom tools menu. The **Component Editor Tools** panel in the Scene view shows available custom tools for the current selection.
    
*   Editor: Added pre-checkout and pre-submit user-specified callbacks for VCS integration. Allows users to create callbacks that can modify Asset lists and changeset selections/descriptions at checkout and submit time.
    
    Pre-checkout callback can:
    
    *   Add and remove assets from the list of those that will be checked out
    *   Create a new changeset to check the specified asset list in
    *   Nominate an existing changeset to check the specified asset list in
    *   Return false from the callback to block checkout
    
    Pre-submit callback can:
    
    *   Add and remove assets from the list of those that will be submitted
    *   Create a new changeset to submit specified asset list in
    *   Nominate an existing changeset to submit the specified asset list in
    *   Rename an existing changeset then submit it and
    *   Return false from the callback to block submission
*   Editor: Added Scene visibility controls to the Hierarchy window for controlling the visibility of GameObjects in the Scene view. Users can toggle visibility for individual GameObjects, or GameObjects and their children. A global visibility toggle hides/shows everything in the scene.
    
*   Editor: Added support for referencing Assembly Definitions with GUIDs instead of assembly names. Users can enable this setting via the **Use GUIDs** property in the Assembly Definition Inspector. This is now the default setting for new Assembly Definition files.
    
*   Editor: Added `CSHARP_7_3_OR_NEWER` preprocessor directive when compiling C# 7.3 on .NET 4.x scripting runtime.
    
*   Editor: Exposed `AdvancedDropdown` API for implementing searchable `AddComponent` style dropdowns.
    
*   Editor: Made editor on-demand shader compilation asynchronous, not blocking the editor while compiling the shader on the first time usage. Rendering happens with a replacement shader until the actual shader variant is available. To enable or disable this feature, go to Project Settings > Editor > Asynchronous Shader Compilation.