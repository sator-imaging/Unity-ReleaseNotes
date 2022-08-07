# Unity 2018.4.18
https://unity3d.com/unity/whats-new/2018.4.18

## Known Issues in 2018.4.18f1

<ul>
<li><p>Animation: Animator.Update CPU time spikes when multiple animations are playing (<a href="https://issuetracker.unity3d.com/issues/animator-dot-update-cpu-time-spikes-when-multiple-animations-are-playing">1184690</a>)</p></li>
<li><p>Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.</p></li>
<li><p>Scene Management: Prefabs lose their values if scripts are removed then reintroduced (<a href="https://issuetracker.unity3d.com/issues/prefabs-lose-their-values-if-scripts-are-removed-then-reintroduced">1216914</a>)</p></li>
<li><p>macOS: If the Android Tools are not installed through the Hub, macOS 10.15 (Catalina) default security settings will prevent the Android NDK binaries being executed. These settings have to be changed or a signed Android NDK (r16b) will be needed to build Android. More information here: https://developer.android.com/ndk/downloads/older_releases.</p></li>
<li><p>tvOS:  "Menu" button on Siri Remote returns "Joystick1Button19" instead of "Joystick1Button0" (<a href="https://issuetracker.unity3d.com/issues/tvos-menu-button-on-siri-remote-returns-joystick1button19-instead-of-joystick1button0">1214948</a>)</p></li>
</ul>
