# Unity 2018.2
https://unity3d.com/unity/whats-new/unity-2018.2.0

## The following are changes and fixes to 2018.2.0 features and regressions...


### Fixes
<ul>
<li><p>Editor: Fixed Visual Studio reloads all package .csprojs when adding or removing a .cs file in the project (<a href="https://issuetracker.unity3d.com/issues/visual-studio-reloads-all-package-csprojs-when-adding-or-removing-a-cs-file-in-the-project">1051901</a>, 1051902)</p></li>
<li><p>Graphics: Fix framebuffer cleared to black when using Vuforia or other native rendering plugins with OpenGL ES (<a href="https://issuetracker.unity3d.com/issues/vuforia-canvas-is-rendered-black-with-ar-camera-when-running-vuforias-build-with-mali-gpu">1046360</a>)</p></li>
<li><p>Package Manager: Fixed the <em>package not found</em> errors when creating a new project while offline. (1056225)</p></li>
<li><p>Scripting: Added missing 2017_4_OR_NEWER symbol to 2018.x (<a href="https://issuetracker.unity3d.com/issues/unity-2017-4-or-newer-preprocessor-is-not-recognised-when-using-number-if-unity-2017-4-or-newer-in-a-script">1050962</a>, 1056576)</p></li>
<li><p>Scripting: Make Gradient APIs accessible from threads again (<a href="https://issuetracker.unity3d.com/issues/scripting-slash-particles-gradient-scripting-api-thread-checks-have-changed-after-bindings-upgrade">1050296</a>)</p></li>
<li><p>Scripting Upgrade: Fix System.IO.IOException when reading from Process output (1047186)</p></li>
<li><p>UI: Fix case 1056226: Show realtime shadow options when using mixed and realtime lights. (<a href="https://issuetracker.unity3d.com/issues/ui-baked-and-realtime-shadow-options-are-no-longer-displayed">1056226</a>, 1056228)</p></li>
<li><p>XR: Fixed a JobTempAlloc memory leak when unloading an ARFoundation scene (1051049)</p></li>
</ul>

#### Revision: 787658998520
