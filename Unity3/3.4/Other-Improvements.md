# Unity 3.4
https://unity3d.com/unity/whats-new/unity-3.4

## Other Improvements

<ul>
<li>Mac App Store: 
<ul>
<li>Added a feature to perform receipt validation for the Mac App Store.</li>
</ul></li>
<li>Scripting: 
<ul>
<li>Ability to control the order that scripts are executed in. Use Edit-&gt;Project Settings-&gt;Script Execution Order.</li>
<li>Texture2D.SetPixels32/GetPixels32 for much faster pixel operations.</li>
<li>Added Caching.MarkAsUsed function. This is used to ensure that some files are not thrown out of the least-recently-used cache if you know that they will be used in the future.</li>
</ul></li>
<li>Input: 
<ul>
<li>Win7 touchscreen input now fully supported.</li>
<li>Input.eatKeyPressOnTextFieldFocus added to be able to control input behavior during textfield focus. This is default true from 3.4 and forth. Set this to false to achieve pre 3.4 behavior.</li>
<li>Key input (i.e. Input.GetKeyDown) is now suppressed when a textfield is active. This is enabled only content built with 3.4 and later. To query key input during an active textfield, use Event.current in OnGUI.</li>
<li>Fixed support for mouse deltas from Apple's Magic Trackpad.</li>
</ul></li>
<li>MonoDevelop: 
<ul>
<li>Scripting projects are now built the same way that Unity builds them.</li>
<li>Now compiles Boo and UnityScript.</li>
</ul></li>
<li>Profiling: 
<ul>
<li>Intel GPA 4.0 Platform Analyzer profiler is supported for Windows Standalone Players.</li>
</ul></li>
<li>Javascript improvements: 
<ul>
<li>Allow characters in #pragma lines.</li>
<li>Array.slice(startIndex) must return all elements starting from startIndex.</li>
<li>Array.slice accepts negative indexes counting from the end of the array: [1, 2, 3, 4].slice(-2) // =&gt; [3, 4]</li>
<li>Proper support for do-while loops</li>
<li>Proper support for generic dictionaries of functions:

<ul>
<li>var dict = new Dictionary.();</li>
<li>dict["foo"] = function() print("foo");</li>
<li>dict["foo"] (); // prints foo</li>
</ul></li>
</ul></li>
<li>Importers: 
<ul>
<li>Implemented 3 minute timeout for 3DStudio Max FBX conversion.</li>
<li>Only show import settings on root asset. Showing them on every sub-asset could lead to the false impression that every sub-asset can have individual import settings.</li>
</ul></li>
<li>Other improvements: 
<ul>
<li>Removed tray icon for Windows Standalones when in batchmode allowing apps to run as a service.</li>
<li>Removed option 'Always Show Watermark' from the Player Settings.</li>
</ul></li>
</ul>
