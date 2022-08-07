# Unity 2018.3.7
https://unity3d.com/unity/whats-new/2018.3.7

## Fixes

<ul>
<li><p>Fixed security vulnerability. (<a href="/security#CVE-2019-9197">CVE-2019-9197</a>).</p></li>
<li><p>Analytics: Fixed issue: usage statistics will no longer be sent when editor analytics is disabled.</p></li>
<li><p>2D: Fixed "Invalid SortingGroup index set in Renderer" warning from occurring after removing Sorting Group component on an object with nested Sorting Groups. (1106381)</p></li>
<li><p>2D: Fixed Sprites randomly flipping when moving/zooming camera (1117333)</p></li>
<li><p>Android: Fixed hang at exit if submitting AndroidJavaProxy/Runnable to UI thread. (<a href="https://issuetracker.unity3d.com/issues/android-androidjavarunnable-causes-player-to-timeout-slash-hang-when-quitting">1113139</a>, 1124900)</p></li>
<li><p>Android: Fixed an out of memory issue happening on Adreno devices on GLES. (1111097)</p></li>
<li><p>Asset Bundles: Fixed error when loading an object from an asset bundle on the first frame of a scene load operation under certain conditions. (<a href="https://issuetracker.unity3d.com/issues/editor-serialization-assetbundle-dot-loadassetasync-corrupting-last-asset-in-a-set">1094045</a>)</p></li>
<li><p>Build Pipeline: Removed unnecessary files from mac standalone build, reducing the size by about 500kb. (1111649)</p></li>
<li><p>Editor: Fixed error in ScriptExecutionOrder Editor when exiting play mode. (1119209)</p></li>
<li><p>Editor: Fixed issue where EditorPrefs wouldn't be saved on editor close when using Rider as an external script editor (1110859)</p></li>
<li><p>Editor: Fixed issue where if the user cancels a non scripts only build it will cache an incomplete form of the player data cache which on a subsequent scripts only build will cause the build to fail and then crash the editor. Canceled builds will now clean up the cache and an additional check was added to VerifyBuildSetup to fail the build properly if there is no cached player data. (<a href="https://issuetracker.unity3d.com/issues/deployment-management-editor-crashes-while-making-script-only-build-if-regular-build-was-cancelled-before">1114580</a>, 1123801)</p></li>
<li><p>Graphics: OpenGL &amp; Vulkan: Fixed shader code generation for InterlockedMax(). (1124926)</p></li>
<li><p>Graphics: Vulkan: "Attempting to draw with missing bindings" is now a warning instead of an error. (1100647)</p></li>
<li><p>Graphics: Vulkan: Fixed restoring a fullscreen window from minimized state on Windows (1090059)</p></li>
<li><p>Graphics: Vulkan: Improved async readback performance. (<a href="https://issuetracker.unity3d.com/issues/vulkan-poor-performance-when-using-asyncgpureadback-dot-request">1123745</a>)</p></li>
<li><p>iOS: Stretching image across the entire screen when resolution is set to one that does not match the aspect ratio of the screen. (<a href="https://issuetracker.unity3d.com/issues/ios-iphonex-incorrect-tap-position-is-returned-on-the-certain-screen-areas">1077959</a>, 1103189)</p></li>
<li><p>Mobile: Fixed Screen.width and Screen.height don't update at the same time as Screen.orientation (<a href="https://issuetracker.unity3d.com/issues/android-screen-dot-width-and-screen-dot-height-dont-update-at-the-same-time-as-screen-dot-orientation">1013176</a>, 1094317)</p></li>
<li><p>Mono: Fixed "DllNotFoundException: MonoPosixHelper" exception being thrown when MonoPosixHelper APIs are used (<a href="https://issuetracker.unity3d.com/issues/android-dllnotfoundexception-monoposixhelper">1045644</a>, 1122898)</p></li>
<li><p>Prefabs: Fixed crash when passing invalid paths to PrefabUtility.LoadPrefabContents. (1116603)</p></li>
<li><p>Prefabs: Fixed crash when entering play mode while having a locked inspector on a GameObject with AudioSource. (1114376)</p></li>
<li><p>Prefabs: Updated RectTransforms to correctly position and parent on creation. (1124325)</p></li>
<li><p>Shaders: Fixed a missing interpolator in GL shader outputs. (1122033)</p></li>
<li><p>Terrain: Fixed issue where control key and mouse wheel does not adjust the Stamp Height value for the Stamp Terrain brush (1108352)</p></li>
<li><p>UI: UI: PhysicsRaycaster and Physics2DRaycaster now support multiple-displays. (<a href="https://issuetracker.unity3d.com/issues/physicsraycaster-does-not-work-with-multiple-displays">1027701</a>)</p></li>
</ul>

#### Changeset: 9e14d22a41bb
