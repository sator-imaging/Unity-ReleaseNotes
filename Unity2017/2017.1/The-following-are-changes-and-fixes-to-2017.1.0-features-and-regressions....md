# Unity 2017.1
https://unity3d.com/unity/whats-new/unity-2017.1.0

## The following are changes and fixes to 2017.1.0 features and regressions...


### Changes
<ul>
<li>Android: Removed tapjacking protection because it causes touch input to be lost when a transparent overlay is shown on top of the Unity view</li>
</ul>

### Fixes
<ul>
<li>Animation: Fixed humanoid body position not working in additive (916487)</li>
<li>Editor: Fixed moving multiple objects makes only one of them to move according to handles</li>
<li>Graphics: Fixed crash when using RenderTextureFormat.RFloat in a  command buffer (898318)</li>
<li>Graphics: Fixed issue where a ComputeBuffer applied to a Material Block doesn't take effect when drawing via DrawMesh*Indirect (913828)</li>
<li>Linux: Work around TLS/allocator deadlock in new glibc</li>
<li>Multiplayer: Fixed memory leak of NetworkTransport::Send() (923903)</li>
</ul>
