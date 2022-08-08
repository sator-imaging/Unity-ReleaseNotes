# Unity 3.4.1

https://unity3d.com/unity/whats-new/unity-3.4.1

## Features and improvements



*   IME input:
    *   Exposed Input.imeCompositionMode, Input.compositionString and Input.compositionCursorPos to allow IME input handling in custom GUI code. This enables easy text entry for East Asian languages such as Chinese, Japanese, Korean, and other languages with complex characters.
    *   Windows: disable any IME input when not editing a text field (or Input.imeCompositionMode is set to IMECompositionMode.Off), to make game input work properly without the need to switch input settings.
*   Following improvements were added to example project (AngryBots):
    *   Proxy level and splash screen in order to reduce unresponsive load time on handheld and webplayer.
    *   Response to Android menu/back/quit buttons.
    *   Upper right corner pause button, opening up a menu with resume (unpause), full screen (on stand-alone and web player), mute, restart, and quit (on standalone and handhelds).