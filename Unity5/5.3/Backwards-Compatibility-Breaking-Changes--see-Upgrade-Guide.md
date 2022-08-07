# Unity 5.3
https://unity3d.com/unity/whats-new/unity-5.3

## Backwards Compatibility Breaking Changes, see Upgrade Guide

<ul>
<li>Graphics: Added custom near plane slider for spot light shadows instead of auto-calculation, defaults to 0.2. Scenes might need re-tuning.</li>
<li>Graphics: Implemented shadow bias for point lights. Previously was not implemented, might need re-tuning.</li>
<li>Physics: HingeJoints now have orientation to be compatible with Unity 4. The Rigidbody that share the GameObject with the HingeJoint will view the Joint anchor as a left-hand coordinate system. This means the Rigidbody will view positive angles as going clockwise around the Joint anchor. The HingeJoint "Connected Body" will view the Joint anchor as a right-hand coordinate system. This means the Connected Body will view positive angles as going counter-clockwise around the Joint anchor.</li>
<li>Physics: Obsoleted enum JointDriveMode and JointDrive.mode</li>
<li>Physics: When changing a mesh and subsequently setting it as the sharedMesh of a MeshCollider we now update collision mesh instead of ignoring the changes.</li>
<li>Shaders: “Precompiled” shaders (e.g. pasting result from “show generated code” into shader asset itself) are not working anymore. This was deprecated before in Unity 5.2.</li>
<li>Shaders: Smoothness curve of Standard shader matches Substance Painter and Marmoset Toolbag2 (only when tools are using GGX) very closely now. Your smoothness textures might need an update.</li>
<li>Shaders: To improve visual quality of specular highlight Standard shader is now using GGX distribution function. Previously Blinn-Phong was used.</li>
<li>VR: Oculus 0.8 Runtime required for Windows.</li>
</ul>
