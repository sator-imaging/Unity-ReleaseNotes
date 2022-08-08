# Unity 2018.4.25

https://unity3d.com/unity/whats-new/2018.4.25

## Known Issues in 2018.4.25f1



*   Animation: Animator.Update CPU time spikes when multiple animations are playing ([1184690](https://issuetracker.unity3d.com/issues/animator-dot-update-cpu-time-spikes-when-multiple-animations-are-playing))
    
*   Asset Importers: Crash on VertexDeclarationD3D11::GetInputLayout when importing a broken FBX file ([1239074](https://issuetracker.unity3d.com/issues/crash-on-vertexdeclarationd3d11-getinputlayout-when-importing-a-broken-fbx-file))
    
*   Audio: Editor crashes on changing 'System Sample Rate' when Audio track preview is being played in Timeline window ([1232743](https://issuetracker.unity3d.com/issues/audio-editor-crashes-on-changing-system-sample-rate-when-audio-track-preview-is-being-played-in-timeline-window))
    
*   MacOS: \[Mac\] Many artifacts can be seen in Scene View when Scene Light is enabled and HDR is on with Metal API and Mac OS X 10.15.4 ([1240265](https://issuetracker.unity3d.com/issues/mac-many-artifacts-can-be-seen-in-scene-view-when-scene-light-is-enabled-on-with-metal-api-and-mac-os-x-10-dot-15-dot-4))
    
*   Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.
    
*   Profiling: Performance issue in "Profiler" UI with increasing number of events ([967289](https://issuetracker.unity3d.com/issues/performance-issue-in-profiler-ui-with-increasing-number-of-events))
    
*   Scene Management: Unity crashes when opening a project with two identical scenes, one of them being unloaded ([1069650](https://issuetracker.unity3d.com/issues/unity-crashes-when-opening-a-project-with-two-identical-scenes-one-of-them-being-unloaded))
    
*   macOS: If the Android Tools are not installed through the Hub, macOS 10.15 (Catalina) default security settings will prevent the Android NDK binaries being executed. These settings have to be changed or a signed Android NDK (r16b) will be needed to build Android. More information here: https://developer.android.com/ndk/downloads/older\_releases.