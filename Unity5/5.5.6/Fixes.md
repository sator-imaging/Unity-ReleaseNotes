# Unity 5.5.6
https://unity3d.com/unity/whats-new/unity-5.5.6

## Fixes

<ul>
<li>Android: Fixed black screen on startup on Android Oreo devices. (945338, 946061)</li>
<li>Animation: Fixed alpha channel being animated when in linear color mode. (935087)</li>
<li>Editor: Fixed the callback registration crashing when entering playmode. (873467)</li>
<li>Graphics: [Metal] Fixed Z-fighting artifacts on certain devices. (950978)</li>
<li>Graphics: Fixed an occasional flicker of graphics elements on metal. (910406)</li>
<li>Graphics: Fixed Sprite Mode regression in the Inspector Import Settings so it defaults to Single rather than None, when an image was imported. (921598)</li>
<li>Graphics: Fixed Texture2D.ReadPixels reading from the wrong location on iOS/Metal when reading a section of an image. (826244)</li>
<li>iOS: Addressed a compatibility issue that was preventing apps from compiling for the iOS 11 Simulator. (934878, 953124)</li>
<li>Metal: Fixed a shader compilation regression on macOS 10.11.6 and iOS 8.x and earlier. (952020, 952233)</li>
<li>Mono: Avoid stack overflow from occurring in Unity liveness logic (asset GC). Note that this has been fixed only for both standalone and mobile platforms. (935563)</li>
<li>OSX: Fixed editor crash when using GLCore on High Sierra with Intel 6xxx series GPU. (963868) (956156)</li>
<li>UI: Fixing an issue with Input Field caret not masking properly. (743134)</li>
<li>UI: Fixed an issue whereby the CanvasManager cleared the stencil buffer every frame. (905337, 958707)</li>
<li>XR: Fixed a crash in ovrp_SetOverlayQuad3 in player when entering/exiting fullscreen mode on PC. (913717)</li>
</ul>

#### Revision: 3fb31a95adee
