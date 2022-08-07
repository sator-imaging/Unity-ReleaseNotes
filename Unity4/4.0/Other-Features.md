# Unity 4.0
https://unity3d.com/unity/whats-new/unity-4.0

## Other Features

<ul>
<li>Added a new development console to show error messages on screen in development player builds.</li>
<li>Android: Added Eclipse project generation.</li>
<li>Android: Support for APK Expansion Files (OBBs) - effectively enabling applications larger than 50Mb in the Google Play Store.</li>
<li>iOS: Screen.SetResolution now works on iOS too.</li>
<li>iOS: Target Resolution Player Setting was redesigned to better suite development workflow on multiple iOS devices. Two new “Auto (Best performance)” and “Auto (Best Quality)” settings allow Unity Runtime to choose most optimal rendering resolution according to device GPU capabilities.</li>
<li>Debugger: Web players can now be attached to and debugged just like standalones.</li>
<li>Editor: Add components and scripts to Game Objects easier and faster through the new Add Component drop-down directly inside the Inspector.</li>
<li>Editor: Create your own Inspector GUI for custom classes or attributes and see it used across all scripts that use those classes or attributes.</li>
<li>Fonts: Custom fonts can now use arbitrary character rectangles instead of a fixed grid.</li>
<li>Fonts: Font character placement properties are now accessible from scripting.</li>
<li>Fonts: Imported fonts can now be converted to editable custom fonts from the gear menu.</li>
<li>Gradient (known from the Shuriken editor) is now exposed to scripts: Gradient, GradientColorKey, GradientAlphaKey.</li>
<li>Navigation: NavMeshAgent supports prioritized levels of avoidance.</li>
<li>Navigation: NavMeshObstacle component added.</li>
<li>New Cursor API was introduced: 
<ul>
<li>Cursor API supports both software and hardware cursors.</li>
<li>Support for hardware cursors on the following platforms: Windows, Mac OS X, Linux, Flash.</li>
<li>Configure the default cursor in your projects’ Player Settings.</li>
</ul></li>
<li>License: New activation system was developed: Ability to un-license a machine yourself!

<ul>
<li>Continuous license and content updates.</li>
<li>Unity Account login for certain license types.</li>
<li>Surveys for certain license types.</li>
</ul></li>
<li>New Web Player Update mechanism, which allows multiple runtime versions to be installed at the same time: 
<ul>
<li>Allows running beta content with the beta runtime without having to install a beta plugin (beta runtime will be downloaded automatically).</li>
<li>Optionally allows testing release content using the beta runtime (by default it will be played back using the release runtime), using the context menu.</li>
<li>Allows switching between development and non-development players without plugin reinstallations, using the context menu.</li>
<li>Please note: in order for this to work, web plugin bundled with this build must be installed on user machine.</li>
</ul></li>
<li>Flash: Assembly validation for Flash supported/unsupported API's. If .NET feature or API is not available the validator will notify the user in the log, before compiling.</li>
<li>Plugins: Added Texture.GetNativeTexturePtr() that you can use in native code plugins. Can now directly access textures on non-OpenGL platforms as well! Example plugin in Low-level Native Plugin Interface documentation page shows how to.</li>
</ul>
