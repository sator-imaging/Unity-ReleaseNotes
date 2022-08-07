# Unity 2017.4.19
https://unity3d.com/unity/whats-new/2017.4.19

## Fixes

<ul>
<li><p>2D: Fixed Unity Editor crash during Sprite Atlas packing. (<a href="https://issuetracker.unity3d.com/issues/during-sprite-atlas-packing-unity-editor-crashes">1029266</a>)</p></li>
<li><p>Android: Fixed for Android Dynamic feature crashes the application when running the build via Android Studio. (1100785)</p></li>
<li><p>Android: Fixed instancing not working in some situations on Adreno GPUs (<a href="https://issuetracker.unity3d.com/issues/lwrp-android-model-materials-disappear-but-the-shadows-remain-on-adreno-630-gpu">1053324</a>, 1102804)</p></li>
<li><p>Android: Fixed instancing not working in some situations on PowerVR GPUs (1109159)</p></li>
<li><p>Animation: Fixed avatar preview pan position being reset whenever editing animation events. (<a href="https://issuetracker.unity3d.com/issues/fbx-import-animation-preview-postion-reset-when-adding-an-animation-event">1067998</a>)</p></li>
<li><p>Editor: Fixed curve editor and dopesheet controls disappearing when entering play mode in the editor. (<a href="https://issuetracker.unity3d.com/issues/animation-window-curves-stutter-slash-partially-disappears-when-entering-play-mode">1035934</a>, 1040997)</p></li>
<li><p>Editor: Fixed issue where specifying frustum view point would actually use it as base for the near plane. (1081967)</p></li>
<li><p>Editor: Fixed this issue by restricting the insertion of menu items into a given submenu to a prescribed limit of 1000 items and displays a warning about the same. (1039181)</p></li>
<li><p>Graphics: Fixed JobTempAlloc memory leak and random crash when rendering a scene with a SpriteRenderer when using Graphics Jobs. (1100859)</p></li>
<li><p>Graphics: Fixed submitting non-instanced property arrays via DrawMeshInstanced. (<a href="https://issuetracker.unity3d.com/issues/graphics-dot-drawmeshinstanced-fails-to-apply-array-properties-from-a-materialpropertyblock">1010738</a>, 1108825)</p></li>
<li><p>IL2CPP: Fixed crash when using the Environment.MachineName property on some machines when targeting UWP and make it return results consistent with the Standalone Player. (<a href="https://issuetracker.unity3d.com/issues/system-dot-environment-dot-machinename-crashes-on-il2cpp-on-long-machine-names-with-uwp-builds">1093953</a>)</p></li>
<li><p>IL2CPP: Fixed InvalidCastException that can sometimes happen when passing managed object that derives from a native Windows Runtime class to native code. For instance, this happens when deriving from Windows.UI.Xaml.Control.ContentDialog and trying to show it. (<a href="https://issuetracker.unity3d.com/issues/uwp-contentdialog-throws-an-exception-on-il2cpp-backend">1104540</a>)</p></li>
<li><p>Mobile: Fixed crash that happens if native library initialization fails for any reason (1097013)</p></li>
<li><p>Scripting: Fixed an issue with static members such as generic classes with their argument being an array type not being reported the memory snapshot API. (<a href="https://issuetracker.unity3d.com/issues/packedmemorysnapshot-type-contains-staticfieldbytes-but-has-no-static-field">984330</a>)</p></li>
<li><p>Scripting: Fixed random crash in Asset GC. (1091878)</p></li>
<li><p>Shuriken: Fixed <code>Renderer.bounds</code> returning the wrong bounds when multiple renderers were on the same GameObject. (<a href="https://issuetracker.unity3d.com/issues/editor-particle-system-editor-show-bounds-displays-the-incorrect-bounds-when-a-meshrenderer-is-attached-to-the-same-gameobje">1088716</a>, 1089020)</p></li>
<li><p>UI: Fixed InputField gets corrupted and ArgumentOutOfRangeException is thrown when using certain emojis. (1050713)</p></li>
<li><p>UI: Fixed material being made dirty when rendering with a RectMask2D. (<a href="https://issuetracker.unity3d.com/issues/canvas-batching-system-dirties-project-user-created-materials-when-using-rect-mask-2d">967024</a>)</p></li>
<li><p>UI: Fixed performance regression with RectTransform animation (<a href="https://issuetracker.unity3d.com/issues/performance-ui-animators-dot-update-performance-regression-from-the-2018-dot-1-version">1104878</a>)</p></li>
<li><p>Unity Test Runner: Fixed non-printable characters in native test name output are now printed correctly. (1044529)</p></li>
</ul>

#### Changeset: 47cd37c28be8
