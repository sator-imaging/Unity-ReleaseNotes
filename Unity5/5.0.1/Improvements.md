# Unity 5.0.1

https://unity3d.com/unity/whats-new/unity-5.0.1

## Improvements



*   Android: Added framebuffer clear on devices that would prefer framebuffer discard but don't have the required GLES extension.
*   Android: Added profiling stats for blit to screen and input processing.
*   Android: Joystick input optimization, fixes slowdown on some older devices.
*   Android: Parsing device specific XML font configurations to determine system/fallback fonts in addition to the hard-coded list of font names (in 4.6.4 too).
*   Android: Splash screen is now shown in full screen mode.
*   BlackBerry: Passport device now supports landscape orientation.
*   Bug reporter: Added info about license type.
*   Editor: Android; added ability to configure JDK path in the Editor preferences (in 4.6.4 too).
*   Editor: Android TV; added configuration option for D-pad and gamepad support level.
*   GI: Added pushoff for baked lighting, can be used to fix AO artefacts.
*   GI: Allow higher AO exponent in Lighting window.
*   GI: Don't calculate AO when AO exponent is 0.
*   GI: Fixed inconsistent Enlighten build timings; now it should correspond to wall clock time (unless you move at near speed of light relative to your computer, in which case it might still be wrong).
*   GI: Moved baked tag to the proper place in UI.
*   GI: Output more stats per system and in total: vertex count, face count, chart count and texel count.
*   GI: Removed an unnecessary warning that realtime GI is not supported on PS3 and Xbox360 when finishing a bake in non-continuous mode.
*   GI: Sped up baked lightmap compositing.
*   GI: Spit out timings of the precompute and bake to the Editor log. Timer resets when clearing GI data, exiting continuous mode or cancelling a bake.
*   GI: Take texture transparency into account when calculating AO.
*   GI: Users will now be warned when building scenes with Precomputed Realtime GI ticked on platforms that do not support Realtime GI.
*   Graphics: Shaders now read consistent values across platforms for vertex properties that are missing in a Mesh. We have adopted the OpenGL standard, which is that normals default to (0,0,1) and tangents default to (1,0,0).
*   iOS: Improve launch screen support:
    *   Added option to disable launch screen.
    *   Added option to display relatively sized image on a specific background.
*   iOS: Short term fix for occasional input stuttering (in 4.6.4 too).
*   iOS/Metal: Defer \[CAMetalLayer nextDrawable\] until it is actually needed (helps with occasional framerate hiccups) (in 4.6.4 too).
*   Linux: Query Mesa driver for amount of video memory when feasible.
*   Physics 2D: Allow SurfaceEffector2D to control whether friction or bounce is used upon contact.
*   Physics 2D: Allow SurfaceEffector2D to control whether the impulse force is applied to the center-of-mass or contact-point.
*   Physics 2D: Improve PointEffector2D.distanceScale tooltip/documentation.
*   Physics 2D: Joint2D property 'collideConnected' renamed to 'enableCollision' to match 3D physics.
*   Physics 2D: PlatformEffector2D property renames based upon feedback: oneWay->useOneWay, sideFriction->useSideFriction and sideBounce->useSideBounce.
*   Platforms: Unity Professional users can now optionally show the builtin Unity Splash Screen on applicable platforms, in Player Settings.
*   Version Control: Added shortcut to save changeset window.
*   Version Control: Added "delete empty changesets" button.
*   Version Control: Close change window automatically on success.
*   Version Control: New changesets default to expanded now.