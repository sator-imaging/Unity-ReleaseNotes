# Unity 2018.4.16

https://unity3d.com/unity/whats-new/2018.4.16f1

## Known Issues in 2018.4.16f1



*   Animation: Animator.Update CPU time spikes when multiple animations are playing ([1184690](https://issuetracker.unity3d.com/issues/animator-dot-update-cpu-time-spikes-when-multiple-animations-are-playing))
    
*   Asset Bundles: Building asset bundles when build path doesn't exist causes a failed assertion on "pluginAppendices.size() <= 1" ([1203242](https://issuetracker.unity3d.com/issues/building-asset-bundles-causes-an-assertion-pluginappendices-dot-size-equals-1-on-the-editor))
    
*   Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.
    
*   Profiling: Profiler stucks with Autoconnected Player option and can't be switched back to Editor when AndroidPlayer is selected ([1193777](https://issuetracker.unity3d.com/issues/profiler-stucks-with-autoconnected-player-option-and-cant-be-switched-back-to-editor-when-androidplayer-is-selected))
    
*   Shuriken: Semaphore.WaitForSignal under Canvas.BuildBatch causes a slow editor in Play mode ([1178300](https://issuetracker.unity3d.com/issues/semaphore-dot-waitforsignal-causes-a-slow-editor-when-entering-play-mode))