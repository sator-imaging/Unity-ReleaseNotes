# Unity 6000.0.86f1 LTS
Published at Thu, 12 Nov 2026 09:43:45 GMT  
https://unity.com/releases/editor/whats-new/6000.0.86f1

# Known Issues in 6000.0.86f1

- `Android`: Back gesture/button closes the app after returning from background when "Run In Background" and "Predictive Back Support" are enabled
    ([UUM-159613](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159613))

- `Editor Installers`: [macOS] Player libraries are code signed with bespoke entitlements
    ([UUM-156884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156884))

- `Shader System`: Player stops responding permanently when scenes are repeatedly switched with SceneManager.LoadSceneAsync
    ([UUM-156125](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156125))

- `Video`: Crash on BitmapDataToImageReference when opening a project with a specific .mp4 video file
    ([UUM-160889](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-160889))



# 6000.0.86f1 Release Notes

## Improvements

- `Asset Import`: Improved the security of model import by updating the bundled Autodesk FBX SDK to 2020.3.11, addressing two buffer-overflow vulnerabilities in FBX file parsing.
    (UUM-155199)

- `License`: Updated the Licensing Client to v1.19.0, which starts faster.



## API Changes

- `iOS`: Added: Added iPhone 18 Pro, iPhone 18 Pro Max and iPhone Duo device generation enums and screen cutouts.



## Fixes

- `2D`: Fixed a "No script asset for ShadowCasterPath" warning when you undo or redo a Shadow Caster 2D shape edit in Play mode.
    ([UUM-152935](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152935))

- `2D`: Fixed a NullReferenceException when a Light 2D created from a script is set to Freeform without a shape path.
    ([UUM-154810](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154810))

- `2D`: Fixed a Shadow Caster 2D keeping its old shadow after the tiles of a Tilemap Collider 2D are removed at runtime.
    ([UUM-149925](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149925))

- `2D`: Fixed an issue where a LineRenderer or TrailRenderer with Mask Interaction set to None was clipped by a Sprite Mask when another LineRenderer or TrailRenderer using the same material had Mask Interaction enabled.
    ([UUM-158602](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158602))

- `2D`: Fixed an issue where a Point Light 2D lost its cookie sprite when a project saved in Unity 6.0 or 6.3 was opened in a newer version.
    ([UUM-156931](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156931))

- `2D`: Fixed shadows from a Shadow Caster 2D that uses a Collider 2D \(for example a Tilemap Collider 2D\) as its casting source flickering in the Scene and Game views.
    ([UUM-147033](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147033))

- `2D`: Fixed sprites and UI not rendering on some OpenGL ES devices when the 2D Renderer Depth/Stencil Buffer setting is disabled.
    ([UUM-159093](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159093))

- `2D`: Fixed URP 2D editor-only icons being included in player builds.
    (UUM-144935)

- `Android`: Backported crash fixes for Android optimized frame pacing \(Swappy\).
    (UUM-153366)

- `Android`: Fixed an issue on OpenGL where Unity's render thread would attach/detach to the JVM multiple times in a frame, causing unnecessary allocations.
    (UUM-155309)

- `Android`: Fixed Android native libraries having a GNU_RELRO segment that was not aligned to 16 KB. `libc++_shared.so` will stay unaligned until the next NDK update.
    ([UUM-156603](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156603))

- `Android`: Fixed mouse movement producing scroll values when the cursor is locked.
    ([UUM-156720](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156720))

- `Android`: Fixed WebCamTexture taking several seconds to resume after the app regains focus or another app releases the camera, for example in split-screen mode.
    (UUM-155066)

- `Android`: Updated the bundled Android SDK cmdline-tools to 21.0, so emulators for Android 17 \(API 37.0\) created with its avdmanager start correctly.
    (UUM-157110)

