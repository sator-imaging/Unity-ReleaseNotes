# Unity 2017.4.13f1
https://unity3d.com/unity/whatsnew/unity-2017.4.13

## Fixes

<ul>
<li><p>2D: Fixed Unity crashing on MonoStringNew when entering Play Mode after reopening the project and loading resources. (<a href="https://issuetracker.unity3d.com/issues/sprite-atlas-unity-crashes-on-monostringnew-when-entering-play-mode-after-reopening-the-project-and-loading-resources">1066715</a>)</p></li>
<li><p>Android: Allow Power VR devices to render at custom resolution with BlitType:Auto. (<a href="https://issuetracker.unity3d.com/issues/android-resolution-does-not-changes-when-changing-it-with-blit-type-auto-on-power-vr-devices">1022974</a>, 1066224)</p></li>
<li><p>Android: Increased JVM heap size from 2gb to 4gb. (<a href="https://issuetracker.unity3d.com/issues/android-gradle-build-fails-when-building-project-with-asset-bundle">969563</a>)</p></li>
<li><p>Asset Import: Fixed crash when re-importing assets for some global settings. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-on-std-tree-std-tmap-traits-core-basic-string-char-core-stringstoragedefault-when-reimporting-assets">1079532</a>, 1081907)</p></li>
<li><p>Asset Pipeline: Fixed crash when re-importing assets for some global settings. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-on-std-tree-std-tmap-traits-core-basic-string-char-core-stringstoragedefault-when-reimporting-assets">1079532</a>, 1081907)</p></li>
<li><p>Editor: Fixed colliding file ids in YAMLMerge not tracking already remapped keys. (1076700)</p></li>
<li><p>Editor: Fixed UnityConnectSettings initialization. (<a href="https://issuetracker.unity3d.com/issues/editor-exits-with-return-code-0-even-with-compilation-errors-when-unity-analytics-is-enabled">1058840</a>)</p></li>
<li><p>IL2CPP: Fixing an issue with certain unprintable characters in C# source code causing failed compilations when they are copied to the C++ code as comments. (1049221)</p></li>
<li><p>iOS: Fixed CoreLocation framework being included even if the location API is not used. (<a href="https://issuetracker.unity3d.com/issues/ios-update-location-service-api-according-to-the-new-app-store-guidelines-apps-will-be-rejected-starting-spring-2019">1076345</a>)</p></li>
<li><p>iOS: Fixed standard shader artifacts on mobiles. (1087277)</p></li>
<li><p>iOS: Fixed unassigned icon warning in Xcode when locale is not using "." as the decimal separator. (<a href="https://issuetracker.unity3d.com/issues/dot-net4-dot-x-using-french-as-default-language-on-mac-building-ios-app-gives-unassigned-icon-warning-in-xcode">1058928</a>)</p></li>
<li><p>iOS: Fixed unassigned icon warning in Xcode when locale is not using "." as the decimal separator. (<a href="https://issuetracker.unity3d.com/issues/dot-net4-dot-x-using-french-as-default-language-on-mac-building-ios-app-gives-unassigned-icon-warning-in-xcode">1058928</a>)</p></li>
<li><p>Kernel: Fixed ParticleSystemGeometryJob::ScheduleJobs crash when deleting GameObject. (<a href="https://issuetracker.unity3d.com/issues/crash-on-particlesystemgeometryjob-schedulejobs-when-deleting-gameobject">1051704</a>, 1081788)</p></li>
<li><p>Particles: Fixed temp memory not being cleaned up even when simulation doesn't need advancing. (<a href="https://issuetracker.unity3d.com/issues/particle-system-using-skinnedmeshrenderer-shape-generate-warning-and-error-when-timescale-is-set-to-0">1028462</a>)</p></li>
<li><p>Physics: Fixed an issue where physics internal data wasn't being updated if the scene only contained static colliders, causing issues with shape casts. (<a href="https://issuetracker.unity3d.com/issues/windows-physics-dot-spherecast-does-not-properly-detect-collisions-when-clicking-on-certain-objects-spots">1064897</a>)</p></li>
<li><p>Physics: Fixed issue where physics internal query data may not be updated if there are only static colliders in scene, causing shape cast issue. (<a href="https://issuetracker.unity3d.com/issues/windows-physics-dot-spherecast-does-not-properly-detect-collisions-when-clicking-on-certain-objects-spots">1064897</a>)</p></li>
<li><p>SceneManager: Fixed crashes caused by incorrectly activated children of inactive parents. (<a href="https://issuetracker.unity3d.com/issues/crash-on-particlesystemgeometryjob-schedulejobs-when-deleting-gameobject">1051704</a>, 1081788)</p></li>
<li><p>Shaders: Fixed Android + Vulkan shader compilation failure. (1080403)</p></li>
<li><p>Shuriken: Added handling of NaN coming from PhysX due to internal bug. (<a href="https://issuetracker.unity3d.com/issues/invalid-worldaabb-console-errors-are-thrown-after-particle-collisions-in-the-scene">943649</a>, 1063373)</p></li>
<li><p>XR: Fixed issue of error spam when depth buffer sharing was enabled during Holographic Remoting or Simulation. (<a href="https://issuetracker.unity3d.com/issues/windowsmr-failure-to-get-rendering-parameters-for-main-camera-when-depth-buffer-sharing-is-enabled">1047269</a>)</p></li>
</ul>

#### Revision: 6902ad48015d
