# Unity 6000.0.70f1 LTS
发布于 Tue, 10 Mar 2026 09:16:20 GMT
https://unity.com/releases/editor/whats-new/6000.0.70f1

# 6000.0.70f1 中的已知问题

- `6000.3.0a4,6000.0.62f1`: 取消上一次输入后，选择同一输入字段时，输入字段不会更新
    ([uum-133712](https://issuetracker.unity3d.com/issues/input-field-does-not-update-when-selecting-the-same-input-field-after-previous-input-was-canceled))

- `6000.5.0a3,6000.4.0b8,6000.3.8f1,6000.0.68f1`: [iOS] 在 Info.plist 中添加 UIApplicationSceneManifest 时，应用程序运行时不会调用 Application.deepLinkActivated
    ([uum-135497](https://issuetracker.unity3d.com/issues/ios-application-dot-deeplinkactivated-does-not-get-invoked-while-app-is-running-when-uiapplicationscenemanifest-is-added-in-info-dot-plist))

- `IL2CPP`: [iOS] [Android] 在 IL2CPP 构建过程中外部库泛型失败
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- 金属命令缓冲区超时错误后游戏冻结
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `金属"`: MacOS 在编辑器中的最小项目在播放模式下出现卡顿
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `Windows`: 启用 "在后台运行 "并切换活动窗口时，播放器会挂起
    ([uum-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))

在 DirectX 12 独占全屏模式下切换焦点时播放器崩溃
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))

[硅] 当 Razer Synapse 应用程序打开项目时，os_unfair_recursive_lock_lock_with_options 会崩溃
    ([uum-135043](https://issuetracker.unity3d.com/issues/silicon-crash-on-os-unfair-recursive-lock-lock-with-options-when-opening-a-project-while-the-razer-synapse-app-is-open))



# 6000.0.70f1 发布说明

## 功能

- 编辑器添加了洞察力和引擎诊断（默认关闭）。




## 6000.0.70f1 中软件包的更改