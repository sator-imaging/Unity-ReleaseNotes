# Unity 5.1
https://unity3d.com/unity/whats-new/unity-5.1

## Changes

<ul>
<li>Animation: Added warning message for transitions without any condition. Those transitions are ignored.</li>
<li>Animation: Animator.speed can only be negative when the recorder is enabled. Now when the recorder is offline we do clamp the speed to 0 to avoid negative speed.</li>
<li>Animation: Transitions now have a fixed duration by default. Before Transition duration was in normalized time.</li>
<li>Animation Window: Dope sheet editor uses Command instead of Control for toggle-selecting on Mac OS</li>
<li>Animation Window: Double-clicking a key in the curve editor now selects the whole curve. Double-clicking part of the curve still creates a new key at this position</li>
<li>Editor: Incremental naming of instantiated GameObjects to use format: MyName, MyName (1), MyName (2)</li>
</ul>

#### 
<ul>
<li>Editor: Renamed and added new GizmoType enum values to be more explicit about how they work with selection hierarchy. See the docs.</li>
<li>Editor: Ensure GameView is un-maximized on Editor start up.</li>
<li>GI: Auto baking is now disabled by default in 2D projects.</li>
<li>GI: Change the "continuous baking" label to something shorter and better. Is now "Auto" with a tooltip added.</li>
<li>GI: When hard shadows are selected baking will use a directional spread of 0 and a point radius of 0. Also, the UI for spread/point are disabled when shadows are not set to soft.</li>
<li>Graphics: Deprecated player settings useDirect3D11, targetGlesGraphics, targetIOSGraphics properties. Use SetGraphicsAPIs and friends.</li>
<li>Graphics: LOD fade mode is now assigned to the whole LODGroup as None, Cross-fade or SpeedTree.</li>
<li>Graphics: Make Material(string) constructor script API obsolete with a warning. Support for creating fixed function shaders at runtime will be removed in the future.</li>
<li>Input: Default binding for 'Fire3' in new projects changed from Left Cmd to Left Shift, for benefit of Windows user experience.</li>
<li>iOS: By default iOS builds now only support Metal &amp; OpenGL ES 2.0. If you need OpenGL ES 3.0, you can specify that under player settings.</li>
<li>Networking: The NetworkView component from the old network system was marked as deprecated.</li>
<li>Physics: Enabling the HingeJoint Motor overrides the spring, if the spring was enabled. If the motor is again disabled the spring will be restored. This restores Unity4 functionality.</li>
<li>Physics: HingeJoint MinBounce and MaxBounce are replaced by a single 'bounciness' for both limit ends.  The new bounciness will be set to the largest of the old MinBounce and MaxBounce.</li>
<li>Physics: New HingeJoint initialization fixes target angle being measured incorrectly.</li>
<li>Shaders: OpenGL ES 3.0+ will use a new shader compiler backend. Based on HLSL + HLSLCrossCompiler + glsl-optimizer. This enables compute shaders on ES3.1 and other modern features. Existing Cg/HLSL compute, geometry and tessellation shaders can be used via automatic translation as well as with direct GLSL snippets. Note: Memory layout rule differences between DX and GL must be taken into account on the buffer data uploads.</li>
<li>Substance: Substances are now supported in both 32b and 64b iOS simulator builds.</li>
<li>Terrain: TerrainData.alphamapTextures is now exposed to script.</li>
<li>Version Control: Allow edit of imported/native asset with respect to meta/asset file being checked out</li>
<li>WebGL: Memory size is now written to the generated HTML to make it easier to change it without rebuilding the player.</li>
<li>WebGL: Player Settings UI is now consistent with other platforms.</li>
<li>WebGL: Static batching is now disabled by default to improve build sizes.</li>
<li>WebGL: Switch audio format used to AAC.</li>
</ul>
