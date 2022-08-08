# Unity 3.5.5

https://unity3d.com/unity/whats-new/unity-3.5.5

## Fixes



*   Android: Fixed black screen on Kindle when accessing Quick Settings.
*   Android: Script debugging yields/coroutines could sometimes cause a crash - this has been fixed.
*   Android: Fixed gl context-recreation. Now you can change AA or DisplayBuffer bitness at runtime even if post-effects are used.
*   Editor: Windows now draw correctly when fullscreen on OSX 10.8 Mountain Lion
*   Editor: Fixed dependency on X11 of pvr texture tool.
*   Editor: Allow importing assets with leading spaces on Windows.
*   Graphics: Fixed surface shaders regression in 3.5.3 that assumed custom surface output structure always has "Specular" member that is a scalar
*   Graphics: Fixed VRAM amount detection on some Intel SandyBridge / IvyBridge GPUs.
*   Graphics: Fixed rendering cameras in editor batch mode
*   Graphics: Fixed crash in particle system when source mesh has no normal or tangents
*   Graphics: Allow editor to build shaders in -nographics batch mode
*   iOS: Fixed Texture2D.ReadPixels on iOS6.
*   iOS: Fixed crash with suspending while video is playing.
*   iOS: Fixed more splash issues.
*   iOS: SystemInfo.deviceUniqueIdentifier no longer uses deprecated UIDevice.uniqueIdentifier.
*   iOS: Updated iPad2 detection to handle newly released one.
*   Mac Web Player: Fix focus handling when browser window loses focus.
*   Mobile: fixed broken lighting when dynamically batching uniformly scaled meshes.
*   MonoDevelop: Fixed cursor display on Mac Retina displays.
*   Navmesh: Fix for regression in 3.5.3 - where long paths some times be discarded when stoppingDistance > 0.
*   Script: Fixed crash when calling material.GetFloat(null).
*   Substance: Substances with bitmap inputs were not regenerating correctly.
*   Substance: Fix garbage collecting.
*   Substance: Cache fixes.