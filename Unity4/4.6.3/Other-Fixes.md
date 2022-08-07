# Unity 4.6.3
https://unity3d.com/unity/whats-new/unity-4.6.3

## Other Fixes

<ul>
<li>2D: Detect when Sprite.Create is called with an invalid rectangle.</li>
<li>2D: Fixed sprite UV calculation when mipmapped NPOT sprites were used for sliced UI elements.</li>
<li>AI: Fixed crash when exceeding maximum polygon count in a tile (4096).</li>
<li>AI: Fixed no result when calling NavMesh.SamplePosition with infinity range argument.</li>
<li>AI: NavMeshObstacle carving tessellation fixes.</li>
<li>AI: Prevent occasional hang when path is requested to an invalid position (degenerate values).</li>
<li>Android: Added support for ATC decompression on x86.</li>
<li>Android: Fixed black screen when using some ImageEffects on Adreno 2xx devices.</li>
<li>Android: Fixed crash on some NullReferenceExceptions.</li>
<li>Android: Fixed TextureAtlasses with only RGBA4444 textures.</li>
<li>Animation: Fixed animation event not always fired when they are at the limit of transition end.</li>
<li>BlackBerry: Deploy tools on OSX now have execute flag set properly.</li>
<li>Deployment Management: Prevent simultaneous launches of Unity loading wrong project.</li>
<li>Editor: Fixed occasional crash when switching between DX9 and DX11 in the editor.</li>
<li>iOS: Fixed a crash due to unaligned memory access.</li>
<li>iOS: Fixed a crash in physics code on iOS 6.x and older.</li>
<li>iOS: Fixed a typo in UnityRegisterMainViewControllerListener().</li>
<li>iOS: Fixed Chinese/Japanese keyboard dismissing itself when scrolling suggestions on iPhone.</li>
<li>iOS: Fixed crashes on iOS 5 devices.</li>
<li>iOS: Fixed performance drop for iPhone 6+ in Zoomed Mode.</li>
<li>iOS: Fixed sound stopping to work when using OnAudioFilterRead.</li>
<li>iOS: Fixed the issue where Unity doesn't check if startUnity() has been called.</li>
<li>iOS: Fixed various issues with Xcode project handling.</li>
<li>Linux: Fixed "fullscreen to native resolution" for window managers that resize the window many times while full-screening.</li>
<li>Oculus Plugin: Fixed editor crash when trying to open a project with Oculus Plugin present and an issue with Plugins not being detected if moved in the Plugins folder.</li>
<li>Physics: Changing only Z position of an object which has a Rigidbody2D component no longer disturbs its X/Y interpolation.</li>
<li>Scripting: Fixed issue in Mono that threw "Mono.Security.Protocol.Tls.TlsException: Bad record MAC" exception.</li>
<li>Scripting: Fixed plugin verification crash on reload/shutdown.</li>
<li>Scripting: Fixed regression in StopCoroutine(Coroutine) error message.</li>
<li>Scripting: Fixed rare crashes on Webplayer which is most likely to happen on x64.</li>
<li>Shaders: Fixed some blending modes (e.g. One Zero, Zero Zero) only working in editor.</li>
<li>UI: Disabling an InputField clears the caret data now.</li>
<li>UI: Fixed a memory leak with Text objects.</li>
<li>UI: Fixed an issue where the ObjectField was not configured to look at the correct time.</li>
<li>UI: Fixed an issue with calling disabled from OnEndEdit.</li>
<li>UI: Fixed a render-to-texture issue of UI elements.</li>
<li>UI: Fixed keyboard not displaying on mobile devices.</li>
<li>UI: Fixed menu items in GameObject &gt; UI menu not having spaces between words. They now match component names as shown in the Inspector and in the Component menu.</li>
<li>UI: Fixed screen space camera canvas using a uninitialized camera.</li>
<li>UI: Fixing issue with setting InputField.value on mobile devices.</li>
<li>UI: Make “ignore parent group” work properly with selectable and Graphic.</li>
<li>UI: Maximum allowed internal font size (after pixels per unit have been applied) is now clamped to a maximum of 1000 to prevent majority of cases of the font rendering becoming very slow.</li>
<li>UI: Prevent characterCountVisible from getting the length of a null string.</li>
<li>UI: Prevent deleting selection from calling OnValueChanged multiple times.</li>
<li>UI: Prevent InputField caret from positioning based on layout.</li>
<li>Webcam: Fixed webcam detection on x86 first time creating WebCamTexture with empty device name.</li>
<li>WebPlayer: Unity 2.x content is no longer supported on modern OSes (Windows 8+, Mac OS X 10.9+).</li>
<li>Windows Standalone: Adding/removing game controllers should be detected more reliably now.</li>
<li>Windows Standalone: Fallback to XInput 1.0 when XInput 1.3 is not installed on the system.</li>
<li>Windows Store Apps: Fixed architecture specific plugin copying.</li>
<li>Windows Store Apps: Fixed InvokeOnAppThread/InvokeOnUIThread from scripts.</li>
</ul>
