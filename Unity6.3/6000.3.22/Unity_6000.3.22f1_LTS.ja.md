# Unity 6000.3.22f1 LTS
公開日時：2026年8月13日（木） 06:39:34 GMT  
https://unity.com/releases/editor/whats-new/6000.3.22f1

# 6000.3.22f1 の既知の問題

- `6000.0.11f1`: StreamingAssets フォルダに保存されたシーンでライティングをベイクする際、_platform_memcmp の処理中にクラッシュする
    ([UUM-149240](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149240))

- `6000.3.0a1`: ライティング可視化オーバーレイを「プレビュー」に切り替えた際に、PVRAtlassingData::Build でクラッシュし、メモリリークが発生する
    ([UUM-149471](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149471))

- `アセットインポーター`: プレイモードに入った際に「(Unity) WriteObjectToVector」でエディターがクラッシュする
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: コマンドバッファのタイムアウトエラー発生後にゲームがフリーズする
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- テキスト (TextMeshPro): TMPro Font Asset Creator でマルチスレッドのフォントアトラスを生成する際、UNITY_FT_Load_Glyph でクラッシュする
    ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

bee_backend が複数実行されているときに mono_log_write_logfile でクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

Font Atlasの生成時に、複数のスタックトレースが発生してクラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.3.22f1 リリースノート

## 改善点

- `エディタ`: 地形: 同一の非インスタンス化されたディテールプロトタイプを使用する地形タイル間で、ディテールアトラステクスチャが共有されるようになりました。これにより、複数のタイルからなる地形構成におけるメモリ使用量が大幅に削減されます。
    (UUM-148356)



## APIの変更

- `Android`: 追加: SDK Platform 37のサポートを追加しました



## 修正

