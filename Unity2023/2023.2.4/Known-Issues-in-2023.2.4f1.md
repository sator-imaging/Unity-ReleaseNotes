# Unity 2023.2.4

https://unity.com/releases/editor/whats-new/2023.2.4

## Known Issues in 2023.2.4f1



*   3D Physics: Crash on OverlapSphereCommandJob when entering the Play Mode ([UUM-33459](https://issuetracker.unity3d.com/issues/crash-on-overlapspherecommandjob-when-entering-the-play-mode))
    
*   Asset - Database: Crash on Object::IncrementPersistentDirtyIndex when upgrading project version ([UUM-57909](https://issuetracker.unity3d.com/issues/crash-on-object-incrementpersistentdirtyindex-when-upgrading-project-version))
    
*   Asset Bundles: UV1 data is lost during AssetBundle build when Optimize Mesh Data is on ([UUM-57201](https://issuetracker.unity3d.com/issues/uv1-data-is-lost-during-assetbundle-build-when-optimize-mesh-data-is-on))
    
*   Audio Authoring: Crash on AudioUtil\_CUSTOM\_HasAudioCallback when exiting Play Mode while the Inspector is displaying a GameObject with a script attached ([UUM-58481](https://issuetracker.unity3d.com/issues/crash-on-audioutil-custom-hasaudiocallback-when-exiting-play-mode-while-the-inspector-is-displaying-a-gameobject-with-an-empty-script-attached))
    
*   Audio Authoring: Wrong tooltip when hovering over the "Load In Background" property of an audio clip ([UUM-27581](https://issuetracker.unity3d.com/issues/wrong-tooltip-when-hovering-over-the-load-in-background-property-of-an-audio-clip))
    
*   Audio Random Container: Windows get messed up due to ARC ([UUM-55116](https://issuetracker.unity3d.com/issues/windows-get-messed-up-due-to-arc))
    
*   Culling: Crash on PrepareDrawShadowsCommandStep1 when selecting a camera while the Occlusion Culling window is open ([UUM-506](https://issuetracker.unity3d.com/issues/crash-on-preparedrawshadowscommandstep1-when-selecting-a-camera-while-the-occlusion-culling-window-is-open))
    
*   DOTS: \[Mobile\] Player freezes on "UnityClassic::Baselib\_SystemFutex\_Wait" or silently crashes ([UUM-41806](https://issuetracker.unity3d.com/issues/android-player-freezes-on-unityclassic-baselib-systemfutex-wait-or-silently-crashes))
    
*   IAP: \[Android\] The Player crashes with a "JNI ERROR (app bug)" error when the global reference table gets overflowed by BillingClientStateListener ([UUM-55105](https://issuetracker.unity3d.com/issues/android-the-player-crashes-with-a-jni-error-app-bug-error-when-the-global-reference-table-gets-overflowed-by-billingclientstatelistener))
    
*   IL2CPP: \[Android\] Crash on Android when AndroidJavaProxy is calling from multiple threads ([UUM-49357](https://issuetracker.unity3d.com/issues/android-crash-on-android-when-androidjavaproxy-is-calling-from-multiple-threads))
    
*   Input: Crash on InputDeviceIOCTL when closing Unity editor ([UUM-10774](https://issuetracker.unity3d.com/issues/crash-on-inputdeviceioctl-when-closing-unity-editor))
    
*   Mono: Crash in CollectManagedImportDependencyGetters inside OpenScene in batch mode ([UUM-57742](https://issuetracker.unity3d.com/issues/crash-in-collectmanagedimportdependencygetters-inside-openscene-in-batch-mode))
    
*   Packman: Users cannot export bundled plugins into a .unitypackage anymore ([UUM-37376](https://issuetracker.unity3d.com/issues/console-error-error-while-exporting-package-no-assets-to-export-only-folders-did-you-mean-to-use-exportpackageoptions-dot-recurse-when-trying-to-export-a-bundle-file-as-a-package))
    
*   PhysX Integration: ConfigurableJoint's drives behave differently after the PhysX 4.1.2 update ([UUM-55081](https://issuetracker.unity3d.com/issues/rigidbody-components-values-do-not-translate-to-the-physx-calculations-when-they-are-being-overridden-via-a-script))
    
*   Platform Audio: Audio is delayed by ~0,5 sec after starting to play it in the Android/iOS Player ([UUM-41494](https://issuetracker.unity3d.com/issues/audio-is-delayed-by-05-sec-after-starting-to-play-it-in-the-android-slash-ios-player))
    
*   Platform Audio: \[WebGL\] A looping audio sounds different on WebGL than in the editor/native desktop player ([UUM-12530](https://issuetracker.unity3d.com/issues/webgl-a-looping-audio-sounds-different-on-webgl-than-in-the-editor-slash-native-desktop-player))
    
*   Progressive Lightmapper: The Editor becomes unresponsive and memory allocation errors are spammed in the Console when Generating Lightning ([UUM-58017](https://issuetracker.unity3d.com/issues/the-editor-becomes-unresponsive-and-memory-allocation-errors-are-spammed-in-the-console-when-generating-lightning))
    
*   Scene Management: Crash on GameObject::QueryComponentByType when opening a project ([UUM-58461](https://issuetracker.unity3d.com/issues/crash-on-gameobject-querycomponentbytype-when-opening-a-project))
    
*   Serialization: Crash on EditorOnlyPlayerSettings::GetDefaultTextureCompressionFormat when selecting a Texture 2D asset ([UUM-55126](https://issuetracker.unity3d.com/issues/crash-on-editoronlyplayersettings-getdefaulttexturecompressionformat-when-selecting-a-texture-2d-asset))
    
*   Shortcut Management: Scene view Camera cannot be moved with WASD/QE keys when the Right Mouse Button is held down and the Mouse is not moved ([UUM-57993](https://issuetracker.unity3d.com/issues/scene-view-camera-cannot-be-moved-with-wasd-slash-qe-keys-when-the-right-mouse-button-is-held-down-and-the-mouse-is-not-moved))
    
*   XR SRP: \[Quest\] Stutter/Frame Pacing with OculusRuntime.WaitToBeginFrame when the Player is built ([UUM-27247](https://issuetracker.unity3d.com/issues/quest-stutter-slash-frame-pacing-with-oculusruntime-dot-waittobeginframe-when-the-player-is-built))