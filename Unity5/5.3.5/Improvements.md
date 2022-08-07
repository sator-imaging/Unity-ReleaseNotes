# Unity 5.3.5
https://unity3d.com/unity/whats-new/unity-5.3.5

## Improvements

<ul>
<li>Android: IL2CPP - Stripping of symbols and debug info is now enabled by default. Development builds still have symbols which makes for a slightly larger binary.</li>
<li>Asset Bundles: Added offset argument to AssetBundle.CreateFromFile and AssetBundle.LoadFromFile methods.</li>
<li>Asset Bundles: Output the CRC value for the manifest asset bundle.</li>
<li>Asset Management: Introduced AssetDatabase.GetAssetDependencyHash method which returns the hash of all the dependencies of an asset.</li>
<li>Cluster Rendering: Improved cluster networking layer and reduced instability while using cluster input.</li>
<li>Graphics: Dynamic batching was reintroduced for particles, lines and trails. (766802)</li>
<li>IL2CPP: Reduce the binary size and build time for projects which make use of many C# attributes.</li>
<li>iOS: Added a compile flag in the trampoline code in order to allow disable the filtering of emoji characters.</li>
<li>iOS: Added device support for iPhone SE and iPad Pro 9.7".</li>
<li>OpenGL: ComputeBuffer now uses the same data layout as Direct3D whenever automatically translated shaders are used. Therefore no more special layout handling for ComputeBuffer.SetData/GetData is needed based on the graphics API and any such user code should be removed. The only exception is with manually written GLSL shaders. In that case the OpenGL data layout rules must be taken into account.</li>
<li>Networking: Added support for IPv6 networks in UdpClient. (767741)</li>
<li>VR: Updated Oculus API and plugin to version 1.3.2. Downloading 1.3.2 OVRPlugin from Oculus is no longer necessary.</li>
<li>Windows Store: On IL2CPP scripting backend, Unity players are now shipped as DLLs rather than static libraries. This significantly reduces platform support module installation size as well as decreases generated C++ code linking time.</li>
</ul>
