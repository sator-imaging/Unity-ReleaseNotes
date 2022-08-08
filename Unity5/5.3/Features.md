# Unity 5.3

https://unity3d.com/unity/whats-new/unity-5.3

## Features



*   2D : [2D Placeholder Assets Creation Tools](http://docs.unity3d.com/Manual/SpriteCreator.html) ![description](/sites/default/files/5.3.0-relnotes-2d-placeholder-creation-tools.png) ![description](/sites/default/files/5.3.0-relnotes-2d-placeholder-assets.png)
*   Android: Java call stack is now available in C# exceptions in AndroidJavaException.StackTrace
*   Animation: [Import of Euler curves](http://docs.unity3d.com/Manual/AnimationEulerCurveImport.html) and runtime Euler interpolation
*   Asset Bundles: LZ4 compression support - realtime decompression, LZ4 compressed cached bundles
*   Graphics: [Asynchronous Texture Upload](http://docs.unity3d.com/Manual/AsyncTextureUpload.html)
*   GI: Enlighten Clustering and Lit Clustering scene view modes ![description](/sites/default/files/5.3.0-relnotes-clustering-mode.png) ![description](/sites/default/files/5.3.0-relnotes-lit-clustering-mode.png)
*   Graphics: Scripting API for blend shapes
*   Graphics: New OpenGL Core (GL3/4) back-end for Mac OS X editor and player
*   Graphics: Remote Frame Debugger ![description](/sites/default/files/image00_0.png)
*   Graphics: [RenderDoc graphics debugger](http://docs.unity3d.com/Manual/RenderDocIntegration.html) integrated with Unity Editor
*   Graphics: Sparse texture support for OpenGL Core and OpenGL ES
*   iOS: iOS 9 app slicing support
*   iOS: iOS 9 on demand resource support
*   iOS: iPad Pro pencil support added. Look for altitudeAngle, azimuthAngle, pressure
*   iOS: Touch.radius and pressure support added
*   iOS: Touch.type enum introduced, now it is possible to detect stylus/pencil touches versus regular touches
*   iOS: Added Bitcode support. Now iOS apps by default will include Bitcode. Bitcode adds up to 130 MB to the executable size, though this size is not accounted by App Store as distribution size. It will be stripped from your binaries by App Store servers, before your app is delivered to the users. You can inspect Bitcode in your executable by using _otool -l_ command and looking for LLVM sections there.
*   Mecanim: Human Pose API. Enables humanoid live retargeting. It reads or writes a HumanPose from or to a humanoid skeleton rigs.
*   Metal support for OS X Standalone players (Editor support will come later). To enable, set Metal as first device in "Graphics APIs for Mac" section in build settings.
*   MonoDevelop: Updated to version 5.9.4
*   Networking: Support for "Host Migration" in multiplayer games that use the high level API (NetworkMigrationManager component added). When the host of a game is lost, this lets the one of the other clients become the new host and the game can continue.
*   Particles: All UI settings exposed to scripting API ![description](/sites/default/files/5.3.0-relnotes-particles-api-script.png)
    
*   Particles: Custom pivot point support ![description](/sites/default/files/5.3.0-relnotes-particles-pivot.png)
    
*   Particles: Rendering alignment (World, View, Local) ![description](/sites/default/files/5.3.0-relnote-particles-alignment.png)
    
*   Particles: 3D Rotation ![description](/sites/default/files/5.3.0-relnotes-particles-rotation.png)
    
*   Particles: It is now possible to scale an entire particle system using its transform component. The Shape scaling mode is also present, which preserves the old behavior of only scaling the source positions. ![description](/sites/default/files/5.3.0-relnotes-particles-scaling-mode.png)
    
*   Particles: SkinnedMeshRenderer shape source (plus extra options for mesh emitter shapes) ![description](/sites/default/files/5.3.0-relnotes-particles-skinned-mesh-render.png)
    
*   Particles: 2D Collisions ![description](/sites/default/files/5.3.0-relnotes-particles-2d-collisions.png)
    
*   Particles: A new Inherit Velocity Module, which encompasses the old behaviour, but also adds support for inheriting velocity throughout the lifetime of a particle system using curves ![description](/sites/default/files/5.3.0-relnotes-particles-inherit-velocity.png)
    
*   Physics2D: Added BuoyancyEffector2D component. ![description](/sites/default/files/5.3.0-relnotes-buoyancy-effector.png) ![description](/sites/default/files/5.3.0-relnotes-buoyancy-example.png)
    
*   Physics2D: Added FixedJoint2D component. ![description](/sites/default/files/5.3.0-relnotes-fixed-joint.png)
    
*   Physics2D: Added FrictionJoint2D component. ![description](/sites/default/files/5.3.0-relnotes-friction-joint.png)
    
*   Physics2D: Added RelativeJoint2D component. ![description](/sites/default/files/5.3.0-relnotes-relative-joint.png)
    
*   Physics2D: Added TargetJoint2D component. ![description](/sites/default/files/5.3.0-relnotes-relative-joint.png)
    
*   Physics2D: All 2D joints can now automatically configure the connected anchor point (see 'Auto Configure Connected Anchor' on 2D joints) ![description](/sites/default/files/5.3.0-relnotes-auto-configure-connector-anchor.png)
    
*   Physics2D: All 2D joints can now be broken with a configurable maximum force or torque (see 'Break Force' and 'Break Torque' on 2D joints) ![description](/sites/default/files/5.3.0-relnotes-break-force.png)
    
*   Physics2D: DistanceJoint2D and SpringJoint2D can now automatically configure the distance (see 'Auto Configure Distance’ on these joints) ![description](/sites/default/files/5.3.0-relnotes-physics2d-distance-joint-distance.png) ![description](/sites/default/files/5.3.0-relnotes-physics2d-spring-joint-distance.png)
    
*   Physics2D: Rigidbody2D mass can be automatically calculated via collider mass (see 'Use Auto Mass' on Rigidbody2D and ‘Density’ on Collider2D) ![description](/sites/default/files/5.3.0-relnotes-rigid-body-collider-mass.png)
    
*   Physics2D: SliderJoint2D can now automatically configure the angle (see 'Auto Configure Angle' on this joint). ![description](/sites/default/files/5.3.0-relnotes-slider-joint.png)
    
*   Physics: Expose a set of functions to run physics queries against oriented boxes (e.g.: Physics.OverlapBox, Physics.BoxCastAll)
    
*   Physics: Expose non-allocating versions of physics queries functions that accept a buffer to store the results in, as an input parameter (e.g.: Physics.RaycastNonAlloc)
*   Scripting: JSON API. Provides an easy and fast way to convert objects to and from JSON format.
*   SpeedTree: SpeedTree billboards can cast and receive shadows now. ![description](/sites/default/files/5.3.0-relnotes-speedtree-billboard-shadows.jpg)
*   Testing: [Editor Tests Runner integration](http://docs.unity3d.com/Manual/testing-editortestsrunner.html) ![description](/sites/default/files/5.3.0-relnotes-editor-test-runner_0.png)
    
*   Services: [In-App Purchasing (IAP)](http://docs.unity3d.com/Manual/UnityIAP.html) accessible via the cloud services window
    
*   UnityWebRequest: Implemented Android and iOS backend
*   VR: Head-Tracked Splash Screen
    *   Enabled on all Unity VR supported platforms.
    *   Head-tracked splash screen is shown as early as possible while asynchronously loading the first scene.
    *   Splash screen is customizable for Unity Pro. Users can set an image in PlayerSettings -> Virtual Reality Splash Image which will be shown as if on a wall in a black room while loading the first scene.
    *   Splash screen is tied to the "Show Unity Splash Screen" option and can be disabled in Unity Pro.
*   WebGL: Add WebCamTexture support
*   Windows Store: Added support for IL2CPP scripting backend