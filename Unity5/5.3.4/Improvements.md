# Unity 5.3.4
https://unity3d.com/unity/whats-new/unity-5.3.4

## Improvements

<ul>
<li>Android: Audio; don't select OpenSL output if the native device params are too bad for fast path (fixes audio issues on some buggy devices).</li>
<li>Android: Buildpipe; updated SDK tools requirements for the Editor.</li>
<li>Android: Editor; added Marshmallow to the list of APIs.</li>
<li>Android: IL2CPP; use Android NDK x64 on x64 Windows Editor.</li>
<li>Android: Soft Input; get rid of hardcoded text color, switch to Light theme.</li>
<li>Editor: Added warning dialog if there is any version difference between editor and last project save.</li>
<li>Metal: Add -force-metal switch to force Metal rendering on OSX/iOS.</li>
<li>OpenGL Core: A whole bunch of fixes, particularly on Macs. See Fixes list below.</li>
<li>Scripting: introduced global define UNITY_5_3_OR_NEWER, which can be used for conditionally compile code that is compatible only with Unity 5.3 or newer.</li>
<li>Win / OSX Standalone: Add -hideWindow command line option to launch standalone applications with the window hidden.</li>
<li>Windows: Added a new command line argument for standalone builds: -window-mode. Options: borderless, exclusive. It lets users override the default fullscreen window behavior.</li>
</ul>
