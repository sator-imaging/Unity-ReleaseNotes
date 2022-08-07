# Unity 5.0.1
https://unity3d.com/unity/whats-new/unity-5.0.1

## Improvements

<ul>
<li>Android: Added framebuffer clear on devices that would prefer framebuffer discard but don't have the required GLES extension.</li>
<li>Android: Added profiling stats for blit to screen and input processing.</li>
<li>Android: Joystick input optimization, fixes slowdown on some older devices.</li>
<li>Android: Parsing device specific XML font configurations to determine system/fallback fonts in addition to the hard-coded list of font names (in 4.6.4 too).</li>
<li>Android: Splash screen is now shown in full screen mode.</li>
<li>BlackBerry: Passport device now supports landscape orientation.</li>
<li>Bug reporter: Added info about license type.</li>
<li>Editor: Android; added ability to configure JDK path in the Editor preferences (in 4.6.4 too).</li>
<li>Editor: Android TV; added configuration option for D-pad and gamepad support level.</li>
<li>GI: Added pushoff for baked lighting, can be used to fix AO artefacts.</li>
<li>GI: Allow higher AO exponent in Lighting window.</li>
<li>GI: Don't calculate AO when AO exponent is 0.</li>
<li>GI: Fixed inconsistent Enlighten build timings; now it should correspond to wall clock time (unless you move at near speed of light relative to your computer, in which case it might still be wrong).</li>
<li>GI: Moved baked tag to the proper place in UI.</li>
<li>GI: Output more stats per system and in total: vertex count, face count, chart count and texel count.</li>
<li>GI: Removed an unnecessary warning that realtime GI is not supported on PS3 and Xbox360 when finishing a bake in non-continuous mode.</li>
<li>GI: Sped up baked lightmap compositing.</li>
<li>GI: Spit out timings of the precompute and bake to the Editor log. Timer resets when clearing GI data, exiting continuous mode or cancelling a bake.</li>
<li>GI: Take texture transparency into account when calculating AO.</li>
<li>GI: Users will now be warned when building scenes with Precomputed Realtime GI ticked on platforms that do not support Realtime GI.</li>
<li>Graphics: Shaders now read consistent values across platforms for vertex properties that are missing in a Mesh. We have adopted the OpenGL standard, which is that normals default to (0,0,1) and tangents default to (1,0,0).</li>
<li>iOS: Improve launch screen support: 
<ul>
<li>Added option to disable launch screen.</li>
<li>Added option to display relatively sized image on a specific background.</li>
</ul></li>
<li>iOS: Short term fix for occasional input stuttering (in 4.6.4 too).</li>
<li>iOS/Metal: Defer [CAMetalLayer nextDrawable] until it is actually needed (helps with occasional framerate hiccups) (in 4.6.4 too).</li>
<li>Linux: Query Mesa driver for amount of video memory when feasible.</li>
<li>Physics 2D: Allow SurfaceEffector2D to control whether friction or bounce is used upon contact.</li>
<li>Physics 2D: Allow SurfaceEffector2D to control whether the impulse force is applied to the center-of-mass or contact-point.</li>
<li>Physics 2D: Improve PointEffector2D.distanceScale tooltip/documentation.</li>
<li>Physics 2D: Joint2D property 'collideConnected' renamed to 'enableCollision' to match 3D physics.</li>
<li>Physics 2D: PlatformEffector2D property renames based upon feedback: oneWay-&gt;useOneWay, sideFriction-&gt;useSideFriction and sideBounce-&gt;useSideBounce.</li>
<li>Platforms: Unity Professional users can now optionally show the builtin Unity Splash Screen on applicable platforms, in Player Settings.</li>
<li>Version Control: Added shortcut to save changeset window.</li>
<li>Version Control: Added "delete empty changesets" button.</li>
<li>Version Control: Close change window automatically on success.</li>
<li>Version Control: New changesets default to expanded now.</li>
</ul>
