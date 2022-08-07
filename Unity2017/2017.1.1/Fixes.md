# Unity 2017.1.1
https://unity3d.com/unity/whats-new/unity-2017.1.1

## Fixes

<ul>
<li>2D: Fixed an issue where adjusting Collider2D's Offset when Using Tiled Draw Mode and Auto Tiling would result in inconsistent behaviour.     -  (917931) </li>
<li>2D: Fixed an issue where Sprite from the same atlas not hashed &amp; packed correctly.    -  (927372)</li>
<li>2D: Fixed an issue where the Editor became unresponsive when switching from OpenGL to Metal with a tiled sprite in the scene.     -  (918524)</li>
<li>2D: Fixed an issue whereby Sprite Atlas variant would pack without an error when master was compressed with crunched.     -  (935388)</li>
<li>2D: Fixed console showing error when multiple selecting asset while locking Sprite Atlas inspector and Pack.  -  (920773)</li>
<li>Android: [VideoPlayer] H264 video doesn't loop on HTC One (OS 4.2.2)  -  (925738) </li>
<li>Android: Apps no longer signed with signature scheme v2 when building for oculus.          </li>
<li>Android: Buildpipe - Correctly split resources between APK and OBB when building with LZ4.    -  (920359)</li>
<li>Android: Fixed a development build crash on Android 4.2.2 with VideoCore GPU.     -  (922553) </li>
<li>Android: Fixed a Vulkan error when trying to use anisotropic filtering on Mali GPUs.       </li>
<li>Android: Fixed an issue having lots of VBOs allocated even for an empty scene on Android during application startup.  -  (937875)</li>
<li>Android: Fixed an issue where spot and point lights were too bright on low-end devices.   -  (918785) </li>
<li>Android: Fixed an issue where spot and point lights were too bright on low-end devices.   -  (918785) </li>
<li>Android: Fixed an issue with alpha texture size in ETC1 texture compression with split alpha.     -  (918605)</li>
<li>Android: Fixed the issue where OBB was not available after installing from Google Play on some phones until device was restarted.</li>
<li>Android: Gradle - Do not explicitly set debuggable attribute when building with Gradle to avoid lint security warning.    -  (910280)</li>
<li>Android: Gradle - Handle too many errors; filter out warnings and detect too long error list.      </li>
<li>Android: Gradle - Make sure unity3d and other files from raw/ are uncompressed in the APK.    -  (924518)</li>
<li>Android: SoftInput - Fixed the autocorrection not being disabled on Samsung phones.   -  (906014) </li>
<li>Android: SoftInput - Fixed the NamePhonePad flag.     -  (924515)</li>
<li>Animation: Fixed a crash in Animator Editor window when closing Unity.    -  (918033)</li>
<li>Animation: Fixed a crash in Animator Editor window when closing Unity.    -  (918032)</li>
<li>Animation: Fixed a crash that was caused during the assignment of an incomplete AnimatorController stored in an AssetBundle.  -  (927443)</li>
<li>Animation: Fixed a crash when changing number of input in AnimationLayerMixerPlayable at runtime.     -  (922283)</li>
<li>Animation: Fixed a crash when changing OverrideController during interrupted transition.  -  (928601)</li>
<li>Animation: Fixed a glitch that was causing a stuttering in the Animation curve when rotating a GameObject in the Animation window.    -  (930335)</li>
<li>Animation: Fixed a regression that was preventing Math symbols from being evaluated in the Animation window's input field.    -  (930987)</li>
<li>Animation: Fixed an issue of AnimatorState's WriteDefaults not working properly on very specific setups.  -  (893779) </li>
<li>Animation: Fixed an issue where the Animation events would not trigger if animation had less than two frames.     -  (921121) </li>
<li>Animation: Fixed an issue where the Animator's State Machine would start to flicker in Playmode if the Animator window was too small to display the active State.     -  (917195) </li>
<li>Animation: Fixed an issue whereby AnimatorState's WriteDefaults was not working properly on very specific setups.     -  (893779) </li>
<li>Animation: Fixed bad frame when changing Playable Graph during StateMachineBehaviours.      </li>
<li>Animation: Fixed Generic animation layers affecting base humanoid root motion.    -  (928562)</li>
<li>Asset Bundles: Fixed an issue where calling LoadAllAssets with a type parameter could cause loading errors.   -  (930819) </li>
<li>Asset Bundles: Fixed an issue where IK float values weren't blending.     -  (920973) </li>
<li>Build Pipeline: Fixed an assert and potential crash when building projects with Materials or Shader Variant Collections which reference missing shaders ie deleted.   -  (885275) </li>
<li>Build Pipeline: Fixed an issue with enabling Split Application Binary flag in Android player settings would affect other platforms.   -  (919307)</li>
<li>Build Pipeline: Fixed incorrect mesh channel stripping when mesh was used as a shape emitter in particle systems.     -  (917568) </li>
<li>Collab: Added softlocks to project browser in single-column mode.     -  (918761)</li>
<li>Collab: Fixed an issue where user was not prompted to save local scene edits before updating.     -  (907960)</li>
<li>Collab: Fixed update, immediately cancel, update again, crash.    -  (923508)</li>
<li>Collaborate: Fixed an issue with the initial collaborate publish where it will continuously retry upon failure.   -  (932469)</li>
<li>Editor: Calculate mipmap count properly when importing NPOT textures with '-nographics'.  -  (925913) </li>
<li>Editor: Ensure that an asset preview is always provided.  -  (858928) </li>
<li>Editor: Fixed a case of "Generate Lighting" drop down menu being hidden when inspector was resized to minimal width.  -  (915524) </li>
<li>Editor: Fixed a crash when loading scenes created in Unity versions before 2017.1 with specific lighting setup.   -  (932793)</li>
<li>Editor: Fixed a performance regression that cause very long startup time when invoking a test run.    -  (900957) </li>
<li>Editor: Fixed an issue in the Inspector Window that prevented the 'Nothing Selected' component from being shown.  -  (925505)</li>
<li>Editor: Fixed in-launcher names of projects loaded via relative path.     -  (873823) </li>
<li>Editor: Fixed LookDev rendering issues:&nbsp;Frame to object feature, Initial position of prefabs in LookDev. -     </li>
<li>Editor: Fixed one case of importing projects from very old Unity versions.      </li>
<li>Editor: Fixed player build success notification.  </li>
<li>Editor: Fixed screen capture.     -  (932630) </li>
<li>Editor: Fixed Security Vulnerability UNITYSEC-844-<a href="/security">https://unity3d.com/security</a>    </li>
<li>Editor: Fixed the inability to rename a objects in the Hierarchy view if LookDev was open.    -  (908324)</li>
<li>GI: Fix to only show clustering view when realtime GI is on, or when baking is on with Enlighten.     -  (911953)</li>
<li>GI: Progressive Lightmapper: Fixed a crash in light probe rendering occurring when changing or removing probes.  </li>
<li>GI: Progressive Lightmapper: Fixed an issue where alpha cutoff was not properly converting values.    </li>
<li>GI: Progressive Lightmapper: Fixed an issue where auto-mode did not detect when changing material values for alpha cutoff.  </li>
<li>Graphics: Changed every instance of the string "Custom Texture" to "Custom Render Texture" in menus and tooltips.     -  (924625) </li>
<li>Graphics: Cubemap Custom Render Texture initialization is now applied to all faces (regardless of active face update flags).       </li>
<li>Graphics: Don't enable blending on unsupported pixel formats on Metal.    -  (920781) </li>
<li>Graphics: Ensure textures are not created with too high mip count on Metal.   -  (915959)</li>
<li>Graphics: Fixed "Tiled GPU perf. warning: RenderTexture color surface was not cleared/discarded doing..." in Unity when emulating OpenGL ES 2.0 or 3.0.   -  (909148) </li>
<li>Graphics: Fixed a crash in Custom Render Texture when switching target platforms in the Editor.   -  (925171) </li>
<li>Graphics: Fixed a crash on exit from fullscreen player when using OpenGLCore graphics API.    -  (922715) </li>
<li>Graphics: Fixed a crash when a valid Mesh had no submeshes.   -  (918642) </li>
<li>Graphics: Fixed a crash when adding CommandBuffers during OnPreCull callabck and visualizing occlusion data with lighting enabled.    -  (902870) </li>
<li>Graphics: Fixed a crash when instancing is enabled on specific Material.  -  (911654) </li>
<li>Graphics: Fixed a crash when using Compute Shader with very large number of thread groups i.e. greater than 500,000.  -  (826751)</li>
<li>Graphics: Fixed a crash when Vulkan loader was installed but no drivers were installed and Vulkan was used as the default API.    -  (898184) </li>
<li>Graphics: Fixed a deadlock when building lighting in Editor or during a player build.     -  (918993) </li>
<li>Graphics: Fixed a rare (could happen in very complex scenes) crash/hang when graphics jobs were enabled.  -  (918788)</li>
<li>Graphics: Fixed a rare case when shader compilation failed with error message "Failed to find parameters of a compiled D3D9 shader".  -  (918636) </li>
<li>Graphics: Fixed a rare crash caused by recursive rendering ie. Camera.Render() or Water rendering.    -  (878317) </li>
<li>Graphics: Fixed an issue where lights did not render correctly when using a camera with a RenderTexture and non-fullscreen viewport.  -  (910659) </li>
<li>Graphics: Fixed an issue where overlapping cameras drawing to the same target would not composite correctly.  -  (923842) </li>
<li>Graphics: Fixed an issue whereby Terrain not showing wireframe in shaded-wireframe mode.  -  (922739) </li>
<li>Graphics: Fixed an issue which after clearing occlusion data occlusion view volumes were still visible.   -  (911910)</li>
<li>Graphics: Fixed an occasional glitch when rendering lines/trails.     -  (903807) </li>
<li>Graphics: Fixed different sampling on sRGB RenderTextures compared to non-sRGB RenderTextures when in Gamma space in standalone players.  -  (909829) </li>
<li>Graphics: Fixed dynamic batching overwriting the vertex colour stream on untextured meshes.   -  (803067) </li>
<li>Graphics: Fixed GPU profiler block for Custom Texture Update.          </li>
<li>Graphics: Fixed importing of single channel uint16 textures.  -  (909569) </li>
<li>Graphics: Fixed incorrect shadows appearing in the scene view when visualizing occlusion culling.     -  (694728)</li>
<li>Graphics: Fixed lighting rendering when using multiple cameras and at least one camera renders to a RenderTexture.    -  (903537) </li>
<li>Graphics: Fixed loading shaders in a variant collection not loading the variants from all passes which match.          </li>
<li>Graphics: Fixed memory leak in Editor scene view.     -  (916425)</li>
<li>Graphics: Fixed memory leak in Texture2DArray and CubeMapArrayTexture.    -  (920547)</li>
<li>Graphics: Fixed Mesh becoming offset and scaled when accessing 'mesh' property on a MeshFilter on a static GameObject and static batching was enabled.    -  (733687) </li>
<li>Graphics: Fixed Nav Mesh Preview in Scene View being affected by lighting.    -  (913612) </li>
<li>Graphics: Fixed OpenGL debug labels when using OpenGL ES.     </li>
<li>Graphics: Fixed OpenGL ES debug labels.   </li>
<li>Graphics: Fixed rendering issues when using a camera with a RenderTexture and non-fullscreen viewport.    -  (910036) </li>
<li>Graphics: Fixed runtime crash when modifying skinned mesh and GPU Skinning is enabled.    -  (811757) </li>
<li>Graphics: Fixed sRGB flag returning false on the LDR target texture from a HDR to LDR image effect in a linear project.   -  (912603) </li>
<li>Graphics: Fixed the scale and rotation matrix on the PreviewRenderUnility Camera having no effect.    -  (914676) </li>
<li>Graphics: Improved line and trail rendering, when trying to display overlapping/nearby points     -  (848934, 827583) </li>
<li>Graphics: Rendering optimistion for GLES graphics API.    -  (917105)</li>
<li>IL2CPP: Fixed a crash in QueryComponentByType when animation was used with engine code stripping enabled and there was no Sprite Renderer component in any scene in the build.    -  (919058) </li>
<li>IL2CPP: Fixed various crashes.    -  (929802, 930163, 930252) </li>
<li>IL2CPP: Prevent a compilation error in the generated code for some Windows Store apps.<br> 
<ul>
<li>Prevent a failure during code conversion when a constrained method call is made on a volatile type.</li>
<li>Prevent a possible crash in List.AddRange.     -  (921467, 936096, 929802, 930163) </li>
</ul></li>
<li>iOS: Fixed 'Stale touch detected!' error message that showed up after minimizing, re-opening an app and immediate start tapping the screen with multiple fingers.     -  (934901)</li>
<li>iOS: Fixed an issue where Unity would not generate icons for Spotlight and Notifications in a Xcode project.  -  (918406)</li>
<li>iOS: Fixed auto-rotation on ReplayKit.    -  (911935) </li>
<li>iOS: Fixed trampoline compilation issues for iOS 11 simulator.         </li>
<li>iOS: Rewrote the internal clock system and replaced it with a system that took into account the time when the device was asleep. Also, the startup time is now calculated more accurately.    -  (912594)</li>
<li>iOS: Use YIELD for atomic_pause on ARM.   -  (938975)</li>
<li>Launcher: Fixed an issue that Web Signin would print loading error in Editor.log (with access token).     -  (938693)</li>
<li>Launcher: Fixed the issue where Remember me did not work when using the Web hosted sign in.     </li>
<li>Launcher: Fixed the issue where Remember me did not work when using the Web hosted sign in.   </li>
<li>Launcher: Fixed the launcher offline issue.   -  (938742) </li>
<li>Linux: Addiitonal fix for initializing screen dimensions (mouse input).   -  (880426) </li>
<li>Linux: Associate provided icon with player window now.    -  (912675) </li>
<li>Linux: Fallback to xinerama/xvidmode for video modes initialization if xrandr fails.       </li>
<li>Linux: Use default player icon when none is provided.     -  (912675) </li>
<li>Mono: Restored the "Use micro mscorlib" stripping option for Android.     -  (916064) </li>
<li>Multiplayer: Fixed an issue where reliable messages exchanging had been staled after a couple of hours.    </li>
<li>Multiplayer: Fixed an issue where reliable messages&nbsp;exchanging&nbsp;had been staled after couple of hours.</li>
<li>Networking: UnityWebRequest: Fixed an issues where cookies were not sent on redirect.     -  (832192) </li>
<li>OSX: Fixed a crash when WebCamTexture is used.    -  (917133) </li>
<li>Particles: Detect when a new mesh is selected in the Shape Module, and update the Scene View preview accordingly.     -  (900928) </li>
<li>Particles: Ensure trails are properly initialized when particles are being manipulated via script.    -  (899881) </li>
<li>Particles: Fixed an issue where bounding boxes were too small on some systems, causing culling problems.  -  (914333) </li>
<li>Particles: Fixed mesh particles becoming inverted when using render alignment- View.      -  (927395) </li>
<li>Particles: Fixed use of Unscaled delta time in Edit Mode.     -  (910018) </li>
<li>Physics: Fixed an issue where ContactPoint2D.normalImpulse and ContactPoint2D.tangentImpulse were always zero when accessing via callbacks.   -  (927637) </li>
<li>Platforms: Fixed a crash when '-cleanedLogFile' was passed but no log file name was given.    -  (859361) </li>
<li>Scripting Upgrade: Fixed a crash when System.Reflection.Emit was used to generate assemblies for the AppDomain.AssemblyResolve event.     -  (920772) </li>
<li>Scripting Upgrade: Fixed an exception when calling 'System.Reflection.MonoProperty.GetterAdapterFrame' on AOT platforms.  -  (930594) </li>
<li>Scripting Upgrade: Fixed export package window tree structure.    -  (934518) </li>
<li>Scripting Upgrade: Fixed memory corruption/crash after domain reload when using Assembly.Load(Byte[]).    -  (923165) </li>
<li>Scripting Upgrade: Improved distribution of Guid.GetHashCode().   -  (930644) </li>
<li>Scripting: Fixed a crash when invoking LINQ expressions in Editor.    -  (920085) </li>
<li>Scripting: Fixed a potential domain reload issue in play mode when trying to validate scripts.    -  (926516) </li>
<li>Scripting: Fixed an issue when using SimplifyPoints and the provided array was too small.      </li>
<li>Scripting: Fixed an issue where the send function from our synchronization context would fail to execute on the main thread.  -  (934819) </li>
<li>Scripting: Fixed managed debugger on Windows hanging when all scripts with OnAudioFilterRead have been disabled.  -  (918651) </li>
<li>Scripting: Fixed scripting exception being logged as Info instead of Error.   -  (912719) </li>
<li>Scripting: Fixed WWW class being unsafe for multiple invocations of Dispose().    -  (931213) </li>
<li>Services: Fixed an issue where Performance Reporting symbol upload tool could crash.  -  (927884)</li>
<li>Shaders: Fixed GLSL shader compile errors due to lack of default precision specifier.     -  (899502) </li>
<li>Shaders: Vulkan - Fixed a rare incorrect shader generation on expressions with write masks.   -  (908903)</li>
<li>Terrain: Fixed a crash that could happen when you have a very large number of terrains with SpeedTree trees on them.  -  (929987) </li>
<li>Terrain: Fixed an issue where error messages about JobTempAlloc would appear in player output log if trees were used on a terrain.    -  (898262) </li>
<li>Timeline: Fixed a crash when using Timeline with a MacOS player.  -  (926710) </li>
<li>Timeline: Fixed inconsistencies in root motion position between Editor and Player.    -  (926701) </li>
<li>Timeline: Fixed root motion on humanoid characters when there were no base animation clips.   -  (934535)</li>
<li>Timeline: Fixed View Settings in Timeline getting reset when going into Play Mode.    -  (923506)</li>
<li>Timeline: Rebuild Graph performances improvements.<br> 
<ul>
<li>Preventing clips from drawing outside of the visible area.      </li>
</ul></li>
<li>UI: Fixed memory leaks caused by unreleased Meshs in the UI Profiler.     -  (912789)</li>
<li>UI: GraphicRaycaster and EventSystem performance improvements.    -  (934842)</li>
<li>UI: InputField - For Name content type, use NamePhonePad touch screen keyboard type   -  (924515)</li>
<li>UI: Sprite Atlas variant will display correct on Image component.     -  (935390)</li>
<li>Universal Windows Platform: Fixed building generated UWP projects with Visual Studio 2017.3 when using .NET scripting backend. </li>
<li>UWP: Fixed the issue where locking the mouse in UWP player would cause wrong values returned from Input.GetAxis() on the next Update.     -  (911008) </li>
<li>Video: Fixed MovieTexture support for Metal.  -  (911115) </li>
<li>WebGL: Fixed compilation crashing with node on windows 7 64 bits.     -  (929988) </li>
<li>WebGL: Fixed Corrupted Sprites on MS Edge.    -  (904449) </li>
<li>WebGL: Fixed Corrupted Sprites on MS Edge.    -  (904449) </li>
<li>Windows: Crash dumps are written to users' Persistent Data Path, resolving an issue where installing Unity games to Program Files caused crash dumps to fail.     -  (928646)</li>
<li>WWW: Return null from WWW.error if there's no error, now. This was causing issues in Android when attempting to display information fetched from Facebook.    -  (934502)</li>
<li>XR: Added missing Editor icons for world anchor, spatial mapping, touch input, and audio spatialization components.   -  (857023) </li>
<li>XR: Added VRUsage parameter to GetTemporary(). This fixes an issue with blitting to a temporary renderTexture.    -  (918634) </li>
<li>XR: Fixed an issue where stereo Convergence setting had no actual impact.     -  (923806)</li>
</ul>

#### Revision: 5d30cf096e79
