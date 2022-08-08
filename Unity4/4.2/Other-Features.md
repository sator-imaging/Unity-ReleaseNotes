# Unity 4.2

https://unity3d.com/unity/whats-new/unity-4.2

## Other Features



*   Audio: Added Bypass Listener and Bypass Reverb Zones properties that enable turning off listener effects independently from the effects on the audio source. Thus, Bypass Effects only turns off the effects on the AudioSource, and the 3 flags can be combined freely.
*   Audio: Added Disable Audio property in Audio project settings to deactivate the audio system in standalone builds. Note that this also affects the audio of MovieTextures. In the editor the audio system is still on and will support previewing audio clips, but AudioSource.Play calls and playOnAwake will not be handled in order to simulate behavior of the standalone build.
*   Audio: Added "Prepare iOS For Recording" property in Player Settings (iOS > Other Settings in the inspector). Turning it on will avoid the stalls that otherwise happen when starting or stopping the Microphone object.
*   Editor: Editor extensions can now get a callback when Unity is about to open an asset. Use this callback to open an asset inside Unity before its opened in an external tool. Decorate a static method with the attribute UnityEditor.Callbacks.OnOpenAsset.
*   Linux: Added basic webcam support for video4linux2-supported devices.
*   Linux: Implement headless player; this will not require Xlib (requires Unity Pro).
*   Mac OS X: 64 bit standalone player support (x86\_64 and Universal).
*   Mecanim: Avatar Creation API, for avatar creation from scripts at runtime or in the editor.
*   Mecanim: Synchronized Layers option to override state durations.
*   Mecanim: You can now set the default layer weight in the editor for your animator controller layer.