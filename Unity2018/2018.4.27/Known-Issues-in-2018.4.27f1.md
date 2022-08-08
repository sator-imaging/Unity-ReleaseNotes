# Unity 2018.4.27

https://unity3d.com/unity/whats-new/2018.4.27

## Known Issues in 2018.4.27f1



*   AI: A NavMeshAgent GameObject teleports to a near NavMeshSurface when collided with a moving NavMeshObstacle ([1072945](https://issuetracker.unity3d.com/issues/a-navmeshagent-gameobject-teleports-to-a-near-navmeshsurface-when-collided-with-a-moving-navmeshobstacle))
    
*   Audio: Unity crashes in Play Mode at FMOD\_Resampler\_Linear ([928576](https://issuetracker.unity3d.com/issues/unity-crashes-in-play-mode-at-fmod-resampler-linear))
    
*   MacOS: \[Mac\] Many artifacts can be seen in Scene View when Scene Light is enabled and HDR is on with Metal API and Mac OS X 10.15.4 ([1240265](https://issuetracker.unity3d.com/issues/mac-many-artifacts-can-be-seen-in-scene-view-when-scene-light-is-enabled-on-with-metal-api-and-mac-os-x-10-dot-15-dot-4))
    
*   MacOS: \[OSX\] Shader import in an external exFAT drive crashes Unity ([727114](https://issuetracker.unity3d.com/issues/osx-shader-import-in-an-external-exfat-drive-crashes-unity))
    
*   Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.
    
*   Scene Management: Building project when two identical scenes are open crashes the editor ([1266194](https://issuetracker.unity3d.com/issues/building-project-when-two-identical-scenes-are-open-crashes-the-editor))
    
*   Scripting: Building a project crashes when a Script Component has serialized array of a type that contains a serialized PropertyName field ([1267271](https://issuetracker.unity3d.com/issues/building-a-project-crashes-when-a-script-component-has-serialized-array-of-a-type-that-contains-a-serialized-propertyname-field))
    
*   Shader System: \[Bug\] "min16f as def32" modifier in FXC bytecode not honored when converting to SPIR-V/ESSL ([1228687](https://issuetracker.unity3d.com/issues/min16f-as-def32-modifier-in-fxc-bytecode-not-honored-when-converting-to-spir-v-slash-essl))
    
*   Windows: Cannot activate license within a docker container ([1193364](https://issuetracker.unity3d.com/issues/cannot-activate-license-within-a-docker-container))
    
*   Windows: Crash on D3D12SwapChain::CreateHWND when CreateSwapChainForHwnd returns E\_INVALIDARG ([1223896](https://issuetracker.unity3d.com/issues/crash-on-d3d12swapchain-createhwnd-when-createswapchainforhwnd-returns-e-invalidarg))
    
*   macOS: If the Android Tools are not installed through the Hub, macOS 10.15 (Catalina) default security settings will prevent the Android NDK binaries being executed. These settings have to be changed or a signed Android NDK (r16b) will be needed to build Android. More information here: https://developer.android.com/ndk/downloads/older\_releases.