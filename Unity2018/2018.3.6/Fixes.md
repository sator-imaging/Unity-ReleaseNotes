# Unity 2018.3.6
https://unity3d.com/unity/whats-new/2018.3.6

## Fixes

<ul>
<li><p>2D: Fixed crash on when passing array of nulls to SpriteAtlas.Add. (<a href="https://issuetracker.unity3d.com/issues/crash-on-spriteatlas-add-when-passing-array-of-nulls-to-spriteatlas-dot-add">1089125</a>, 1120906)</p></li>
<li><p>Animation: Fixed a crash when parenting an GameObject during an AnimationEvent. (1115423)</p></li>
<li><p>Asset Pipeline: Optional parameter added to SceneManager.UnloadScene function allowing to unload assets embedded in a scene without calling UnloadUnusedAssets. (<a href="https://issuetracker.unity3d.com/issues/default-skybox-cubemap-is-not-re-used-when-reloading-scene-multiple-times-and-causes-memory-leak">998958</a>, 1111167)</p></li>
<li><p>Build Pipeline: Fixed rare data corruption when building asset bundles with LZMA compression. (<a href="https://issuetracker.unity3d.com/issues/when-building-a-lot-of-assetbundles-some-bundles-will-result-in-corrupted-resources-dot-resources-or-dot-ress-will-be-0-bytes">1118331</a>)</p></li>
<li><p>DX12: Fixed a crash when switching to exclusive fullscreen.</p></li>
<li><p>Editor: Fixed an issue where text flickers when displaying a button or label using the IMGUI that has a long text with wordwrap enabled. (1106201)</p></li>
<li><p>Editor: Fixed crash and validation errors when opening editor windows. (1085277)</p></li>
<li><p>Graphics: Disabled GPU skinning in the Editor when Graphics Emulation is enabled. (1107282)</p></li>
<li><p>Graphics: Fixed an issue where Light Probe Proxy Volumes did not function correctly with Vulkan as the graphics API. (<a href="https://issuetracker.unity3d.com/issues/vulkan-light-probe-settings-use-proxy-volume-on-meshrenderers-and-skinnedmeshrenderers-is-wrong">988476</a>)</p></li>
<li><p>Graphics: Improved terrain painting that produces quantization when using OpenGL API. (1114680)</p></li>
<li><p>Graphics: Vulkan: Various stability, performance and correctness fixes.</p></li>
<li><p>Graphics: Vulkan: Various stability, performance and correctness fixes.</p></li>
<li><p>Graphics: [ShaderGraph] Fixed Transparent preview not clearing framebuffer. (1068062)</p></li>
<li><p>IL2CPP: Add support for marshaling fields which are arrays of structs which in turn have arrays as fields. (<a href="https://issuetracker.unity3d.com/issues/marshal-dot-sizeof-throws-an-exception-in-il2cpp-builds-when-the-object-contains-an-array-of-objects-with-arrays">1106047</a>)</p></li>
<li><p>IL2CPP: Added protocol support for IPv6 on Windows. (1099133)</p></li>
<li><p>IL2CPP: Correctly indicate that IPv6 is not supported on non-IPv6 platforms. (1108823)</p></li>
<li><p>IL2CPP: Emit proper C++ code when type names include characters that are not valid for C++ source code. (1108435)</p></li>
<li><p>IL2CPP: Fixed a crash when using the Environment.MachineName property on some machines when targeting UWP and make it return results consistent with the Standalone Player. (<a href="https://issuetracker.unity3d.com/issues/system-dot-environment-dot-machinename-crashes-on-il2cpp-on-long-machine-names-with-uwp-builds">1093953</a>)</p></li>
<li><p>IL2CPP: Fixed an intermittent crash in the native linker on Android. (1108960)</p></li>
<li><p>IL2CPP: Fixed InvalidCastException that can sometimes happen when passing managed object that derives from a native Windows Runtime class to native code. For instance, this happens when deriving from Windows.UI.Xaml.Control.ContentDialog and trying to show it. (<a href="https://issuetracker.unity3d.com/issues/uwp-contentdialog-throws-an-exception-on-il2cpp-backend">1104540</a>)</p></li>
<li><p>IL2CPP: Generate proper C++ code for an out parameter used as SizeParamIndex. (<a href="https://issuetracker.unity3d.com/issues/uwp-il2cpp-build-generates-incorrect-code-when-using-marshalasattribute-on-a-intptr-parameter">1115412</a>)</p></li>
<li><p>IL2CPP: Handle null explicitly casted to an array and indexed. (1115145)</p></li>
<li><p>IL2CPP: Loaded field addresses via unsigned native integer types properly. (1104370)</p></li>
<li><p>IL2CPP: Prevent a compilation error in generated C++ code when the ldtoken opcode is used in some cases. (1108435)</p></li>
<li><p>IL2CPP: Prevent an compilation error in generated C++ code when an enum field is marshaled. (<a href="https://issuetracker.unity3d.com/issues/editor-throws-multiple-errors-when-trying-to-build-project-with-il2cpp">1104889</a>)</p></li>
<li><p>IL2CPP: Prevent an exception during IL2CPP code conversion that can happen with Trace statements in some cases. (1120880)</p></li>
<li><p>IL2CPP: Prevented a crash at runtime with the .NET 4.x equivalent scripting runtime that can occcur when an enum is nested in a generic type. (1113091)</p></li>
<li><p>IL2CPP: Properly generate code using the in modifier for parameters on abstract methods in a generic type. (1103142)</p></li>
<li><p>Package Manager: Fixed moving files in the editor project view (drag and drop) not working in local packages. (<a href="https://issuetracker.unity3d.com/issues/files-are-duplicated-when-moving-them-in-local-package">1114391</a>, 1117976)</p></li>
<li><p>Particles: Fixed erroneous Particle System error message: "Sub-emitters must be children of the system that spawns them". (<a href="https://issuetracker.unity3d.com/issues/sub-emitters-must-be-children-of-the-system-that-spawns-them-error-is-shown-even-though-sub-emitters-are-correctly-parented">949522</a>, 1089804)</p></li>
<li><p>Particles: Fixed Frame Debugger failing to show draw call information for Particle Systems. (1107382)</p></li>
<li><p>Particles: Fixed incorrect curve evaluation when using the Limit Velocity over Lifetime module with a micture of optimized and non-optimzied curves. (1096701)</p></li>
<li><p>Particles: Fixed particle bounds when using Sprites in the Texture Sheet Animation Module. (<a href="https://issuetracker.unity3d.com/issues/particles-get-out-of-particle-system-bounds-when-using-texture-sheet-animation">1107722</a>)</p></li>
<li><p>Particles: Fixed particle trails could being culled incorrectly when using the World Space trails option. (<a href="https://issuetracker.unity3d.com/issues/particle-system-trails-are-culled-while-still-within-camera-bounds">1089679</a>)</p></li>
<li><p>Particles: Fixed regression bug where offscreen Particle Systems failed to play. (1114729)</p></li>
<li><p>Particles: Fixed scaling regression bugs with Particle Systems. (<a href="https://issuetracker.unity3d.com/issues/particles-do-not-inherit-scale-from-parents-when-scaling-mode-is-set-to-hierarchy-and-simulation-space-is-set-to-world">1112937</a>, 1116160)</p></li>
<li><p>Particles: Fixed Velocity Module Speed Modfiier not applied to the initial simulation step of newly spawned particles. (<a href="https://issuetracker.unity3d.com/issues/particle-system-scatters-differently-when-in-play-mode">1111134</a>)</p></li>
<li><p>Particles: Update particle bounce light immediately when the multiplier is changed on the Light. (1102543)</p></li>
<li><p>Physics: Ensure that ContactPoint2D and Collision2D types do not get stripped causing a crash. (1121995)</p></li>
<li><p>Prefabs: Fixed references to Prefabs from scene getting lost if prefab is modified. (1116476)</p></li>
<li><p>Prefabs: Updated Undo to return Prefab instances with missing assets to previous state correctly. (<a href="https://issuetracker.unity3d.com/issues/undo-after-selecting-unpack-prefab-completely-on-an-instance-with-missing-asset-does-not-properly-return-to-previous-state">1056446</a>, 1120322)</p></li>
<li><p>Scripting Upgrade: Fixed crash in ScriptUpdater.exe when code contains qualified references to methods of type that were statically imported (#using static). (<a href="https://issuetracker.unity3d.com/issues/apiupdater-crashes-when-script-has-qualified-access-to-statically-imported-types">1081267</a>)</p></li>
<li><p>Shaders: Fixed incorrect shader code generation with tessellation shaders when using the Vulkan API. (1092160)</p></li>
<li><p>Universal Windows Platform: Fixed IL2CPP crashing when using certain new types (like Windows.Foundation.GuidHelper.Equals) in Windows SDK 17763 or newer.</p></li>
<li><p>Universal Windows Platform: Fixed memory leaks on .NET backend when calling Mesh.SetVertices(), Mesh.SetUVs(), Mesh.SetTriangles() methods. (<a href="https://issuetracker.unity3d.com/issues/uwp-memory-leaks-on-net-backend-when-calling-mesh-dot-setvertices-mesh-dot-setuvs-mesh-dot-settriangles-methods">1042218</a>)</p></li>
<li><p>Windows: Fixed setting refresh rate in exclusive fullscreen mode having no effect on D3D11 and D3D12. (<a href="https://issuetracker.unity3d.com/issues/screen-dot-setresolution-ignores-prefferedrefreshrate-variable-and-sets-it-to-what-is-set-as-refresh-rate-through-windows">975924</a>)</p></li>
<li><p>XR: XR devices in new input system package are now all Y-up is away from the user. (<a href="https://issuetracker.unity3d.com/issues/xr-joystick-y-values-do-not-adhere-to-inputsystem-convention">1091918</a>)</p></li>
</ul>

#### Changeset: a220877bc173
