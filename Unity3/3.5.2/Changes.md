# Unity 3.5.2
https://unity3d.com/unity/whats-new/unity-3.5.2

## Changes

<ul>
<li>Added Resources.UnloadAsset(Object asset) function. This is useful for unloading large individual assets if you know they are no longer used and you don't want to call Resources.UnloadUnusedAssets().</li>
<li>Editor: Introduced [Callbacks.PostProcessBuild] script attribute. It will execute the attributed method after the player has been built.</li>
<li>Editor: Introduced [Callbacks.PostProcessScene] script attribute. It will execute the attributed method when the current scene has been processed.</li>
<li>Flash: Has build targets for different FlashPlayer version 11.0, 11.1 and 11.2. No Flash Player version specific implementations exposed yet, but setting 11.2 means using a faster code path; better performance.</li>
<li>Flash: www.GetAudioClip() now works, only for non streaming mp3's.</li>
<li>Flash: WWW support</li>
<li>Flash: WWWForm Support</li>
<li>Flash: Assetbundle support</li>
</ul>
