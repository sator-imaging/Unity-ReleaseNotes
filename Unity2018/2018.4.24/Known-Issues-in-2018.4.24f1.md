# Unity 2018.4.24

https://unity3d.com/unity/whats-new/2018.4.24

## Known Issues in 2018.4.24f1



*   Animation: Animator.Update CPU time spikes when multiple animations are playing ([1184690](https://issuetracker.unity3d.com/issues/animator-dot-update-cpu-time-spikes-when-multiple-animations-are-playing))
    
*   Asset Importers: Crash on VertexDeclarationD3D11::GetInputLayout when importing a broken FBX file ([1239074](https://issuetracker.unity3d.com/issues/crash-on-vertexdeclarationd3d11-getinputlayout-when-importing-a-broken-fbx-file))
    
*   Cloth: Cloth has graphical artifacts when an object moves out of the camera ([1254174](https://issuetracker.unity3d.com/issues/cloth-has-graphical-artifacts-when-an-object-moves-out-of-the-camera))
    
*   Mono: Crash on buffer\_add\_value\_full when debugging with code editor attached ([1249172](https://issuetracker.unity3d.com/issues/macos-crash-on-buffer-add-value-full-when-debugging-with-code-editor-attached))
    
*   Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.
    
*   Shuriken: Crash on CreateDirect3D11SurfaceFromDXGISurface when calling DrawRenderer with a Trail Renderer ([1216216](https://issuetracker.unity3d.com/issues/crash-on-createdirect3d11surfacefromdxgisurface-when-calling-drawrenderer-with-a-trail-renderer))
    
*   macOS: If the Android Tools are not installed through the Hub, macOS 10.15 (Catalina) default security settings will prevent the Android NDK binaries being executed. These settings have to be changed or a signed Android NDK (r16b) will be needed to build Android. More information here: https://developer.android.com/ndk/downloads/older\_releases.