# Unity 3.5.3
https://unity3d.com/unity/whats-new/unity-3.5.3

## Improvements

<ul>
<li>Audio: Fixed audio distortion when using gapless MP3 encoding.</li>
<li>Cache Server: Fixed connection issues.</li>
<li>Development players will now show file names and line numbers in stack traces again.</li>
<li>Graphics: Added Optimize Mesh Data option to Player Settings. Turning it on will remove unused mesh components (e.g. will remove all tangent vectors if none of your shaders use normal mapping). Use this both for game size and runtime performance.</li>
<li>Graphics: Added Camera.transparencySortMode to control how transparent objects are sorted. If you use a perspective camera for a 2D game, you can have proper object sorting now!</li>
<li>Graphics: Mesh.Clear now will keep the existing vertex layout; this is more efficient if you are recreating meshes at runtime. If you want to completely clear the mesh, including vertex format layout, use mesh.Clear(false).</li>
<li>iOS: now automatic inclusion of native plugins will also respect "Symlink Unity libraries" flag. Turn this flag off when making archive builds.</li>
<li>Native Client: Fixed crashes in script code in 64-bit NaCl (64-bit Windows or Linux).</li>
<li>Profiler: Reduced memory footprint of profiler when viewing large frames (deep profile)</li>
<li>Web Player: Make browser more responsive to user input on Windows.</li>
</ul>
