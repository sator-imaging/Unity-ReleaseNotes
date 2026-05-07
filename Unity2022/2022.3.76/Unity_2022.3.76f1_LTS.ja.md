# Unity 2022.3.76f1 LTS
公開日時: Wed, 06 May 2026 09:39:50 GMT
https://unity.com/releases/editor/whats-new/2022.3.76f1

# 2022.3.76f1 の既知の問題

- `メタル`: コマンドバッファのタイムアウトエラーの後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))



# 2022.3.76f1 リリースノート

## 修正

- `アセットパイプライン`: Unityマニュアルのアクセラレータダウンロードリンクを最新バージョンに更新。
    (EAD-2077)

- `エディター`: エディターでコンテンツファイルをロード、アンロードする際のデッドロックの競合状態を修正。
    (UUM-137677)

- `エディター`: OpenGL ES を搭載した Mali GPU 上でステンシルのみのフォーマットを使用した場合のクラッシュを回避。
    ([UUM-111344](https://issuetracker.unity3d.com/issues/android-crash-on-startup-when-depth-stencil-format-is-set-to-s8-uint))

- `エンジン診断`: スタックトレースを Engine Diagnostics にアップロードする際のリトライロジックを追加。
    (UUM-137962)

- `エンジン診断`: CrashReportingSettings.captureEditorExceptions が有効な場合に、エディターの例外が Engine Diagnostics にレポートされない問題を修正しました。
    ([UUM-136672](https://issuetracker.unity3d.com/issues/diagnostics-does-not-report-editor-exceptions-when-using-crashreportingsettings-dot-captureeditorexceptions))

- `Graphics`: LJT-01-003脆弱性の悪用によるサービス拒否を防ぐために、"ImageConversion "クラスによって使用されるJPEGデコーダーに予防策を追加しました。Unityは、1000回のプログレッシブスキャンをデコードした後、JPEGファイルのデコードを自動的に中断するようになりました。
    (UUM-129186)

- `Graphics`: Adreno デバイス上で GPU スキニングを使用した際のクラッシュを修正しました。
    ([UUM-93243](https://issuetracker.unity3d.com/issues/crash-on-apigles-clearbuffersubdata-when-running-the-player-a-second-time-on-meta-quest-2))

- `Graphics`: DX12、Metal、およびレガシーVulkanデバイスでScalableBufferManagerを使用した場合に、MSAA CameraDepthTextureのリサイズに一貫性がない問題を修正しました。 スタンドアロンまたはAndroidプレーヤーをビルドする際に、ベクター型シェーダーの暗黙の切り捨て警告が投げられる問題を修正しました。
    ([uum-100367](https://issuetracker.unity3d.com/issues/android-ios-macos-inconsistent-cameradepthtexture-behavior-when-using-scalablebuffermanager-across-devices))

- `Graphics`: ユニフォームバッファバインディングに無効なバインディングスロットが渡された場合の OpenGLES のクラッシュを修正しました。
    (UUM-138897)

- `IL2CPP`: libil2cpp コードの C++ 警告を修正。
    (UUM-138294)

- `IL2CPP`: 無効なコード生成の原因となる C++ ポインタエイリアスの問題を修正。
    ([UUM-132447](https://issuetracker.unity3d.com/issues/ios-stripping-issue-on-xcode-26-when-use-incremental-gc-is-disabled))

- `iOS`: UISceneライフサイクルイベントのさらなる改善 - ユニバーサルなディープリンクの処理、Awake( \)で見逃さないように、AbsoluteURLセットを早めに移動。
    (UUM-140746)

- `ネットワーキング`: パッケージマネージャからアセットストアからアセットをダウンロードしようとするとTLSハンドシェイクエラーになるMbedTLSのリグレッションを修正しました。他の HTTPS エンドポイントもこのリグレッションの影響を受ける可能性がありました。
    (UUM-141298)

- `ネットワーキング`: MbedTLSをバージョン3.6.6に更新して、いくつかの(マイナーでおそらく爆発不可能な) セキュリティ脆弱性に対処しました。
    (UUM-140908)

- `スクリプト`: ScriptingCoverage::FilterRecordedMethods にメインスレッドガードを追加し、スクリプトのリロード中のスレッドセーフを実現。
    ([UUM-137724](https://issuetracker.unity3d.com/issues/crash-on-mono-jit-runtime-invoke-when-disabling-the-debug-mode-with-the-code-coverage-enabled))




## 2022.3.76f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.ide.rider`: [3.0.39](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) から [3.0.40](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) へ。

- `com.unity.services.user-reporting`: [2.0.14](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html) から [2.0.15](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html) へ。

- `com.unity.xr.core-utils`: [2.5.3](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html)から[2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.6//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.10.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.10//changelog/CHANGELOG.html) から [1.11.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.11//changelog/CHANGELOG.html) に変更。