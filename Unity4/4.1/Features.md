# Unity 4.1
https://unity3d.com/unity/whats-new/unity-4.1

## Features

<ul>
<li>Profiler: Memory profiler makes it posible to view a snapshot of currently loaded game objects and assets, and shows the reason why an object is in memory. Memory usage of a player can also be viewed by connecting to the player from the editor. 
<ul>
<li>Simple vs. Complex view type dropdown button in the memory area.</li>
</ul></li>
<li>Substance: Procedural textures are now supported at runtime on iOS and Android (ARM v7a only, NEON needed for optimal performance).</li>
<li>Mecanim: 2D Blend Nodes for Blend Trees. 2D Blend Nodes are like regular blend nodes except you can blend based on two float parameters instead of one. Supported 2D blend types are Simple Directional, Freeform Directional, and Freeform Cartesian.</li>
<li>Graphics: Custom Material Editors! A shader can have CustomEditor keyword which points to an editor class that derives from MaterialEditor. This is useful for setting per material shader keywords from the UI.</li>
<li>Graphics: Per-material shader keywords. You can now set shader keywords on a per material basis. This allows for less work maintaining shaders and turning on and off parts of a shader with keywords.</li>
<li>iOS: full multi-screen support (AirPlay). Look for added Display class for an array of connected displays (only iOS is properly implemented now - all other platforms will have only one display in there).</li>
<li>Mac OS X Standalone: added GameCenter support.</li>
<li>Graphics: Rendering with shader replacement now supports lighting. If you render a camera with a replacement shader, the camera will pick the shader that corresponds to the current camera rendering path (forward / deferred / vertex lit).</li>
<li>Graphics: Camera.SetTargetBuffers added, allowing you to set buffers to draw to from RenderTexture or from screen; or to share depth buffer between different cameras.</li>
<li>Added Transform.hasChanged flag that can be used to check if the transform's position/rotation/scale has been altered since the last time hasChanged was set to 'false'.</li>
<li>Audio: Added scripting API support for sample-precision stitching of audio clips and synchronized DSP effects (AudioSettings.dspTime, AudioSource.PlayScheduled, AudioSource.SetScheduledStartTime, AudioSource.SetScheduledEndTime)</li>
<li>Editor: Console can now be filtered by Errors, Warnings, and Logs.</li>
<li>Shadows: Hardware shadow map filtering on capable mobile platforms (EXT_shadow_samplers; most recent iOS devices, very few Android devices yet). Makes shadow edges look a bit nicer, at some performance cost (used only when Light has shadows set to "Soft").</li>
<li>Mecanim: API for recording.</li>
<li>Mecanim: Can now change AnimatorController at runtime.</li>
</ul>
