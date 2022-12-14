# Unity 3.5.6

https://unity3d.com/unity/whats-new/unity-3.5.6

## Fixes



*   Audio: Fixed AudioClip SetData and GetData to handle when the array passed in is longer than the clip itself.
*   Android: Fixed a rare case where libmono.so / libunity.so would not load due to "unable to link library".
*   Android: Added exception checking / propagation for script-based JNI Calls (AndroidJava\* / AndroidJNI\*).
*   Android: Enforce that System.Net.Sockets use is only allowed with an Android Pro license.
*   Android: Loading a lot of assets through Resources.Load() could create a memory-leak-like behavior - this has been fixed.
*   Android: Fixed EGL context recreation when post-effects are used.
*   Android: Fixed reverse portrait mode.
*   Android: Webcam resolution and frame rate selection is now more accurate.
*   Android: Webcam now works on Ice Cream Sandwich and JellyBean devices.
*   Android: Webcam now works on Motorola and OMAP devices.
*   Android: Microphone resources are now properly released when pausing the application.
*   Android: Audio should now play without any clicking noise on Kindle and Nook, although latency is still pretty bad.
*   Android: It should now be possible to play and record audio at the same time.
*   Android: Fixed issue where files with 'meta' in their name was not package in the apk.
*   Android: Gyro.attitude did not compensate for screen orientation, nor device natural orientation (phone/tablet) - this has been fixed.
*   Android: Restarting an application right after calling Application.Quit() could cause a race condition between quitting the old and starting the new process.
*   Android: Input.multiTouchEnabled was returning false before the screen received an initial touch.
*   Android: Changed some tags in the AndroidManifest to have required="false".
*   Android: Fixed a problem where non-development ('release') builds would fail to load on devices with kernel 3.4 and later.
*   Android: Autorotation with only either portrait or landscape modes is now enforced by the manifest as well.
*   Android: Fixed a fullscreen video issue where the video wouldn't display due to orientation being changed.
*   Android: Fixed an issue where the fullscreen video in some cases would start to play even though it was not yet visible.
*   Android: Fullscreen video no longer plays while the lock-screen is in effect.
*   Android: Back button will quit the application while the first level has not yet been loaded.
*   Android: Added Nexus7 (1280x800) to GameView settings.
*   Android: Runtime class Ping now works.
*   Android: Made sure OnScreenKeyboard can be opened again after being closed due to lost focus.
*   Android: Changing system time/date while application was running would cause an ANR.
*   Android: Fixed camera initialization on platforms without fps range support
*   Serialization: For non-webplayer-targets, scenes (implicitly) referencing assets placed under the Resources folder will now always have the assets placed together with the scene (and not in the resources.assets).
*   Editor: Updated PVR Texture Tool to 3.0@2144429
*   Graphics: Fixed batching issue with multiple lightmaps in the scene (now we sort by lightmap as well).
*   Graphics: Fixed error "Adding renderer during rendering is not allowed" when using Trail Renderer with reflective water.
*   Mobile: Texture.ReadPixels is no longer delayed, but prints error instead if called at the wrong time
*   iOS: Fixed ios6 compatibility.
*   iOS: Fixed various orientation issues.
*   iOS: Fixed basic license splashscreen compatibility with Xcode 4.5.
*   iOS: Added support for iPhone 5 tall splash screen.
*   iOS: Added support for rendering @ full res on iPhone 5.
*   iOS: Added iOS 6.0 target selection in PlayerSettings.
*   iOS: extracted video view controller to trampoline, provided ios6 specific interface to allow orientation control on ios6 and proper handling of orientation requests coming from video controller.
*   iOS: added supportedInterfaceOrientationsForWindow workaround for game center and friends, make it support all orientations.
*   iOS: fixed splash orientation issues on ios6 phone-like devices.
*   iOS: Unity Remote fixed to support iPhone 5 res.
*   Native Client: Fixed race condition when loading mono assemblies.
*   Terrain: Fixed crash when setting heightmapMaximumLOD to out-of-range values.
*   Webplayer: Fixed crash when running in-process in Firefox 15.
*   Windows: Fixed issue where batchmode players and webplayers could be limited only to run on cpu0