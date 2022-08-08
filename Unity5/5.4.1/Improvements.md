# Unity 5.4.1

https://unity3d.com/unity/whats-new/unity-5.4.1

## Improvements



*   Core: Added support for loading serialized files stored with versions >= 5.5.0a4.
*   DX11: Improved texture upload performance for compressed, floating point and RGBA32 formats (also in 5.3.6p3) (812350).
*   Graphics: GPU Instancing - it is no longer an error to use instanced shaders on renderers that don't support instancing (SkinnedMeshRenderer, SpriteRenderer, etc.).
*   Graphics: GPU Instancing - for statically batched MeshRenderers, using an instanced shader now will not break static batching. If you want renderers to be instancing batched, please consider disable static batching flag (816786).
*   Linux: Removed 16GB total memory limit.
*   Networking: Projects using UnityWebRequest from UnityEngine.Experimental.Networking should now be auto-upgraded to use its new location in UnityEngine.Networking.
*   VR: Mac version of the editor can now add OpenVR as a VR platform when targeting the Windows player.
*   VR: Stereo View and Projection Matrices can be set individually through scripting API.
*   VR: Updated the following Image Effects from the Standard Assets to work with Single-Pass Stereo: Ambient Obscurance, Camera Motion Blur. (811571)
*   VR: Upgraded SDKs - Oculus to 1.7, GearVR to 1.7.1, OpenVR to 1.0.2.
*   Windows Store: Windows Extension SDK references will now be automatically added to Assembly-CSharp projects.