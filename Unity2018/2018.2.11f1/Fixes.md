# Unity 2018.2.11f1
https://unity3d.com/unity/whatsnew/unity-2018.2.11

## Fixes

<ul>
<li><p>Android: Fixed pink shader when using UI with ETC1 split alpha texture (<a href="https://issuetracker.unity3d.com/issues/android-mobile-does-not-render-texture-when-compress-using-etc1-split-alpha-channel-is-checked-in-android-override-settings">1067933</a>)</p></li>
<li><p>Animation: Fixed regression when changing hierarchy under an Animator (<a href="https://issuetracker.unity3d.com/issues/2018-dot-2-regression-animation-binding-breaks-after-activating-gameobject">1080559</a>)</p></li>
<li><p>Editor: Disabled Drag &amp; Drop of packaged textures onto GameObjects in the scene because the generated material cannot be saved. (<a href="https://issuetracker.unity3d.com/issues/materials-are-not-accessible-when-created-from-textures-in-packages-folder">1057779</a>, 1082420)</p></li>
<li><p>Editor: Disabled incomplete drag &amp; drop functionality for packaged textures onto scene objects. (<a href="https://issuetracker.unity3d.com/issues/materials-are-not-accessible-when-created-from-textures-in-packages-folder">1057779</a>)</p></li>
<li><p>Editor: Fixed Assert.Ignore() tests do not exit Play Mode (<a href="https://issuetracker.unity3d.com/issues/playmode-tests-do-not-exit-play-mode-in-2018-dot-2-versions-of-unity">1071127</a>, 1082180)</p></li>
<li><p>Editor: Fixed exception being thrown when a callback was registered with Editor.finishedDefaultHeaderGUI and an Editor's header was drawn via Editor.DrawHeader() when there was GUI state on the internal stack (e.g., change checks, disabled groups), as in the ModelImporter's Animation tab (<a href="https://issuetracker.unity3d.com/issues/registering-for-finisheddefaultheadergui-causes-animation-clip-inspector-to-throw-errors">1070848</a>, 1078001)</p></li>
<li><p>Graphics: Fixed an issue where texture presets in project templates were forcing textures with alpha to RGB format (ignoring alpha channels) by default on Android and iOS. (<a href="https://issuetracker.unity3d.com/issues/lwrp-slash-vrlw-on-android-ui-images-transparency-doesnt-work">1079066</a>, 1082125)</p></li>
<li><p>Graphics: Fixed crash in texture mip map streaming (1083008)</p></li>
<li><p>IL2CPP: Fixed load indirect instructions to always use a temporary instead of pushing a pointer expression on the value stack, which can cause incorrect behavior in certain cases. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-c-number-reference-parameter-causes-indexoutofrangeexception-on-il2cpp-backend">1077373</a>)</p></li>
<li><p>IL2CPP: Fixed for an issue that can be encountered when trying to set a field value via reflection that has a previously unused type. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-assertion-error-being-fired-when-setting-fieldinfo-dot-setvalue-to-null">1078167</a>)</p></li>
<li><p>IL2CPP: Fixed an issue with certain unprintable characters in C# source code causing failed compilations when they are copied to the C++ code as comments. (1049221)</p></li>
<li><p>IL2CPP: Fixed assumption that a class with a method named Invoke is a delegate. (<a href="https://issuetracker.unity3d.com/issues/il2cpp-async-operation-causes-nullreferenceexception-in-the-build-when-scripting-backend-is-il2cpp">1075581</a>)</p></li>
<li><p>IL2CPP: Fixed an error during code conversion when both a pinned and unpinned pointer type are used as local variables and the debugger is enabled. (1070548)</p></li>
<li><p>iOS: Fixed unassigned icon warning in Xcode when locale is not using "." as the decimal separator (<a href="https://issuetracker.unity3d.com/issues/dot-net4-dot-x-using-french-as-default-language-on-mac-building-ios-app-gives-unassigned-icon-warning-in-xcode">1058928</a>)</p></li>
<li><p>iOS: Fixed input event time not relative to new input system time. https://github.com/Unity-Technologies/InputSystem/issues/242</p></li>
<li><p>iOS: Fixed stylus events not coming  Pen device instead of Touchscreen device in the new input system.</p></li>
<li><p>iOS: Fixed stylus not returning normalized pressure value in the new input system. https://github.com/Unity-Technologies/InputSystem/issues/121</p></li>
<li><p>iOS: Fixed using French as default language on Mac, building iOS app giving unassigned icon warning in Xcode (<a href="https://issuetracker.unity3d.com/issues/dot-net4-dot-x-using-french-as-default-language-on-mac-building-ios-app-gives-unassigned-icon-warning-in-xcode">1058928</a>)</p></li>
<li><p>Package Manager: Fixed dependent modules not treated as disabled if a module built-in package is disabled in Packman UI.</p></li>
<li><p>SceneManager: Fixed crashes caused by incorrectly activated children of inactive parents (<a href="https://issuetracker.unity3d.com/issues/crash-on-particlesystemgeometryjob-schedulejobs-when-deleting-gameobject">1051704</a>, 1081785)</p></li>
</ul>

#### Revision: 38bd7dec5000
