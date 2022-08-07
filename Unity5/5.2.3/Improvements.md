# Unity 5.2.3
https://unity3d.com/unity/whats-new/unity-5.2.3

## Improvements

<ul>
<li>Added warning for NetworkIdentity on child game objects.</li>
<li>Better error messages when network packets larger than MTU are generated by internal multiplayer systems.</li>
<li>GI: Added the "Min Chart Size" option on the MeshRenderer to allow for lowering chart size in case stiching is not needed.</li>
<li>GI: Added the "Ignore Normals" option on the MeshRenderer to skip comparing normals when detecting charts for realtime GI. This can be necessary when using hand authored UVs to avoid chart splits.</li>
<li>GI: Upgraded Enlighten to 2.22 UN20: 
<ul>
<li>An issue has been fixed where AMD Opteron CPUs produced different atlas packing to Intel Xeon CPUs.</li>
<li>A crash affecting Linux binaries on CPUs lacking SSE3 instructions has been fixed.</li>
<li>PS4 SDK used is 3.000.</li>
<li>iOS stays on the old Enlighten build for a moment.</li>
</ul></li>
<li>IL2CPP: Allow null checks, array bounds checks, and divide by zero checks to be selectively included or omitted from generated C++ code by using a C# attribute on type, method, or property definitions.</li>
<li>iOS/IL2CPP:   Enable incremental build support using the "Append" option. Keep the generated code stable across additional, removal, and changes for string literals and non-generic types.</li>
<li>Networking:   Added more logging info on too-large packets when object state updates exceed the MTU.</li>
<li>Networking: Added log messages to identify the object and script that cause too-large packets to be generated.</li>
<li>StackTraceLogType.None now works on iOS and Android.</li>
<li>Physics:  Expose the error tolerance on SpringJoint. This allows the springs to have a rest length shorter than the default 2.5 cm.</li>
<li>(587995) - Physics:   Always render the outline of a PolygonCollider2D in dark-green so that if an edge is discarded, it still shows.</li>
<li>(718508) -  Physics:  Increase precision of Physics2D.OverlapArea &amp; Physics2D.OverlapCircle methods.</li>
<li>Unity Ads:    Update to Unity Ads 1.5.3</li>
<li>VR:   A camera can now target the main display backbuffer in VR mode by setting "Target Eye" to "None (Main Display)".</li>
<li>VR:   Updated the OVRPlugin. Oculus Runtime 0.8 is required to use Oculus VR with this patch.</li>
<li>VR:   Update to Oculus OVRPlugin.</li>
</ul>