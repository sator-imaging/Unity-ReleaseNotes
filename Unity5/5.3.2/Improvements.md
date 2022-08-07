# Unity 5.3.2
https://unity3d.com/unity/whats-new/unity-5.3.2

## Improvements

<ul>
<li>Compute: Improved compute shader import times, particularly on Windows. Since 5.1 we were always compiling them for GL4.3+GLES3.1 too, while most people only need DX11. (706098)</li>
<li>Editor: Added link to learn more about Unity Cloud Build in the Build Player window.</li>
<li>Editor/Scenes: Add Scene.GetRootGameObjects() to return the root game objects of the scene.</li>
<li>Editor/Scenes: Add SceneManager.CreateScene() API to allow creating new empty scene at runtime.</li>
<li>GI: Light probes and ambient (everything with SH calculations) match ground truth more closely now. (754898)</li>
<li>IL2CPP: Optimize method prologues for code size and incremental builds.</li>
<li>iOS: Added bitcode support. (752178)</li>
<li>iOS/IL2CPP: Added support for Xcode 7.3 (don't use __declspec attributes).</li>
<li>Samsung TV: Added support for 2016 TVs.</li>
<li>Tizen: Now supports tizenstore URL protocol to open up Tizen store pages.</li>
<li>tvOS: Enable Dynamic GI.</li>
<li>VR: Applications that lost focus no longer throttle the CPU.</li>
</ul>
