# Unity 3.4.1
https://unity3d.com/unity/whats-new/unity-3.4.1

## Fixes


### Editor
<ul>
<li>Icons on newly created Prefabs no longer stay after the Prefab is deleted from the scene.</li>
<li>Fixed crash on Windows related to AssetStore server side errors.</li>
<li>Fixed right click menu for keys on curves in the AudioSource Component not working when a AudioLowPassFilter component was also attached.</li>
<li>Fixed crash when changing .meta files and the .meta data file is disagreeing with the changes.</li>
<li>Only display progress bar when it changes at least one percentage point, fixes crash due to out of memory and faster asset scan speed.</li>
<li>Fixed texture importer rescan memory leak, which caused out of memory crashes.</li>
<li>Clear log callback when unloading domains, fixes crash when hitting Play button.</li>
<li>Fixed auto release leaks in progress bars on Mac OS X.</li>
<li>Fixed potential crash in curve editing for audio sources.</li>
<li>Fixed render texture creation error when searching in the project view.</li>
</ul>

### Runtime
<ul>
<li>Fix intermittent crash-on-reload on Windows.</li>
<li>Fixed crash on exit when "Exit on Suspend" was checked on iOS.</li>
<li>Fixed crash on exit in forced OpenGL mode on Windows.</li>
<li>Fixed webplayer graphical glitches existing in Safari on Mac OS X Lion for some AMD graphics cards.</li>
<li>Fixed crash in skinning meshes with invalid bone indices or when mesh has just been updated.</li>
<li>Fixed crash in SSE2 skinning code when reading out of bounds.</li>
<li>Fixed regression against Unity 3.3 when using RenderTexture.GetTemporary with cubemaps.</li>
</ul>

### Standard assets
<ul>
<li>Added missing Pro Water shaders.</li>
</ul>

### Javascript
<ul>
<li>Implicit downcasts (for example, assignment from a variable of type Object to a variable of type String) will now be reported as warnings instead of errors in strict mode.</li>
</ul>

### MonoDevelop
<ul>
<li>Fixed US International input method to allow input of ' and ".</li>
<li>Better window resizing on Mac OS X Lion.</li>
</ul>
