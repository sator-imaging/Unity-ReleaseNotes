# Unity 4.3
https://unity3d.com/unity/whats-new/unity-4.3

## Known issues

<ul>
<li>Automatic sprite slicing will deliver imperfect results when slicing compressed textures.</li>
<li>Google Native Client support is not functional in Unity 4.3. If you need to publish to Native Client you can still use Unity 4.2.2.</li>
<li>Mecanim: Disabled keyframing of human transform in the animation windows. </li>
<li>Mecanim: When the same clip is used many time in a controller, you can't override a specific occurrence of that clip with an AnimationControllerOverride. All the occurrence of the same clip will be replace by the override.</li>
<li>Mecanim: Can't create or edit additional curves in Animations import window. Workaround: Be sure to have the Preview Window opened before opening the Curves tab</li>
<li>Switching from Generic to Humanoid rig when using source Avatar may break animation import. Simply set Source to None, apply, and set back to proper Source.</li>
<li>The script debugger will sometimes hang on OSX Mavericks.</li>
<li>Windows: The Unity Web Player is currently only available on 32-bit architectures. Users running 64-bit IE11 on Windows 7, 8, or 8.1 will not be able to run the Unity Web Player. Development of a 64-bit Web Player is in progress.</li>
</ul>