- `Animation`: Crash when calling AnimationUtility.SetAdditiveReferencePose\` with a null clip or referenceClip.
    ([UUM-150816](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150816))

- `Asset Bundles`: Fixed AssetBundle content hashes changing between builds of unchanged content with Addressables or the Scriptable Build Pipeline, causing players to redownload unmodified bundles. Affected bundles get a new hash on the first build after upgrading.
    ([UUM-148841](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148841))

- `Asset Import`: Fixed the Linux Editor sometimes exiting while importing crunch-compressed textures, with "crn_threading_pthreads.cpp\(194\): Failure: semaphore: sem_wait\(\) or sem_timedwait\(\) failed" in the log. The crunch compressor treated an interrupted wait as a fatal error; it now retries the wait.
    ([UUM-150055](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150055))

- `Asset Pipeline`: Asset Pipeline: Fixing hang at startup when directory monitoring doesn't receive expected notification about changed file\(s\).
    ([UUM-149019](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149019))

- `Audio`: Fixed an assertion \(m_ModifiedClips.empty\(\)\) that was logged on exiting Play Mode after playing an AudioSource whose clip had loaded while Unity Audio was toggled off and back on during Play Mode.
    ([UUM-148749](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148749))

- `Build System`: Added MSBUILDDEBUGPATH to other method used when invoking dotnet.

- `Build System`: Bee_backend's stale output removal should not recheck the same file indefinitely.
    (UUM-158568)

- `Build System`: Don't hang the Editor when a previous bee_backend is still running.
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

- `DX12`: Fixed crash on D3D12SwapChain::Present when using AddComputePass with EnableAsyncCompute\(true\).
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `DX12`: Fixed IUnityGraphicsD3D12::GetNextFrameFenceValue\(\) returning a fence value that could complete before the commands a native plugin recorded into Unity's current command list when graphics jobs are enabled.
    (UUM-156768)

- `Editor`: Fixed bug where attempting to switch to a saved Editor layout while a window with unsaved changes was open could make it impossible to cancel the layout change.
    ([UUM-150448](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150448))

- `Editor`: Fixed bug where `InstantiateAsync` would not account for parent transform scale when `Instantiate` would.
    ([UUM-154591](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154591))

- `Editor`: Fixed player builds failing with error CS0117 when scripts use UnityEngine.Device.SystemInfo.processorModel, processorManufacturer, or supportsMachineLearning.
    ([UUM-154729](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154729))

- `Editor`: Fixed Prefab fields partially saving after selecting the name field with Auto Save enabled.
    ([UUM-157667](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157667))

- `Editor`: Fixed the TrueTypeFontImporter Help button link.
    ([UUM-144647](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144647))

- `Editor`: Updated included VCRedist to 14.51.36247 for the Windows Editor.
    (UUM-156578)

- `Editor`: URP: Save URP asset before starting an asset bundle build.
    ([UUM-153206](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153206))

- `Editor`: When graphics jobs is enabled the Editor now draw renderers whose shader variant compiled during the frame. Asset previews and one-shot renders which were previously blank due to a missing shader should now draw as expected via the SRP Batcher fallback path.
    (UUM-147205)

- `Editor`: \[Android\] Display an error informing users of the reason a device went offline during apk installation on Unity 6.0.
    (UUM-151550)

- `Engine Diagnostics`: Crash, exception and ANR reports captured before remote configuration now keep their essential attributes, including the session they occurred in.
    (UUM-159169)

- `Engine Diagnostics`: Fixed a possible crash when a crash report was logged from a worker thread while the Engine Diagnostics configuration was being applied.
    (UUM-158113)

- `GI`: Fixed a bug where reflection probes sometimes would not be re-baked when baking lighting, if only URP-specific settings were modified.
    ([UUM-133949](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-133949))

- `GI`: Fixed Adaptive Probe Volumes placing probes as if the scene had no geometry when baking with Vulkan on AMD GPUs.
    ([UUM-137732](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-137732))

- `GI`: Fixed speckles/white spots with APV.
    ([UUM-133626](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-133626))

- `Graphics`: Fixed a crash on quit in players that use split graphics jobs with DirectX 12 on Universal Windows Platform.
    (UUM-152563)

- `Graphics`: Fixed an assert "Metal: memoryless texture requires 2D texture." that the Editor logged on Metal when it rendered single-pass XR to memoryless texture arrays.
    (UUM-154442)

- `Graphics`: Fixed an issue where a Line Renderer or Trail Renderer using a 2D sprite material became invisible after turning off Preview in the Animation window or after calling Renderer.SetPropertyBlock.
    ([UUM-156620](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156620))

- `Graphics`: Fixed an issue with mip streaming when using Vulkan and GraphicsJobs.
    (UUM-137032)

- `Graphics`: Fixed memory corruption when BC-compressed textures are decompressed on the CPU, such as when the GPU does not support the format, and a mip level is smaller than 4x4 or not a multiple of 4 in size.
    (UUM-154799)

- `Graphics`: `SystemInfo.supportsParallelPSOCreation` now correctly returns `true` on<br>
    Android devices with a single core enabling parallel PSO creation.
    (UUM-153032)

- `HDRP`: Fixed "Default" being added to some Enum Material properties.
    ([UUM-134256](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134256))

- `HDRP`: Fixed a dark outline appearing around geometry against the sky when MSAA and a cloud layer are enabled.
    ([UUM-150911](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150911))

- `Input System`: This fixes Windows' Xbox Game Bar and macOS overlays \(Spotlight et al\). On Windows, Steam/Discord/NVIDIA overlays work as always.
    ([UUM-150045](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150045))

- `iOS`: Fixed a crash when `application:openURL` or `application:continueUserActivity` was called before Unity initialized.
    ([UUM-151801](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151801))

- `Kernel`: Fixed crash in NativeSlice caused by 32bit integer overflow.
    (UUM-154594)

- `License`: Fixed an issue where the Editor continued without a license, and exited with code 0 in batch mode, when it could not connect to the Unity Licensing Client.
    ([UUM-151817](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151817))

- `License`: Fixed the license error dialog looping on Retry and close when two Editors of the same version required incompatible Licensing Client versions.
    (UUM-153121)

- `Linux`: Fixed a crash on Linux when the Editor was launched with -nographics but without -batchmode; the Editor now reports the invalid arguments and exits with code 1.
    ([UUM-154576](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154576))

- `macOS`: Allow the system to sleep when Screen.sleepTimeout is set to SleepTimeout.SystemSetting and the System Setting is not Never.
    ([UUM-150222](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150222))

- `macOS`: Fixed the Editor slowing down in batch mode and automated test runs on macOS when one of its windows lost focus.

- `Networking`: Unity Transport: Fix a small memory leak that would occur when creating TLS/DTLS sessions.
    ([UUM-151755](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151755))

- `Scripting`: Fixed an issue where cancelling an Awaitable.NextFrameAsync or Awaitable.EndOfFrameAsync awaitable during a frame update could make an unrelated Awaitable complete early with a default result.
    ([UUM-156357](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156357))

- `Shaders`: Fixed a crash when calling RenderingCommandBuffer.SetKeyword with null compute shader.
    ([UUM-158327](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158327))

- `Shaders`: Fixed a crash when executing a RenderingCommandBuffer with a SetKeyword on a null or destroyed material.
    ([UUM-157105](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157105))

- `Shaders`: Fixed a possible Editor crash when shader messages were read while a shader variant compiled in the background.
    (UUM-154510)

- `Shaders`: Fixed crash in Editor when an uncompiled or broken shader is being rendered on a Canvas.
    ([UUM-153265](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153265))

- `Shaders`: Fixed Material.GetPropertyNames crashing when the provided value is outside of the valid enumeration range.
    ([UUM-157945](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157945))

- `SRP Core`: Fixed render passes not being merged on older iOS devices \(Apple GPU family 3 and below\) once a native pass was considered to be over the on-tile pixel storage limit, which serialized the whole frame into one native pass per render pass.
    ([UUM-148865](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148865))

- `SRP Core`: Fixed the Render Graph closing a native render pass after 8 raster render passes even when they used fewer than 8 native subpasses, which made the next pass, such as the URP UI overlay, load its attachments again from memory.
    ([UUM-158401](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158401))

- `UI Toolkit`: Fixed an AnimationCurve UXML attribute losing its value after saving when a key had a very large value.
    ([UUM-156823](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156823))

- `UI Toolkit`: Fixed artifacts around letters when text uses a Font Asset with a small atlas padding and a zero or negative outline width.
    ([UUM-146020](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146020))

- `UI Toolkit`: Fixed the Dynamic Atlas Viewer showing no atlas after the UI Toolkit Debugger window was recreated, such as when maximizing and restoring a docked window or toggling UI Toolkit Live Reload on the debugger.
    ([UUM-150663](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150663))

- `URP`: Fixed "CommandBuffer: temporary render texture not found while executing" warnings on DX11 when Compatibility Mode is enabled and an Overlay Camera uses a different Renderer than its Base Camera.
    ([UUM-117369](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-117369))

- `URP`: Fixed "Default" being added to some Enum Material properties.
    ([UUM-134256](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134256))

- `URP`: Fixed a bug where URP attempts to use a stripped variant when using deferred rendering with additional light shadows disabled, but shadowmasks enabled.
    ([UUM-153600](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153600))

- `URP`: Fixed an issue where the Renderer List and Culling samples in the URP RenderGraph Samples logged errors every frame when used with a 2D Renderer that has Depth/Stencil Buffer disabled.
    ([UUM-157948](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157948))

- `URP`: Fixed Shader Graphs importing to different shader code, and AssetBundles getting different hashes, depending on whether a Shader Graph with Support LOD Cross Fade enabled had been imported earlier in the same editor session.
    (UUM-155529)

- `XR`: Fixed SubsystemWithProvider.Start not throwing an ArgumentNullException when called after the subsystem was destroyed, which restarted the destroyed provider.
    ([UUM-151411](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151411))




## Package changes in 6000.0.86f1

## Packages updated

- `com.unity.2d.animation`: [10.2.3](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.2//changelog/CHANGELOG.html) to [10.2.4](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.2//changelog/CHANGELOG.html)

- `com.unity.2d.psdimporter`: [9.1.2](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.1//changelog/CHANGELOG.html) to [9.1.3](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.1//changelog/CHANGELOG.html)

- `com.unity.2d.tilemap.extras`: [4.1.1](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@4.1//changelog/CHANGELOG.html) to [4.1.2](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@4.1//changelog/CHANGELOG.html)

- `com.unity.burst`: [1.8.30](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) to [1.8.31](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.13.6](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.13//changelog/CHANGELOG.html) to [2.14.0](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.14//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.4.0](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.4//changelog/CHANGELOG.html) to [1.4.2](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.4//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: [3.8.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.8//changelog/CHANGELOG.html) to [3.8.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.8//changelog/CHANGELOG.html)

- `com.unity.services.cloudsave`: [3.4.0](https://docs.unity3d.com/Packages/com.unity.services.cloudsave@3.4//changelog/CHANGELOG.html) to [3.4.2](https://docs.unity3d.com/Packages/com.unity.services.cloudsave@3.4//changelog/CHANGELOG.html)

- `com.unity.services.wire`: [1.6.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.6//changelog/CHANGELOG.html) to [1.6.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.6//changelog/CHANGELOG.html)

- `com.unity.test-framework.performance`: [3.5.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.5//changelog/CHANGELOG.html) to [3.7.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.7//changelog/CHANGELOG.html)

- `com.unity.xr.oculus`: [4.5.4](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html) to [4.5.6](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: [2.0.15](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) to [2.0.16](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.12.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.12//changelog/CHANGELOG.html) to [1.12.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.12//changelog/CHANGELOG.html)

- `com.unity.cloud.draco`: [5.5.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.5//changelog/CHANGELOG.html) to [5.6.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.6//changelog/CHANGELOG.html)

- `com.unity.cloud.ktx`: [3.7.1](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.7//changelog/CHANGELOG.html) to [3.8.0](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.8//changelog/CHANGELOG.html)

- `com.unity.xr.compositionlayers`: [2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.6//changelog/CHANGELOG.html) to [2.6.1](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.6//changelog/CHANGELOG.html)

**Packages added**

- [com.unity.steamworks-api@1.0.0](https://docs.unity3d.com/Packages/com.unity.steamworks-api@1.0//changelog/CHANGELOG.html)