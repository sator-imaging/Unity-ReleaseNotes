# Unity 2018.2.15f1
https://unity3d.com/unity/whatsnew/unity-2018.2.15

## Fixes

<ul>
<li><p>Android: Fixed gradle builds failing due to jcenter download failures. (<a href="https://issuetracker.unity3d.com/issues/gradle-build-fails-when-downloading-files-from-jcenter">1093946</a>, 1095913)</p></li>
<li><p>Android: Fixed gradle daemons not killed in batch mode. (<a href="https://issuetracker.unity3d.com/issues/android-the-java-dot-exe-process-that-executed-gradle-is-not-terminated-when-a-build-in-batch-mode-is-completed">1073824</a>, 1090861)</p></li>
<li><p>Audio: Fixed ease in/ease out in Timeline when using an Audio Source. (1084540)</p></li>
<li><p>Editor: Fixed an issue where red text could appear in the Project search bar along with "style not found" console warnings, while searching in play mode. (<a href="https://issuetracker.unity3d.com/issues/red-text-in-project-search-bar-when-searchingwhile-in-play-mode">1086419</a>, 1091552)</p></li>
<li><p>GI: Fixed an issue which prevented render targets being used as a source for reflection probes. (<a href="https://issuetracker.unity3d.com/issues/graphics-impossible-to-use-a-cube-render-texture-as-custom-reflection-probe">1029512</a>)</p></li>
<li><p>Graphics: Fixed a legacy cubemap crash when its parameters are changed. (<a href="https://issuetracker.unity3d.com/issues/legacy-cubemap-crashes-when-parameters-are-changed">1038653</a>, 1085557)</p></li>
<li><p>iOS: Fixed an issue where the namespace UnityEditor.iOS.Xcode was not found when running the Editor in batch mode. (<a href="https://issuetracker.unity3d.com/issues/unityeditor-dot-ios-dot-xcode-is-not-found-when-running-editor-in-batch-mode">1018716</a>, 1083343)</p></li>
<li><p>iOS: Fixed an issue where the screen could be cut off/corrupted when launching from an associated domain link. (1093922)</p></li>
<li><p>Multiplayer: Fixed UNetWeaver error arised when used Entities package and then creating a NetworkBeahaviour. (<a href="https://issuetracker.unity3d.com/issues/getting-unetweaver-errors-when-using-entities-and-creating-a-networkbehaviour">1052489</a>)</p></li>
<li><p>Particles: Fixed the last mesh in multi-mesh systems was being ignored. (<a href="https://issuetracker.unity3d.com/issues/particle-system-mesh-render-mode-incorrectly-randomize-multiple-meshes">1060973</a>, 1068211)</p></li>
<li><p>Scripting: Fixed crash with message box "GetThreadContext failed". (1082246)</p></li>
<li><p>Scripting Upgrade: Fixed ArgumentException: "GCHandle value belongs to a different domain" during WebRequest. (1091744)</p></li>
<li><p>Scripting Upgrade: Fixed crash when using Debug.Log. (1073634)</p></li>
<li><p>Scripting Upgrade: Fixed for libMonoPosixHelper.so cannot be found. (<a href="https://issuetracker.unity3d.com/issues/libmonoposixhelper-dot-so-cannot-be-found">1077828</a>)</p></li>
<li><p>Scripting Upgrade: Fixed IEnumerable.ToArray() incorrectly producing 'null' elements. (1066693)</p></li>
<li><p>Scripting Upgrade: Fixed random crash on x86 Linux with TLS connections ("GCHandle value belongs to a different domain"). (<a href="https://issuetracker.unity3d.com/issues/x86-linux-player-webrequest-returns-error-argumentexception-gchandle-value-belongs-to-a-different-domain">1082650</a>, 1091745)</p></li>
<li><p>Shuriken: Fixed where the last mesh in multi-mesh systems was being ignored. (<a href="https://issuetracker.unity3d.com/issues/particle-system-mesh-render-mode-incorrectly-randomize-multiple-meshes">1060973</a>)</p></li>
<li><p>Timeline: Fixed audio ease in and ease out broken when assigned to an audio source. (1084540)</p></li>
</ul>

#### Revision: 65e0713a5949
