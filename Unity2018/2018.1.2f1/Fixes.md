# Unity 2018.1.2f1
https://unity3d.com/unity/whatsnew/unity-2018.1.2

## Fixes

<ul>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/984967/">984967</a>) - Android: Fixed setting Screen.fullScreen = false does not leave fullscreen mode.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/969473/">969473</a>) - Android: Fixed android activity indicator showing navigation bar, and disapearing on touch.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/965024/">965024</a>) - Android: Fixed possible crash with Performance Reporting enabled.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/980524/">980524</a>) - Editor: Fixed profiler binary log file being locked until Editor restart.</li>
<li>(1006497) - Editor: Fixed self profiling errors in deep profiling mode.</li>
<li>(None) - Editor: Fixed "warning" profiler samples visualization in the Hierarchy View.</li>
<li>(1008911) - IMGUI: Fixed some GUI TextArea overloads incorrectly rendering as single line.</li>
<li>(None) - XR: Fixed the VRModule getting incorrectly stripped if il2cpp was enabled and nothing referenced VRModule.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1014048/">1014048</a>) - 2D: Fixed Undo operations on the Tile palette where Undo changes are not displayed.</li>
<li>(1032009) - 2D: Fixed Tiles not showing up visually on the Tile palette.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1018424/">1018424</a>) - 2D: Fixed "Invalid AABB" Exception occuring when adding SpriteShape controller to Scene with empty sprites list.</li>
<li>(1021441) - Android: Android: Fixed shader clip support on devices with Adreno 4x and later.</li>
<li>(None) - Graphics: Enabled 32bit index buffers on Intel GPUs starting macOS 10.13.4.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/970414/">970414</a>) - Particles: Fixed MissingReferenceException errors in the console caused by the Standard Particle Shader UI.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1006947/">1006947</a>) - Particles: Set up batching info for systems with 0 particles, to improve dynamic batching.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1013161/">1013161</a>) - Particles: Fixed the getter for the rateOverDistance script API property did not work correctly.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1017529/">1017529</a>) - Particles: Fixed LineRenderer sometimes failing to update after changing the startWidth/endWidth properties from script.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1006435/">1006435</a>) - Particles: Fixed crash when using curves set to different modes per axis, in the Velocity Module.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/994938/">994938</a>) - Particles: Fixed situation where particle bounds could be calculated incorrectly, when using Shape Module scale.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/998680/">998680</a>) - Particles: Fixed "Invalid AABB b0" errors when ParticleSystem.Emit is called.</li>
<li>(1009868) - Graphics: Fixed incorrect normal mapping on the LineRenderer due to incorrect Tangents.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1012983/">1012983</a>) - Particles: Fixed pivot offset not taking Transform scale into account when using Mesh particles.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1010992/">1010992</a>) - Particles: Fixed crash when changing Max Particles setting during Play Mode when using the Noise Module.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1005222/">1005222</a>) - Particles: Fixed issue where Trail would start dropping points 1 frame late, after calling Clear.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1007147/">1007147</a>) - Particles: Added error when using Texture in the Shape Module that is not set to Read/Write.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/985457/">985457</a>) - Graphics: Fixed GLCore API crash when using indirect buffer as rw buffer.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1001595/">1001595</a>) - Timeline: Fixed Memory Leak from Animation Tracks when using AssetBundles.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1011557/">1011557</a>) - Graphics: Fixed SRP crash.</li>
<li>(None) - Package Manager: Fixed issues when a custom registry URL included a path after the host name was configured.</li>
<li>(1027346) - Graphics: Fixed Android/OpenGLES Cubemap native texture not being registered correctly causing cubemap CopyTexture to native texture to fail. This also fixed Oculus Cubemap overlays not rendering.</li>
<li>(1025562) - XR: Fixed incorrect FPS when switching into VR mode on mobile devices.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/988019/">988019</a>) - Graphics: Fixed depth buffer when using cube map array.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1008501/">1008501</a>) - Editor: Fixed The Editor is failing to check the CacheServer when increasing AssetPostProcessor Version and adding new assets.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1025354/">1025354</a>) - IL2CPP: Added generic argument types to inflated generic method names that are shown in missing method exceptions.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1020262/">1020262</a>) - IL2CPP: Fixed an issue with call-by-reference method arguments not being properly preserved in certain circumstances.</li>
<li>(1019586) - IL2CPP: Fixed an error during code conversion related to a missing RGCTX entry for type T that can occur with an unbox opcode for a nullable type.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/995136/">995136</a>) - IL2CPP: Improved the speed of System.Object.ReferenceEquals() method.</li>
<li>(1022765) - IL2CPP: Fixed object files in msvc response files not separated with newlines instead of spaces. Prevents long-line errors in large builds.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1022755/">1022755</a>) - IL2CPP: Fixed the behavior of BinaryFormatter with the new scripting runtime.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1005597/">1005597</a>) - IL2CPP: Fixed crash when calling NativeArray.Equals.</li>
<li>(None) - IL2CPP: Fixed memory corruption in threadpool code, which sometimes manifested as a crash when scheduled work to threadpool.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/964886/">964886</a>) - Animation: Fixed an issue where modifying a Playable Graph playing AnimationClips in Editor would not play newly added clips.</li>
<li>(1034871) - XR: Added 64bit Google VR libraries to match the experimental 64bit support for Android.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/991264/">991264</a>) - Animation: Fixed crash when you modify a controller in a PlayableGraph while in playmode.</li>
</ul>

#### Revision: a46d718d282d
