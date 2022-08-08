# Unity 4.1.2

https://unity3d.com/unity/whats-new/unity-4.1.2

## Fixes



*   Android: Fixed touch and stylus input on devices having a single surface emitting both at the same time.
*   Android: Fixed performance regression with static batching.
*   Android: Added a workaround for android issue 41755 - ANR when using apple magic mouse.
*   Android: Fixed an issue where "Stream from disc" audio was really slow when used with the "Split Application Binary" option.
*   Android: Fixed an issue where "Stream from disc" audio was broken when used with the "Split Application Binary" option.
*   DX11: Fixed GPU profiler not working (regression in 4.1).
*   Fix Crash in libmono.so due to GC\_abort.
*   Fix ArgumentException: Invalid platform target" when trying to switch platform.
*   Graphics: Fixed Graphics.activeColorBuffer, activeDepthBuffer etc. crash when there's no active render target (regression in 4.1).
*   GUI: Modal GUI windows are now always on top of all other Unity GUIs, regardless of GUI.depth value.
*   GUI: When right-clicking on a window, context-menu events are once again being fired properly.
*   Native Client: Fixed "Development Player" label showing on non-development players.
*   Shuriken: Fixed an issue where particle rotations were broken.
*   Social API: Fixed problem loading leaderboard scores in Mac OS X 10.8 GameCenter.
*   UnityEngine.dll and UnityEditor.dll are no longer signed/strong-named. Compiled assemblies can once again reference the UnityEditor and UnityEngine namespaces.
*   Web Player: Chain of Trust system now requires signed assemblies to be loaded with new Security.LoadAndVerifyAssembly method in order to be eligible to call Security.GetChainOfTrustValue. Values stored in the Chain of Trust are still only accessible to assemblies signed with the specified public key.
*   Webplayer: Fixes a bug where using the WWW class in the web player would cause 50ms hiccups for each instance.
*   Webplayer: Application.ExternalEval and Application.ExternalCall will now properly escape Javascript strings with embedded escape sequences.