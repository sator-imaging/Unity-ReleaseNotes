# Unity 4.1
https://unity3d.com/unity/whats-new/unity-4.1

## Improvements

<ul>
<li>Android: Added caching of shader binaries for faster load time, if available in the GLES driver (GL_OES_get_program_binary extension).</li>
<li>Android: Propagation of native crashes (callstack etc.) to the Google Play Error Reporter. This include native plugins and script callstacks.</li>
<li>Android: Added multiple render target support on NVIDIA (GL_NV_draw_buffers and GL_NV_fbo_color_attachments).</li>
<li>Audio: Added AudioSource.ignoreListenerPause to enable playback of sounds in menus and editor extensions while AudioListener.pause=true</li>
<li>Audio: It is now possible to query play position and Microphone read position from a different thread than the main thread. This can be used to lower the latency of processing microphone input, by adaptively regulating playback speed.</li>
<li>Editor: Scene view can be set to render with shader replacement, SceneView.SetSceneViewShaderReplace.</li>
<li>Editor: CustomEditors can now optionally apply for subclasses of the class they're editing. Use [CustomEditor(typeof(MyClass), true)] to also make a custom editor work for MyClass' children</li>
<li>Editor: Confirmation for losing prefab connection now only comes up once when dragging multiple child objects out of a prefab.</li>
<li>Editor: Display Unity version in Project Wizard dialog title.</li>
<li>Editor: Files with the FNT extension will now be imported as TextAssets (before they were of unknown type).</li>
<li>Editor: It's now possible to move MonoBehaviours from one game object to another via drag &amp; drop.</li>
<li>Graphics: Added depth parameter to GL.Clear, for cases when you want to clear depth buffer to non-1.0 value.</li>
<li>Graphics: Added SystemInfo.maxTextureSize.</li>
<li>Graphics: ARGBHalf, RGHalf, RHalf, R8 render texture formats supported on modern OpenGL &amp; OpenGL ES 2.0 devices.</li>
<li>Graphics: Improved handling of non-power-of-two texture sizes. 
<ul>
<li>On most platforms, a NPOT-sized texture without mipmaps and with Clamp wrapping mode will be actually represented as NPOT size texture on the GPU. This lowers memory usage and greatly improves loading times for NPOT texture sizes.</li>
<li>NPOT-sized uncompressed textures with mipmaps are faster as well, if the GPU supports arbitrary texture sizes (most modern PC GPUs do).</li>
<li>Added SystemInfo.npotSupport.</li>
</ul></li>
<li>Input: You can now control which layers get OnMouse* events via Camera.eventMask. Setting it to zero turns off the mouse events, improving performance.</li>
<li>Installers: New icons and other artwork for OS X installers.</li>
<li>iOS: "iPhoneBundleIdentifier not set up" demoted to warning.</li>
<li>iOS: Device physical architecture is reported more accurately, though in lowercase (like 'armv7s').</li>
<li>iOS: Info.plist now will be appended instead of overwriting it.</li>
<li>iOS: Minor PhysX performance improvements.</li>
<li>iOS: Total amount of physical memory is reported more accurately.</li>
<li>Linux: Associate project icon with player window.</li>
<li>Linux: Implement nographics batch mode.</li>
<li>Linux: Statically link libstdc++ for greater compatibility with older installations.</li>
<li>Mecanim: AssetBundles work with Mecanim.</li>
<li>Mecanim: Ability to drag States and StateMachines into sub StateMachines.</li>
<li>Mecanim: Mirror and Cycle offset available on States and BlendTree leafs (no need to duplicate animation for mirroring anymore).</li>
<li>Mecanim: Allow multi-editing of Animator components.</li>
<li>Mecanim: Context menu to delete States and StateMachines.</li>
<li>Mecanim: Copy Paste of State/StateMachine also copies missing parameters.</li>
<li>Mecanim: Transitions are only reorderable in the context of a State.</li>
<li>Profiler: It is now possible to connect to a player by manually typing the IP of the device where the player is running - in case of multiple players on the same IP, it will connect to the player listening on the lowest port (which is randomly assigned).</li>
<li>Resources.UnloadUnusedAssets() has been rewritten. It is around 4x faster than in Unity 4.0 and works much better in a game that streams levels in and out. The unloading is now using precise garbage collection (previously it was based on Mono's built-in GC, which is conservative). Fixes strange corner cases with the old system, where in the worst case it could reload prefabs from disk during unloading.</li>
<li>Shaders: Added SubShader tag "ForceNoShadowCasting". When this tag is present, no shadows will be cast from this object, even if shader has a shadow caster pass somewhere.</li>
<li>Shaders: Sampler precision support for mobile, you can use sampler2D_half, sampler2D_float, samplerCUBE_half, samplerCUBE_float types which will translate into mediump &amp; highp samplers for GLES2.0.</li>
<li>Shaders: Shaders will now use the shadow caster pass of the selected subshader if a shadow pass exists. If no shadow pass exists it will fallback to the default shadow pass.</li>
<li>Substance: decrease the memory overhead of Substance instances created at runtime.</li>
<li>Substance: If present, the more user friendly input "labels" are displayed in the Inspector instead of the input "names".</li>
<li>Substance: Input groups and HSL adjustments are now presented as foldouts in the Inspector.</li>
<li>Substance: Less code is embedded in the various Unity players.</li>
<li>Substance: lower memory consumption when dealing with multi-graph Substances.</li>
<li>Substance: New "Use caching" load behavior for Substances (textures are written to disk/flash after being generated and are reloaded from there at subsequent app/game launches).</li>
<li>Substance: On mobile platforms "Compressed" Substance textures are now compressed at runtime to DXT or PVRTC if supported by the GPU.</li>
<li>Substance: Procedural textures can now be read in the runtime API (ProceduralTexture.GetPixels32). Substances must be set to RAW and have the isReadable property set for GetPixels32 to work.</li>
<li>Substance: Updated Substance engines for all platforms (faster rendering, better threading, lower memory consumption).</li>
<li>Substance: XML presets can now be read from / applied to substances in the runtime API.</li>
</ul>
