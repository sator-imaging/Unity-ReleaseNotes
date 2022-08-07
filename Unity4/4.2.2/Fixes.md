# Unity 4.2.2
https://unity3d.com/unity/whats-new/unity-4.2.2

## Fixes

<ul>
<li>Graphics: Fixed RenderTexture reload warnings in editor's mobile graphics emulation mode, when deferred lighting is used with no lights present.</li>
<li>Graphics: Fixed Image Effects crash in some cases when an effect does camera.Render() from inside of OnRenderImage (regression in 4.2).</li>
<li>Shadows: Fixed broken soft shadows in scene view when Linear color space + skybox are used (regression in 4.2).</li>
<li>Editor: Fixed major progress bar leak on OSX editor.</li>
<li>BlackBerry: Fixed case where large device hardware PINs would not work with debug token reading/creation.</li>
<li>BlackBerry: Player settings now include stripping level option.</li>
<li>Memory: Fixed memory leak when instantiating materials from code.</li>
<li>iOS: Fixed documentation for Texture2D.CreateExternalTexture.</li>
<li>iOS: Fixed Build&amp;Run with Xcode 5.</li>
<li>iOS: Fixed status bar issue on iOS7.</li>
<li>iOS: Fixed WebCamTexture problems on iOS7.</li>
<li>iOS: Fixed crash if user selected OpenGL ES 3.0 graphics API (OpenGL ES 3.0 is currently Android-only).</li>
<li>Android: Yet another fix for "Unable to find suitable jdk installation".</li>
</ul>
