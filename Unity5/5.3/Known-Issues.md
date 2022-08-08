# Unity 5.3

https://unity3d.com/unity/whats-new/unity-5.3

## Known Issues



*   [On Windows 7 32-bit, editor will not start](http://issuetracker.unity3d.com/issues/editor-doesnt-start-up-on-windows-xp-32bit) Should be fixed in the next patch release.
*   Editor hangs after pressing "Add new branch group" button within Tree Editor window in the Inspector (OSX). Should be fixed in a following patch release.
*   [Editor often crashes on Windows 10 when locking Windows, when using DirectX 9](http://issuetracker.unity3d.com/issues/dx9-unity-crashed-in-gfxdeviced3d9-drawbuffers-due-to-handled3ddevicelost-when-locking-windows)
*   [ETC1 compression format not playing well with Asset bundles generated with 5.2](http://issuetracker.unity3d.com/issues/sprites-when-loading-asset-bundles-that-were-built-with-5-dot-2-and-uses-etc1-plus-alpha-format-it-shows-up-wrong-on-5-dot-3)
*   Legacy Animation: Changes to the lights in 5.3 have caused an issue so that it currently is not possible to animate lights using the Legacy animation system. We are aware of this and working on a fix. We will keep you all updated with the progress.
*   [Multiple displays do not report the correct resolution when using non-native resolutions, they report the screen resolution and not the game resolution.](http://issuetracker.unity3d.com/issues/build-canvas-elements-are-placed-incorrectly-when-setting-non-native-resolution-in-standalone-build) For Patch 1, the UI system has had multiple display support disabled on all platforms except WiiU and 3DS.
*   [Particle billboard shadows are not oriented correctly](http://issuetracker.unity3d.com/issues/shadows-shape-of-shadows-cast-by-particles-changes-depending-on-an-angle-they-are-viewed-at) in 5.3, but should be fixed in 5.4
*   [Particle normals are different between versions 5.1 and 5.2](http://issuetracker.unity3d.com/issues/renderer-particle-normals-direction-is-incorrect). A fix will arrive in a patch release.
*   [Particle system with Skinned Mesh Renderer as shape has its particles emitted in wrong position and rotation](http://issuetracker.unity3d.com/issues/shapemodule-particle-system-with-skinned-mesh-renderer-as-shape-has-its-particles-emitted-in-wrong-position-and-rotation) A fix will arrive in patch release.
*   [Unity hangs when selecting objects in scene view](http://issuetracker.unity3d.com/issues/unity-hangs-when-selecting-objects-in-the-scene-view). Fix is in-bound for patch release, but still undergoing testing.
*   SSR (Screen Space Reflections) image effect will be available during the 5.3 release cycle on the forums and asset store. We have a few minor issues to address still before we feel it is ready to be built-in.
*   OpenGL (new GLCore backend)
    *   GPU Profiler disabled for OpenGL on OSX in Editor. Works with Standalone Player still.
    *   White artifacts on update of editor windows like resizing
*   [Player crashes on iOS 6 on startup](http://issuetracker.unity3d.com/issues/ios-crash-when-deploying-to-ios6)
*   [UI: Root Canvas with no UI will not render Child Canvas](http://issuetracker.unity3d.com/issues/ui-ui-objects-are-not-displayed-in-unity-samples-ui-project). Fix will arrive in a patch release.
*   [UWP does not build on recently released Windows SDK (version 10.0.10586.0)](http://forum.unity3d.com/threads/warning-do-not-update-to-windows-sdk-10-0-10586-0-just-yet.371074/) . A fix will arrive in a patch release.