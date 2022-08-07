# Unity 4.1.2
https://unity3d.com/unity/whats-new/unity-4.1.2

## Fixes

<ul>
<li>Android: Fixed touch and stylus input on devices having a single surface emitting both at the same time.</li>
<li>Android: Fixed performance regression with static batching.</li>
<li>Android: Added a workaround for android issue 41755 - ANR when using apple magic mouse.</li>
<li>Android: Fixed an issue where "Stream from disc" audio was really slow when used with the "Split Application Binary" option.</li>
<li>Android: Fixed an issue where "Stream from disc" audio was broken when used with the "Split Application Binary" option.</li>
<li>DX11: Fixed GPU profiler not working (regression in 4.1).</li>
<li>Fix Crash in libmono.so due to GC_abort.</li>
<li>Fix ArgumentException: Invalid platform target" when trying to switch platform.</li>
<li>Graphics: Fixed Graphics.activeColorBuffer, activeDepthBuffer etc. crash when there's no active render target (regression in 4.1).</li>
<li>GUI: Modal GUI windows are now always on top of all other Unity GUIs, regardless of GUI.depth value.</li>
<li>GUI: When right-clicking on a window, context-menu events are once again being fired properly.</li>
<li>Native Client: Fixed "Development Player" label showing on non-development players.</li>
<li>Shuriken: Fixed an issue where particle rotations were broken.</li>
<li>Social API: Fixed problem loading leaderboard scores in Mac OS X 10.8 GameCenter.</li>
<li>UnityEngine.dll and UnityEditor.dll are no longer signed/strong-named. Compiled assemblies can once again reference the UnityEditor and UnityEngine namespaces.</li>
<li>Web Player: Chain of Trust system now requires signed assemblies to be loaded with new Security.LoadAndVerifyAssembly method in order to be eligible to call Security.GetChainOfTrustValue. Values stored in the Chain of Trust are still only accessible to assemblies signed with the specified public key.</li>
<li>Webplayer: Fixes a bug where using the WWW class in the web player would cause 50ms hiccups for each instance.</li>
<li>Webplayer: Application.ExternalEval and Application.ExternalCall will now properly escape Javascript strings with embedded escape sequences.</li>
</ul>
