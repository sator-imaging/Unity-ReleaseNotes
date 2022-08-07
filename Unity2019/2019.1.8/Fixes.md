# Unity 2019.1.8
https://unity3d.com/unity/whats-new/2019.1.8

## Fixes

<ul>
<li><p>Android: Added support for supplementary Unicode characters for UnitySendMessage. (1059652, 1147133)</p></li>
<li><p>Asset Import: Fixed an issue where AssetPostprocessor::GetVersion() did not affect AssetDependencyHash on first import. (<a href="https://issuetracker.unity3d.com/issues/assetpostprocessor-getversion-does-not-affect-assetdependencyhash-on-first-import">1146482</a>, 1158850)</p></li>
<li><p>Asset Import: Fixed plugins marked as compatible with any platform not being copied to Lumin build archives. (1117516, 1150827)</p></li>
<li><p>Editor: Fixed crash when opening a window in nographics mode. (<a href="https://issuetracker.unity3d.com/issues/unity-unit-tests-process-terminated-in-cli-mode-because-of-xr-manager">1147223</a>, 1159456)</p></li>
<li><p>Editor: Fixed game view scale in play mode for mobile platforms. (<a href="https://issuetracker.unity3d.com/issues/game-tab-window-rescales-when-entering-the-play-mode">1140742</a>, 1151179)</p></li>
<li><p>Editor: Fixed opening a window in -nographics mode crashing the editor. (<a href="https://issuetracker.unity3d.com/issues/unity-unit-tests-process-terminated-in-cli-mode-because-of-xr-manager">1147223</a>, 1159455)</p></li>
<li><p>Graphics: Fixed an issue where meshes passed to static batcher can arrive in a different order on different PCs. (1098137, 1149325)</p></li>
<li><p>Graphics: Fixed ShadowMask rendering with SRP Batcher. (1146861, 1147164)</p></li>
<li><p>IL2CPP: Fixed a hang during async write operations on Windows platforms. (1156384, 1159009)</p></li>
<li><p>IL2CPP: Fixed a memory leak when interfaces are set up for doubly nested arrays. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-race-condition-in-vm-class-setupinterfaces">1151219</a>, 1155403)</p></li>
<li><p>IL2CPP: Fixed an issue in the IL2CPP runtime that can cause intermittent crashes when dealing with certain kinds of generic method metadata. (<a href="https://issuetracker.unity3d.com/issues/ios-il2cpp-crash-on-il2cpp-metadata-il2cpptypehash-hash-when-the-sr-debugger-is-opened-and-closed">1145468</a>, 1156080)</p></li>
<li><p>IL2CPP: Fixed incorrect behavior of Bind a Unix socket on Posix platforms. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-the-sockaddr-un-structure-is-not-properly-filled-when-trying-to-bind-or-connect-to-a-unix-domain-socket">1150549</a>, 1155414)</p></li>
<li><p>IL2CPP: Fixed incorrect code generation for multidimensional arrays used as fields of structs. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-webgl-build-fails-when-multidimensional-arrays-are-present-in-project">1155344</a>, 1158620)</p></li>
<li><p>IL2CPP: Fixed incorrect code generation of delegate types using NativeArray. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-2019-dot-1-delegate-with-nativearray-as-parameter-type-triggers-an-compiler-error">1156422</a>)</p></li>
<li><p>IL2CPP: Fixed incorrect loading of static field initializer data when the field is of type ReadOnlySpan. (<a href="https://issuetracker.unity3d.com/issues/unsafe-memory-marshal-fails-on-il2cpp-backend">1146277</a>, 1154770)</p></li>
<li><p>IL2CPP: Fixed Unity TLS being incorrectly stripped with Medium and High Managed Stripping Levels. (<a href="https://issuetracker.unity3d.com/issues/https-web-request-fail-with-with-notsupportedexception-could-not-find-tls-provider-mono-dot-appletls-dot-appletlsprovider">1134343</a>, 1154766)</p></li>
<li><p>Prefabs: Reflection CubeMap for default reflection in Prefab Mode has been replaced with a lower resolution and without a sun (which caused multiple highlights).</p></li>
<li><p>Profiler: Fixed incorrect memory reported for render texture. (<a href="https://issuetracker.unity3d.com/issues/taking-editor-sample-adds-up-released-render-textures-memory-usage">1094084</a>, 1151142)</p></li>
<li><p>SceneManager: Fixed drag and drop replacing of prefab when dragging variant to project folder. (<a href="https://issuetracker.unity3d.com/issues/namebased-replace-prevents-creation-of-prefab-variant-when-using-drag-and-drop">1152704</a>, 1154214)</p></li>
<li><p>SceneManager: Updated documentation of SaveAsPrefab with a note about namebased replace. (1152708, 1154228)</p></li>
<li><p>Scripting: Fixed TouchScreenKeyboard API no longer causes errors on platforms without on-screen keyboard support. (1141643, 1145444)</p></li>
<li><p>Shaders: Fixed shader include errors after package updates. (<a href="https://issuetracker.unity3d.com/issues/shader-error-causes-screen-to-go-black-when-postprocessing-is-on">1141216</a>, 1155956)</p></li>
<li><p>Universal Windows Platform: Fixed particles flickering on ARM64 builds. (<a href="https://issuetracker.unity3d.com/issues/uwp-arm64-the-particles-in-particle-system-flickers-on-arm64-devices">1104677</a>, 1156848)</p></li>
<li><p>Universal Windows Platform: Fixed reference rewriter complaining about managed code referencing fields from winmd files when those fields are of types that project to CLR from Windows Runtime. (<a href="https://issuetracker.unity3d.com/issues/reference-rewriter-errors-when-building-uwp-against-the-insider-windows-sdk">1146307</a>, 1159988)</p></li>
<li><p>Universal Windows Platform: Fixed reference rewriter errors when building UWP against the insider Windows SDK. (<a href="https://issuetracker.unity3d.com/issues/reference-rewriter-errors-when-building-uwp-against-the-insider-windows-sdk">1146307</a>, 1159988)</p></li>
<li><p>Universal Windows Platform: Fixed System.IO APIs not working on files outside of application and AppData directories on IL2CPP scripting backend. (<a href="https://issuetracker.unity3d.com/issues/uwp-il2cpp-file-dot-exists-method-returns-false">1063768</a>, 1156200)</p></li>
<li><p>Universal Windows Platform: Fixed UnityEngine.WSA.Application.windowActivated and UnityEngine.WSA.Application.windowSizeChanged events not firing. (<a href="https://issuetracker.unity3d.com/issues/uwp-il2cpp-unityengine-dot-wsa-dot-application-dot-windowactivated-is-removed-by-il2cpp-managed-bytecode-stripping">1146982</a>, 1159985)</p></li>
<li><p>XR: Fixed issue with respecting the build setting for enabling remoting in a player. (1099398, 1160286)</p></li>
</ul>
