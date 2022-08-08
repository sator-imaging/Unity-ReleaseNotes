# Unity 4.1

https://unity3d.com/unity/whats-new/unity-4.1

## Changes



*   Audio: AudioSource.Play(offset) is now considered deprecated. It will still work as before, but will output a warning. Instead, users are encouraged to use AudioSource.PlayDelayed(delay) which takes a delay parameter in seconds instead of a sample count in the arbitrarily chosen 44100 reference rate that was used previously.
*   DestroyImmediate is no longer allowed to be called from within animation events.
*   Editor: Removed buttons in Console window for Open Editor Log and Open Player Log (on OS X) and put them into the custom menu for the Console instead (accessed through the upper right corner of the window).
*   iOS: Changed how VRAM amount is estimated and reported, now it is 1/4 of total physical memory.
*   iOS: Keyboard handling extracted to trampoline.
*   Mecanim: Avatar body and skeleton mask has been merged into AvatarMask to simplify the workflow. Any created object of type AvatarBodyMask or AvatarSkeletonMask should be converted to AvatarMask. Any AvatarSkeletonMask set into a layer mask would be lost, you need to manually re assign the mask.
*   Mecanim: CycleOffset is set automatically to 0.5 for clips that are being mirrored in States/BlendTrees.
*   Mecanim: In model importer animation tab for humanoid clip, the option Keep Additionnal bone has been removed since you can now choose wanted transform in the Avatar mask.
*   Static batching no longer supports generating triangle strips.
*   UnityEngine.dll and mscorlib.dll are no longer accepted as assets.