- `Adaptive Performance`: 「Adaptive Performance」がエンジンモジュールに移行された後、プレイヤー内でVisual Scriptingノード（\(bottleneck, thermal、performance level、boost、performance mode、および scaler イベント）が、Adaptive Performance がエンジンモジュールに移行した後にプレイヤー内で発火しなくなる問題を修正しました。これらのイベントは、`VISUAL_SCRIPTING_ENABLED` 定義が有効な Adaptive Performance サンプルパッケージアセンブリから、Visual Scripting の `EventBus` へ転送されるようになりました。
    (UUM-135587)

- `Adaptive Performance`: パッケージ操作中にAdaptive Performanceの設定を無効化するようにしました。
    ([UUM-140197](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140197))

- `Android`: Android サポートがインストールされている際に、Unity の環境設定のテキストフィールドでラグが発生する問題を修正しました。
    (UUM-147435)

- `Audio`: エディタを数日間起動したままにしていた後に発生していた、オーディオサブシステムでロックを取得する際、アクセスバージョンが奇数でなければならないというアサーションに関する問題を修正しました。
    ([UUM-146734](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146734))

- `エディタ`: 非アクティブなレンダリングパイプラインを破棄する際に `activeRenderPipelineDisposed` が発火しないようにするため、静的関数 `CleanupRenderPipelineIfActive` を追加しました。
    ([UUM-148022](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148022))

- `エディタ`: 「環境設定」ウィンドウの「インデックス設定」に、有効な検索用語/キーワードをいくつか追加しました。
    ([UUM-146350](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146350))

- `エディタ`: スプラッシュスクリーンが無効になっている状態で `SplashScreen.Stop(FadeOut)` を呼び出しても、アプリケーションがフリーズしなくなりました。
    (UUM-143481)

- `エディタ`: Windows エディタに同梱されている実行ファイルのうち、以前は署名されていなかったもののいくつかにコード署名を行い、ウイルス対策ソフトウェアによってブロックされることがある問題を解消しました。
    (UUM-147382)

- `エディタ`: UITK エディタのテキストにおける高度なフォント機能を無効化しました。
    ([UUM-147689](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147689))

- `エディタ`: プレイモード中の「ビルドプロファイル」設定における「削除」ボタンを無効化しました。
    ([UUM-143194](https://issuetracker.unity3d.com/issues/adaptive-performance-settings-in-the-build-profile-window-can-be-removed-when-in-play-mode-which-results-in-serializedobjectnotcreatableexception-errors-thrown))

- `エディタ`: スクリプティング定義設定リストでスクリプティング定義の値を追加した後、ビルドプロファイルのフォーカスが外れた際に表示されるプロンプトで「元に戻す」をクリックしても、新しく追加された値が削除されないというバグを修正しました。
    ([UUM-147113](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147113))

- `エディタ`: ATG で複数行の省略記号を使用する際に発生していたクラッシュを修正しました。
    (UUM-147865)

- `エディタ`: Android プロバイダでの「適応型パフォーマンス設定」の削除時にエラーが発生する問題を修正しました。
    ([UUM-143194](https://issuetracker.unity3d.com/issues/adaptive-performance-settings-in-the-build-profile-window-can-be-removed-when-in-play-mode-which-results-in-serializedobjectnotcreatableexception-errors-thrown))

- `エディタ`: Linux版エディタで、2Dタイルパレットウィンドウを開いた直後にウィンドウが閉じてしまう問題を修正しました。
    ([UUM-146416](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146416))

- `エディター`: ATG におけるタブ幅が原因で発生していたクラッシュを修正しました。
    (UUM-147528)

- `エディター`: テスト実行のたびにテクスチャのインポートを強制することで、テスト時の不安定さを修正しました。
    (UUM-122895)

- `エディター`: インスペクターでスクリプトが存在しないコンポーネントから「コンポーネントの削除」メニューが表示されない問題を修正しました。
    ([UUM-146874](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146874))

- `エディタ`: オブジェクトピッカーを開いた際、現在割り当てられているオブジェクトまでスクロールされない問題を修正しました。
    ([UUM-143327](https://issuetracker.unity3d.com/issues/object-picker-scrolls-incorrectly-depending-on-which-asset-was-selected-previously-when-in-grid-view))

- `エディタ`: スクリプト: AI Assistant パッケージ（または単純名が重複するアセンブリを導入する任意のパッケージ）をインストールした後にコンソールに表示される「Lifecycle ERROR」および「NullReferenceException」エラーを修正しました。
    ([UUM-135379](https://issuetracker.unity3d.com/issues/console-displays-lifecycle-error-and-nullreferenceexception-errors-after-ai-assistant-installation))

- `エディター`: 管理者権限でUnityを実行する際のWinEditorの警告ダイアログのテキストを更新しました。
    ([UUM-146796](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146796))

- `GI`: 「ライティング」ウィンドウで「ソース」を変更した際に、カスタム環境反射キューブマップが失われる問題を修正しました。
    (UUM-133122)
	
- `HDRP`: 「フォワードのみのシェーダーモード」でクリアコートの値が 0 の場合、クリアコートマテリアルがスクリーンスペース反射を生成する問題を修正しました。
    ([UUM-84980](https://issuetracker.unity.com/issues/8208/clear-coat-materials-produce-screen-space-reflections-when-the-clear-coat-value-is-0-in-forward-only-lit-shader-mode))

- `iOS`: iOSのコントロールセンターを引き下ろすと、Unityアプリのオーディオ再生が停止してしまうバグを修正しました。
    ([UUM-145522](https://issuetracker.unity3d.com/issues/ios-audio-is-cut-out-when-accessing-ios-control-center))

- `iOS`: Apple GPUファミリー1～3において、MSAA深度を含むレンダリングパスのマージが時折失敗する問題を修正しました。
    ([UUM-147831](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147831))

- `iOS`: 旧型デバイス（AppleFamily3 以前）におけるシェーダーのウォームアップ問題を修正しました。
    ([UUM-147933](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147933))

- `iOS`: 2019年以降に発売されたiPadでApple Pencilを使用する際に発生していた警告を修正しました。
    ([UUM-147481](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147481))

- `Linux`: 新しいカーネルバージョンでワイヤレス Xbox 360 コントローラーを使用する際、D-Pad の入力が誤った方向に割り当てられる問題を修正しました。
    ([UUM-136083](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-136083))

- `Linux`: Linux上でBluetooth経由でXboxコントローラーを接続した際、Unity Input Systemにおいて一部のXboxコントローラー入力が本来とは異なるボタンに割り当てられてしまう問題を修正しました。
    ([UUM-144216](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144216))

- `macOS`: macOSのサーバービルドでlibMonoPosixHelper.dylibが見つからない問題を修正しました。
    ([UUM-141263](https://issuetracker.unity3d.com/issues/macos-server-cannot-find-libmonoposixhelper-dot-dylib-when-calling-gzipstream))

- `マルチプレイヤー`: マルチプレイヤープレイモードが有効になっていない、またはそのパッケージがインストールされていないプロジェクトにおいて、エディタウィンドウのレイアウトを読み込むと、破損した「読み込みに失敗しました」というマルチプレイヤープレイモードウィンドウが表示され、その周囲にウィンドウをドッキングしようとするとNullReferenceExceptionが発生する問題を修正しました。
    ([UUM-146870](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146870))

- `パッケージマネージャー`: アセットストア上のカスタマイズされた UPM パッケージが「未インストール」と表示される問題を修正しました。
    ([UUM-131282](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-131282))

- `QNX`: 起動時のタイミングにより、報告されたユーザー時間がオーバーフローする可能性がありました。
    (UUM-148079)

- `スクリプティング`: ドメインのリロード時に、古くなった GC ハンドルに対する予防的なチェックおよび修正を追加しました。
    ([UUM-122598](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-performing-various-actions-with-the-cesium-package-installed))

- `シリアライゼーション`: メインスレッド外で WeakReferences が破棄されていたために発生していたクラッシュを修正しました。これは、WeakReferences はメインスレッドからのみ解放されるという Mon の GC の前提と競合していました。これにより、ガベージコレクタ内部で最終的に発生していたクラッシュが修正されました。
    (UUM-143324)

- `SRP Core`: サンプルごとのシェーディングをサポートしていない OpenGL ES 3.1 デバイスで、MSAA テクスチャをコピーする際に発生していたシェーダーエラーを修正しました。これらのデバイスでは、通常のブリット処理にフォールバックするようになりました。
    (UUM-147215)

- `UI Toolkit`: `display: none` で非表示にした後、再度表示された際に、ワールド空間の `UIDocument` が一時的に位置がずれて表示される 1 フレームの不具合を修正しました。
    (UUM-119563)

- `UI Toolkit`: ドメインのリロードによって中断された際に、Object Picker ウィンドウが破損する問題を修正しました。
    ([UUM-144436](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144436))




## 6000.3.22f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.netcode`: [1.14.0](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html) から [1.14.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html)

- `com.unity.recorder`: [5.1.6](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) から [5.1.7](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) へ

- `com.unity.searcher`: [4.9.4](https://docs.unity3d.com/Packages/com.unity.searcher@4.9//changelog/CHANGELOG.html) から [4.9.5](https://docs.unity3d.com/Packages/com.unity.searcher@4.9//changelog/CHANGELOG.html)

- `com.unity.xr.meta-openxr`: [2.3.1](https://docs.unity3d.com/Packages/com.unity.xr.meta-openxr@2.3//changelog/CHANGELOG.html) から [2.3.2](https://docs.unity3d.com/Packages/com.unity.xr.meta-openxr@2.3//changelog/CHANGELOG.html) へ

- `com.unity.netcode.gameobjects`: [2.13.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html) から [2.13.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html) へ

- `com.unity.multiplayer.tools`: [2.2.9](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) から [2.2.10](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) へ

- `com.unity.services.deployment`: [1.7.1](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.7//changelog/CHANGELOG.html) から [1.7.2](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.7//changelog/CHANGELOG.html) へ

- `com.unity.polyspatial`: [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.1//changelog/CHANGELOG.html) から [3.2.2](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.2//changelog/CHANGELOG.html) へ

- `com.unity.polyspatial.visionos`: [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.1//changelog/CHANGELOG.html) から [3.2.2](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.2//changelog/CHANGELOG.html) へ

- `com.unity.polyspatial.xr`: [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.1//changelog/CHANGELOG.html) から [3.2.2](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.2//changelog/CHANGELOG.html) へ

- `com.unity.polyspatial.extensions`: [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.1//changelog/CHANGELOG.html) から [3.2.2](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.2//changelog/CHANGELOG.html)

- `com.unity.xr.visionos`: [3.1.5](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.1//changelog/CHANGELOG.html) から [3.2.2](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.2//changelog/CHANGELOG.html) へ

- `com.unity.services.multiplayer`: [2.2.4](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.2//changelog/CHANGELOG.html) から [2.3.0](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.3//changelog/CHANGELOG.html) へ