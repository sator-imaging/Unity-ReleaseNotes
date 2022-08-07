# Unity 2018.4.17 
https://unity3d.com/unity/whats-new/2018.4.17f1

## Known Issues in 2018.4.17f1

<ul>
<li><p>2D: Crash on memory allocation when double-clicking a Sprite which size is reassigned in OnDrawGizmos (<a href="https://issuetracker.unity3d.com/issues/crash-on-memory-allocation-when-double-clicking-a-sprite-which-size-is-reassigned-in-ondrawgizmos">1211482</a>)</p></li>
<li><p>Animation: Animator.Update CPU time spikes when multiple animations are playing (<a href="https://issuetracker.unity3d.com/issues/animator-dot-update-cpu-time-spikes-when-multiple-animations-are-playing">1184690</a>)</p></li>
<li><p>Asset Bundles: Asset Bundles fail to load when using async loading methods (<a href="https://issuetracker.unity3d.com/issues/asset-bundles-fail-to-load-when-using-async-loading-methods">1215446</a>)</p></li>
<li><p>Asset Bundles: Building asset bundles when build path doesn't exist causes a failed assertion on "pluginAppendices.size() &lt;= 1" (<a href="https://issuetracker.unity3d.com/issues/building-asset-bundles-causes-an-assertion-pluginappendices-dot-size-equals-1-on-the-editor">1203242</a>)</p></li>
<li><p>Graphics - General: Shader is rendered incorrectly when loaded from an Asset Bundle made in Unity 2017.4 in a newer version  (<a href="https://issuetracker.unity3d.com/issues/shader-is-rendered-incorrectly-when-loaded-from-an-asset-bundle-made-in-unity-2017-dot-4-in-a-newer-version">1195750</a>)</p></li>
<li><p>IMGUI: Editor crashes silently when assertion is not met after calling EditorGUILayout.EnumPopup (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-silently-when-assertion-is-not-met-after-calling-editorguilayout-dot-enumpopup">1209597</a>)</p></li>
<li><p>Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.</p></li>
<li><p>Shuriken: Semaphore.WaitForSignal under Canvas.BuildBatch causes a slow editor in Play mode (<a href="https://issuetracker.unity3d.com/issues/semaphore-dot-waitforsignal-causes-a-slow-editor-when-entering-play-mode">1178300</a>)</p></li>
<li><p>Windows: UnityWebRequest fails to verify certificate when "Let's Encrypt Authority X1" certificate is present in system trust store (<a href="https://issuetracker.unity3d.com/issues/unitywebrequest-fails-to-verify-certificate-when-lets-encrypt-authority-x1-certificate-is-present-in-system-trust-store">1215665</a>)</p></li>
<li><p>macOS: If the Android Tools are not installed through the Hub, macOS 10.15 (Catalina) default security settings will prevent the Android NDK binaries being executed. These settings have to be changed or a signed Android NDK (r16b) will be needed to build Android. More information here: https://developer.android.com/ndk/downloads/older_releases.</p></li>
</ul>
