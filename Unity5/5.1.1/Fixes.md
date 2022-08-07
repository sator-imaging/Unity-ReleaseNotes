# Unity 5.1.1
https://unity3d.com/unity/whats-new/unity-5.1.1

## Fixes

<ul>
<li>AI: Fixed NavMeshAgent path re-planning (typically after carving) when agents are assigned a path via SetPath.</li>
<li>AI: Fixed issue causing spurious error message "ag.remainingDistance &gt;= 0.0f" for agents waiting at OffMeshLinks.</li>
<li>AI: Fixed problem with performance when scene constains only idle agents with small radii.</li>
<li>Android: Now Application.systemLanguage will return Chinese Traditional or Chinese Simplified instead of just Chinese.</li>
<li>APIUpdater: Fixed crash when scripts contains some specific generic type / method usages.</li>
<li>APIUpdater: Fixed editor hang updater consent dialog is displayed while user is performing a drag &amp; drop.</li>
<li>Audio: If the audio output device fails to init, then init to the null device to prevent crash.</li>
<li>Audio: The Disable Audio option now prevents FMOD from initializing and allocating resources which are exclusive on some platforms.</li>
<li>CEF: Fixed crash when opening the asset store when no network.</li>
<li>Cloud Service: Fix for using another encoding for the url.</li>
<li>Editor: Fixed bad scene view performance when lots of light gizmos are drawn.</li>
<li>Editor: Fixed: Missing icon in Mecanim Transition inspector.</li>
<li>Editor: Profiler GameObject count in scene no longer increases when selecting camera.</li>
<li>Editor: Undo for editing capsule collider.</li>
<li>Editor: Undo for GameObject &gt; Toggle Active State in main menu.</li>
<li>GI: Fixed static lightmap baking on a rectangular terrain.</li>
<li>GLES: Fixed crash on Vivante GPUs when using binary shaders.</li>
<li>Graphics: Fixed inaccurate screenspace scissoring of lights with large range.</li>
<li>Graphics: Fixed assertion when LODGroup is scaled to zero.</li>
<li>Graphics: Fixed command buffer RenderTargetIdentifier with RenderTexture argument.</li>
<li>Graphics: Fixed regression in handling "external" textures (Texture2D.CreateExternalTexture).</li>
<li>Graphics: Fixed rendering issues after native rendering plugin GL.IssuePluginEvent() calls on OpenGL ES platforms.</li>
<li>Input: Update mouse position when it is outside of rendered area in Windows standalone.</li>
<li>iOS/IL2CPP: Avoid adding includes and methods (for method declaration includes) for types generated to terminate generic type recursion. iOS/IL2CPP: Correct an error in generated code when a constrained generic parameter type is used in a nested lambda expression.</li>
<li>iOS/IL2CPP: Correct code generation for a generic type with another generic type as a constraint when the generic parameter for the constraint is a value type.</li>
<li>iOS/IL2CPP: Corrected the implementation of the ldvirtftn opcode for types using a constrained generic generic parameter.</li>
<li>iOS/IL2CPP: Correctly invoke an action pointing to an extension method.</li>
<li>iOS/IL2CPP: Emit memory barriers to ensure the correct acquire and release semantics are enforced for loads and stores of volatile fields.</li>
<li>iOS/IL2CPP: Ensure that background threads which are not explicitly joined have their resources freed so that the runtime does not leak thread handles.</li>
<li>iOS/IL2CPP: Fixed a crash which occurred during a call to Socket.SetSocketOption with the AddMembership or DropMembership names.</li>
<li>iOS/IL2CPP: Fixed managed stack traces.</li>
<li>iOS/IL2CPP: Fixed&nbsp;a code generation issue when using static constructors in base generic classes.</li>
<li>iOS/IL2CPP: Generate correct C++ code for a generic virtual method which returns an IEnumerator and has a generic constraint defined on the method it overrides.</li>
<li>iOS/IL2CPP: Implement embedded resources for IL2CPP.</li>
<li>iOS/IL2CPP: Prevent a crash when a thread with a name is finalized.</li>
<li>iOS/IL2CPP: Prevent IL2CPP from throwing an exception at conversion time for a generic type deriving from a generic interface.</li>
<li>iOS/IL2CPP: Fixed WWWForm.data property getter being extremely slow on IL2CPP.</li>
<li>iOS/IL2CPP: Fixed a case where static constructor would not be called if an object is constructed within Unity internally.</li>
<li>iOS/IL2CPP: Fixed an issue which sometimes caused IL2CPP to not call static constructors when Unity created class instances from native code.</li>
<li>iOS/IL2CPP: Static constructor of base type now gets correctly called if a derived class does not have one when creating an object of a derived type.</li>
<li>iOS/Metal: Fixed crash when using preloaded shaders.</li>
<li>iOS: Fixed crash on A7 SoC when locking the screen.</li>
<li>iOS: Fixed rendering issues when dismissing presenting view controller which overrides orientation constraints.</li>
<li>iOS: Fixed simulator crashing on startup due to "Symbol not found: __ZN5metal16g_CurrentEncoderE".</li>
<li>iOS: Now Application.systemLanguage will return Chinese Traditional or Chinese Simplified instead of just Chinese.</li>
<li>Linux: Fixed nonASCII input regression.</li>
<li>Mecanim: Changing AnimatorState runtime speed from positive to negative value should now correctly play the animation clip backward.</li>
<li>Mecanim: Fixed AnimatorState.speed with a value of 0 should now correctly pause the animation clip.</li>
<li>Mecanim: Fixed broken copy paste.</li>
<li>Mecanim: Fixed firing multiple events at 0.</li>
<li>ModuleManager: Fixed exception when opening the Module Manager window.</li>
<li>OpenGL: Fixed crash when trying to use unified OpenGL GfxDevice on MacOSX.</li>
<li>Plugins: Fixed Standalone settings, toggle buttons were showing platforms as disabled while in reality they were enabled.</li>
<li>PS3/PS4: Fixed some separate alpha blending shader states not working properly.</li>
<li>Samsung TV: Fixed an issue where games launched on the 2014 TVs without using the Unity Launcher would crash.</li>
<li>Scripting: Fixed debugger deadlock on OSX.</li>
<li>Scripting: Fixed MonoDevelop incorrectly stepping over recursive methods.</li>
<li>Scripting: Fixed Unity crash when using newer versions of the soft debugger client in MonoDevelop.</li>
<li>Terrain: Fixed occasional&nbsp;incorrect SpeedTree LOD.</li>
<li>Tizen: Display software keyboard correctly in landscape.</li>
<li>Tizen: Fixed some typed characters not displaying correctly.</li>
<li>Tizen: Removed unnecessary texture compression selector in the build window.</li>
<li>Tizen: Resolved "Failed to wait on semaphore" errors when script debugging.</li>
<li>Tizen: Resolved build failures when various non-alphanumeric are entered into the product description.</li>
<li>Tizen: Resolved rendering errors with Landscape Right screen orientation.</li>
<li>Tizen: Set the supported screen sizes key in the manifest. Not doing so results in Tizen store rejections.</li>
<li>Tizen: Text typed into software keyboard is now displayed.</li>
<li>Tizen: Updated product description field to prevent text wrapping issues.</li>
<li>Tizen: Video playback is now supported.</li>
<li>TreeEditor: Fixed incorrect labels and tooltips.</li>
<li>UNET: Client is not sending/receiving packets and does not disconnect.</li>
<li>UNet: Fixed an issue whereby NetworkTransform could corrupt SyncVars.</li>
<li>UNet: Fixed an issue whereby Network Serializer breaks on some 64-bit values.</li>
<li>UNet: Wrong interpolation in NetworkTransform has been fixed.</li>
<li>UNet: Added fixes for multiple NetworkClient objects.</li>
<li>UNET: Fixed: Memory continuously builds up with uNet server simply activated.</li>
<li>UNET: Fixed: Ping from obsolete connection can cause problem with functionality of new connection.</li>
<li>UNET: Fixed: Reliable sequenced channel for reused (disconnect then connect) connection stop working.</li>
<li>UNett: Fix for bad error message on networked commands.</li>
<li>Unified GL: Fixed mobile bloom and mobile blur shaders (and anything else that used array inputs).</li>
<li>Unified GL: Fixed VFACE translation. Unified GL: Shader .cginc include files failed to load if the file to be included had UTF BOM. Fixed.</li>
<li>VR: Render scale now functions correctly with 0.6 Oculus SDK.</li>
<li>VR: Render scale now works in deferred mode.</li>
<li>VR: VR.loadedDevice now works at runtime.</li>
<li>WebPlugin: Fixed cross-domain policy bypass issue (reported by Jouko Pynnonen of Klikki Oy).</li>
<li>XboxOne: Fixed a crash that occurs in the debug player at startup.</li>
</ul>
