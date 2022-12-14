# Unity 4.5.2

https://unity3d.com/unity/whats-new/unity-4.5.2

## Fixes



*   2D : SpriteRenderers with a negative scale can now batch together with SpriteRenderers with a positive scale.
*   2D : Sprite references will not break if sprites are renamed or deleted using the Sprite Editor.
*   Android : Fixed the build failure on latest Android SDK (v23)
*   Android : Switched to UTF encoding for compiling java resource files
*   Asset Management : Assets referenced by GUIStyle are no longer incorrectly collected by UnloadUnusedAssets
*   AI : NavMesh carving obstacles are spatially sorted for robustness.
*   Asset Import : Autodesk Maya 2015 not supported, MEL scripts need to be updated
*   Audio : Fixed regression with AudioClips that are flagged as streaming
*   Core : Added AssetBundle.CreateFromMemoryImmediate, to create AssetBundles from a byte array synchronously.
*   Core : Asset Bundle Export performance increase
*   Documentation : Updated documentation based on user feedback and minor bugs found
*   Documentation : Add a section on script serialisation and serialisation in general.
*   Documentation : Array doesn't display methods twice anymore
*   Documentation : Fixed documentation layout on mobile browsers (as well as small doc improvements)
*   Editor : Fixed issue with prefabs not maintaining new position if moved in hierarchy.
*   Editor : Added preference setting to enable alphabetical hierarchy sorting.
*   Editor : Fixed performance issues with large & flat scene hierarchies (new hierarchy window in 4.5 was slower on them).
*   Editor : Fixed issue with object Transform being set to the origin when Prefab was dropped into hierarchy window.
*   Editor : Killed annoying cmd windows that was popping up during android deployment
*   Editor : Fixed Asset Store window showing up blank in DirectX 11 mode on some laptop graphics cards
*   Editor : Don't show any blinking cmd windows while launching the dab server
*   Editor : Fixed erroneous "Mismatched serialisation in the builtin class 'Mesh'" errors when loading meshes imported with Unity 3.5.0.
*   Editor : Fixed security issues when trying to set Android SDK location under non-admin account
*   Editor : Fixed console not having a scroll bar for error detail
*   Graphics : Fixed light matrix (\_LightMatrix0) not always being set to shaders in deferred lighting.
*   Graphics : Fixed Camera's Depth & DepthNormals textures sometimes using the wrong filtering mode.
*   Graphia's : Fixed light Halo not initially rendering, unless there is another Halo component in the scene.
*   Graphics : Particle Sub Emitter not playing after Pause()
*   Image Effects : Fixed CameraMotionBlurDX11 shader having a syntax error. Whoops!
*   Linux : Fixed regression in mouse look behaviour.
*   Linux : Deploy more configuration metadata with standalone players
*   Mecanim : Fixed errors/crash when using Animator:GetCurrentAnimationClipState on layers
*   Mecanim : Fixed transitioning into empty state on a synced layer.
*   Mecanim: Fixed transition to self speed during AnyState transition.
*   Mecanim : Improved performance of activating the Animator.
*   Mecanim : Improved memory usage per instance.
*   Physics 2D : Display a warning against a 2D collider when it is unable to create a Box2D collision shape due to it not meeting Box2D constraints.
*   Physics 2D : Only update 2D rigid-body position and/or rotation as transform position/rotation changes respectively.
*   Physics 2D : Stop a crash when removing 2D rigid-body during a collision callback.
*   Physics 2D : Add missing "distance" property to RaycastHit2D.
*   Physics 2D : Ensure that reference angle is maintained for both HingeJoint2D and SliderJoint2D when a component change occurs.
*   Physics 2D : Fix occasional crash when unloading scenes with lots of 2D static colliders.
*   Physics 2D : Stop 2D colliders from being generated twice upon start-up.
*   Physics 2D : Fix how rotational inertia and centre-of-mass is calculated.
*   Rendering-Other : Clear back-buffer after resolution change on Windows.
*   Rendering-Other : Fixed GLES3 shader compiling failure on non-const global initialisation. Note that this has been fixed only for Android in this patch.
*   Scripting : Fixed Socket.ExclusiveAddressUse using UDP to work on Linux
*   Scripting : Fixed support for serialising array of generic types
*   Scripting : Fixed step-out in debugger behaving as continue in some scenarios.
*   Scripting : Reduce spam from serialisation depth warning to a single warning.
*   Scripting : Fixed double-clicking a C# script will open MonoDevelop instead of Visual Studio.
*   Serialization : Fixed GraphicsSettings reset on project open if using text serialisation mode.
*   Shaders : Fixed preprocessor regressions in HLSL-to-GLSL translation (token pasting, macros with line continuations, other complex macros).
*   Shaders : Fixed surface shader regression with multiple spaces between "pragma" and "surface".
*   Shaders: Fixed GLES3 shader compiling failure on non-const global initialisation.
*   Substance : Fix rare semaphore-related error message.
*   Substance : Fix rare hangs/crashes when building user projects.
*   Substance : Decrease memory footprint after initial scene load
*   Substance : Fixed potential crash when baking ProceduralTextures to compressed formats
*   Webplugin : Fixed a crash where decompression threads were still working, even though the plugin was being closed.
*   Windows Phone 8/ Windows Store Apps : Fixed small memory leak in animation system.
*   Windows Phone 8/ Windows Store Apps : Fixed animating camera and 2D sprite properties.
*   Windows Phone 8/ Windows Store Apps : Unity will now properly post-process .winmd files.
*   Windows Phone 8/ Windows Store Apps : Unity will properly fix InternalsVisibleToAttribute on post-processing.
*   Windows Phone 8/ Windows Store Apps : Fixed MonoBehaviour serialisation when SerializableAttribute is not specified in base classes.
*   Windows Phone 8/ Windows Store Apps : Unity will now correctly recognise System.Nullable <-> Windows.Foundation.IReference type alias when checking for unavailable APIs
*   Windows Phone 8/ Windows Store Apps : Shader depth bias (Offset) will now correctly work on DX11 feature level 9.x.
*   Windows Store Apps : Unity C# projects can be rebuilt multiple times without file copying errors.
*   Windows Store Apps : Fixed NullReferenceException when building with SDK 8.0