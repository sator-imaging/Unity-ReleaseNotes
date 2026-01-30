# Unity 6000.3.6f1 LTS
公開日時: Thu, 29 Jan 2026 10:44:38 GMT
https://unity.com/releases/editor/whats-new/6000.3.6f1

# 6000.3.6f1 の既知の問題点

- 6000.0.54f1: プロファイルアナライザーの比較ツールで 2 つのプロファイラーキャプチャをロードすると 100% クラッシュする
    ([uum-132332](https://issuetracker.unity3d.com/issues/100-percent-crash-rate-when-loading-two-profiler-captures-in-the-profile-analyzer-compare-tool))

- 6000.0.55f1,6000.3.0a4:UIを切り替えながらマルチプレイヤールームを作成するとRaiseExceptionでクラッシュする
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- 6000.0.64f1: [DX12] [Win11 ARM64] 新しいプロジェクトを作成しようとするとマシンがクラッシュして再起動する
    ([uum-131104](https://issuetracker.unity3d.com/issues/dx12-win11-arm64-machine-crashes-and-restarts-while-trying-to-create-a-new-project))

- 6000.1.0a2,6000.0.64f1: シングルパスステレオレンダリングでプレイモードに入るとスカイボックスしか表示されない
    ([uum-132342](https://issuetracker.unity3d.com/issues/single-pass-stereo-rendering-shows-only-skybox-when-entering-play-mode))

- 6000.3.0a1:ドメインの再読み込みが発生すると、アニメーションウィンドウをドッキングする前に最後に選択したアセットが選択される
    ([uum-131198](https://issuetracker.unity3d.com/issues/last-selected-asset-before-docking-animation-window-gets-selected-when-a-domain-reload-occurs))

- 6000.3.0a1: [WinEditor] ネイティブダイアログボックスの検索中にフォーカスが外れるとエディタが「フリーズ」する問題
    ([uum-132303](https://issuetracker.unity3d.com/issues/the-editor-freezes-and-leaks-memory-when-cancelling-the-switch-of-the-default-render-pipeline-while-using-the-advanced-object-selector))

- 6000.3.0b1,6000.0.65f1: QualitySettings.maxQueuedFramesを1に設定してDX12を使用するとエディタがフリーズする
    ([uum-131962](https://issuetracker.unity3d.com/issues/editor-freezes-when-qualitysettings-dot-maxqueuedframes-is-set-to-1-and-dx12-is-used))

- 6000.5.0a1,6000.3.2f1：DX12を使用し、すべてのスプラインノットを選択すると、複数のスタックトレースでクラッシュする
    ([uum-131707](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-using-dx12-and-selecting-all-spline-knots))

- iOS：  スプラッシュ画面の表示(Show Splash Screen)が有効で、Unityをライブラリとして使用してプロジェクトをビルドすると、レンダリングがフリーズし、UnityGfxDeviceWorkerがクラッシュする。
    ([uum-130881](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-and-unitygfxdeviceworker-crash-when-show-splash-screen-is-enabled-and-project-is-built-using-unity-as-a-library))

- メタル  コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- Metal: [iOS] iOSのスプラッシュ画面の後に画面が点滅する
    ([uum-121453](https://issuetracker.unity3d.com/issues/ios-screen-flashing-after-the-ios-splash-screen))

- プラットフォームオーディオ：[Windows] エディターで様々なアクションを実行するとAudioManager::InitFMODでクラッシュする
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))

- SRPテンプレート：削除されたVRモジュールの依存関係がURPサンプルのコンパイルを妨げる
    ([uum-130083](https://issuetracker.unity3d.com/issues/removed-vr-module-dependency-prevents-urp-sample-from-compiling))

- uGUIコントロール：[iOS][Android] UGUI入力フィールドのOnSubmitイベントが、モバイルでキーボードを離した後に無期限にトリガーされる
    ([uum-130350](https://issuetracker.unity3d.com/issues/ios-android-onsubmit-event-is-triggered-indefinitely-on-ugui-input-field-after-dismissing-keyboard-on-mobile))

- : 空白のURPプロジェクトでプレイモードに入ったり出たりする際のエディタのメモリリーク
    ([uum-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))

- SVG ファイルをインポートするとサイレントクラッシュする。
    ([uum-132415](https://issuetracker.unity3d.com/issues/silent-crash-when-importing-svg-files))



# 6000.3.6f1 リリースノート

## 修正

- 適応パフォーマンス：アダプティブパフォーマンスの非開発ビルドにおけるロギングを修正。
    (UUM-131941)

- エディター：小さすぎる要素を修正するためにツールバー要素の最大幅を変更。
    (STO-3747)

- エディター：BIDI ラッピングのオーバーフローを修正。
    (UUM-128666)

- エディター：マルチスレッド使用時の Text の NULL 例外を修正。
    (UUM-132168)

- エディター：UGUIを修正しました。
    一部のディスプレイ解像度でScroll Rectが慣性を失う問題を修正。
    ([UUM-99716](https://issuetracker.unity3d.com/issues/scroll-view-is-not-moving-by-inertia-after-scrolling-by-click-and-dragging-when-editor-window-is-minimized-and-canvas-render-mode-is-set-to-world-space))

- エディター：Linuxエディタでは、環境設定フォルダが存在しない場合、起動時に作成するようになりました。作成できない場合、Editor.logにエラーが書き込まれます。
    ([uum-128719](https://issuetracker.unity3d.com/issues/linux-preferences-directory-is-not-created-when-the-editor-is-installed-or-launched))

- マルチプレイ：Androidサポートがインストールされているが、Android SDKがUnityエディタにリンクされていない場合、マルチプレイヤープレイモードの「ローカルインスタンス」リストが空に表示され、ArgumentNullExceptionがスローされます。
    ([uum-131458](https://issuetracker.unity3d.com/issues/multiplayer-play-mode-local-instances-list-appears-empty-and-throws-an-argumentnullexception-when-android-support-is-installed-but-android-sdk-is-not-linked-to-the-unity-editor))

- パッケージマネージャ：Asset Store上でUPMパッケージをアップデートする際に、プログレスインジケーターが機能しない問題を修正しました。
    (UUM-115289)

- UI ツールキット：スプライトのロードを修正しました。
    ([UUM-131361](https://issuetracker.unity3d.com/issues/trygetvalue-fails-to-parse-uss-variable-into-sprite-when-using-customstyleproperty))




## 6000.3.6f1 におけるパッケージの変更点

## 更新されたパッケージ

- com.unity.animation.rigging：[1.4.0](https://docs.unity3d.com/Packages/com.unity.animation.rigging@1.4//changelog/CHANGELOG.html) から [1.4.1](https://docs.unity3d.com/Packages/com.unity.animation.rigging@1.4//changelog/CHANGELOG.html) へ。

- com.unity.inputsystem：[1.17.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.17//changelog/CHANGELOG.html) から [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html) へ。

- com.unity.performance.profile-analyzer：[1.2.4](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html) から [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) に変更。

- com.unity.services.cloud-build：[2.0.6](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.0//changelog/CHANGELOG.html) から [2.0.7](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.0//changelog/CHANGELOG.html) へ

- com.unity.multiplayer.tools：[2.2.6](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)から[2.2.7](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)