# Unity 4.6.6
https://unity3d.com/unity/whats-new/unity-4.6.6

## Fixes

<ul>
<li>Android: Fixed player crash when audio is disabled.</li>
<li>Android: Fixed sound glitches when using FastMixer audio on GearVR.</li>
<li>Animation: Fixed a memory leak when "Optimize Game Objects" was used without a skeleton.</li>
<li>Editor: Android - Fixed updating SDK on x86 Java on Windows.</li>
<li>Graphics: Fix for a crash when swapping skinned meshes under GLES3.</li>
<li>Graphics: Fixed inaccurate screenspace scissoring of lights with large range.</li>
<li>Input: Input.GetJoystickNames() no longer returns a single blank entry when no joysticks are attached.</li>
<li>Input: Update mouse position when it is outside of rendered area in Windows standalone.</li>
<li>Input: Update rect used to clip Input.mousePosition when Windows Standalone window is resized.</li>
<li>iOS: Allow to append builds made with different scripting backend.</li>
<li>iOS: Correctly set 5.1.1 SDK according to user prefs.</li>
<li>iOS: Fixed crash on A7 devices when locking the screen.</li>
<li>iOS: Fixed memory leak in iOS WebCamTexture.GetPixels().</li>
<li>iOS: Fixed Xcode 6.3 Build &amp; Run.</li>
<li>iOS: Fixed Xcode project supported platforms and SDKs settings.</li>
<li>iOS/IL2CPP: Added support for string.Normalize.</li>
<li>iOS/IL2CPP: Correct code generation for a generic type with another generic type as a constraint when the generic parameter for the constraint is a value type.</li>
<li>iOS/IL2CPP: Corrected the implementation of the ldvirtftn opcode for types using a constrained generic generic parameter.</li>
<li>iOS/IL2CPP: Correctly invoke an action pointing to an extension method.</li>
<li>iOS/IL2CPP: Correctly lazy initialize the type information when Type.GetDeclaringType is called.</li>
<li>iOS/IL2CPP: Emit memory barriers to ensure the correct acquire and release semantics are enforced for loads and stores of volatile fields.</li>
<li>iOS/IL2CPP: Ensure that background threads which are not explicitly joined have their resources freed so that the runtime does not leak thread handles.</li>
<li>iOS/IL2CPP: Fixed a case where static constructor would not be called if an object is constructed within Unity internally.</li>
<li>iOS/IL2CPP: Fixed a code generation issue when using static constructors in base generic classes.</li>
<li>iOS/IL2CPP: Fixed a crash which occurred during a call to Socket.SetSocketOption with the AddMembership or DropMembership names.</li>
<li>iOS/IL2CPP: Fixed code generation for binary comparisons containing expressions</li>
<li>iOS/IL2CPP: Fixed memory leak when using audio callbacks.</li>
<li>iOS/IL2CPP: Fixed System.Environment.TickCount on iOS.</li>
<li>iOS/IL2CPP: Fixed unordered comparison opcodes code generation.</li>
<li>iOS/IL2CPP: Fixed WebClient requests using a timeout.</li>
<li>iOS/IL2CPP: Fixed WWWForm.data property getter being extremely slow on IL2CPP.</li>
<li>iOS/IL2CPP: Implemented embedded resources for IL2CPP.</li>
<li>iOS/IL2CPP: Optimized code generation for exception handling and finally statements.</li>
<li>iOS/IL2CPP: Prevent a crash when a thread with a name is finalized.</li>
<li>iOS/IL2CPP: Prevent IL2CPP from throwing an exception at conversion time for a generic type deriving from a generic interface.</li>
<li>iOS/IL2CPP: Static constructor of base type now gets correctly called if a derived class does not have one when creating an object of a derived type.</li>
<li>iOS/IL2CPP: Treat the [MarshalAs(UnmanagedType.LPStruct)] like a by reference parameter by marshaling it as a pointer.</li>
<li>iOS/IL2CPP: Using AudioSettings.Reset() no longer crashes on IL2CPP.</li>
<li>iOS/IL2CPP:Avoid adding includes and methods (for method declaration includes) for types generated to terminate generic type recursion.</li>
<li>Linux: Fixed applying vsync and antialiasing changes without changing quality level.</li>
<li>Linux: Fixed cursor visibility regression when cursor is locked.</li>
<li>Linux: Support more standard screen resolutions.</li>
<li>MonoDevelop: Fixed issue with Attach to Process dialog making MonoDevelop unresponsive on OSX.</li>
<li>MonoDevelop: Fixed issue with file tabs being unresponsive after using auto-hide of panels.</li>
<li>OpenGL: Re-enable various graphics features (shadows etc.) on newer Intel drivers on Windows.</li>
<li>Physics 2D: Don't suppress gravity when a Rigidbody2D.MovePosition is taking place.</li>
<li>Physics 2D: Ensure that 2D Box/Circle cast methods support shape being overlapped initially (case 692409).</li>
<li>Physics 2D: Ensure that a 2D joint created from script is correctly enabled.</li>
<li>Physics 2D: Setting center-of-mass on a Rigidbody2D now doesn't result in bad rotational inertia.</li>
<li>Scripting: Fixed a deadlock in the editor that could happen when pressing the play button while a debugger was still attached.</li>
<li>Scripting: Fixed debugger deadlock on OSX.</li>
<li>Scripting: Fixed MonoDevelop incorrectly stepping over recursive methods.</li>
<li>Scripting: Fixed Unity crash when using newer versions of the soft debugger client in MonoDevelop</li>
<li>UI: Correctly populate PointerEventData.worldPosition and PointerEventData.worldNormal for right-mouse-button and middle-mouse-button events.</li>
<li>UI: Fixed UI elements failing to render in Scene View.</li>
<li>UnityObject: Handle Chrome (v42) that might have NPAPI plugin support disabled.</li>
<li>WebPlugin: Fixed cross-domain policy bypass issue (reported by Jouko Pynnonen of Klikki Oy).</li>
<li>Windows Phone/Store: Fixed assembly converter crashing when a type generic class derives from a generic class which has a generic parameter that is array of generic parameters of the derived class (e. g. class Derived : MyBase).</li>
<li>Windows Standalone: Added hint to AMD driver that it should use the discrete GPU rather than integrated GPU if available.</li>
<li>Windows Standalone: Filter device notifications to HID-class devices only, resolving spurious RID.Hid warnings</li>
<li>Windows Store Apps/Windows Phone 8.1: Unity will correctly hide password when using GUI*.PasswordField on touch based devices.</li>
</ul>
