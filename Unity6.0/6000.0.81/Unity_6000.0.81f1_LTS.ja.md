# Unity 6000.0.81f1 LTS
公開日時：2026年8月6日（木）09:43:51 GMT  
https://unity.com/releases/editor/whats-new/6000.0.81f1

# 6000.0.81f1 の既知の問題

- `6000.0.6f1`: [RenderGraph][D3D12] D3D12SwapChain::Present 実行時にクラッシュ  EnableAsyncCompute(true) および UseTexture を併用した際に D3D12SwapChain::Present でクラッシュする
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `アセットインポーター`: プレイモードに入ると、「(Unity) WriteObjectToVector」の処理中にエディターがクラッシュする
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: コマンドバッファのタイムアウトエラー発生後にゲームがフリーズする
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

低スペック端末でストリーミングクリップを含む AudioSource を一時停止した際に ARC クラッシュが発生する
 ([UUM-148440](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148440))

bee_backendが複数実行されている際に、mono_log_write_logfileの呼び出しでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

フォントアトラスの生成時に複数のスタックトレースが発生し、クラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.0.81f1 リリースノート

## APIの変更

- `Android`: 追加: SDK Platform 37 のサポートを追加



## 修正

- `Android`: Androidサポートがインストールされている際に、Unityの設定画面のテキストフィールドでラグが発生する問題を修正しました。
    (UUM-147435)

- `Android`: ```Screen.brightness``` に負の値を指定した場合、デバイスの推奨画面輝度が復元されるようになりました。
    ([UUM-145925](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145925))

- `Android`: AGP 9 の R8 キープルールに関する厳格な適用基準を緩和しました。
    ([UUM-147136](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147136))

- `Animation`: クラッシュの可能性を防ぐため、Animation Playable Outputのバインドおよびアンバインドの検証処理を再実装しました。
    ([UUM-146750](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146750))

