# Unity 2018.2.12f1
https://unity3d.com/unity/whatsnew/unity-2018.2.12

## Fixes

<ul>
<li><p>Android: Allow Power VR devices rendering at custom resolution with BlitType:Auto. (<a href="https://issuetracker.unity3d.com/issues/android-resolution-does-not-changes-when-changing-it-with-blit-type-auto-on-power-vr-devices">1022974</a>, 1063419)</p></li>
<li><p>Animation: Fixed crash when using the GameObjectRecorder with an invalid EditorCurveBinding. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-on-unityengine-animation-getfloatvalue-when-using-gameobjectrecorder-dot-takesnapshot">1076523</a>)</p></li>
<li><p>Asset Import: Fixed crash when re-importing assets for some global settings. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-on-std-tree-std-tmap-traits-core-basic-string-char-core-stringstoragedefault-when-reimporting-assets">1079532</a>, 1081911)</p></li>
<li><p>Build Pipeline: Fixed crash in "il2cpp::utils::Debugger::InitializeTypeSourceFileMap()" at startup. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-dot-net-4-dot-x-crash-in-il2cpp-utils-debugger-initializetypesourcefilemap-at-startup">1051393</a>)</p></li>
<li><p>Editor: Fix colliding file ids in YAMLMerge not tracking already remapped keys. (1076698)</p></li>
<li><p>Graphics: Fixed a race condition in the culling code that would free memory of a job that is still in-flight leading to a crash in the editor. (<a href="https://issuetracker.unity3d.com/issues/unity-crashes-when-legacy-deferred-rendering-path-is-used-in-scene-which-contains-shadows">1062032</a>)</p></li>
<li><p>IL2CPP: Add support for building with Xcode 10 and the macOS 10.14 SDK.</p></li>
<li><p>IL2CPP: Fixed memory mapped files with an offset not being handled correctly. (<a href="https://issuetracker.unity3d.com/issues/memorymappedfile-class-crashes-on-il2cpp-builds">1082118</a>)</p></li>
<li><p>IL2CPP: Fixed proper C++ code not being generated for unsafe C# which accesses an array element via a pointer. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-unity-editor-fails-to-build-when-auto-generating-a-c-number-array-of-pointers-in-c">1081052</a>)</p></li>
<li><p>IL2CPP: Fixed the proper default p/invoke function name for Win32 API functions not being called. (1079850)</p></li>
<li><p>IMGUI: Fixing issue with 16bit chars not displaying correctly. (<a href="https://issuetracker.unity3d.com/issues/korean-ime-certain-combinations-of-korean-letters-get-deleted-from-the-inputfield-upon-typing">1067159</a>)</p></li>
<li><p>iOS: Fixed "textures used in draw call" not using our hash_set instead of std::set. (1061553)</p></li>
<li><p>iOS: Fixed Screen.safeArea not being reported correctly when orientation is changed. (<a href="https://issuetracker.unity3d.com/issues/ios-iphonex-screen-dot-safearea-is-ignored-in-portrait-mode-until-screen-orientation-is-changed">1028312</a>, 1037753)</p></li>
<li><p>Physics: Fixed contact callback assertion errors when using multi-threaded 2D physics. (<a href="https://issuetracker.unity3d.com/issues/multithreaded-physics2d-fires-asserts-related-to-contacts2d">1042478</a>)</p></li>
<li><p>Physics: Fixed intermittent editor crash when using multi-threaded 2D physics. (<a href="https://issuetracker.unity3d.com/product/unity/issues/guid/1082697">1082697</a>)</p></li>
<li><p>Physics: FIxed Joint2D.breakForce and Joint2D.breakTorque not able to be set to infinity. (<a href="https://issuetracker.unity3d.com/issues/invalid-assign-attempt-error-is-thrown-when-trying-to-set-joint2ds-breakforce-and-breaktorque-to-infinity-via-script">1065618</a>)</p></li>
<li><p>Physics: Fixed OnCollisionEnter2D occasionally returning zero normal/tangent impulse when using Continuous Collision Detection mode on a Rigidbody2D. (<a href="https://issuetracker.unity3d.com/issues/continous-sometimes-relativevelocity-returned-in-oncollisionenter2d-is-zero">1080330</a>)</p></li>
<li><p>Physics: Fixed OnCollisionEnter2D occasionally returning zero relative-velocity when using Continuous Collision Detection mode on a Rigidbody2D. (<a href="https://issuetracker.unity3d.com/issues/collision2d-dot-contacts-often-reports-a-normalimpulse-of-0-for-heavy-collisions">1037965</a>)</p></li>
<li><p>Scripting: Fixed incorrect Transform.hierarchyCount and Transform.hierarchyCapacity properties. (<a href="https://issuetracker.unity3d.com/issues/transform-dot-hierarchycount-always-returns-0-regardless-of-the-number-of-transforms-in-the-transforms-hierarchy-data-structure">1079998</a>, 1082886)</p></li>
<li><p>Scripting: Fixed TLS related crash. (1073395)</p></li>
<li><p>Scripting Upgrade: Fixed crash when calling Application.Unload. (<a href="https://issuetracker.unity3d.com/issues/application-dot-unload-crashes-with-the-4-dot-x-scripting-runtime">1060891</a>)</p></li>
<li><p>Scripting Upgrade: Fixed potential deadlock on OSX. (1077203)</p></li>
<li><p>Scripting Upgrade: Fixed SslStream/UnityTlsContext not reporting gracefully closed Streams on read. (1076788)</p></li>
<li><p>Shaders: Added two env vars to override the default shader compiler timeouts: UNITY_SHADER_COMPILER_TASK_TIMEOUT_MINUTES overrides the timeout for waiting a response from a compiler task (compile, preprocess, disassemble)
UNITY_SHADER_COMPILER_CONNECT_TIMEOUT_SECONDS overrides the initial connection creation timeout. (1038278)</p></li>
<li><p>Shaders: Added two env vars to override the default shader compiler timeouts: UNITY_SHADER_COMPILER_TASK_TIMEOUT_MINUTES overrides the timeout for waiting a response from a compiler task (compile, preprocess, disassemble)
UNITY_SHADER_COMPILER_CONNECT_TIMEOUT_SECONDS overrides the initial connection creation timeout. (1072458)</p></li>
<li><p>Shuriken: Fixed syncing transforms when acquiring the light prefab in particle systems. (<a href="https://issuetracker.unity3d.com/issues/particle-system-updates-lights-when-there-are-no-active-particles">1064232</a>)</p></li>
<li><p>Timeline: Fixed temporary game object being created for custom tracks by Timeline Editor. (<a href="https://issuetracker.unity3d.com/issues/timeline-creates-a-dummy-object-when-trackbindingtype-of-a-script-component-is-specified">1082600</a>)</p></li>
<li><p>Timeline: Fixed timeline scrubbing for subemitters with autorandomseed. (<a href="https://issuetracker.unity3d.com/issues/timelines-control-track-overrides-the-auto-random-seed-with-the-same-value-for-all-nested-particle-systems">1076850</a>)</p></li>
<li><p>Timeline: Fixed tooltip typo in control tracks. (<a href="https://issuetracker.unity3d.com/issues/random-seeds-tooltip-of-the-timelines-control-track-has-a-typo">1083618</a>)</p></li>
<li><p>XR: Fixed incorrect device position when building ARCore apps targeting x86.</p></li>
</ul>

#### Revision: 0a46ddfcfad4
