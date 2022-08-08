# Unity 5.1

https://unity3d.com/unity/whats-new/unity-5.1

## Changes



*   Animation: Added warning message for transitions without any condition. Those transitions are ignored.
*   Animation: Animator.speed can only be negative when the recorder is enabled. Now when the recorder is offline we do clamp the speed to 0 to avoid negative speed.
*   Animation: Transitions now have a fixed duration by default. Before Transition duration was in normalized time.
*   Animation Window: Dope sheet editor uses Command instead of Control for toggle-selecting on Mac OS
*   Animation Window: Double-clicking a key in the curve editor now selects the whole curve. Double-clicking part of the curve still creates a new key at this position
*   Editor: Incremental naming of instantiated GameObjects to use format: MyName, MyName (1), MyName (2)

*   Editor: Renamed and added new GizmoType enum values to be more explicit about how they work with selection hierarchy. See the docs.
*   Editor: Ensure GameView is un-maximized on Editor start up.
*   GI: Auto baking is now disabled by default in 2D projects.
*   GI: Change the "continuous baking" label to something shorter and better. Is now "Auto" with a tooltip added.
*   GI: When hard shadows are selected baking will use a directional spread of 0 and a point radius of 0. Also, the UI for spread/point are disabled when shadows are not set to soft.
*   Graphics: Deprecated player settings useDirect3D11, targetGlesGraphics, targetIOSGraphics properties. Use SetGraphicsAPIs and friends.
*   Graphics: LOD fade mode is now assigned to the whole LODGroup as None, Cross-fade or SpeedTree.
*   Graphics: Make Material(string) constructor script API obsolete with a warning. Support for creating fixed function shaders at runtime will be removed in the future.
*   Input: Default binding for 'Fire3' in new projects changed from Left Cmd to Left Shift, for benefit of Windows user experience.
*   iOS: By default iOS builds now only support Metal & OpenGL ES 2.0. If you need OpenGL ES 3.0, you can specify that under player settings.
*   Networking: The NetworkView component from the old network system was marked as deprecated.
*   Physics: Enabling the HingeJoint Motor overrides the spring, if the spring was enabled. If the motor is again disabled the spring will be restored. This restores Unity4 functionality.
*   Physics: HingeJoint MinBounce and MaxBounce are replaced by a single 'bounciness' for both limit ends. The new bounciness will be set to the largest of the old MinBounce and MaxBounce.
*   Physics: New HingeJoint initialization fixes target angle being measured incorrectly.
*   Shaders: OpenGL ES 3.0+ will use a new shader compiler backend. Based on HLSL + HLSLCrossCompiler + glsl-optimizer. This enables compute shaders on ES3.1 and other modern features. Existing Cg/HLSL compute, geometry and tessellation shaders can be used via automatic translation as well as with direct GLSL snippets. Note: Memory layout rule differences between DX and GL must be taken into account on the buffer data uploads.
*   Substance: Substances are now supported in both 32b and 64b iOS simulator builds.
*   Terrain: TerrainData.alphamapTextures is now exposed to script.
*   Version Control: Allow edit of imported/native asset with respect to meta/asset file being checked out
*   WebGL: Memory size is now written to the generated HTML to make it easier to change it without rebuilding the player.
*   WebGL: Player Settings UI is now consistent with other platforms.
*   WebGL: Static batching is now disabled by default to improve build sizes.
*   WebGL: Switch audio format used to AAC.