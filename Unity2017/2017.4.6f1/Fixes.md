# Unity 2017.4.6f1
https://unity3d.com/unity/whatsnew/unity-2017.4.6

## Fixes

<ul>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1015836/">1015836</a>) - 2D: Fixed Sprite Pivot setting appears when Sprite Mode is set to Multiple but does not appear when it's set to Single.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/955571/">955571</a>) - AI: Fixed <code>AyncOperation</code>s started with the <code>NavMeshBuilder</code> possibly crashing when being used in quick succession.</li>
<li>(1021442(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/966038/">966038</a>)) - Android: Fixed shader clip support on devices with Adreno 4x and later.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1037638/">1037638</a>) - Android: Fixed the issue that GI assets for the first scene have been added to the obb with "Split Application Binary" enabled.</li>
<li>(1030201(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/961655/">961655</a>)) - Android: Fixed using memalign on Android due to compatibility issues causing crashes on some devices.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1029856/">1029856</a>) - Animation: Fixed performance issues in the clip drop down menu of the animation window when editing large amount of clips.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/980970/">980970</a>) - Asset Pipeline: Fixed crash on UnwrapImpl::GenerateSecondaryUVSet when re-importing certain model with "Generate Lightmap UVs" setting enabled.</li>
<li>(1035068) - Global Illumination: Fix HDR lightmap texture encoding in Gamma Color Space.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1006916/">1006916</a>) - Global Illumination: Fixed Anti-aliasing Samples value change from Lightmap Parameters not being taken into account after a lightmap bake.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1038465/">1038465</a>) - IL2CPP: Corrected invalid code generated for a lock on UWP in some cases.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1020341/">1020341</a>) - IL2CPP: Fixed DllNotFoundException when accessing NetworkInformation on UWP.</li>
<li>(None) - iOS: Optimization to iPhoneTime:GetTimeSinceStartup.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1011604/">1011604</a>) - iOS: Fixed crash when usbmuxd proxy is still running during app exit.</li>
<li>(1043428) - PS4: Fixed UnityWebRequests on PS4.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/856344/">856344</a>) - Scene Management: Fixed modifying asset import settings from script changes 'timeCreated' in the meta-file, breaking asset representation determinism.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/996473/">996473</a>) - Scripting: Resolved reference assemblies correctly from any folder in project.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1011626/">1011626</a>) - Scripting: Fixed memory profiler.</li>
<li>(1039434) - Scripting: Fixed crash when accessing custom attribute data.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1035692/">1035692</a>) - Scripting: Fixed crash when loading some assemblies due to invalid metadata parsing.</li>
<li>(992166) - Scripting: Fixed VS project generation to use modular Unity Engine dlls.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/898536/">898536</a>) - Shaders: Fixed enum fields not working with float values.</li>
<li>(1037720) - Web: Fixed UnityWebRequest POST failure with multipart sections.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/943241/">943241</a>) - WebGL: Fixed MS Edge detection.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1003917/">1003917</a>) - WebGL: Added workaround for Chrome Audio Auto-play policy.</li>
<li>([965647, 1003912](https://issuetracker.unity3d.com/product/unity/issues/guid/965647, 1003912/)) - WebGL: Fixed usage of deprecated WebAudio setters.</li>
<li>(<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1017515/">1017515</a>) - Windows: Fixed deadlock on exit when using OnAudioFilterRead with il2cpp scripting backend.</li>
<li>(1039050) - XR: Updated Unity branded default Daydream Launcher images.</li>
<li>(1048091) - XR: Resolved issues with User-Presence not working properly in the Editor for Windows Mixed Reality applications.</li>
<li>(1048089) - XR: Resolved issue with the OS minimizing the Editor when playing a Mixed Reality application on Windows RS4.</li>
<li>(1033915) - XR: Fixed flickering issue in rendered eyes due to incorrect pause handling behavior.</li>
</ul>

#### Revision: c24f30193bac
