# Unity 4.6.4
https://unity3d.com/unity/whats-new/unity-4.6.4

## Improvements

<ul>
<li>Android: Parsing device specific XML font configurations to determine system/fallback fonts.</li>
<li>Asset Loading: Added an offset to AssetBundle.CreateFromFile, to load the asset bundle starting at an offset in the file.</li>
<li>Editor: Android; added the ability to configure JDK path in the Editor preferences.</li>
<li>Graphics: Increased maximum texture size to 4096 for -nographics batch mode devices. Helps build servers.</li>
<li>iOS: Make startup more robust (esp. regarding locking device on startup).</li>
<li>iOS: Short term fix for occasional input stuttering.</li>
<li>iOS: Xcode 6.3 support.</li>
<li>iOS/Metal: Optimized static batching and dynamic geometry handling.</li>
<li>iOS/Metal: Defer [CAMetalLayer nextDrawable] until it is actually needed; should help with occasional framerate hiccups.</li>
</ul>
