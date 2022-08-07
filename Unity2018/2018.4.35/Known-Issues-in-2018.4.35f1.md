# Unity 2018.4.35
https://unity3d.com/unity/whats-new/2018.4.35

## Known Issues in 2018.4.35f1

<ul>
<li><p>macOS: If the Android Tools are not installed through the Hub, macOS 10.15 (Catalina) default security settings will prevent the Android NDK binaries being executed. These settings have to be changed or a signed Android NDK (r16b) will be needed to build Android. More information here: https://developer.android.com/ndk/downloads/older_releases.</p></li>
<li><p>Package Manager: Immutable packages altered by the API Updater are reverted to their original state when packages are resolved, which can lead to slower import performance in that context.</p></li>
<li><p>Packman: User can't easily configure location of both UPM and Asset Store package local cache (<a href="https://issuetracker.unity3d.com/issues/user-cant-easily-configure-location-of-both-upm-and-asset-store-package-local-cache">1317232</a>)</p></li>
<li><p>Windows: The Cursor is visible when Cursor.visible is set to false and new InputSystem package is used (<a href="https://issuetracker.unity3d.com/issues/the-cursor-dot-visible-equals-false-does-not-work-when-inputsystem-package-is-installed">1273522</a>)</p></li>
<li><p>Packman:  Package Manager doesn't show available updates (<a href="https://issuetracker.unity3d.com/issues/package-manager-doesnt-show-available-updates">1304459</a>)</p></li>
<li><p>Polybrush: [PolyBrush] Something went wrong saving brush settings Warning is thrown when Saving a Brush after opening the PolyBrush Window (<a href="https://issuetracker.unity3d.com/issues/polybrush-something-went-wrong-saving-brush-settings-warning-is-thrown-when-saving-a-brush-after-opening-the-polybrush-window">1315475</a>)</p></li>
</ul>
