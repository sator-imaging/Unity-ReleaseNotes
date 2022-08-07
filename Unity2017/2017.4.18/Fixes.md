# Unity 2017.4.18
https://unity3d.com/unity/whats-new/2017.4.18

## Fixes

<ul>
<li><p>2D: Fixed a crash when packing certain Sprite Atlas on Android. (<a href="https://issuetracker.unity3d.com/issues/editor-crashes-on-blockmask-fillspritedata-when-packing-certain-sprite-atlas-on-android-platform">1017666</a>, 1101608)</p></li>
<li><p>Android: Fixed Android Gradle manifest merging when plugins are missing SDK target version in manifest. (<a href="https://issuetracker.unity3d.com/issues/android-read-external-storage-gets-added-twice-to-android-manifest-while-ignoring-the-maxsdkversion">1084622</a>, 1090922)</p></li>
<li><p>Android: Texture2DArray and Texture3D now check if the filtering mode is supported by the GPU and downgrade when necessary. (1066181)</p></li>
<li><p>IL2CPP: Fixed crash when using StructLayout attribute and specifying a Pack value. (1099207)</p></li>
<li><p>iOS: Fixed a crash when using using static const std::string in Xcode 9. (<a href="https://issuetracker.unity3d.com/issues/ios-native-static-const-std-string-causes-crash-in-signal-sigkill-when-using-xcode-9">1050875</a>, 1102753)</p></li>
<li><p>iOS: Fixed AudioClips with future timestamps import issue. (<a href="https://issuetracker.unity3d.com/issues/editor-didnt-recognize-audio-files-if-file-created-data-is-greater-than-your-actual-data-time-is">951169</a>, 1104104)</p></li>
<li><p>Kernel: Fixed an issue which could cause an error when reading files from disk. (1092419)</p></li>
<li><p>Mobile: Android gradle daemons are now killed when the editor is shut down instead of after every build. (<a href="https://issuetracker.unity3d.com/issues/do-not-kill-other-gradle-daemons-when-build-completes">1041385</a>)</p></li>
<li><p>Package Manager: Fixed an issue where errors were not handled in a consistent manner when a package cannot be found on the registry.</p></li>
<li><p>Shaders: Allow loading shaders from AssetBundles that were created in 2017.2. (1091064)</p></li>
<li><p>WebGL: Fixed camera viewport rect bug in WebGL + Linear color space. (<a href="https://issuetracker.unity3d.com/issues/webgl-linear-color-space-camera-viewport-rect-problem-in-built-game">957652</a>)</p></li>
<li><p>WebGL: Fixed canvas resize when using Linear color space. (<a href="https://issuetracker.unity3d.com/issues/webgl-canvas-size-slash-resolution-will-not-scale-in-browser-when-using-linear-color-space">977579</a>)</p></li>
</ul>

#### Changeset: a9236f402e28
