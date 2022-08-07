# Unity 2017.4.11f1
https://unity3d.com/unity/whatsnew/unity-2017.4.11

## Fixes

<ul>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/955711/">955711</a>) - 2D: Fix Compressed ETC Variant Sprite Atlases become corrupted when changing their scale with target platform set to Android.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/953849/">953849</a>) - Android: Fixes issue where Android keyboard crashes app when selecting text in Input field on some Sony and Samsung devices.</li>
<li>(None) - Animation: Changed default StateMachine node width so that all nodes align vertically.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1066253/">1066253</a>) - Editor: Fixed an issue where supply a null parameter to UpdateTransformMask would cause Unity to crash while importing/re-importing - an FBX asset.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/975732/">975732</a>) - Editor: Fix assets are not created from drop down menu if any projectSettings are opened in inspector.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1010840/">1010840</a>) - Editor: GPU Profiling depends on the real state of graphics jobs and not project settings; '-force-gfx-jobs off' will allow profiling - and profiling in Editor is now possible.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1065223/">1065223</a>) - IL2CPP: Fixed deadlock on exit when calling back to managed code on a thread that doesn't exit before player shutdown.</li>
<li>(1071863 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1027837/">1027837</a>)) - Input: Fixed mouse event callbacks for multiple camera viewports.</li>
<li>(1076353 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1054444/">1054444</a>)) - Physics: Fixed a crash triggered by changing cook option on a deactivated mesh collider.</li>
<li>(1076350 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1025263/">1025263</a>)) - Physics: Fix a performance regression when using Continuous collision detection on kinematic bodies.</li>
<li>(1072966 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/825035/">825035</a>)) (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1043613/">1043613</a>) - Prefab: Reverting changes on applied prefab - crashes Unity.</li>
<li>(1006498 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/996666/">996666</a>)) - Profiler: Fixed self profiling errors in deep profiling mode.</li>
<li>(1073342) - PS4: Billboarding tree rendering now works correctly when using PSVR.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1051378/">1051378</a>) - UI: Fixed issue where animation would take precedence over layout component positioning.</li>
<li>(None) - Version Control: Editor Fix potential crash when calling Provider.GetLatest Jake Turner.</li>
<li>(1072548) - Vita: Fixed failure when creating Vita patch packages containing files of 2GB or larger.</li>
<li>(1029569) - XR: Fix failure to render Splash Screen when using Oculus.</li>
<li>(1067986 (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1025433/">1025433</a>) - XR: Fix Play mode crash when continually running Windows MR in editor.</li>
</ul>

#### Revision: 8c6b8ef6d111
