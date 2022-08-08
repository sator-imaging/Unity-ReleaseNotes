# Unity 3.5

https://unity3d.com/unity/whats-new/unity-3.5

## iOS Features



*   Implemented Build&Run support for Xcode 4.x. (Not compatible with Xcode 3.x, but can be turned off in Editor settings).
*   Accelerometer frequency now is controlled from Player Settings.
*   Application.targetFrameRate works. Removed kFPS constant due to this. 30 FPS is default.
*   Added "Show Loading Indicator" option, to show spinner when loading game.
*   GameCenter support added through the Social API (does not include matchmaking and voice features at the moment).
*   Added iAd support.
*   Added push notification support.
*   Added Compass and Gyroscope support.
*   Added Camera support.
*   Added Microphone support.
*   Image Filters now determine the format for intermediate Render Targets from currently bound FrameBuffer (most usual - default Display Buffer). So if you use a 16bit Display Buffer you will get 16bit rt (RGB565). While this makes image filters a bit faster, it also is more GLES-conformant. If you want to use Image Filters that needs alpha channel or see banding, please set "Use 32-bit Display Buffer" checkbox in Player Settings, or use newly added Handheld.use32bitDisplayBuffer API.