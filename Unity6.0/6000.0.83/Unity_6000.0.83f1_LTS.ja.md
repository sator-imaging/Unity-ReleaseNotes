# Unity 6000.0.83f1 LTS
公開日時：2026年9月2日（水）10:47:00 GMT  
https://unity.com/releases/editor/whats-new/6000.0.83f1

# 6000.0.83f1 の既知の問題

- `2021.3.34f1`: 再生モードで音量を変更すると、オーディオミキサーからクリック音がする
    ([UUM-150250](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150250))

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true) および UseTexture を指定して AddComputePass を使用すると、D3D12SwapChain::Present でクラッシュする
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

bee_backendが複数実行されている場合、mono_log_write_logfileでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

フォントアトラスの生成時に複数のスタックトレースが発生し、クラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.0.83f1 リリースノート

## 変更点

- `Mono`: ToFileDescriptor からアサーションを削除
    ([UUM-145761](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145761))



## 修正

- `AI`: サポートされていない設定の結果、NavMeshAgent が任意の方向にジャンプして、自身の NavMeshObstacle コンポーネントから離れようとしていました。現在は、エージェントが安定した一方向に移動するようになりました。
    (UUM-141803)

- `AI`: ボックス型の NavMeshObstacle 内に生成またはテレポートされた NavMeshAgent は、その障害物から抜け出せませんでした。
    ([UUM-146477](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146477))

- `Android`: Androidの「External Tools」設定パネルにおける配置の不具合を修正しました。
    (UUM-148378)

- `Audio`: 読み込み中のストリーミングクリップを含むAudioRandomContainerを一時停止した際に発生していたクラッシュを修正しました。
    (UUM-148440)

- `Audio`: オーディオ設定のリセット後に、一部のオーディオクリップで LoadState が無効になる問題を修正しました。
    ([UUM-147700](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147700))

- `コードエディタ`: [環境設定] > [外部ツール] 内の「引数をリセット」ボタンについて、フォーカスが移動した後にのみ更新されるのではなく、即座に「外部スクリプトエディタの引数」フィールドが更新されるように修正しました。
    (UUM-150210)

- `エディタ`: コピー操作中に存在しないアセットを削除しようとしてしまう問題を修正しました。
    ([UUM-144993](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144993))

- `エディタ`: ビルド中にアクセラレータから切断された際に発生するクラッシュを修正しました。
    ([UUM-148391](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148391))

- `エディタ`: フローティング表示のビデオクリップインスペクタのプレビューエラーおよび表示上の警告を修正しました。
    ([UUM-147192](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147192))

- `エディタ`: トリミングやオフセットが適用された動画をインポートまたはトランスコードする際に、Windows版エディタがクラッシュする問題を修正しました。
    ([UUM-146426](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146426))

- `EmbeddedLinux`: システムに `wl_seat` が存在しない場合に発生していたクラッシュを修正しました。
    (UUM-148754)

- `GI`: StreamingAssets内に配置されたシーンのライティングをベイクする際に発生していたクラッシュを修正しました。
    ([UUM-149240](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149240))

- `Graphics`: GRDが有効な場合、staticShadowCasterの変更が正しく反映されるようになりました。
    ([UUM-140724](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140724))

- `Graphics`: Vulkan Player が 'PlayerSettings.vulkanNumSwapchainBuffers' の値を反映せず、代わりに 3 つのスワップチェーンバッファという固定数を使用していた問題を修正しました。
    (UUM-148724)

- `Graphics`: 「Unityの『Screen』サイズを最小化」という最適化設定でXRを使用する際、ミップマップレベルの計算が不正確になる問題を修正しました。<br>
    XRにおけるカメラ矩形は、SRPにおいてステレオの合計寸法ではなく、片目ごとの寸法を正しく返すようになりました。これは、ミップマップストリーミングや解像度依存のUI/テキストレンダリングなど、解像度依存の計算にカメラ矩形に依存するすべてのシステムに影響します。必要に応じて、ミップマップストリーミングの設定やUIのスケーリングを調整してください。
    ([UUM-47681](https://issuetracker.unity3d.com/issues/calculated-mipmap-level-does-not-taking-xr-resolution-into-account))

- `SRP Core`: AMDUnityPlugin が静的にリンクされた CRT を使用するように修正しました。
    (UUM-147060)

- `uGUI`: 「Overflow」が「Ellipsis」に設定されている大きな Text \(TMP\) GameObject を使用する際、`IndexOutOfRangeException` が発生する問題を修正しました。
    ([UUM-134477](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-index-was-outside-the-bounds-of-the-array-dot-error-is-thrown-when-large-text-tmp-gameobject-overflow-field-is-set-to-ellipsis))

- `UI Toolkit`: 内部の描画範囲リストが部分的に埋まっている状態でリストが拡大した際、ワールド空間での UI レンダリング中に ArgumentException が発生する問題を修正しました。
    (UUM-149611)

- `UI Toolkit`: 8 つ以上のボタンが存在する場合に、ToggleButtonGroup の値がラップしてしまう問題を修正しました。
    ([UUM-149531](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149531))

- `VFX Graph`: URP におけるフラスタムカリングの不具合を修正しました。
    ([UUM-138375](https://issuetracker.unity3d.com/issues/vfx-graph-particles-are-not-culled-when-using-urp-and-frustum-culling-is-enabled-on-vfx-mesh-output))

- `Video`: NVIDIAの「Fast」垂直同期が有効な場合、Direct3DでStop\(\)後に動画が再生できなくなる問題を修正しました（デコードデバイスが失われ、回復されなかったため）。
    ([UUM-135548](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-135548))

- `Video`: WebM Vorbis オーディオトラックが 0 Hz、0 チャンネルと報告される問題を修正しました。
    (UUM-144045)




## 6000.0.83f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.netcode`: [1.14.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html) から [1.14.2] へ(https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: [3.7.3](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html) から [3.7.4](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html) へ

- `com.unity.services.wire`: [1.4.4](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html) から [1.5.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.5//changelog/CHANGELOG.html) へ

- `com.unity.timeline`: [1.8.12](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) から [1.8.13](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) へ

- `com.unity.visualscripting`: [1.9.11](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) から [1.9.12](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) へ