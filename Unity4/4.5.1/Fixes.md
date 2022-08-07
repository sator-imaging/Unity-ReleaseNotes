# Unity 4.5.1
https://unity3d.com/unity/whats-new/unity-4.5.1

## Fixes

<ul>
<li>2D: Very thin down-scaled textures will now produce sprites correctly.</li>
<li>2D: Fixed auto-simplification of sprite meshes. Considerably less vertices/triangles will be generated.</li>
<li>Editor: Fixed ETC2/ASTC texture display for lower mip levels when the editor is run in DX11 mode</li>
<li>Graphics: Fixed GUIText not being shown if it only consists of Unicode characters</li>
<li>iOS: Fixed case of resolution/orientation setting when Unity player takes only part of the screen</li>
<li>iOS: Fixed Unity Remote touch event queuing under stress conditions</li>
<li>iOS: Fixed 2D rendering when sprite does not have tangents, but has normals</li>
<li>iOS: fixed autorotation issues on iOS 8</li>
<li>iOS: fixed Xcode project build under Xcode6 preview</li>
<li>iOS: fixed splashscreen misrecognition for iOS Free license users on iPad-only apps</li>
<li>iOS: fixed corner case of RenderTexture creation</li>
<li>iOS: fixed lighting being broken while starting in landscape orientation</li>
<li>Linux/OSX: Fix linear lighting when antialiasing is enabled in upscaled fullscreen mode.</li>
<li>Linux: Fix initial cursor visibility setting when antialiasing is enabled.</li>
<li>Linux: Fix asset bundle caching.</li>
<li>MonoDevelop: Fix to correctly close MonoDevelop when not in focus on OS X. MonoDevelop will no longer prevent logging out.</li>
<li>OSX: Fix stack trace generation on crash.</li>
<li>OSX: Fixed PS3/PS4 bluetooth pads crashing editor when run.</li>
<li>Windows Phone/Windows Store Apps: Unity now correctly marshals Collision2D.relativeVelocity to C# code</li>
<li>Windows Phone: Fixed clearing splashscreen if camera in first scene has no clear flag</li>
<li>Windows Phone: Input.gyro.gravity now correctly returns data from orientation sensor</li>
<li>Windows Phone: Fixed an issue which caused compressed meshes to blink in certain situations</li>
<li>Windows Phone/Windows Store Apps: Unity will now correctly build player if plugins use .NET 4.5 APIs that are not available in .NET 3.5</li>
<li>Windows Phone: Input.GetJoystickNames now returns an empty string rather than preventing player build</li>
<li>Windows Phone/Windows Store Apps: Fixed an issue which caused player crash when Collider2D NonAlloc API variants were used</li>
</ul>
