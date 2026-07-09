# Unity 6000.0.79f1 LTS
公開日時: 2026年7月8日(水) 14:28:55 GMT  
https://unity.com/releases/editor/whats-new/6000.0.79f1

# 6000.0.79f1 の既知の問題

- `6000.0.67f1`: [iOS] iOSのコントロールセンターにアクセスすると音声が途切れる
    ([UUM-145522](https://issuetracker.unity3d.com/issues/ios-audio-is-cut-out-when-accessing-ios-control-center))

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true) および UseTexture を指定して AddComputePass を使用する際、D3D12SwapChain::Present でクラッシュする
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `アセットインポーター`: プレイモードに入ると、「(Unity) WriteObjectToVector」の処理中にエディターがクラッシュする
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: コマンドバッファのタイムアウトエラー発生後にゲームがフリーズする
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

bee_backendが複数実行されている際にmono_log_write_logfileでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

フォントアトラスの生成時に、複数のスタックトレースが発生してクラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.0.79f1 リリースノート

## 改善点

- `ビルドシステム`: 同梱の 7-Zip をバージョン 26.02 に更新しました。

- `グラフィックス`: ミップマップストリーミングのマニュアルページを更新し、UnityがメッシュのUVデータとカメラ位置からミップマップレベルをどのように選択するかを説明しました。また、Unityがレベルを計算できないオブジェクト（\(パーティクルシステムなどの手続き的に生成されたジオメトリを含む\)）の挙動を明確化し、`Texture2D.requestedMipmapLevel` のコード例を追加しました。
    ([UUM-131691](https://issuetracker.unity3d.com/issues/texture-rendered-at-different-fidelity-with-particle-system-renderer-when-using-a-different-material-derived-from-the-same-texture-with-identical-settings))



## 変更点

- `Android`: Gradle を 9.1.0 に、AGP を 9.0.0 にアップグレードしました。



## 修正点

- `2D`: Light2Dのシリアライゼーションに関する競合を修正しました。
    (UUM-141743)

- `2D`: 品質設定がカメラターゲット記述子に反映されない問題を修正しました。
    ([UUM-141000](https://issuetracker.unity3d.com/issues/quality-fields-are-not-propagated-to-the-camera-target-descriptor-when-using-renderer2ds-rendergraph-path))

- `AI`: UNITY_DELETE の代わりに UNITY_FREE を誤って使用したことにより発生していたメモリリークを修正しました。
    (UUM-144085)

- `Android`: ターゲットアーキテクチャごとに分割された APK がすべて同じバージョンコードを受け取ってしまう問題を修正しました。
    ([UUM-144372](https://issuetracker.unity3d.com/issues/arm64-and-armv7-apks-return-the-same-version-code-when-split-apks-by-target-architecture-is-enabled))

- `Android`: 使用されていない Tools 26.1.1 のダウンロードファイルを空のフォルダに置き換えました。
    (UUM-141878)

- `ドキュメント`: UITK ポップアップのサンプルコードと手順に、背景情報と詳細を追加しました。

- `ドキュメント`: VFX オペレーター「Reciprocal」の誤った「out」プロパティを更新しました。
    (UUM-144446)

- `エディタ`: モデルインポーターがプロジェクト全体でテクスチャを検索しないようにするオプションを追加しました。
    (UUM-137345)

- `エディタ`: オーディオ: 破損したオーディオミキサーアセットを含むプロジェクトを開いた際にエディタがクラッシュする問題を修正しました。
    ([UUM-143706](https://issuetracker.unity3d.com/issues/crash-on-audiomixercontroller-removeinvalidsendlevelguidsrecursive-when-opening-a-project-with-specific-audio-files-for-the-first-time))

- `エディタ`: エディタのシャットダウン中に、マネージドの DomainUnload ハンドラが UnityEngine.Object の null チェックを実行した際に発生していたクラッシュ（\(ProfilerMutexLock / assertion gPersistentManager \!= NULL\)）を修正しました。
    ([UUM-144371](https://issuetracker.unity3d.com/issues/crash-on-profilermutexlock-when-closing-a-project-with-specific-assets))

- `Editor`: Wayland上で実行中に、ファイルをエディタにドラッグする際に発生していたLinuxEditorのエラーを修正しました。
    ([UUM-111593](https://issuetracker.unity3d.com/issues/linux-the-error-releasebutton-expects-buttonid-is-thrown-when-trying-to-add-file-using-drag-and-hold-in-the-project-window))- `エディタ`: Wayland上で実行中に、ファイルをエディタにドラッグして追加しようとした際に発生していたLinuxエディタのエラーを修正しました。    ([UUM-111593](https://issuetracker.

- `エディタ`: `RedrawFromNative` 実行中に新しいウィンドウが開いたり閉じたりすると、InspectorWindow で例外が発生する問題を修正しました。
    ([UUM-141990](https://issuetracker.unity3d.com/issues/invalidoperationexception-is-thrown-when-clicking-ctrl-plus-z-after-opening-gradient-editor))

- `エディタ`: Perforce 内の追跡対象外のフォルダに対して VCCache が無限の再クエリループに陥る問題を修正しました。
    ([UUM-143313](https://issuetracker.unity3d.com/issues/cpu-usage-spikes-when-perforce-version-control-is-set-up-and-ai-assistant-is-installed))

- `Editor`: ベクトルのハッシュコード計算を改善しました。
    ([UUM-143005](https://issuetracker.unity3d.com/issues/hdrp-bloom-renders-with-a-purple-blue-or-green-anomaly-in-the-game-view-カメラのアナモルフィック設定が1に設定され、アスペクト比が16で割り切れる値であり、グラフィックスAPIがDX11またはDX12に設定されている状態で、ブルーム・アナモルフィック・ボリューム設定を切り替えた際))

- `エディター`: ローカルドキュメントが誤って削除されていましたが、復元されました。
    (UUM-143984)

- `エディター`: プレハブが予約済みフィールドを使用している場合に発生していたクラッシュを防止しました。
    ([UUM-144557](https://issuetracker.unity3d.com/issues/crash-on-saveprefabasset-when-selecting-a-specific-prefab))

- `エディタ`: オブジェクトセレクタで選択操作を行った際にネイティブのモーダルダイアログが開く場合、セレクタがフリーズするのを防ぎました。
    ([UUM-139847](https://issuetracker.unity3d.com/issues/object-selector-becomes-unresponsive-when-selecting-root-ui-document-as-data-source-for-add-binding-in-ui-builder))

- `Graphics`: IDATチャンクが破損したPNGファイルを読み込もうとした際に、「ImageConversion.LoadImage」でメモリリークが発生する問題を修正しました。
    ([UUM-143641](https://issuetracker.unity3d.com/issues/alloc-temp-main-leaks-a-persistent-4096-byte-allocation-when-imageconversion-dot-loadimage-fails-to-decode-a-png-with-valid-headers-but-corrupted-idat-chunk-data))

- `Graphics`: Windows で Vulkan を使用し、Split Graphics Jobs を実行する際、キャッシュに null が挿入され、その結果、DrawCalls が閉じられたコマンドバッファへの描画を試み、クラッシュを引き起こす問題を修正しました。
    (UUM-132307)

- `IL2CPP`: Linux 上で空の .usym ファイルが生成される問題を修正しました。
    ([UUM-142527](https://issuetracker.unity3d.com/issues/linux-stack-trace-file-path-and-line-number-information-is-missing-when-il2cpp-stacktrace-information-is-set-to-method-name-file-name-and-line-number))

- `入力システム`: Windows において、ベンダー定義のレポート数が大きい HID デバイス（例: `ReportCount=1024`）で、重複した記述子要素が出力されることにより、デバイスの `capabilities` 文字列が膨大になるバグを修正しました。記述子は正しいサイズになり、デバイスの実際のコントロールには影響がありません。
    (UUM-144506)

- `カーネル`: 多数の外部スレッドおよび手動ジョブが関与するジョブシステムにおける潜在的なデッドロックを修正しました。
    (UUM-143073)

- `Linux`: LinuxエディタからWindowsプレーヤーをビルドしたり、Visual Studioソリューションを作成したりする際のバグを修正しました。
    ([UUM-140187](https://issuetracker.unity3d.com/issues/linuxeditor-building-for-windows-throws-agilitysdk-dll-could-not-be-retrieved-ビルドプラットフォームをWindowsに切り替える前に「Visual Studioソリューションの作成」が有効になっていた場合))

- `Linux`: 新しい入力システムにおいて、タッチスクリーンでのダブルタップが認識されない問題を修正しました。
    ([UUM-145665](https://issuetracker.unity3d.com/issues/linux-double-taps-on-touch-screens-are-not-recognized-on-new-input-system))

- `ネットワーク`: UnityWebRequestにおいて、アップロードリクエストを再開した際に、エラー26または65（「必要なデータの巻き戻しができませんでした」）がログに記録されることがある問題を修正しました。
    ([UUM-144767](https://issuetracker.unity3d.com/issues/webrequest-missing-curlopt-seekfunction-causes-curl-error-26-on-post-retry-with-reused-connections))

- `Physics`: マルチボックス・プルーニング・ブロードフェーズを使用していない物理シーンで `Physics.RebuildBroadphaseRegions` メソッドが呼び出された際に発生する可能性があったクラッシュを修正しました。
    ([UUM-144472](https://issuetracker.unity3d.com/issues/physics-dot-rebuildbroadphaseregions-does-not-repopulate-them-with-pre-existing-shapes))

- `Physics`: `Physics.RebuildBroadphaseRegions` を呼び出した際、既存の Collider コンポーネントが新しく生成されたブロードフェーズ領域から除外されてしまう問題を修正しました。
    ([UUM-144472](https://issuetracker.unity3d.com/issues/physics-dot-rebuildbroadphaseregions-does-not-repopulate-them-with-pre-existing-shapes))

- `Profiler`: ProfilerSymbolsDelayedDeletion::AddCloneObject でのクラッシュを修正しました。
    ([UUM-144194](https://issuetracker.unity3d.com/issues/crash-on-profilersymbolsdelayeddeletion-addcloneobject-when-deserializing-an-object-instantiate-marker-with-a-dangling-slash-corrupt-name-string))

- `UI Toolkit`: タッチデバイスを使用して SceneView 内で GameObject をドラッグする際、ツールバーや他のエディタウィンドウを横切る移動中に動作が停止する問題を修正しました。
    ([UUM-142652](https://issuetracker.unity3d.com/issues/gameobject-movement-in-scene-view-becomes-stuttery-and-intermittently-freezes-when-using-non-standard-pointers-across-editor-tabs-or-window-boundaries))

- `URP`: URP スタンドアロン プレイヤー ビルドにおいて、Player ログにリーク警告が表示されていたメモリリークの問題を修正しました。
    ([UUM-115886](https://issuetracker.unity3d.com/issues/jobtempalloc-memory-leak-warning-is-thrown-when-the-player-is-shut-down))

- `Windows`: スタンドアロン・プレイヤービルドで入力マネージャーを使用する際、Windowsのペン入力でマウスポインタイベント（`Input.GetMouseButtonDown`）が生成されない問題を修正しました。
    ([UUM-140737](https://issuetracker.unity3d.com/issues/windows-pen-input-does-not-generate-mouse-pointer-events-when-using-input-manager))

- `Windows`: Windowsのタッチスクリーンデバイスでピンチジェスチャーを実行した後、UIツールキットのボタンがタッチ操作に反応しなくなる問題を修正しました。
    ([UUM-138595](https://issuetracker.unity3d.com/issues/ui-toolkit-buttons-stop-responding-to-single-taps-when-a-multi-touch-gesture-is-performed-with-the-new-input-system-on-windows-touch-devices))

- `Windows`: Windows IL2CPP ビルドで LNK1104 エラーが発生する問題を修正しました。
    ([UUM-139929](https://issuetracker.unity3d.com/issues/build-fails-with-a-link-error-when-building-for-windows-x64-with-il2cpp-and-having-visual-studio-2026-and-2022-installed))




## 6000.0.79f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.netcode`: [1.13.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html) から [1.14.0](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html) へ

- `com.unity.nuget.newtonsoft-json`: [3.2.1](https://docs.unity3d.com/Packages/com.unity.nuget.newtonsoft-json@3.2//changelog/CHANGELOG.html) から [3.2.2](https://docs.unity3d.com/Packages/com.unity.nuget.newtonsoft-json@3.2//changelog/CHANGELOG.html) へ

- `com.unity.services.cloudcode`: [2.7.1](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.7//changelog/CHANGELOG.html) から [2.10.2](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.10//changelog/CHANGELOG.html) へ

- `com.unity.services.core`: [1.16.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.16//changelog/CHANGELOG.html) から [1.18.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.18//changelog/CHANGELOG.html)

- `com.unity.services.economy`: [3.5.1](https://docs.unity3d.com/Packages/com.unity.services.economy@3.5//changelog/CHANGELOG.html) から [3.5.3](https://docs.unity3d.com/Packages/com.unity.services.economy@3.5//changelog/CHANGELOG.html) へ

- `com.unity.services.leaderboards`: [2.2.1](https://docs.unity3d.com/Packages/com.unity.services.leaderboards@2.2//changelog/CHANGELOG.html) から [2.3.3](https://docs.unity3d.com/Packages/com.unity.services.leaderboards@2.3//changelog/CHANGELOG.html) へ

- `com.unity.multiplayer.tools`: [2.2.8](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) から [2.2.9](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) へ

- `com.unity.services.deployment.api`: [1.0.0](https://docs.unity3d.com/Packages/com.unity.services.deployment.api@1.0//changelog/CHANGELOG.html) から [1.1.3](https://docs.unity3d.com/Packages/com.unity.services.deployment.api@1.1//changelog/CHANGELOG.html) へ

**追加されたパッケージ**

- [com.unity.xr.compositionlayers@2.5.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.5//changelog/CHANGELOG.html)