# Unity 6000.0.67f1 LTS
公開日時: Wed, 04 Feb 2026 11:53:51 GMT
https://unity.com/releases/editor/whats-new/6000.0.67f1

# 6000.0.67f1 の既知の問題

- 6000.0.55f1,6000.3.0a4`：UI を切り替えながらマルチプレイヤールームを作成すると RaiseException でクラッシュする
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- 6000.1.0a2,6000.0.64f1`：シングルパスステレオレンダリングでプレイモードに入るとスカイボックスだけが表示される
    ([uum-132342](https://issuetracker.unity3d.com/issues/single-pass-stereo-rendering-shows-only-skybox-when-entering-play-mode))

- 6000.3.0b1,6000.0.65f1`：QualitySettings.maxQueuedFramesを1に設定してDX12を使用するとエディタがフリーズする
    ([uum-131962](https://issuetracker.unity3d.com/issues/editor-freezes-when-qualitysettings-dot-maxqueuedframes-is-set-to-1-and-dx12-is-used))

- `6000.5.0a4`:プロファイラ (スタンドアロン) ウィンドウが開かない
    ([uum-131071](https://issuetracker.unity3d.com/issues/profiler-standalone-window-doesnt-open))

- IL2CPP`：[iOS] [Android] IL2CPP ビルド中に外部ライブラリジェネリックが失敗する
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- iOS`：  スプラッシュ画面の表示]が有効で、Unityをライブラリとして使用してプロジェクトをビルドすると、レンダリングがフリーズし、UnityGfxDeviceWorkerがクラッシュする
    ([uum-130881](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-and-unitygfxdeviceworker-crash-when-show-splash-screen-is-enabled-and-project-is-built-using-unity-as-a-library))

- メタル`：  コマンドバッファタイムアウトエラーの後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- Metal`：[iOS] iOS のスプラッシュ画面の後に画面が点滅する
    ([uum-121453](https://issuetracker.unity3d.com/issues/ios-screen-flashing-after-the-ios-splash-screen))

- Platform Audio`：[Windows] エディターで様々なアクションを実行すると AudioManager::InitFMOD でクラッシュする
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))

- ([uum-126803]()) : 空白のURPプロジェクトでプレイモードに入ったり出たりする際にエディターのメモリーリークが発生する。
    ([uum-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))



# 6000.0.67f1 リリースノート

## 改良点

- Shadergraph`：swizzleノードの入力スロットが不正な状態になってしまう問題を追加。ノードの入力スロットと出力スロットが常にスウィズルマスクを反映するように動作を変更。
    ([uum-120808](https://issuetracker.unity3d.com/issues/shader-graph-swizzle-node-input-slash-output-and-mask-update-incorrectly-after-undo))



## 修正

- `2D`:ユーザーが任意の位置で空のブラシでペイントし、(0, 0, 0)でタイルをクリアする問題を修正。
    ([uum-128709](https://issuetracker.unity3d.com/issues/painting-on-a-tilemap-erases-random-tile-when-an-empty-tile-was-selected-in-the-tilemap-palette))

- `2D`:タイルパレットウィンドウのパン中にユーザーのポインタがタイルパレットウィンドウから離れた場合、ユーザーがタイルパレットウィンドウをパンし続けることができる問題を修正し、タイルパレットウィンドウの外でのパンを非アクティブにしました。
    ([uum-128466](https://issuetracker.unity3d.com/issues/tile-palette-grid-keeps-panning-when-the-mouse-click-is-released-outside-of-the-grid))

- ドキュメント`：Create a Profiler モジュールページへのリンクを修正しました。

- エディター`：WorldToGUIPoint` と `OnDrawGizmos` API の動作を改善。

- Graphics`：MSAA メモリレス深度バッファを解決する際の Metal Validation エラーによるクラッシュを修正。
    (UUM-125478)

- uGUI`：overrideSorting=trueでCanvasを破壊することで孤児になったUI要素のマスキングを修正。
    ([UUM-127287](https://issuetracker.unity3d.com/issues/canvas-masking-is-not-updated-when-destroying-the-canvas-component-with-an-overridesorting))

- バージョン管理`：2.11.2のWaitForPendingOperations.cs.metaの無効な重複GUIDによるコンパイルエラーを修正。

- バージョン管理`：Unity 6.3以下のバージョンでエディター内部へ直接アクセスできるように修正。




## 6000.0.67f1でのパッケージ変更点

## 更新されたパッケージ

- com.unity.charactercontroller`：[1.4.1](https://docs.unity3d.com/Packages/com.unity.charactercontroller@1.4//changelog/CHANGELOG.html) から [1.4.2](https://docs.unity3d.com/Packages/com.unity.charactercontroller@1.4//changelog/CHANGELOG.html) へ。

- com.unity.animation.rigging`：[1.4.0](https://docs.unity3d.com/Packages/com.unity.animation.rigging@1.4//changelog/CHANGELOG.html) から [1.4.1](https://docs.unity3d.com/Packages/com.unity.animation.rigging@1.4//changelog/CHANGELOG.html) へ。

- com.unity.collab-proxy`：[2.11.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) から [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) に変更。

- com.unity.ide.rider`：[3.0.38](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) から [3.0.39](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- com.unity.inputsystem`：[1.17.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.17//changelog/CHANGELOG.html) から [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html)

- com.unity.mobile.android-logcat`：[1.4.6](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) から [1.4.7](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) に変更。

- com.unity.performance.profile-analyzer`：[1.2.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html) から [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) に変更。

- com.unity.services.analytics`：[6.2.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html)から[6.2.1](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html)

- com.unity.testtools.codecoverage`：[1.2.6](https://docs.unity3d.com/Packages/com.unity.testtools.codecoverage@1.2//changelog/CHANGELOG.html) から [1.3.0](https://docs.unity3d.com/Packages/com.unity.testtools.codecoverage@1.3//changelog/CHANGELOG.html) に変更。

- com.unity.xr.hands`：[1.7.2](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html) から [1.7.3](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html) に変更。

- com.unity.profiling.systemmetrics.mali`：[1.1.0](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) から [1.1.1](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) に変更。

- `com.unity.multiplayer.tools`：[2.2.6](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)から[2.2.7](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)

- com.unity.ai.navigation`：[2.0.9](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) から [2.0.10](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) へ。