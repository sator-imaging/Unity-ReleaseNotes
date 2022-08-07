# Unity 5.3
https://unity3d.com/unity/whats-new/unity-5.3

## Features

<ul>
<li>2D : <a href="http://docs.unity3d.com/Manual/SpriteCreator.html">2D Placeholder Assets Creation Tools</a> <img src="/sites/default/files/5.3.0-relnotes-2d-placeholder-creation-tools.png" alt="description">
<img src="/sites/default/files/5.3.0-relnotes-2d-placeholder-assets.png" alt="description"></li>
<li>Android: Java call stack is now available in C# exceptions in AndroidJavaException.StackTrace</li>
<li>Animation: <a href="http://docs.unity3d.com/Manual/AnimationEulerCurveImport.html">Import of Euler curves</a> and runtime Euler interpolation</li>
<li>Asset Bundles: LZ4 compression support - realtime decompression, LZ4 compressed cached bundles</li>
<li>Graphics: <a href="http://docs.unity3d.com/Manual/AsyncTextureUpload.html">Asynchronous Texture Upload</a></li>
<li>GI: Enlighten Clustering and Lit Clustering scene view modes <img src="/sites/default/files/5.3.0-relnotes-clustering-mode.png" alt="description">
<img src="/sites/default/files/5.3.0-relnotes-lit-clustering-mode.png" alt="description"></li>
<li>Graphics: Scripting API for blend shapes</li>
<li>Graphics: New OpenGL Core (GL3/4) back-end for Mac OS X editor and player</li>
<li>Graphics: Remote Frame Debugger <img src="/sites/default/files/image00_0.png" alt="description"></li>
<li>Graphics: <a href="http://docs.unity3d.com/Manual/RenderDocIntegration.html">RenderDoc graphics debugger</a> integrated with Unity Editor</li>
<li>Graphics: Sparse texture support for OpenGL Core and OpenGL ES</li>
<li>iOS: iOS 9 app slicing support</li>
<li>iOS: iOS 9 on demand resource support</li>
<li>iOS: iPad Pro pencil support added. Look for altitudeAngle, azimuthAngle, pressure</li>
<li>iOS: Touch.radius and pressure support added</li>
<li>iOS: Touch.type enum introduced, now it is possible to detect stylus/pencil touches versus regular touches</li>
<li>iOS: Added Bitcode support. Now iOS apps by default will include Bitcode. Bitcode adds up to 130 MB to the executable size, though this size is not accounted by App Store as distribution size. It will be stripped from your binaries by App Store servers, before your app is delivered to the users. You can inspect Bitcode in your executable by using <em>otool -l</em> command and looking for LLVM sections there.</li>
<li>Mecanim: Human Pose API. Enables humanoid live retargeting. It reads or writes a HumanPose from or to a humanoid skeleton rigs.</li>
<li>Metal support for OS X Standalone players (Editor support will come later). To enable, set Metal as first device in "Graphics APIs for Mac" section in build settings.</li>
<li>MonoDevelop: Updated to version 5.9.4</li>
<li>Networking: Support for "Host Migration" in multiplayer games that use the high level API (NetworkMigrationManager component added). When the host of a game is lost, this lets the one of the other clients become the new host and the game can continue.</li>
<li><p>Particles: All UI settings exposed to scripting API <img src="/sites/default/files/5.3.0-relnotes-particles-api-script.png" alt="description"></p></li>
<li><p>Particles: Custom pivot point support <img src="/sites/default/files/5.3.0-relnotes-particles-pivot.png" alt="description"></p></li>
<li><p>Particles: Rendering alignment (World, View, Local) <img src="/sites/default/files/5.3.0-relnote-particles-alignment.png" alt="description"></p></li>
<li><p>Particles: 3D Rotation <img src="/sites/default/files/5.3.0-relnotes-particles-rotation.png" alt="description"></p></li>
<li><p>Particles: It is now possible to scale an entire particle system using its transform component. The Shape scaling mode is also present, which preserves the old behavior of only scaling the source positions. <img src="/sites/default/files/5.3.0-relnotes-particles-scaling-mode.png" alt="description"></p></li>
<li><p>Particles: SkinnedMeshRenderer shape source (plus extra options for mesh emitter shapes) <img src="/sites/default/files/5.3.0-relnotes-particles-skinned-mesh-render.png" alt="description"></p></li>
<li><p>Particles: 2D Collisions <img src="/sites/default/files/5.3.0-relnotes-particles-2d-collisions.png" alt="description"></p></li>
<li><p>Particles: A new Inherit Velocity Module, which encompasses the old behaviour, but also adds support for inheriting velocity throughout the lifetime of a particle system using curves <img src="/sites/default/files/5.3.0-relnotes-particles-inherit-velocity.png" alt="description"></p></li>
<li><p>Physics2D: Added BuoyancyEffector2D component. <img src="/sites/default/files/5.3.0-relnotes-buoyancy-effector.png" alt="description">
<img src="/sites/default/files/5.3.0-relnotes-buoyancy-example.png" alt="description"></p></li>
<li><p>Physics2D: Added FixedJoint2D component. <img src="/sites/default/files/5.3.0-relnotes-fixed-joint.png" alt="description"></p></li>
<li><p>Physics2D: Added FrictionJoint2D component. <img src="/sites/default/files/5.3.0-relnotes-friction-joint.png" alt="description"></p></li>
<li><p>Physics2D: Added RelativeJoint2D component. <img src="/sites/default/files/5.3.0-relnotes-relative-joint.png" alt="description"></p></li>
<li><p>Physics2D: Added TargetJoint2D component. <img src="/sites/default/files/5.3.0-relnotes-relative-joint.png" alt="description"></p></li>
<li><p>Physics2D: All 2D joints can now automatically configure the connected anchor point (see 'Auto Configure Connected Anchor' on 2D joints) <img src="/sites/default/files/5.3.0-relnotes-auto-configure-connector-anchor.png" alt="description"></p></li>
<li><p>Physics2D: All 2D joints can now be broken with a configurable maximum force or torque (see 'Break Force' and 'Break Torque' on 2D joints) <img src="/sites/default/files/5.3.0-relnotes-break-force.png" alt="description"></p></li>
<li><p>Physics2D: DistanceJoint2D and SpringJoint2D can now automatically configure the distance (see 'Auto Configure Distance’ on these joints) <img src="/sites/default/files/5.3.0-relnotes-physics2d-distance-joint-distance.png" alt="description">
<img src="/sites/default/files/5.3.0-relnotes-physics2d-spring-joint-distance.png" alt="description"></p></li>
<li><p>Physics2D: Rigidbody2D mass can be automatically calculated via collider mass (see 'Use Auto Mass' on Rigidbody2D and ‘Density’ on Collider2D) <img src="/sites/default/files/5.3.0-relnotes-rigid-body-collider-mass.png" alt="description"></p></li>
<li><p>Physics2D: SliderJoint2D can now automatically configure the angle (see 'Auto Configure Angle' on this joint). <img src="/sites/default/files/5.3.0-relnotes-slider-joint.png" alt="description"></p></li>
<li><p>Physics: Expose a set of functions to run physics queries against oriented boxes (e.g.: Physics.OverlapBox, Physics.BoxCastAll)</p></li>
<li>Physics: Expose non-allocating versions of physics queries functions that accept a buffer to store the results in, as an input parameter (e.g.: Physics.RaycastNonAlloc)</li>
<li>Scripting: JSON API. Provides an easy and fast way to convert objects to and from JSON format.</li>
<li>SpeedTree: SpeedTree billboards can cast and receive shadows now. <img src="/sites/default/files/5.3.0-relnotes-speedtree-billboard-shadows.jpg" alt="description"></li>
<li><p>Testing: <a href="http://docs.unity3d.com/Manual/testing-editortestsrunner.html">Editor Tests Runner integration</a> <img src="/sites/default/files/5.3.0-relnotes-editor-test-runner_0.png" alt="description"></p></li>
<li><p>Services: <a href="http://docs.unity3d.com/Manual/UnityIAP.html">In-App Purchasing (IAP)</a> accessible via the cloud services window</p></li>
<li>UnityWebRequest: Implemented Android and iOS backend</li>
<li>VR: Head-Tracked Splash Screen 
<ul>
<li>Enabled on all Unity VR supported platforms.</li>
<li>Head-tracked splash screen is shown as early as possible while asynchronously loading the first scene.</li>
<li>Splash screen is customizable for Unity Pro. Users can set an image in PlayerSettings -&gt; Virtual Reality Splash Image which will be shown as if on a wall in a black room while loading the first scene.</li>
<li>Splash screen is tied to the "Show Unity Splash Screen" option and can be disabled in Unity Pro.</li>
</ul></li>
<li>WebGL: Add WebCamTexture support</li>
<li>Windows Store: Added support for IL2CPP scripting backend</li>
</ul>
