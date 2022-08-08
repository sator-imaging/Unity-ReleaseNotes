# Unity 2018.4.19

https://unity3d.com/unity/whats-new/2018.4.19f1

## Known Issues in 2018.4.19f1



*   Animation: Animator.Update CPU time spikes when multiple animations are playing ([1184690](https://issuetracker.unity3d.com/issues/animator-dot-update-cpu-time-spikes-when-multiple-animations-are-playing))
    
*   Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.
    
*   Profiling: Editor crashes when loading profiler file with memcpy stacktrace ([1131782](https://issuetracker.unity3d.com/issues/editor-crashes-when-loading-profiler-file-with-memcpy-stacktrace))
    
*   Profiling: Performance decrease in EditorOverhead using Deep Profile ([1051094](https://issuetracker.unity3d.com/issues/performance-decrease-in-editoroverhead-using-deep-profile))
    
*   Scene Management: Prefabs lose their values if scripts are removed then reintroduced ([1216914](https://issuetracker.unity3d.com/issues/prefabs-lose-their-values-if-scripts-are-removed-then-reintroduced))
    
*   macOS: If the Android Tools are not installed through the Hub, macOS 10.15 (Catalina) default security settings will prevent the Android NDK binaries being executed. These settings have to be changed or a signed Android NDK (r16b) will be needed to build Android. More information here: https://developer.android.com/ndk/downloads/older\_releases.