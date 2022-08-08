# Unity 4.1

https://unity3d.com/unity/whats-new/unity-4.1

## Improvements



*   Android: Added caching of shader binaries for faster load time, if available in the GLES driver (GL\_OES\_get\_program\_binary extension).
*   Android: Propagation of native crashes (callstack etc.) to the Google Play Error Reporter. This include native plugins and script callstacks.
*   Android: Added multiple render target support on NVIDIA (GL\_NV\_draw\_buffers and GL\_NV\_fbo\_color\_attachments).
*   Audio: Added AudioSource.ignoreListenerPause to enable playback of sounds in menus and editor extensions while AudioListener.pause=true
*   Audio: It is now possible to query play position and Microphone read position from a different thread than the main thread. This can be used to lower the latency of processing microphone input, by adaptively regulating playback speed.
*   Editor: Scene view can be set to render with shader replacement, SceneView.SetSceneViewShaderReplace.
*   Editor: CustomEditors can now optionally apply for subclasses of the class they're editing. Use \[CustomEditor(typeof(MyClass), true)\] to also make a custom editor work for MyClass' children
*   Editor: Confirmation for losing prefab connection now only comes up once when dragging multiple child objects out of a prefab.
*   Editor: Display Unity version in Project Wizard dialog title.
*   Editor: Files with the FNT extension will now be imported as TextAssets (before they were of unknown type).
*   Editor: It's now possible to move MonoBehaviours from one game object to another via drag & drop.
*   Graphics: Added depth parameter to GL.Clear, for cases when you want to clear depth buffer to non-1.0 value.
*   Graphics: Added SystemInfo.maxTextureSize.
*   Graphics: ARGBHalf, RGHalf, RHalf, R8 render texture formats supported on modern OpenGL & OpenGL ES 2.0 devices.
*   Graphics: Improved handling of non-power-of-two texture sizes.
    *   On most platforms, a NPOT-sized texture without mipmaps and with Clamp wrapping mode will be actually represented as NPOT size texture on the GPU. This lowers memory usage and greatly improves loading times for NPOT texture sizes.
    *   NPOT-sized uncompressed textures with mipmaps are faster as well, if the GPU supports arbitrary texture sizes (most modern PC GPUs do).
    *   Added SystemInfo.npotSupport.
*   Input: You can now control which layers get OnMouse\* events via Camera.eventMask. Setting it to zero turns off the mouse events, improving performance.
*   Installers: New icons and other artwork for OS X installers.
*   iOS: "iPhoneBundleIdentifier not set up" demoted to warning.
*   iOS: Device physical architecture is reported more accurately, though in lowercase (like 'armv7s').
*   iOS: Info.plist now will be appended instead of overwriting it.
*   iOS: Minor PhysX performance improvements.
*   iOS: Total amount of physical memory is reported more accurately.
*   Linux: Associate project icon with player window.
*   Linux: Implement nographics batch mode.
*   Linux: Statically link libstdc++ for greater compatibility with older installations.
*   Mecanim: AssetBundles work with Mecanim.
*   Mecanim: Ability to drag States and StateMachines into sub StateMachines.
*   Mecanim: Mirror and Cycle offset available on States and BlendTree leafs (no need to duplicate animation for mirroring anymore).
*   Mecanim: Allow multi-editing of Animator components.
*   Mecanim: Context menu to delete States and StateMachines.
*   Mecanim: Copy Paste of State/StateMachine also copies missing parameters.
*   Mecanim: Transitions are only reorderable in the context of a State.
*   Profiler: It is now possible to connect to a player by manually typing the IP of the device where the player is running - in case of multiple players on the same IP, it will connect to the player listening on the lowest port (which is randomly assigned).
*   Resources.UnloadUnusedAssets() has been rewritten. It is around 4x faster than in Unity 4.0 and works much better in a game that streams levels in and out. The unloading is now using precise garbage collection (previously it was based on Mono's built-in GC, which is conservative). Fixes strange corner cases with the old system, where in the worst case it could reload prefabs from disk during unloading.
*   Shaders: Added SubShader tag "ForceNoShadowCasting". When this tag is present, no shadows will be cast from this object, even if shader has a shadow caster pass somewhere.
*   Shaders: Sampler precision support for mobile, you can use sampler2D\_half, sampler2D\_float, samplerCUBE\_half, samplerCUBE\_float types which will translate into mediump & highp samplers for GLES2.0.
*   Shaders: Shaders will now use the shadow caster pass of the selected subshader if a shadow pass exists. If no shadow pass exists it will fallback to the default shadow pass.
*   Substance: decrease the memory overhead of Substance instances created at runtime.
*   Substance: If present, the more user friendly input "labels" are displayed in the Inspector instead of the input "names".
*   Substance: Input groups and HSL adjustments are now presented as foldouts in the Inspector.
*   Substance: Less code is embedded in the various Unity players.
*   Substance: lower memory consumption when dealing with multi-graph Substances.
*   Substance: New "Use caching" load behavior for Substances (textures are written to disk/flash after being generated and are reloaded from there at subsequent app/game launches).
*   Substance: On mobile platforms "Compressed" Substance textures are now compressed at runtime to DXT or PVRTC if supported by the GPU.
*   Substance: Procedural textures can now be read in the runtime API (ProceduralTexture.GetPixels32). Substances must be set to RAW and have the isReadable property set for GetPixels32 to work.
*   Substance: Updated Substance engines for all platforms (faster rendering, better threading, lower memory consumption).
*   Substance: XML presets can now be read from / applied to substances in the runtime API.