# Unity 4.5.2
https://unity3d.com/unity/whats-new/unity-4.5.2

## Fixes

<ul>
<li>2D : SpriteRenderers with a negative scale can now batch together with SpriteRenderers with a positive scale.</li>
<li>2D : Sprite references will not break if sprites are renamed or deleted using the Sprite Editor.</li>
<li>Android : Fixed the build failure on latest Android SDK (v23)</li>
<li>Android : Switched to UTF encoding for compiling java resource files</li>
<li>Asset Management : Assets referenced by GUIStyle are no longer incorrectly collected by UnloadUnusedAssets</li>
<li>AI : NavMesh carving obstacles are spatially sorted for robustness.</li>
<li>Asset Import : Autodesk Maya 2015 not supported, MEL scripts need to be updated</li>
<li>Audio : Fixed regression with AudioClips that are flagged as streaming</li>
<li>Core : Added AssetBundle.CreateFromMemoryImmediate, to create AssetBundles from a byte array synchronously.</li>
<li>Core : Asset Bundle Export performance increase</li>
<li>Documentation : Updated documentation based on user feedback and minor bugs found</li>
<li>Documentation : Add a section on script serialisation and serialisation in general.</li>
<li>Documentation : Array doesn't display methods twice anymore</li>
<li>Documentation : Fixed documentation layout on mobile browsers (as well as small doc improvements)</li>
<li>Editor : Fixed issue with prefabs not maintaining new position if moved in hierarchy.</li>
<li>Editor : Added preference setting to enable alphabetical hierarchy sorting.</li>
<li>Editor : Fixed performance issues with large &amp; flat scene hierarchies (new hierarchy window in 4.5 was slower on them).</li>
<li>Editor : Fixed issue with object Transform being set to the origin when Prefab was dropped into hierarchy window.</li>
<li>Editor : Killed annoying cmd windows that was popping up during android deployment</li>
<li>Editor : Fixed Asset Store window showing up blank in DirectX 11 mode on some laptop graphics cards</li>
<li>Editor : Don't show any blinking cmd windows while launching the dab server</li>
<li>Editor : Fixed erroneous "Mismatched serialisation in the builtin class 'Mesh'" errors when loading meshes imported with Unity 3.5.0.</li>
<li>Editor : Fixed security issues when trying to set Android SDK location under non-admin account</li>
<li>Editor : Fixed console not having a scroll bar for error detail</li>
<li>Graphics : Fixed light matrix (_LightMatrix0) not always being set to shaders in deferred lighting.</li>
<li>Graphics : Fixed Camera's Depth &amp; DepthNormals textures sometimes using the wrong filtering mode.</li>
<li>Graphia's : Fixed light Halo not initially rendering, unless there is another Halo component in the scene.</li>
<li>Graphics : Particle Sub Emitter not playing after Pause()</li>
<li>Image Effects : Fixed CameraMotionBlurDX11 shader having a syntax error. Whoops!</li>
<li>Linux : Fixed regression in mouse look behaviour.</li>
<li>Linux : Deploy more configuration metadata with standalone players</li>
<li>Mecanim : Fixed errors/crash when using Animator:GetCurrentAnimationClipState on layers</li>
<li>Mecanim : Fixed transitioning into empty state on a synced layer.</li>
<li>Mecanim: Fixed transition to self speed during AnyState transition.</li>
<li>Mecanim : Improved performance of activating the Animator.</li>
<li>Mecanim : Improved memory usage per instance.</li>
<li>Physics 2D : Display a warning against a 2D collider when it is unable to create a Box2D collision shape due to it not meeting Box2D constraints.</li>
<li>Physics 2D : Only update 2D rigid-body position and/or rotation as transform position/rotation changes respectively.</li>
<li>Physics 2D : Stop a crash when removing 2D rigid-body during a collision callback.</li>
<li>Physics 2D : Add missing "distance" property to RaycastHit2D.</li>
<li>Physics 2D : Ensure that reference angle is maintained for both HingeJoint2D and SliderJoint2D when a component change occurs.</li>
<li>Physics 2D : Fix occasional crash when unloading scenes with lots of 2D static colliders.</li>
<li>Physics 2D : Stop 2D colliders from being generated twice upon start-up.</li>
<li>Physics 2D : Fix how rotational inertia and centre-of-mass is calculated.</li>
<li>Rendering-Other : Clear back-buffer after resolution change on Windows.</li>
<li>Rendering-Other : Fixed GLES3 shader compiling failure on non-const global initialisation. Note that this has been fixed only for Android in this patch.</li>
<li>Scripting : Fixed Socket.ExclusiveAddressUse using UDP to work on Linux</li>
<li>Scripting : Fixed support for serialising array of generic types</li>
<li>Scripting : Fixed step-out in debugger behaving as continue in some scenarios.</li>
<li>Scripting : Reduce spam from serialisation depth warning to a single warning.</li>
<li>Scripting : Fixed double-clicking a C# script will open MonoDevelop instead of Visual Studio. </li>
<li>Serialization : Fixed GraphicsSettings reset on project open if using text serialisation mode.</li>
<li>Shaders : Fixed preprocessor regressions in HLSL-to-GLSL translation (token pasting, macros with line continuations, other complex macros).</li>
<li>Shaders : Fixed surface shader regression with multiple spaces between "pragma" and "surface".</li>
<li>Shaders: Fixed GLES3 shader compiling failure on non-const global initialisation.</li>
<li>Substance : Fix rare semaphore-related error message.</li>
<li>Substance : Fix rare hangs/crashes when building user projects.</li>
<li>Substance : Decrease memory footprint after initial scene load</li>
<li>Substance : Fixed potential crash when baking ProceduralTextures to compressed formats</li>
<li>Webplugin : Fixed a crash where decompression threads were still working, even though the plugin was being closed.</li>
<li>Windows Phone 8/ Windows Store Apps : Fixed small memory leak in animation system.</li>
<li>Windows Phone 8/ Windows Store Apps : Fixed animating camera and 2D sprite properties.</li>
<li>Windows Phone 8/ Windows Store Apps : Unity will now properly post-process .winmd files.</li>
<li>Windows Phone 8/ Windows Store Apps : Unity will properly fix InternalsVisibleToAttribute on post-processing.</li>
<li>Windows Phone 8/ Windows Store Apps : Fixed MonoBehaviour serialisation when SerializableAttribute is not specified in base classes.</li>
<li>Windows Phone 8/ Windows Store Apps : Unity will now correctly recognise System.Nullable &lt;-&gt; Windows.Foundation.IReference type alias when checking for unavailable APIs</li>
<li>Windows Phone 8/ Windows Store Apps : Shader depth bias (Offset) will now correctly work on DX11 feature level 9.x.</li>
<li>Windows Store Apps : Unity C# projects can be rebuilt multiple times without file copying errors.</li>
<li>Windows Store Apps : Fixed NullReferenceException when building with SDK 8.0</li>
</ul>
