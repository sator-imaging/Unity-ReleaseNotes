# Unity 2019.1
https://unity3d.com/unity/whats-new/2019.1.0

## Backwards Compatibility Breaking Changes

<ul>
<li><p>2D: Grid Cell Size's z-value for 'Isometric Z as Y' Grids now affects the local z-coordinates of all cells in the Grid.</p></li>
<li><p>2D: The Grid Cell Size's default z-value is set to 1 when creating new Isometric Tilemaps or Tile Palettes.</p></li>
<li><p>Android: Increased required Android build tools version to 28.0.3</p></li>
<li><p>Android: Made blit mode force to "Never blit" when SRP is active.</p></li>
<li><p>Android: Removed the internal build system</p></li>
<li><p>Android: Updated Android Gradle plugin to version 3.2</p></li>
<li><p>Android: Updated bluetooth headset detection on Android 6+ to avoid using deprecated method</p></li>
<li><p>Android: Updated Bundletool to version 0.6.0</p></li>
<li><p>Asset Import: Removed normal calculation options in the Sketchup Importer Inspector.</p></li>
<li><p>Asset Import: <strong>Generate Back Faces</strong> is now enabled by default in the Sketchup Importer Inspector.</p></li>
<li><p>Asset Pipeline: The Model importer mesh read/write setting is now disabled by default.</p></li>
<li><p>Editor: Changed default shortcut for "Stage/Go Back" from O to H to avoid shortcut conflict in project templates.</p></li>
<li><p>Editor: Merged the <strong>Shortcut Profile</strong> drop-down and the <strong>Shortcut Profile</strong> options cog into a single dropdown.</p></li>
<li><p>Editor: Removed support for compiling UnityScript and Boo scripts.</p></li>
<li><p>Editor: Unity no longer tries to attach to a console in the Editor when using batch mode on Windows. Instead, it redirects to stdout. Unity only provides logging if you launch the Editor in such a way that it has a valid stdout handle. As a result, Unity no longer tramples your command window output in batchmode.</p></li>
<li><p>Editor: Updated Editor so that Shortcut Profiles can no longer start or end with spaces. Also disallowed some special characters. (<a href="https://issuetracker.unity3d.com/issues/shortcut-manager-profile-list-does-not-handle-profile-names-properly-when-names-start-with-spaces">1103117</a>)</p></li>
<li><p>Editor: Usage of DescriptionAttribute to change the display name of enum values in the inspector has been removed. (<a href="https://issuetracker.unity3d.com/issues/drawdefaultinspector-displays-enums-differently-from-editorguilayout-dot-enumpopup-when-using-cusom-inspector">1115381</a>, 1130991)</p></li>
<li><p>GI: Moved tetrahedralization code to the player.</p></li>
<li><p>GI: Reduced the frequency with which Unity issues LightmapSettings warnings.</p></li>
<li><p>GI: Stitching and probe deringing are now turned on by default.</p></li>
<li><p>Graphics: Added override for LightmapEmissionFlagsProperty to allow the display of emission GI options without checking for an emissision color property (<code>_EmissionColor</code>).</p></li>
<li><p>Graphics: Attempting to use recursive rendering in SRP now yields an error</p></li>
<li><p>Graphics: CommandBuffer.IssuePluginCustomBlit now passes the depth UnityRenderBuffer to the native plugin if 'dest' is a depth texture.</p></li>
<li><p>Graphics: Disabled support for rendering projectors in Scriptable Render Pipelines.</p></li>
<li><p>Graphics: Dynamic batching checkbox is now hidden if a Scriptable Render Pipeline is active.</p></li>
<li><p>Graphics: LODGroup.ForceLODMask now allows int.MaxValue to force cull the whole LODGroup.</p></li>
<li><p>Graphics: Removed graphics emulation from Editor.</p></li>
<li><p>Graphics: Texture Mipmap streaming in the Unity Editor's Edit Mode now defaults to enabled when <strong>Texture Streaming</strong> is enabled in <strong>Quality Settings</strong>.</p></li>
<li><p>Graphics: The ASTC compressor quality options "fast" and "best" are now different from "normal".</p></li>
<li><p>Graphics: Updated graphics packages (LWRP, HDRP, and Shader Graph) to 5.2.3 and tweaked Scenes inside accordingly.</p></li>
<li><p>Graphics: [Metal] Debug groups are now visible in Release builds.</p></li>
<li><p>iOS: Updated Game View resolution options with iPhone XR/XS/XS Max</p></li>
<li><p>iOS: <code>UnityWebRequest</code> uses a new backend based on <code>NSURLSession</code>. The old <code>NSURLConnection</code> backend is still available and has been commented out in Trampoline.</p></li>
<li><p>Linux: Deprecated Linux x86 and Universal targets. These are due to be removed in future Unity versions.</p></li>
<li><p>Mobile: Changed minimum iOS version to 9.0</p></li>
<li><p>Multiplayer: Moved the multiplayer high level API from an extension DLL to a package. Projects should automatically update with a reference to the package the first time they open in 2019.1.</p></li>
<li><p>Physics: Increased the default maximum angular velocity to 50 radian per second, because the default value was too low.</p></li>
<li><p>Scripting: Added support for serialisation for struct <code>UnityEngine.Rendering.SphericalHarmonicsL2</code>. (922290)</p></li>
<li><p>Universal Windows Platform: Removed the .NET scripting backend.</p></li>
<li><p>WebGL: Removed asm.js PreBuilt Engine option.</p></li>
<li><p>WebGL: Removed <strong>Memory Size</strong> and <strong>Linker Target</strong> options from Editor.</p></li>
<li><p>WebGL: Renamed <code>gameInstance</code> to <code>unityInstance</code>.</p></li>
<li><p>WebGL: Set default compression to Brotli.</p></li>
<li><p>WebGL: Updated Emscripten to version 1.38.11.</p></li>
<li><p>Windows: Changed logfile names to be more consistent with other platforms: <code>Player.log</code> and <code>Player-prev.log</code>. The actual path is the same.</p></li>
<li><p>Windows: Disabled cursor locking and confinement in batch mode.</p></li>
<li><p>XR: Changed Oculus (Standalone) and OpenVR (Standalone) package names to Oculus (Desktop) and OpenVR (Desktop), respectively.</p></li>
<li><p>XR: Oculus Dash and Shared Depth Buffer options are now enabled by default in the Oculus XR settings.</p></li>
</ul>
