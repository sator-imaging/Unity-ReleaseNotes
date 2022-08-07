# Unity 3.5.5
https://unity3d.com/unity/whats-new/unity-3.5.5

## Fixes

<ul>
<li>Android: Fixed black screen on Kindle when accessing Quick Settings.</li>
<li>Android: Script debugging yields/coroutines could sometimes cause a crash - this has been fixed.</li>
<li>Android: Fixed gl context-recreation. Now you can change AA or DisplayBuffer bitness at runtime even if post-effects are used.</li>
<li>Editor: Windows now draw correctly when fullscreen on OSX 10.8 Mountain Lion</li>
<li>Editor: Fixed dependency on X11 of pvr texture tool.</li>
<li>Editor: Allow importing assets with leading spaces on Windows.</li>
<li>Graphics: Fixed surface shaders regression in 3.5.3 that assumed custom surface output structure always has "Specular" member that is a scalar</li>
<li>Graphics: Fixed VRAM amount detection on some Intel SandyBridge / IvyBridge GPUs.</li>
<li>Graphics: Fixed rendering cameras in editor batch mode</li>
<li>Graphics: Fixed crash in particle system when source mesh has no normal or tangents</li>
<li>Graphics: Allow editor to build shaders in -nographics batch mode</li>
<li>iOS: Fixed Texture2D.ReadPixels on iOS6.</li>
<li>iOS: Fixed crash with suspending while video is playing.</li>
<li>iOS: Fixed more splash issues.</li>
<li>iOS: SystemInfo.deviceUniqueIdentifier no longer uses deprecated UIDevice.uniqueIdentifier.</li>
<li>iOS: Updated iPad2 detection to handle newly released one.</li>
<li>Mac Web Player: Fix focus handling when browser window loses focus.</li>
<li>Mobile: fixed broken lighting when dynamically batching uniformly scaled meshes.</li>
<li>MonoDevelop: Fixed cursor display on Mac Retina displays.</li>
<li>Navmesh: Fix for regression in 3.5.3 - where long paths some times be discarded when stoppingDistance &gt; 0.</li>
<li>Script: Fixed crash when calling material.GetFloat(null).</li>
<li>Substance: Substances with bitmap inputs were not regenerating correctly.</li>
<li>Substance: Fix garbage collecting.</li>
<li>Substance: Cache fixes.</li>
</ul>
