# Unity 3.4.2
https://unity3d.com/unity/whats-new/unity-3.4.2

## Fixes


### Editor
<ul>
<li>Fixed crash when editing audio source.</li>
<li>Fixed issues with garbage collection in Asset Store editor bindings which could cause the Asset Store to report JavaScript errors about undefined variables (most frequently "this.fromContext.results", "a.title" or "b.title").</li>
</ul>

### Android
<ul>
<li>Fixed crash with Unity Android non-pro ('basic') license.</li>
<li>Fixed corrupted splash image on Icecream-Sandwich.</li>
<li>Allow audio playback only when application is focused (prevents audio on the unlock screen).</li>
<li>Made sure the on-device-profiler only uses active network interfaces.</li>
<li>Fixed an issue where mscorlib.dll could not be found.</li>
</ul>

### iOS
<ul>
<li>Fixed random crashes when building with Xcode 4.2 (iOS SDK 5.0).</li>
<li>Fixed crash with auto-rotation on iOS 5.</li>
<li>Disabled workaround for ipad2 driver bug with msaa+colormask+blend when running on iOS 5 (was fixed by Apple).</li>
<li>Made Cache Path for AssetBundles be compatible with new Apple Guidelines: /Library/Caches instead of /Documents.</li>
</ul>

### Monodevelop
<ul>
<li>Fixed compilation issues of Javascript.</li>
</ul>

### Webplayer
<ul>
<li>Workaround for NVidia driver issue in Mac OS X 10.7.2, which makes web players display garbage on certain NVidia GPUs.</li>
</ul>
