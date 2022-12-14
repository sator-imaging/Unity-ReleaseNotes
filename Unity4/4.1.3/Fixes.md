# Unity 4.1.3

https://unity3d.com/unity/whats-new/unity-4.1.3

## Fixes



*   Android: Fixed rendering issues on Nexus4 + Android os 4.2.2 when "Use 32bits Display Buffer" is checked, due to Compositor using Default FBO alpha.
*   Editor: Fix Profiler window freeze on Mac OS X 10.8.3 with older NVIDIA GPUs (disabled GPU profiler completely on these systems due to driver bugs).
*   Editor: Fixed forcing texture to be POT if pvrtc compression is selected.
*   Editor: Fixed oversight in fix to crash when loading fonts from asset bundles in editor.
*   Fixed crash when unloading unused assets.
*   iOS: Fixed substance subsystem crash during asset bundle loading when stripping is enabled.
*   iOS: Fixed performance regression with static batching.
*   Mecanim: Blend Tree's mirror and offset parameter were not saved correctly for standalone build.
*   Mecanim: Fix recorder memory leak.
*   Mecanim: Fix crash in Mecanim when using interruptible transition.
*   Mobile: Fixed skinning performance regression.
*   Scripting: Avoid crash if behaviors are destroyed on disable.