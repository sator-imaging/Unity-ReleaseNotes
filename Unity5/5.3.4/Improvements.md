# Unity 5.3.4

https://unity3d.com/unity/whats-new/unity-5.3.4

## Improvements



*   Android: Audio; don't select OpenSL output if the native device params are too bad for fast path (fixes audio issues on some buggy devices).
*   Android: Buildpipe; updated SDK tools requirements for the Editor.
*   Android: Editor; added Marshmallow to the list of APIs.
*   Android: IL2CPP; use Android NDK x64 on x64 Windows Editor.
*   Android: Soft Input; get rid of hardcoded text color, switch to Light theme.
*   Editor: Added warning dialog if there is any version difference between editor and last project save.
*   Metal: Add -force-metal switch to force Metal rendering on OSX/iOS.
*   OpenGL Core: A whole bunch of fixes, particularly on Macs. See Fixes list below.
*   Scripting: introduced global define UNITY\_5\_3\_OR\_NEWER, which can be used for conditionally compile code that is compatible only with Unity 5.3 or newer.
*   Win / OSX Standalone: Add -hideWindow command line option to launch standalone applications with the window hidden.
*   Windows: Added a new command line argument for standalone builds: -window-mode. Options: borderless, exclusive. It lets users override the default fullscreen window behavior.