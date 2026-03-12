# Unity 2022.3.74f1 LTS
Published at Wed, 11 Mar 2026 10:15:36 GMT  
https://unity.com/releases/editor/whats-new/2022.3.74f1

# Known Issues in 2022.3.74f1



* iOS/tvOs: The Target minimum iOS/tvOs version is displayed to 12 when iOS/tvOS 13 is the new minimum since 2022.3.72f1 due to UIScene requirements. Manually raise to 13 to avoid crashes on iOS12 devices that do not support UIScene
* Metal:  Game freezes after command buffer Timeout error
([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))
* Metal: macOS stutters in a minimal project in the Editor in Play Mode
([UUM-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))
* Video: Fix for 2022.3.X: VideoPlayer freezes or stops on certain Android devices when enabling and disabling the Video multiple times
(UUM-112470)
* Windows: Player hangs when the "Run in Background" is enabled and active window is switched
([UUM-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))



# 2022.3.74f1 Release Notes

## Features

* Editor: Added insights and engine diagnostics (off by default).


