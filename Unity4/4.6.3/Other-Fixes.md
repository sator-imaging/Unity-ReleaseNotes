# Unity 4.6.3

https://unity3d.com/unity/whats-new/unity-4.6.3

## Other Fixes



*   2D: Detect when Sprite.Create is called with an invalid rectangle.
*   2D: Fixed sprite UV calculation when mipmapped NPOT sprites were used for sliced UI elements.
*   AI: Fixed crash when exceeding maximum polygon count in a tile (4096).
*   AI: Fixed no result when calling NavMesh.SamplePosition with infinity range argument.
*   AI: NavMeshObstacle carving tessellation fixes.
*   AI: Prevent occasional hang when path is requested to an invalid position (degenerate values).
*   Android: Added support for ATC decompression on x86.
*   Android: Fixed black screen when using some ImageEffects on Adreno 2xx devices.
*   Android: Fixed crash on some NullReferenceExceptions.
*   Android: Fixed TextureAtlasses with only RGBA4444 textures.
*   Animation: Fixed animation event not always fired when they are at the limit of transition end.
*   BlackBerry: Deploy tools on OSX now have execute flag set properly.
*   Deployment Management: Prevent simultaneous launches of Unity loading wrong project.
*   Editor: Fixed occasional crash when switching between DX9 and DX11 in the editor.
*   iOS: Fixed a crash due to unaligned memory access.
*   iOS: Fixed a crash in physics code on iOS 6.x and older.
*   iOS: Fixed a typo in UnityRegisterMainViewControllerListener().
*   iOS: Fixed Chinese/Japanese keyboard dismissing itself when scrolling suggestions on iPhone.
*   iOS: Fixed crashes on iOS 5 devices.
*   iOS: Fixed performance drop for iPhone 6+ in Zoomed Mode.
*   iOS: Fixed sound stopping to work when using OnAudioFilterRead.
*   iOS: Fixed the issue where Unity doesn't check if startUnity() has been called.
*   iOS: Fixed various issues with Xcode project handling.
*   Linux: Fixed "fullscreen to native resolution" for window managers that resize the window many times while full-screening.
*   Oculus Plugin: Fixed editor crash when trying to open a project with Oculus Plugin present and an issue with Plugins not being detected if moved in the Plugins folder.
*   Physics: Changing only Z position of an object which has a Rigidbody2D component no longer disturbs its X/Y interpolation.
*   Scripting: Fixed issue in Mono that threw "Mono.Security.Protocol.Tls.TlsException: Bad record MAC" exception.
*   Scripting: Fixed plugin verification crash on reload/shutdown.
*   Scripting: Fixed regression in StopCoroutine(Coroutine) error message.
*   Scripting: Fixed rare crashes on Webplayer which is most likely to happen on x64.
*   Shaders: Fixed some blending modes (e.g. One Zero, Zero Zero) only working in editor.
*   UI: Disabling an InputField clears the caret data now.
*   UI: Fixed a memory leak with Text objects.
*   UI: Fixed an issue where the ObjectField was not configured to look at the correct time.
*   UI: Fixed an issue with calling disabled from OnEndEdit.
*   UI: Fixed a render-to-texture issue of UI elements.
*   UI: Fixed keyboard not displaying on mobile devices.
*   UI: Fixed menu items in GameObject > UI menu not having spaces between words. They now match component names as shown in the Inspector and in the Component menu.
*   UI: Fixed screen space camera canvas using a uninitialized camera.
*   UI: Fixing issue with setting InputField.value on mobile devices.
*   UI: Make “ignore parent group” work properly with selectable and Graphic.
*   UI: Maximum allowed internal font size (after pixels per unit have been applied) is now clamped to a maximum of 1000 to prevent majority of cases of the font rendering becoming very slow.
*   UI: Prevent characterCountVisible from getting the length of a null string.
*   UI: Prevent deleting selection from calling OnValueChanged multiple times.
*   UI: Prevent InputField caret from positioning based on layout.
*   Webcam: Fixed webcam detection on x86 first time creating WebCamTexture with empty device name.
*   WebPlayer: Unity 2.x content is no longer supported on modern OSes (Windows 8+, Mac OS X 10.9+).
*   Windows Standalone: Adding/removing game controllers should be detected more reliably now.
*   Windows Standalone: Fallback to XInput 1.0 when XInput 1.3 is not installed on the system.
*   Windows Store Apps: Fixed architecture specific plugin copying.
*   Windows Store Apps: Fixed InvokeOnAppThread/InvokeOnUIThread from scripts.