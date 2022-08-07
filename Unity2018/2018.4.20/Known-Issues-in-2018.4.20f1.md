# Unity 2018.4.20
https://unity3d.com/unity/whats-new/2018.4.20

## Known Issues in 2018.4.20f1

<ul>
<li><p>Animation: Animator.Update CPU time spikes when multiple animations are playing (<a href="https://issuetracker.unity3d.com/issues/animator-dot-update-cpu-time-spikes-when-multiple-animations-are-playing">1184690</a>)</p></li>
<li><p>MacOS: [Lighting]Errors in console on changing editor visualization mode to realtime GI if there is a particle system in scene. (<a href="https://issuetracker.unity3d.com/issues/lighting-errors-in-console-on-changing-editor-visualization-mode-to-realtime-gi-if-there-is-a-particle-system-in-scene">1106901</a>)</p></li>
<li><p>Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.</p></li>
<li><p>Profiling: Editor crashes when loading profiler file with memcpy stacktrace (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-when-loading-profiler-file-with-memcpy-stacktrace">1131782</a>)</p></li>
<li><p>Profiling: Performance decrease in EditorOverhead using Deep Profile  (<a href="https://issuetracker.unity3d.com/issues/performance-decrease-in-editoroverhead-using-deep-profile">1051094</a>)</p></li>
<li><p>macOS: If the Android Tools are not installed through the Hub, macOS 10.15 (Catalina) default security settings will prevent the Android NDK binaries being executed. These settings have to be changed or a signed Android NDK (r16b) will be needed to build Android. More information here: https://developer.android.com/ndk/downloads/older_releases.</p></li>
</ul>
