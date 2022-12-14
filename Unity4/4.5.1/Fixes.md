# Unity 4.5.1

https://unity3d.com/unity/whats-new/unity-4.5.1

## Fixes



*   2D: Very thin down-scaled textures will now produce sprites correctly.
*   2D: Fixed auto-simplification of sprite meshes. Considerably less vertices/triangles will be generated.
*   Editor: Fixed ETC2/ASTC texture display for lower mip levels when the editor is run in DX11 mode
*   Graphics: Fixed GUIText not being shown if it only consists of Unicode characters
*   iOS: Fixed case of resolution/orientation setting when Unity player takes only part of the screen
*   iOS: Fixed Unity Remote touch event queuing under stress conditions
*   iOS: Fixed 2D rendering when sprite does not have tangents, but has normals
*   iOS: fixed autorotation issues on iOS 8
*   iOS: fixed Xcode project build under Xcode6 preview
*   iOS: fixed splashscreen misrecognition for iOS Free license users on iPad-only apps
*   iOS: fixed corner case of RenderTexture creation
*   iOS: fixed lighting being broken while starting in landscape orientation
*   Linux/OSX: Fix linear lighting when antialiasing is enabled in upscaled fullscreen mode.
*   Linux: Fix initial cursor visibility setting when antialiasing is enabled.
*   Linux: Fix asset bundle caching.
*   MonoDevelop: Fix to correctly close MonoDevelop when not in focus on OS X. MonoDevelop will no longer prevent logging out.
*   OSX: Fix stack trace generation on crash.
*   OSX: Fixed PS3/PS4 bluetooth pads crashing editor when run.
*   Windows Phone/Windows Store Apps: Unity now correctly marshals Collision2D.relativeVelocity to C# code
*   Windows Phone: Fixed clearing splashscreen if camera in first scene has no clear flag
*   Windows Phone: Input.gyro.gravity now correctly returns data from orientation sensor
*   Windows Phone: Fixed an issue which caused compressed meshes to blink in certain situations
*   Windows Phone/Windows Store Apps: Unity will now correctly build player if plugins use .NET 4.5 APIs that are not available in .NET 3.5
*   Windows Phone: Input.GetJoystickNames now returns an empty string rather than preventing player build
*   Windows Phone/Windows Store Apps: Fixed an issue which caused player crash when Collider2D NonAlloc API variants were used