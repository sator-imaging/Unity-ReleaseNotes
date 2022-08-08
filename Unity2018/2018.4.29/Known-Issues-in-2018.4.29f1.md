# Unity 2018.4.29

https://unity3d.com/unity/whats-new/2018.4.29

## Known Issues in 2018.4.29f1



*   AI: A NavMeshAgent GameObject teleports to a near NavMeshSurface when collided with a moving NavMeshObstacle ([1072945](https://issuetracker.unity3d.com/issues/a-navmeshagent-gameobject-teleports-to-a-near-navmeshsurface-when-collided-with-a-moving-navmeshobstacle))
    
*   Audio: Crash on AudioSource::Stop when exiting Play mode ([1079263](https://issuetracker.unity3d.com/issues/crash-on-audiosource-stop-when-exiting-play-mode))
    
*   Linux: Focus cannot be properly gained on play mode, making keyboard input switch screens ([1109908](https://issuetracker.unity3d.com/issues/linux-focus-cannot-be-properly-gained-on-play-mode-making-keyboard-input-switch-screens))
    
*   Mobile: \[Android\]\[IL2CPP\] App crashes during launch with "Using memoryadresses from more than 16GB of memory" messages on Android 11 ([1284525](https://issuetracker.unity3d.com/issues/android-il2cpp-empty-project-crashes-on-launch-with-using-memoryadresses-from-more-than-16gb-of-memory-messages))
    
*   Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.
    
*   Scene Management: Allocated memory is not cleared when loading and unloading scenes ([1275751](https://issuetracker.unity3d.com/issues/allocated-memory-is-not-cleared-when-loading-and-unloading-scenes))
    
*   Vulkan: Right-clicking panels turns them black when Vulkan is the selected Graphics API ([1283290](https://issuetracker.unity3d.com/issues/right-clicking-panels-turns-them-black-when-vulkan-is-the-selected-graphics-api))
    
*   macOS: If the Android Tools are not installed through the Hub, macOS 10.15 (Catalina) default security settings will prevent the Android NDK binaries being executed. These settings have to be changed or a signed Android NDK (r16b) will be needed to build Android. More information here: https://developer.android.com/ndk/downloads/older\_releases.