# Unity 3.5
https://unity3d.com/unity/whats-new/unity-3.5

## iOS Features

<ul>
<li>Implemented Build&amp;Run support for Xcode 4.x. (Not compatible with Xcode 3.x, but can be turned off in Editor settings).</li>
<li>Accelerometer frequency now is controlled from Player Settings.</li>
<li>Application.targetFrameRate works. Removed kFPS constant due to this. 30 FPS is default.</li>
<li>Added "Show Loading Indicator" option, to show spinner when loading game.</li>
<li>GameCenter support added through the Social API (does not include matchmaking and voice features at the moment).</li>
<li>Added iAd support.</li>
<li>Added push notification support.</li>
<li>Added Compass and Gyroscope support.</li>
<li>Added Camera support.</li>
<li>Added Microphone support.</li>
<li>Image Filters now determine the format for intermediate Render Targets from currently bound FrameBuffer (most usual - default Display Buffer). So if you use a 16bit Display Buffer you will get 16bit rt (RGB565). While this makes image filters a bit faster, it also is more GLES-conformant. If you want to use Image Filters that needs alpha channel or see banding, please set "Use 32-bit Display Buffer" checkbox in Player Settings, or use newly added Handheld.use32bitDisplayBuffer API.</li>
</ul>
