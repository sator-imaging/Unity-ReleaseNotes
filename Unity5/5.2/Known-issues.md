# Unity 5.2

https://unity3d.com/unity/whats-new/unity-5.2

## Known issues



#### We are doing something new by giving more prominence to known issues and the upcoming patch release in which we expect to fix them. So, while the known issue list might look a bit longer, we're doing this to provide transparency and to increase the amount of information you get about our development process.

*   2D: Sprite pivot values currently clamped to 0..1, will be extended to larger values in 5.2.0p1
*   Connect: 'Go to Dashboard' link for Multiplayer leads to Cloud Build
*   Editor: Crash when using injecting proxies (e.g. Lavasoft's webcompanion, Astrill, Qustodio) [713828](http://issuetracker.unity3d.com/issues/untiy-64bit-5-dot-1-1f1-crashing-on-windows-8-dot-1)
*   Editor: Incorrectly reports native plugin collision, even if only one native plugin exists
*   Game input in the Mac Editor may not work after opening a new project. This happens after getting a dialog saying “Moving File Failed”. To work around this issue, close and open the editor. The fix will be in 5.2.0p1 [705555](http://issuetracker.unity3d.com/issues/resource-busy-mac-opening-new-project-throws-resource-busy-dialog-on-mac)
*   Mac: Input system such as mouse click events or key press events stop working when multiple projects are opened. The fix will be in 5.2.0p1 [716221](http://issuetracker.unity3d.com/issues/input-system-mouse-click-slash-key-press-event-is-not-captured-when-a-project-is-opened-using-open-project-option)
*   Layout elements under a ScrollRect component may not work properly. As a workaround a setup can be used where the Content is not a direct child of the ScrollRect but has an intermediary View object in between (the default setup from 5.2 onwards). The fix will be in a patch release
*   Editor: Scene view picking in linear color space does not work for DX11 when MSAA is used (quality: fantastic). Workaround: Use gamma color space, turn off MSAA or switch to DX9. This will be fixed in 5.2.0p1
*   Version Control: Perforce "Moving file failed" message appears when close project, fixed in 5.2.0p1
*   Windows Phone: Solution build fails when product name has non-alphanumeric characters
*   Windows Phone 10: Virtual keyboard doesn't work for UWP apps, will be fixed in 5.2.0p1
*   Windows Store Apps: audio is buggy on Windows 10, will be fixed in 5.2.0p1
*   Universal Windows Platform: Unity C# option doesn't work correctly for Windows 10 Universal apps, will be fixed in 5.2.0p1
*   Windows Store Apps: webcam is crashing on Windows 10, will be fixed in 5.2.0p1
*   VR / Oculus Windows: Linear lighting and MSAA crashes. Must use gamma, no MSAA until 5.2.0p1
*   VR / Oculus Windows: HMD not rendering after reconnect on Win10 with runtime 0.7
*   VR / Oculus Mac: No image to HMD. No workaround until 5.2.0p1
*   VR / Gear VR: Crash with OpenGL ES 2.0. Must use OpenGL ES 3.0 until 5.2.0p1
*   Tizen: Applications currently crash on launch. Will be fixed in a patch-release
*   Tizen: Applications will be rejected by the Tizen Store. Will be fixed in a patch-release