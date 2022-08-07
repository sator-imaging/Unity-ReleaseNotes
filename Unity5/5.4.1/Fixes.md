# Unity 5.4.1
https://unity3d.com/unity/whats-new/unity-5.4.1

## Fixes


#### Unity 5.4.1 also includes relevant fixes from 5.3.6 patch releases.
<ul>
<li>AI: Fixed an issue where 'Not Walkable' objects close to the ground would not create a hole in the navmesh when baked. (820608)</li>
<li>Android: Editor: Added a workaround for AAPT sometimes crashing for no good reason. (797965)</li>
<li>Animation: Fixed a crash that happened when disabling a gameobject during animation-triggered physics callbacks. (813681)</li>
<li>Animation: Fixed a crash inCreateAnimatorGenericBindings when attempting to use AnimationMixerPlayable on start of a game object. (820203)</li>
<li>Animation: Fixed a crash when adding AnimationClip to an enabled Animation component whilst in play mode in the editor. (820586)</li>
<li>Animation: Fixed additive layer using disabled "Resample Animation" blended with layers that have it enabled. (822897)</li>
<li>Animation: Fixed an issue where an assert that couldn't be acted upon was popping in the AvatarMask inspector. (813105)</li>
<li>Collab: Fixed a crash when opening a cloud project named with numbers if you already have a project named the same in your folder. (763383)</li>
<li>DX11: Fixed editor spewing out "Failed to query D3D11 context for ID3DUserDefinedAnnotation interface" error message when run on Windows 7 machine without Windows updates installed. (819707)</li>
<li>Editor: Fixed a bug that launching Editor window will exit after signed on windows. (816567)</li>
<li>Editor: Fixed occasional freeze when profiling over network and connection is lost. (716213)</li>
<li>Editor: Fixed the inspector UI for some Renderers where Light Probe and Reflection Probe options were not displayed correctly. </li>
<li>Fixed performance regression of LightProbes.GetInterpolatedProbe API. &nbsp;&nbsp;GI:</li>
<li>GI: Fixed a crash in Reflection Probe component when multiple scenes are used. (811241)</li>
<li>GI: LightProbes.GetInterpolatedProbe will return a black probe now if there are no light probes in the scene. (815127)</li>
<li>GI: Multi-scene editor. Fixed the lightmap indices not updating for additively loaded scenes in the Editor. (745588)</li>
<li>Graphics: Fixed a crash when running with Graphics Jobs caused by one thread unloading mesh data whilst another thread is using the data. &nbsp;</li>
<li>Graphics: Fixed ForwardAdd pass z-fighting issue when the object is rendered with GPU instancing, for example when you have multiple lights (819088).</li>
<li>Surface shaders are automatically updated to apply the fix.</li>
<li>For custom vert/frag shaders, instead of using the macro "UNITY_USE_CONCATENATED_MATRICES", now please use the new "#pragma force_concat_matrix" directive in the ForwardAdd pass. &nbsp;</li>
<li>Graphics: Fixed image effects being rendered twice when the camera is instantiated from prefab or copying another camera. This issue was in player builds only. (814402, 811236)</li>
<li>Graphics: Fixed Texture3D not accepting floating point formats. (794440)</li>
<li>iOS: Added support for tbd files. (820487)</li>
<li>Kernel: Fixed a crash resulting from undo/redo after revert. (717587, 804333)</li>
<li>Linux: Don't unnecessarily clear mouse position. (816514)</li>
<li>Mono: Properly locate libMonoPosixHelper.dylib file in the editor on OS X when it is used. (810964)</li>
<li>Particles: Fixed an issue where the first vertex of a trail renderer could be missing. (823495)</li>
<li>Particles: Fixed particle system random seed regression. (782232)</li>
<li>Profiler: Fixed GPU profiling showing "N/A" for most draw calls, instead of associating with proper objects. (772640, 817337)</li>
<li>Tizen: Added a method to request the Evas_GL object to possibly be used in plugins. &nbsp;</li>
<li>Tizen: Added API compatibility control. Currently only 2.3 and 2.4 are supported. &nbsp;</li>
<li>Tizen: Fixed a problem where UnityPluginUnload was not called. &nbsp;</li>
<li>Tizen: Fixed problem with hangs when using a static splash screen image. (806041)</li>
<li>Tizen: Fixed the screen dimensions being incorrect when rotating the screen on Tizen while playing video. (805148)</li>
<li>Tizen: Removed an error which wrote privilege value in duplicate in tizen-manifest.xml. &nbsp;</li>
<li>Tizen: Support multiple sensor listener. &nbsp;</li>
<li>UnityWebRequest: Fixed errors in console when downloading texture. (813763)</li>
<li>UnityWebRequest: Fixed memory leak and possible crash when doing multiple request using the same object.</li>
<li>UnityWebRequest: Fixed possible freeze when downloading more than 64k of data using custom download handler. (820517)</li>
<li>UnityWebRequest: Fixed texture download reporting done before texture is actually usable. (814330)</li>
<li>UnityWebRequest: Report downloaded bytes for asset bundles and properly report 1.0 progress when finished. (815185)</li>
<li>VR: Fixed crash when exiting VR in certain cases where the HMD was detected as not connected on the first frame. &nbsp;</li>
<li>VR: Fixed GL.LoadPixelMatrix() not working when Single-Pass Stereo was enabled. (811511)</li>
<li>VR: Fixed possible crash on shutdown. (817745)</li>
<li>VR: Fixed viewport scale issues with OpenVR.</li>
<li>WebGL: Fixed compressed build files (*.gz) creation if they already exist. (818044)</li>
<li>Windows Store: Generate code in exported solution to enter fullscreen if "Default is Fullscreen" is set in player settings. (804577)</li>
<li>Windows Store: Suppress system overlays by default in il2cpp solutions (makes it consistent with .NET). (817285)</li>
<li>WWW: Fixed occasional crashes in il2cpp projects. (796508)</li>
</ul>

#### Revision: 649f48bbbf0f
