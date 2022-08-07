# Unity 4.2
https://unity3d.com/unity/whats-new/unity-4.2

## Upgrade guide

<ul>
<li>See "Changes" section above!</li>
<li>iOS: We renamed AppController.mm/h to UnityAppController.mm/h to highlight the fact that we now allow your own AppDelegate (derived from UnityAppController). If you have plugins including AppController.h you can simply include UnityAppController.h instead. If you have AppController.mm/h in Plugins/iOS folders you can merge and rename them. Anyway, we urge you to consider moving to new AppDelegate model: if you needed to do some view tweaking, now you can do it without ever touching Unity's trampoline, meaning no upgrade pains.</li>
<li>Deprecation heads-up. In the next release (4.3), we plan to drop: 
<ul>
<li>OpenGL ES 1.1 support on mobile (set Rendering Path to VertexLit in player settings and it should be very similar experience on OpenGL ES 2.0)</li>
<li>Pre-DX9 GPU support on PC (Windows/Mac/Linux). This means, NVIDIA GPUs before GeForce FX (2003), AMD GPUs before Radeon 9500 (2002) and Intel GPUs before GMA 900 (2004). Shader Model 2.0 will be the new minimum requirement.</li>
</ul></li>
<li>MonoDevelop may fail to start correctly on Windows if an old version of Gtk# is installed on the system. Please uninstall this version, and install a newer one if still needed.</li>
</ul>
