# Unity 5.1.2
https://unity3d.com/unity/whats-new/unity-5.1.2

## Fixes

<ul>
<li>(699578) -  2D: Fixed the issue where it was unable to set Sprite mode to multiple.</li>
<li>(701438) -  Animation: Animating properties of the material with the custom shader does not cause error on the first play in editor.</li>
<li>(699383) -  Animation: Reject avatar creation when the skeleton is missing intermediary bones.</li>
<li>(665246) -  Animation: Remove relative material property blocks when the animator component is being removed.</li>
<li>(706635) -  Asset Loading: Ignoring hidden dll files.</li>
<li>(690156) -  Asset Management: Now allow prefab instances with a missing prefab template to be reparented.</li>
<li>(670070) -  Audio: Audio clip "Force to Mono" now has an option for applying normalization after downmix.</li>
<li>(705599) -  Audio: Fixed: FSBTool crashed during audio import on Windows XP / N platforms and very short audio files.</li>
<li>(694539) -  CacheServer: Asset bundle names are not properly imported from metafiles.</li>
<li>(702628) -  Deployment Management: Fixed crash when selecting 'Scripting Backend' in standalone Player Settings.</li>
<li>(670391) -  DX11: Don't spam refCount==0 error messages when some 3rd party tools hook into DX11.</li>
<li>(703205) -  DX11: Fixed non-native resolution fullscreen being too dark when in Linear color space.</li>
<li>(686697) - Editor OSX: Fixed custom cursor getting set back to default arrow when used in the editor.</li>
<li>(686697) -  Editor OSX: Fixed games setting the cursor to null wouldn't take affect in the editor.</li>
<li>(692047) -  Editor: Removed MSVCRT dependency for WebGL build.</li>
<li>(705649) -  Editor: Search correct 32/64bit program files on windows for diff tools.</li>
<li>(none) - Editor: Texture3D sizes up to 2048 are now allowed (previously the limit was 1024).</li>
<li>(none) -  GearVR: Removed log spam about user profile.</li>
<li>(705573) -  GI: Fixed intermittent crash related to realtime lightprobes.</li>
<li>(none) - GLES: Fix for TC Particles package from the Asset Store.</li>
<li>(699694) -  GLES: Fixed crash when using multithreaded renderer and using shader that uses vertex colors when the mesh data doesn't contain vertex colors.</li>
<li>(705269) -  GLES: Fixed shader compiler crash for some shaders that use scalar pixel shader inputs, and other issues.</li>
<li>(696397) -  GLES: Fixed standard shader rendering issues with Mali GPUs.</li>
<li>(707361) -  GLES: Fixed tessellation shaders when multiple texcoords are packed into one vec4.</li>
<li>(none) -  GLES: Workaround for Adreno 4xx driver bug where binary shaders would break if the shader program contains geometry shaders.</li>
<li>(700474) -  Graphics: Fixed a bug when loading single channel JPEGs using Texture2D.LoadImage.</li>
<li>(698775) -  Graphics: Fixed issue in Texture2D.LoadImage when loading indexed PNG images that contain an alpha channel.</li>
<li>(689087) -  iOS: Added a limit for iOS acceleration event queue.</li>
<li>(681384) -  iOS: Added additional Japanese fallback font.</li>
<li>(699574) -  iOS: Added iOS Thai font for 8.2.</li>
<li>(701425) -  iOS: Added support for Xcode 6.3.2.</li>
<li>(704699) -  iOS: Added support for Xcode 7 beta.</li>
<li>(689410) -  iOS: Allow to append builds made with different scripting backend.</li>
<li>(705241) -  iOS: Don't add header files to il2cpp Xcode project.</li>
<li>(699907) -  iOS: Don't include managed dll files in il2cpp build.</li>
<li>(710126)  iOS: Fixed a regression which caused appending builds with native plugins to fail</li>
<li>(710818)  iOS: Fixed a regression which disables appending builds in folders more than one level away from the project folder</li>
<li>(702900) - iOS: Fixed stuck "Launch screen type" setting.</li>
<li>(682882) -  iOS: Include iOS Xcode API documentation.</li>
<li>(685439) -  iOS: Lightmapped objects with legacy shaders lit with realtime light in legacy deferred no longer render incorrectly.</li>
<li>(695118) ,(701548) -  iOS/IL2CPP: Added support for PreserveAttribute to prevent classes, methods, fields and properties from being stripped in IL2CPP.</li>
<li>(705724) -  iOS/IL2CPP: Allow Type.GetType(string) to return a proper value on 32-bit ARMv7 builds.</li>
<li>(708137) -  iOS/IL2CPP: Avoid boxing of value types during null checks in generic code.</li>
<li>(700507) -  iOS/IL2CPP: Avoid deadlock during UnloadUnusedAssets.</li>
<li>(691607), (667147) -  iOS/IL2CPP: Corrected an exception during code conversion which has the error message "Invalid global variables count" when converting some UnityScript assemblies.</li>
<li>(704018) -  iOS/IL2CPP: Ensure that GetCurrentMethod returns the proper value, even when the generated native method is inlined.</li>
<li>(none) -  iOS/IL2CPP: Fix embedded resources.</li>
<li>(695179) -  iOS/IL2CPP: Fixed a crash which occurred when Ldvirtftn opcode was used on a non-virtual method.</li>
<li>(691404) -  iOS/IL2CPP: Fixed a rare case when bytecode stripper would incorrectly strip wrong overloaded generic virtual method.</li>
<li>(697860) -  iOS/IL2CPP: Fixed codegen issue when using a field type a struct that has no instance fields.</li>
<li>(696986) -  iOS/IL2CPP: Fixed ConstructorInfo.Invoke() returning null for Nullable types.</li>
<li>(694436) -  iOS/IL2CPP: Fixed IL2CPP generated code in if (...) block if the condition operand was an IntPtr.</li>
<li>(694436) -  iOS/IL2CPP: Fixed IL2CPP generated marshaling code for marshaling IntPtr into any other primitive type.</li>
<li>(702879) -  iOS/IL2CPP: Fixed marshaling arrays of structs marked with [Out] attribute.</li>
<li>(696745) - iOS/IL2CPP: Generate correct C++ code for the IL add opcode with pointers in unsafe C# code.</li>
<li>(699644) -  iOS/IL2CPP: Handle 'void' type parameter.</li>
<li>(706613) -  iOS/IL2CPP: Handle invalid IL generated by UnityScript compiler for delegates.</li>
<li>(698589) -  iOS/IL2CPP: iOS/IL2CPP: Correct RPC implementation for the UnityEngine.Networking namespace.</li>
<li>(696187) -  iOS/IL2CPP: Prevent a C++ compiler error in generated code about an undeclared identifier with the test "Unused local just for stack balance".</li>
<li>(702203) -  iOS/IL2CPP: Prevent a C++ compiler error in generated code which happens when a pointer is assigned a value which is a uintptr_t in converted unsafe C# code.</li>
<li>(691077) - iOS/IL2CPP: Prevent a crash in the NetworkManager initialization when the Stipping Level option is not set to Disabled.</li>
<li>(702696) -  iOS/IL2CPP: Prevent a runtime exception with IL code in an enumerator's MoveNext method when the enumerator's return type is a constrained generic type.</li>
<li>(693259) -  iOS/IL2CPP: Prevent AES encryption types from being incorrectly stripped when they are used.</li>
<li>(703294) -  iOS/IL2CPP: Prevent an exception during code generation when the default value of a field is not the same type as the field.</li>
<li>(695319) -  iOS/IL2CPP: Prevent an intermittent crash on ARM64 when an live object is incorrectly reclaimed but the garbage collector.</li>
<li>(697757) -  iOS/IL2CPP: Prevent the exception: "System.ArgumentException: enumType is not an Enum type." from occurring for a generic type used with an enum type argument.</li>
<li>(704069) -  iOS/IL2CPP: Prevent the player build process from using older generated C++ source files from a previous build.</li>
<li>(708137) -  iOS/IL2CPP: Speed up generic method calls on value types.</li>
<li>(705860) -  iOS/IL2CPP: The Preserve attribute can now be used in the managed code for an assembly to preserve all of the code in an assembly.</li>
<li>(705860) - iOS/IL2CPP: The preserve attribute can now be used with the assembly element in a link.xml file to preserve all of the code in an assembly.</li>
<li>(691008) -  iOS/IL2CPP: When compiling scripts for the player, appropriate UnityEngine.UI.dll will be referenced now.</li>
<li>(704998) -  License: Added network timeout for all pending operations.</li>
<li>(704271) -  License: Clear error message once valid serial is entered.</li>
<li>(700738) -  License: Fixed an issue with Operating System ID changing on Windows 10.</li>
<li>(702313) -  License: License activation staying stuck in Updating or Connecting screen.</li>
<li>(704270) -  License: Replace generic invalid serial message with more meaningful message</li>
<li>(706183) -  Linux: Fixed key release regression.</li>
<li>(none) -  Mecanim: Fixed assert when using Optimize Game Object on object that are parented.</li>
<li>(none) -  Mecanim: Fixed continuity in FixedTime transition with ExitTime.</li>
<li>(none) -  Mecanim: Fixed crash when using AnimatorController in asset bundles.</li>
<li>(697582) -  Merge Tool: Fixwd merging of scenes/prefabs with out of order objects.</li>
<li>(700533) - MonoDevelop: Fixed issue with Attach button in attach to process dialog not responding to clicks.</li>
<li>(673868) -  MonoDevelop: Fixed Unity crash when inspecting enum value in MonoDevelop debugger.</li>
<li>(699556) -  MonoDevelop: Fixed Unity crash when using the debugger to inspect a property that only has a getter that returns a struct. E.g. Sprite.bounds.</li>
<li>(701421) -  Networking: Added missing check for NetworkIdentity on NetworkManager object.</li>
<li>(699613) -  Networking: Added missing error message for more than 32 SyncVars in a NetworkBehaviour script.</li>
<li>(692633) -  Networking: Added missing error message for multiple NetworkManagers in a scene.</li>
<li>(697809) -  Networking: Added missing validation for invalid method signatures on network methods.</li>
<li>(693234) -  Networking: Added missing validation for SyncVars of invalid types.</li>
<li>(697118) -  Networking: Adding missing error message for using network custom attributes in non NetworkBehaviour derived scripts.</li>
<li>(701760) -  Networking: Fix for allowing multiple network components on the same game object.</li>
<li>(697682) -  Networking: Fix for ClientRpc call failing when called on a base class.</li>
<li>(698103) -  Networking: Fix for ClientRpc calls being invoked out of order on localClient.</li>
<li>(696932) -  Networking: Fix for ClientRpc calls not being invoked for scene objects on a local client.</li>
<li>(697824) -  Networking: Fix for exception when sending a game object component as an argument to RPC calls.</li>
<li>(696579) -  Networking: Fix for foldouts in NetworkManager inspector not saving state.</li>
<li>(none) -  Networking: Fix for garbage at the end of broadcast messages.</li>
<li>(697502) -  Networking: Fix for implementing Update() in a class derived from NetworkManager causing client connection callbacks to not be called.</li>
<li>(none) -  Networking: Fix for IsAcksLong flag doesn't work.</li>
<li>(697754) -  Networking: Fix for isServer still being true after server was stopped.</li>
<li>(701235) -  Networking: Fix for not being able to detect idle connections.</li>
<li>(697730) -  Networking: Fix for setting MaxConnection to zero causing exception in NetworkManager.</li>
<li>(697102) -  Networking: Fix for SyncVars not working with script inheritance.</li>
<li>(698321) -  Networking: Fix for UNetWeaver exception generating an exception when SyncListStruct used directly without a derived class.</li>
<li>(698732) -  Networking: Fix for unserializating NetworkIdentity references failing on a dedicated server.</li>
<li>(none) -  Networking: Fixed - localdiscovery doesn't work on osx and ios.</li>
<li>(704949) -  Networking: Fixed the problem with host which was added removed and added back. Last add will finish with error - cannot open socket.</li>
<li>(none) -  Networking: Fixed the problem with long acks.</li>
<li>(701313) -  Networking: Fixed UNetWeaver exception when processing large projects, also improved speed with large projects.</li>
<li>(697117) -  Networking: NetworkTransform now auto-detects CharacterController and pick the correct sync method when added to a game object.</li>
<li>(577228) -  Physics 2D: Ensure that both friction and bounce are updated when the PhysicsMaterial2D is set on a Collider2D from script.</li>
<li>(705901) -  Physics 2D: Ensure that Rigidbody2D interpolation or extrapolation do not modify the Transform Z position.</li>
<li>(703846) -  Physics 2D: Fixed a child Rigidbody2D not correctly updating its position/orientation when it's using interpolation and the parent transform changes.</li>
<li>(683964), (696095) -  Physics 2D: Fixed various One-Way behaviour issues in PlatformEffector2D.</li>
<li>(702907) -  Physics 2D: MotorSpeed on SliderJoint2D is now in meters/sec (linear motor) not degrees/sec (not angular motor).</li>
<li>(697547) -  Physics 2D: Restore the Rigidbody2D linear-velocity after a Rigidbody2D.MovePosition has completed.</li>
<li>(701932) - Physics 2D: Rigidbody2D constraints are now based upon the center-of-mass and not the body position.</li>
<li>(701202) -  Physics 2D: Stop crash if 2D effector is needed but there is none.</li>
<li>(697637) -  Physics 2D: Stop NullReferenceException when editing PolygonCollider2D.</li>
<li>(699169) -  Physics: Fixed a crash when trying to report a MeshCollider error while the MeshCollider's SharedMesh was null.</li>
<li>(685107) -  Physics: Fixed an issue in PhysX where a capsule would fail to collide with a triangle mesh.</li>
<li>(441764) -  Physics: Fixed an issue in PhysX where capsule-capsule collision detection would erroneously fail when the capsules' axes were almost aligned.</li>
<li>(698701), (698702) -  Physics: Fixed HingeJoint SetMotor, SetLimits, SetSpring only being set correctly if the said properties was already enabled.</li>
<li>(697543) -  Physics: Fixed issue in PhysX where PhysX would hang on certain Android devices.</li>
<li>(705471) -  Physics: Fixed problem in PhysX that would cause SphereColliders to bounce when rolling over the triangles of a MeshCollider.</li>
<li>(697849) -  Physics: HingeJoint now correctly measures the hinge angle regardless of the initial rotation between the two hinged bodies.</li>
<li>(686576) -  Revert baked lightmap texture compression quality from best back to normal. Speeds up compositing step.</li>
<li>(none) - Samsung TV: Resolved security issue that allowed for arbitrary code execution.</li>
<li>(none) -  SamsungTV: Fixed security false-positive. The 2013 and 2014 TVs can now be deployed to successfully.</li>
<li>(none) -  Script Editors: Generate and open solution when External Script Editor is set to Xamarin Studio.</li>
<li>(693537) -  Serialization: Disallow EditorOnlyPlayerSettings custom properties usage without initialization</li>
<li>(none) -  Shaders: Fixed broken constant buffer info on OpenGL ES compute shaders with multiple kernels</li>
<li>(705485) -  Shaders: Fixed GLSL/Metal translation of shaders that use all uppercase SV_TARGET semantic.</li>
<li>(670391) -  Shaders: Fixed GLSL/Metal translation of shaders that use non-uppercase SV_Position semantic.</li>
<li>(704497), (704501) - Shaders: Fixed resource binding regression breaking TC Particles asset store package.</li>
<li>(none) -  Shaders: Increased timeout for shader import time processing; helps with complex compute shaders.</li>
<li>(676585) -  Substance: Fix hang/crash when entering playmode with the Profiler window open.</li>
<li>(none) -  Tizen: Added docs about native plugins on Tizen.</li>
<li>(none) -  Tizen: Added Tizen to the default platforms list.</li>
<li>(none) -  Tizen: Fixed plugin loading.</li>
<li>(689600) -  UI: Number of batches created for UI scene back down to 5.0 number.</li>
<li>(697556) -  Unified GL: Fix for DX11-style Depth-of-Field image effect: fix boolean variable handling in shader compiler.</li>
<li>(none) -  Unified GL: Fix for shader errors when swizzles were incorrectly applied to scalar values.</li>
<li>(697556) -  Unified GL: Fixed a crash when current and pending framebuffers have different attachment counts.</li>
<li>(707761) -  Update Checker: Wait for Home Window to be closed before checking for updates</li>
<li>(none) -  VR: Don't update the head pose until Camera has latched the reference frame.</li>
<li>(702042) -  VR: Enabling / disabling virtual reality support in the editor nolonger affects standalone players.</li>
<li>(704263) -  VR: Fix issue where GUI could be inadvertently flipped.</li>
<li>(none) -  VR: Fix issues with VRSettings.loadedDevice</li>
<li>(709060), (703989) -  VR: Fix rendering issues when camera parent is scaled.</li>
<li>(none) -  VR: Fixed anti aliasing.</li>
<li>(none) -  VR: Fixed aspect ratio of game view and standalone window.</li>
<li>(705638) -  VR: Fixed GearVR crash with Android Personal Edition.</li>
<li>(none) -  VR: Fixed linear lighting.</li>
<li>(706852) -  VR: Fixed upgrade issue from 5.1.1 which could result in VR loss of functionality.</li>
<li>(none) -  VR: Reset camera-to-origin pose on scene load to prevent gross error.</li>
<li>(none) -  WebGL: Fixed an issue using System.IO.Compression.DeflateStream API.</li>
<li>(none) -  WebGL: Fixed error messages when refreshing or unloading the page.</li>
<li>(none) -  WebGL: Fixed WWW Downloads failing if they take longer then 5 seconds.</li>
<li>(none) -  WebGL: Prevent a runtime error due to the NetworkManager and MasterServerInterface not being correctly stripped.</li>
<li>(704102) -  Windows Phone 8: Fixed crash when building from Editor.</li>
<li>(694021) - Windows Phone 8.1: Fixed simulator build.</li>
<li>(703879) -  Windows Phone: Fixed build failure when using certain classes from System.Net namespace.</li>
<li>(none) -  Windows Store Apps: Fixed a rare crash at boot when reading AppxManifest.xml.</li>
<li>(693303) -  Windows Store Apps: Fixed extended splash screen sizing on wp8.1 and scaled WSA.</li>
<li>(709350) -  Windows Store Apps/Windows Phone: Fix rare build failure while copying plugins.</li>
<li>(none) - Windows Store Apps/Windows Phone: Fix Universal apps build, when project name contains whitespaces</li>
<li>(702282) -  Windows Store Apps/Windows Phone: Fixed an issue with connecting to server using UNet.</li>
<li>(670992) -  Windows Store Apps/Windows Phone: Fixed serialization when inheriting from class from another assembly with internal field</li>
<li>(699656) -  Windows Store Apps/Windows Phone: Fixed variable synchronization between WinRT and Mono players (UNet).</li>
<li>(695285) -  Xbox One: Disabled standard splash screen on Xbox One, which was showing up as a blank grey screen after the initial OS load splash screen.</li>
<li>(690152) -  Xbox One: Fixed a bug that could cause game chat to fail when more than two players are involved.</li>
<li>(none) -  Xbox One: Socket descriptions now require template to function (as of April XDK). The editor GUI has been updated to make templates mandatory for all socket descriptions.</li>
<li>(none) -  Xbox One: The auto-added port for script debugging now implements a template, and works again. It will also get auto-added if you specify to auto-connect the profiler.</li>
</ul>
