# Unity 6000.0.70f1 LTS
公開日時: Tue, 10 Mar 2026 09:16:20 GMT
https://unity.com/releases/editor/whats-new/6000.0.70f1

# 6000.0.70f1 の既知の問題点

- `6000.3.0a4,6000.0.62f1`: 前の入力をキャンセルした後に同じ入力フィールドを選択すると、入力フィールドが更新されない
    ([uum-133712](https://issuetracker.unity3d.com/issues/input-field-does-not-update-when-selecting-the-same-input-field-after-previous-input-was-canceled))

- `6000.5.0a3,6000.4.0b8,6000.3.8f1,6000.0.68f1`: [iOS] Info.plistにUIApplicationSceneManifestを追加しても、アプリの実行中にApplication.deepLinkActivatedが起動されない。
    ([uum-135497](https://issuetracker.unity3d.com/issues/ios-application-dot-deeplinkactivated-does-not-get-invoked-while-app-is-running-when-uiapplicationscenemanifest-is-added-in-info-dot-plist))

- `IL2CPP`: [iOS] [Android] IL2CPPビルド中に外部ライブラリのジェネリックに失敗する
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- `メタル`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `Windows`: バックグラウンドで実行" が有効でアクティブウィンドウが切り替わるとプレイヤーがハングする
    ([uum-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))

DirectX 12の排他的フルスクリーンモードでフォーカスを切り替えるとプレイヤーがクラッシュする
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))

[Silicon] Razer Synapseアプリを開いているときにプロジェクトを開くとos_unfair_recursive_lock_with_optionsでクラッシュする
    ([uum-135043](https://issuetracker.unity3d.com/issues/silicon-crash-on-os-unfair-recursive-lock-lock-with-options-when-opening-a-project-while-the-razer-synapse-app-is-open))



# 6000.0.70f1 リリースノート

## 機能

- `エディター`: 洞察とエンジン診断を追加。




## 6000.0.70f1 でのパッケージ変更点