- `Audio`: Audio Mixerでスナップショットを削除した際に発生していたエラーを修正しました。
    ([UUM-119443](https://issuetracker.unity3d.com/issues/error-is-thrown-when-deleting-snapshot-with-another-snapshot-present-in-audio-mixer-window))

- `エディタ`: 「環境設定」ウィンドウの「インデックス設定」に、有効な検索用語/キーワードをいくつか追加しました。
    ([UUM-146350](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146350))

- `Editor`: スプラッシュ画面が無効になっている状態で `SplashScreen.Stop(FadeOut)` を呼び出しても、アプリケーションがフリーズしなくなりました。
    (UUM-143481)

- `エディタ`: `AsyncInstantiateOperation` 内で `CancellationTokenSource` オブジェクトが破棄されなかったことに起因するメモリリークを修正しました。
    ([UUM-147016](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147016))

- `Editor`: 管理者権限で Unity を実行している際の WinEditor の警告ダイアログのテキストを更新しました。
    ([UUM-146796](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146796))

- `Graphics`: インジェクションされた RenderObjects パスで動的解像度が有効になっている場合、XR でのレンダリングの問題を修正しました。
    ([UUM-142592](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142592))

- `HDRP`: `ClearBuffer2D` シェーダーを更新し、マルチビューに対応させました。
    ([UUM-137877](https://issuetracker.unity3d.com/issues/hdrp-xr-dx12-ssr-pbr-accumulation-algorithm-artifacts-are-present-in-one-eye-when-using-spi-openxr-rendering-mode))

- `iOS`: iOSのコントロールセンターを引き下ろすと、Unityアプリのオーディオ再生が停止してしまうバグを修正しました。
    ([UUM-145522](https://issuetracker.unity3d.com/issues/ios-audio-is-cut-out-when-accessing-ios-control-center))

- `iOS`: 深度カメラを 2 回目に作成した際にクラッシュする問題を修正しました。
    ([UUM-141173](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141173))

- `Linux`: 新しいカーネルバージョンでワイヤレスXbox 360コントローラーを使用する際、Dパッドの入力が誤った方向に割り当てられる問題を修正しました。
    ([UUM-136083](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-136083))

- `Linux`: Linux上でBluetooth経由でXboxコントローラーを接続した際、Unity Input Systemにおいて一部のXboxコントローラー入力が本来とは異なるボタンに割り当てられてしまう問題を修正しました。
    ([UUM-144216](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144216))

- `macOS`: macOSのサーバービルドでlibMonoPosixHelper.dylibが見つからない問題を修正しました。
    ([UUM-141263](https://issuetracker.unity3d.com/issues/macos-server-cannot-find-libmonoposixhelper-dot-dylib-when-calling-gzipstream))

- `Physics`: 接触距離が正しく処理されていなかったため、ConfigurableJointの設定が距離制約の最大値に達するとジッターが発生する問題を修正しました。
    ([UUM-146852](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146852))

- `Scripting`: ドメインの再読み込み時に、古くなった GC ハンドルに対する予防的なチェックおよび修正を追加しました。
    ([UUM-122598](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-performing-various-actions-with-the-cesium-package-installed))

- `ユニバーサル Windows プラットフォーム (UWP)`: UWP 環境で、マウスの移動によりスクロール操作が再トリガーされる問題を修正しました。
    ([UUM-144660](https://issuetracker.unity3d.com/issues/uwp-mouse-movement-re-triggers-stale-slash-scroll-value-after-the-scroll-wheel-is-used-once))

- `Video`: API Only モードで VideoPlayer を使用し、Unity Audio を無効にしている場合、macOS 上で AudioSampleProvider.sampleFramesAvailable コールバックが決して発火しない問題を修正しました。
    ([UUM-143660](https://issuetracker.unity3d.com/issues/audiosampleprovider-dot-sampleframesavailable-callback-never-fires-when-using-macos))

- `Web`: サーバーが「Content-Length」ヘッダーを設定していない場合、UnityWebRequest でのレスポンス本体のストリーミングに関する問題を修正しました。
    ([UUM-146537](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146537))




## 6000.0.81f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.collections`: [2.6.7](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) から [2.6.8](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) へ

- `com.unity.entities`: [1.4.7](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) から [1.4.8](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) へ

- `com.unity.netcode`: [1.14.0](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html) から [1.14.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html)

- `com.unity.physics`: [1.4.6](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) から [1.4.7](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) へ

- `com.unity.entities.graphics`: [1.4.20](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) から [1.4.21](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) へ

- `com.unity.2d.animation`: [10.2.2](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.2//changelog/CHANGELOG.html) から [10.2.3](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.2//changelog/CHANGELOG.html)

- `com.unity.2d.common`: [9.1.1](https://docs.unity3d.com/Packages/com.unity.2d.common@9.1//changelog/CHANGELOG.html) から [9.1.2](https://docs.unity3d.com/Packages/com.unity.2d.common@9.1//changelog/CHANGELOG.html) へ

- `com.unity.2d.psdimporter`: [9.1.1](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.1//changelog/CHANGELOG.html) から [9.1.2](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.1//changelog/CHANGELOG.html)

- `com.unity.2d.spriteshape`: [10.0.7](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@10.0//changelog/CHANGELOG.html) から [10.1.1](https://docs.unity3d.com/Packages/com.unity.2d.spriteshape@10.1//changelog/CHANGELOG.html)

- `com.unity.2d.tilemap.extras`: [4.1.0](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@4.1//changelog/CHANGELOG.html) から [4.1.1](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@4.1//changelog/CHANGELOG.html) へ

- `com.unity.burst`: [1.8.29](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) から [1.8.30](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) へ

- `com.unity.services.cloudcode`: [2.10.2](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.10//changelog/CHANGELOG.html) から [2.10.4](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.10//changelog/CHANGELOG.html) へ

- `com.unity.services.economy`: [3.5.3](https://docs.unity3d.com/Packages/com.unity.services.economy@3.5//changelog/CHANGELOG.html) から [3.5.4](https://docs.unity3d.com/Packages/com.unity.services.economy@3.5//changelog/CHANGELOG.html) へ

- `com.unity.transport`: [2.7.2](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html) から [2.7.4](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk`: [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.6//changelog/CHANGELOG.html) から [1.7.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.7//changelog/CHANGELOG.html) へ

- `com.unity.microsoft.gdk.tools`: [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.6//changelog/CHANGELOG.html) から [1.7.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.7//changelog/CHANGELOG.html) へ