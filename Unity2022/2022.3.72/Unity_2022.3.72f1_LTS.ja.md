# Unity 2022.3.72f1 LTS
公開日時: Wed, 11 Feb 2026 12:30:31 GMT
https://unity.com/releases/editor/whats-new/2022.3.72f1

# 2022.3.72f1 の既知の問題

- `メタル`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `Video`: 2022.3.Xの修正: 特定のAndroidデバイスで、Videoを何度も有効/無効にすると、VideoPlayerがフリーズまたは停止する。
    (UUM-112470)



# 2022.3.72f1 リリースノート

## 改良点

- `アダプティブ・パフォーマンス`: アダプティブ・パフォーマンスを 4 から 5 にアップグレードし、16KB のサポートと 5.x ラインからのより多くの便利な機能とバグフィックスを追加。
    (UUM-126684)



## 修正

- `Android`: Android テスト "ExportGradleProjectForApk_WithSplitBinary_CreatesOBBAndShowsWarning" の不安定性を修正。
    (UUM-122699)

- `Editor`: カスタムプロパティドロワーがまだ使用されている時にDIsposedになる問題を修正しました。
    ([UUM-132087](https://issuetracker.unity3d.com/issues/propertydrawer-gets-disposed-while-still-being-active-when-adding-a-secondary-component))

- `Graphics`: AssetBundlesからリソース(典型的にはTextures)をロードする時、まれに AsyncResourceUploadBlocking(◆)でデッドロックが発生するのを修正した。
    ([uum-126066](https://issuetracker.unity3d.com/issues/android-the-application-freezes-during-the-assetbundle-loading))

- `iOS`: コンソールアプリでiOS 26のログが&lt;private&gt;として表示されるのを修正しました。
    ([uum-129367](https://issuetracker.unity3d.com/issues/ios-debug-dot-log-appears-as-in-console-app))

- `iOS`: 数字パッドまたは電話パッドキーボードタイプを使用しているときに、画面上のキーボードが再オープンしないのを修正。
    (UUM-132968)

- `Shadergraph`: コピーペーストや複製後にノードが適切に選択されるようになりました。
    ([UUM-110841](https://issuetracker.unity3d.com/issues/nodes-in-shader-graph-are-not-selected-when-they-are-duplicated))

- `バージョン管理`: 2.11.2のWaitForPendingOperations.cs.metaの無効なGUIDの重複によるコンパイルエラーを修正。

- `バージョン管理`: Unity 6.3以下のバージョンでエディター内部へ直接アクセスできるように修正。

- `バージョン管理`: linux でのバージョン管理ネイティブテストでの断続的な失敗を修正。
    (UUM-130258)




## 2022.3.72f1 におけるパッケージの変更

## 更新されたパッケージ

- `com.unity.adaptiveperformance`: [4.0.1](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance@4.0//changelog/CHANGELOG.html) から [5.1.6](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance@5.1//changelog/CHANGELOG.html) へ。

- `com.unity.adaptiveperformance.samsung.android`: [4.0.2](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance.samsung.android@4.0//changelog/CHANGELOG.html)から[5.1.0](https://docs.unity3d.com/Packages/com.unity.adaptiveperformance.samsung.android@5.1//changelog/CHANGELOG.html)

- `com.unity.addressables`: [1.28.1](https://docs.unity3d.com/Packages/com.unity.addressables@1.28//changelog/CHANGELOG.html) から [1.28.2](https://docs.unity3d.com/Packages/com.unity.addressables@1.28//changelog/CHANGELOG.html) に変更。

- `com.unity.burst`: [1.8.27](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) から [1.8.28](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.11.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) から [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html)

- `com.unity.ide.rider`: [3.0.38](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) から [3.0.39](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- `com.unity.inputsystem`: [1.17.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.17//changelog/CHANGELOG.html) から [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html)

- `com.unity.mobile.android-logcat`: [1.4.6](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) から [1.4.7](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) に変更。

- `com.unity.mobile.notifications`: [2.4.2](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html)から[2.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.2.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.2//changelog/CHANGELOG.html) から [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) に変更。

- `com.unity.purchasing`: [4.14.0](https://docs.unity3d.com/Packages/com.unity.purchasing@4.14//changelog/CHANGELOG.html) から [4.14.2](https://docs.unity3d.com/Packages/com.unity.purchasing@4.14//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: [1.23.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html) から [1.23.3](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html) へ。

- `com.unity.services.analytics`: [6.2.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) から [6.2.1](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) に変更。

- `com.unity.xr.arcore`: [5.2.0](https://docs.unity3d.com/Packages/com.unity.xr.arcore@5.2//changelog/CHANGELOG.html) から [5.2.2](https://docs.unity3d.com/Packages/com.unity.xr.arcore@5.2//changelog/CHANGELOG.html) に変更。

- `com.unity.xr.arfoundation`: [5.2.0](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@5.2//changelog/CHANGELOG.html)から[5.2.2](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@5.2//changelog/CHANGELOG.html)

- `com.unity.xr.arkit`: [5.2.0](https://docs.unity3d.com/Packages/com.unity.xr.arkit@5.2//changelog/CHANGELOG.html)から[5.2.2](https://docs.unity3d.com/Packages/com.unity.xr.arkit@5.2//changelog/CHANGELOG.html)

- `com.unity.xr.hands`: [1.7.2](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html) から [1.7.3](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html) に変更。

- `com.unity.profiling.systemmetrics.mali`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) から [1.1.1](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) に変更。

- `com.unity.memoryprofiler`: [1.1.9](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) から [1.1.10](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) に変更。

- `com.unity.dt.app-ui`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.0//changelog/CHANGELOG.html) から [1.3.5](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.3//changelog/CHANGELOG.html) へ。

- `com.unity.microsoft.gdk`: [1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.4//changelog/CHANGELOG.html) から [1.5.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html) に変更。

- `com.unity.microsoft.gdk.tools`: [1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.4//changelog/CHANGELOG.html) から [1.5.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html) に変更。

- `com.unity.microsoft.gdk.discovery`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.1//changelog/CHANGELOG.html) ～ [1.2.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.9.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html) から [1.9.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html) に変更。