# Unity 5.0.3
https://unity3d.com/unity/whats-new/unity-5.0.3

## Fixes

<ul>
<li>Android: Fix for Oculus window buffer memory leak (due to Oculus plugin replacing GL context).</li>
<li>Audio: If audio output device fails to init, then init to the null device.</li>
<li>Audio: The Disable Audio option new prevents FMOD from initializing and allocating resources which are exclusive on some platforms.</li>
<li>Editor: Fixed bad scene view performance when lots of light gizmos are drawn.</li>
<li>Graphics: Fixed command buffer RenderTargetIdentifier with RenderTexture argument.</li>
<li>Graphics: Fixed regression in handling "external" textures (Texture2D.CreateExternalTexture).</li>
<li>iOS: Fixed crash on A7 SoC when locking the screen.</li>
<li>iOS: Fixed rendering issues when dismissing presenting view controller which overrides orientation constraints.</li>
<li>iOS: Fixed simulator crashing on startup due to "Symbol not found: __ZN5metal16g_CurrentEncoderE" (696798).</li>
<li>iOS: Fixed Xcode project supported platforms and SDKs settings.</li>
<li>iOS/IL2CPP: Avoid adding includes and methods (for method declaration includes) for types generated to terminate generic type recursion.</li>
<li>iOS/IL2CPP: Correct an error in generated code when a constrained generic parameter type is used in a nested lambda expression.</li>
<li>iOS/IL2CPP: Correct code generation for a generic type with another generic type as a constraint when the generic parameter for the constraint is a value type.</li>
<li>iOS/IL2CPP: Corrected the implementation of the ldvirtftn opcode for types using a constrained generic generic parameter.</li>
<li>iOS/IL2CPP: Correctly invoke an action pointing to an extension method.</li>
<li>iOS/IL2CPP: Emit memory barriers to ensure the correct acquire and release semantics are enforced for loads and stores of volatile fields.</li>
<li>iOS/IL2CPP: Ensure that background threads which are not explicitly joined have their resources freed so that the runtime does not leak thread handles.</li>
<li>iOS/IL2CPP: Fixed a code generation issue when using static constructors in base generic classes.</li>
<li>iOS/IL2CPP: Fixed a crash which occurred during a call to Socket.SetSocketOption with the AddMembership or DropMembership names.</li>
<li>iOS/IL2CPP: Fixed a case where static constructor would not be called if an object is constructed within Unity internally.</li>
<li>iOS/IL2CPP:&nbsp;Fixed WWWForm.data property getter being extremely slow on IL2CPP.</li>
<li>iOS/IL2CPP: Implemented embedded resources for IL2CPP.</li>
<li>iOS/IL2CPP: Prevent a crash when a thread with a name is finalized.</li>
<li>iOS/IL2CPP: Prevent IL2CPP from throwing an exception at conversion time for a generic type deriving from a generic interface.</li>
<li>iOS/IL2CPP: Static constructor of base type now gets correctly called if a derived class does not have one when creating an object of a derived type.</li>
<li>iOS/Metal: Fixed crash when using preloaded shaders.</li>
<li>Mecanim: Fixed duplicated parameter in blend tree of blend tree</li>
<li>Merge Tool: Fixed auto fallback spec file detection.</li>
<li>Merge Tool: Handle regression in 5.0.1 introduced by stripped prefabs.</li>
<li>Physics: Stop force waking up Rigidbodies when AddForce / AddTorque (family) is called with a zero vector. This fixes Rigidbodies starting to accelerate even though a zero force is applied.</li>
<li>Plugins: Windows plugins won't be included to OSX package, when building for X86 architecture.</li>
<li>PS3/PS4: Fixed some separate alpha blending shader states not working properly.</li>
<li>Scripting: Fixed debugger deadlock on OSX.</li>
<li>Scripting: Fixed MonoDevelop incorrectly stepping over recursive methods.</li>
<li>Scripting: Fixed Unity crash when using newer versions of the soft debugger client in MonoDevelop.</li>
<li>VR: Added 3D splash screen to Unity Personal Edition Builds.</li>
<li>WebPlugin: Fixed cross-domain policy bypass issue (reported by Jouko Pynnonen of Klikki Oy).</li>
<li>Windows Phone/Store: Fixed assembly converter crashing when a type generic class derives from a generic class which has a generic parameter that is array of generic parameters of the derived class (e. g. class Derived : MyBase).</li>
<li>Windows Store Apps/Windows Phone 8.1: Fixed extended splash screen sizing.</li>
</ul>
