# Unity 4.3.1
https://unity3d.com/unity/whats-new/unity-4.3.1

## Fixes

<ul>
<li>2D: Can now create sprites from POT textures in advanced mode.</li>
<li>2D: Destroying a Sprite's texture will not crash the SpriteRenderer that's using it.</li>
<li>2D: Do not trash MaterialPropertyBlock on a SpriteRenderer.</li>
<li>2D: Sprite.textureRectOffset won't crash the editor anymore.</li>
<li>BlackBerry: Fixed garbage collect crash when using threads</li>
<li>BlackBerry: SystemInfo.deviceUniqueIdentifier now returns serial number correctly</li>
<li>Debugger: Avoid deadlocks on OSX</li>
<li>Graphics: Fix "fence == expectedFence" error with GPU skinning</li>
<li>Graphics: Fix GPU Skinning crash on DX11 when the bone count changes.</li>
<li>Graphics: Fixed Intel DX9 GPUs (like Intel 945) incorrectly being labeled as unsupported by Unity.</li>
<li>Graphics: Fixed real-time shadows with orthographic camera and baked occlusion data.</li>
<li>Graphics: Fixed Screen.width and height reporting incorrect values in the Editor.</li>
<li>Graphics: Fixed some setups with shadows &amp; image effects causing crashes in free Unity version.</li>
<li>iOS: Fixed iOS build being non-PIE compatible</li>
<li>Physics: Assert being thrown when 2D collider area is below what Box2D can handle.</li>
<li>Physics: Fixed inability to set 2D rigid-body mass from the scripts.</li>
<li>Physics: Slider Joint 2d properties accept Infinity value and produce runtime errors</li>
<li>Sourcebuild: Fixed running tests in stripped sourcecode builds</li>
<li>WebPlayer Installer: Install x64 content to Program Files instead of Program Files (x86)</li>
<li>WePlayer: Fixed a WTS bug on Windows 8 and 8.1 where the player would think that the screen is locked</li>
<li>Windows Editor/Player: Fixed rendering performance regressions in 4.3.</li>
<li>Windows Editor: Fixed crash on toggling Direct3D 11 mode when profiler window is open.</li>
<li>Windows Store Apps/Windows 8.1: Fix a bug with Independent Input source enabled, the application would report incorrect touch position on some devices, for ex., Surface Pro</li>
<li>Windows Store Apps/Windows 8.1: Fix a bug with Independent Input source enabled, the application will still receive input after loosing and regaining focus.</li>
<li>Windows Store Apps/Windows Phone 8: Fixed random crashes, when putting pressure on GC.</li>
<li>Windows Store Apps: Fixed a bug where the webcam could destroyed before its deinitialization is finished</li>
<li>Windows Store Apps: fixed checking plugin compatibility for .NET 4.5 plugins</li>
<li>Windows Store Apps: fixed lowercase 'y' not working in input controls</li>
<li>Windows Store Apps: fixed setting default cursor in player settings</li>
<li>Windows Store Apps: Fixed the issue where BlockUntilDone in WWW backend would not properly wait until the http task is completely finished</li>
</ul>
