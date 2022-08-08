# Unity 2018.4.22

https://unity3d.com/unity/whats-new/2018.4.22f1

## Known Issues in 2018.4.22f1



*   Animation: Animator.Update CPU time spikes when multiple animations are playing ([1184690](https://issuetracker.unity3d.com/issues/animator-dot-update-cpu-time-spikes-when-multiple-animations-are-playing))
    
*   Graphics - General: 'task.rasterData.vertexBuffer == NULL' errors when using a Particle System ([1226357](https://issuetracker.unity3d.com/issues/task-dot-rasterdata-dot-vertexbuffer-equals-equals-null-errors-when-using-a-particle-system))
    
*   Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.
    
*   Scene Management: Prefab Variant Transform fileId changes ([1238280](https://issuetracker.unity3d.com/issues/prefab-variant-transform-fileid-changes))
    
*   Scene Management: Unity Editor freezes/crashes when opening a specific Scene ([1228147](https://issuetracker.unity3d.com/issues/unity-editor-freezes-slash-crashes-when-opening-a-specific-scene))
    
*   Shuriken: Crash on CreateDirect3D11SurfaceFromDXGISurface when calling DrawRenderer with a Trail Renderer ([1216216](https://issuetracker.unity3d.com/issues/crash-on-createdirect3d11surfacefromdxgisurface-when-calling-drawrenderer-with-a-trail-renderer))
    
*   macOS: If the Android Tools are not installed through the Hub, macOS 10.15 (Catalina) default security settings will prevent the Android NDK binaries being executed. These settings have to be changed or a signed Android NDK (r16b) will be needed to build Android. More information here: https://developer.android.com/ndk/downloads/older\_releases.