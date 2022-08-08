# Unity 4.3

https://unity3d.com/unity/whats-new/unity-4.3

## Changes

- [Deprecated and removed features:](#deprecated-and-removed-features)


*   AI / NavMesh: Support for adding more than one OffMeshLink component to a game object.
*   Android: 32bit display buffer without alpha is now the default to avoid compositor bugs on android.
*   Editor: Make Generate Mip Maps setting in Texture Importer not be bold, for consistency, and make it hide child settings rather than just disabling the GUI, for simplicity.
*   Editor: Respect original shader culling mode in scene view picking.
*   Editor: Changed the resize cursors and added a splitter resize cursor on mac.
*   Editor: Shortcut for Maximize View has changed from Space to Shift+Space. It can now also be configured in the Editor Preferences.
*   Editor: Current layout is now stored per project. New projects will use the last layout as an initial layout state.
*   Editor: MaterialEditor API refactored. Added class MaterialProperty that holds the info & values of the material property, and handles multi-selection & undo (similar to SerializedProperty). MaterialEditor functions now operate on MaterialPropertyValues; and there's a MaterialHelper class to get to them.
*   Editor: Project Browser now sorts folders first on Windows
*   Editor: show warning in inspector when we have npot texture playing with compression in a non-good way
*   Editor: Windows Background color option was removed from Preferences window
*   GameObject.Find doesn't allocate internal memory
*   iOS: Made iOS 4.3 as default target, updated warning for older targets
*   iOS: Added possibility to choose how touches originated from non-unity views are processed. Added possibility to get "raw" touch position (iOS coords).
*   iOS: Added support for rect banners (ios6 feature).
*   iOS: Added support for vendor/advertisement id (iOS6). Changed SystemInfo.deviceUniqueIdentifier logic: on ios7 it will use ad id (if tracking is enabled) and fallback to vendor id otherwise. On pre-ios7 the behavior stays the same (hash of MAC address).
*   iOS: exposed getter for possibly mirrored web cam texture
*   iOS: iAd implementation extracted to trampoline (WARNING: script interface changed). Added c# event to be triggered after user saw advertisement.
*   iOS: Trampoline now expects SDK 5.0 or higher
*   Mac Standalone Player: When in FullscreenWindow fullscreen mode without showing menu bar and dock, disable Application switching, as it would not correctly keep the Dock hidden.
*   Mecanim: Moved Optimized transform hierarchy button from inspector to the context menu
*   Mecanim: AnimationSet renamed AnimatorOverrideController and derives from RuntimeAnimatorController.
*   Mecanim: Removed AnimationSet property from the Animator Component. AnimatorOverrideController derives from RuntimeAnimator it can be asigned directly to the Controller property of the Animator.
*   Mecanim: Root motion can now be affected by Animation Clip from any controller's layer. Before only the first layer could affect the root motion.
*   Mecanim: Renamed AnimatorStateRuntimeModificator to AnimatorStateRuntime
*   Mecanim: AnimationSet refactoring. Removed AnimationSet.ReplaceClip and added a few function for setup.
*   Mecanim: A MatchTarget is now interrupted by a transition. Project created with older version will still have the same behavior than before.
*   Mecanim: Remove Keep Additional Bones for Humanoid Rig at import. Use Skeleton mask instead.
*   NavMesh: calling CompleteOffMeshLink now positions the agent at the OffMeshLink endpoint.
*   NavMesh: enabling carving for an obstacle disables avoidance for that obstacle
*   Physics: Now allowing multiple collider components of the same type on one GameObject
*   Physics: Renamed and documented layer mask constants, Physics.AllLayers, Physics.DefaultRaycastLayers, Physics.IgnoreRaycastLayer
*   Profiler: Some samples are now tagged as warnings in the CPU profiler (i.e. moving of a static collider). The warnings are shown as a count in the 'warnings' column
*   The default GUI font embedded for consoles and other platforms with no access to system fonts has been changed to "Liberation Sans"
*   Version Control: Only kill plugin on initial negotiation errors and not all errors sent from plugin
*   Version Control:Change base path to be projectPath instead assetPath.
*   WebPlayer: Installer now reports anonymous usage statistics to help improve install experience
*   Windows Phone 8/+ Windows Store Apps: Transferred Trial API from UnityEngine.Application to UnityEngine.Windows.LicenseInformation class.

### Deprecated and removed features:

*   Android: Dropped support for Froyo(2.2) and Eclair(2.1).
*   Graphics: Removed support for OpenGL ES 1.x on mobile; ES2.0 will be used by default now. Set rendering path to VertexLit in player settings to best approximate the old behavior.
*   Graphics: Removed support for pre-DX9 GPUs on PC. That is, GPUs made before 2003 (NVIDIA), 2002 (AMD) and 2004 (Intel) will not be supported now.
*   Editor: Removed Unitron (Mac) and UniSciTE (Windows) script editors. The MonoDevelop we ship now is quite good already!
*   Culling: Support for Animation bounding volume culling has been removed. Unity will fall back to renderer based culling instead.