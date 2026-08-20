# Unity 6000.0.82f1 LTS
公開日時：2026年8月19日（水）13:32:25 GMT  
https://unity.com/releases/editor/whats-new/6000.0.82f1

# 6000.0.82f1 の既知の問題

- `6000.0.11f1`: StreamingAssets フォルダに保存されたシーンでライティングをベイクする際、_platform_memcmp の処理中にクラッシュする
    ([UUM-149240](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149240))

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true) および UseTexture を指定して AddComputePass を使用する際、D3D12SwapChain::Present でクラッシュする
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

bee_backendが複数実行されている場合、mono_log_write_logfileでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

フォントアトラスの生成時に、複数のスタックトレースが発生してクラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.0.82f1 リリースノート

## 修正点

- `AI`: navAgent.Move を使用して移動する際、NavMeshAgent が箱状の障害物の角で動かなくなる問題を修正しました。
    ([UUM-136684](https://issuetracker.unity3d.com/issues/navmeshagent-gets-stuck-on-the-corner-of-a-box-shape-navmeshobstacle-when-it-is-moved-with-navagent-dot-move))

- `アセットパイプライン`: アセットパイプライン：プレイモードに入った際に発生する可能性があった、WriteObjectToVector / CreateOrReloadInspectorCopy でのエディタのクラッシュを修正しました。
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `ビルドパイプライン`: メモリ設定 \(メインアロケーター &gt; その他のアロケーター &gt; Remapper の初期容量\) で、PersistentManager.Remapper の容量を確保する機能を追加しました。
    (UUM-136275)

- `DX12`: Windows で Direct3D12 グラフィックス API を使用する際、テクスチャが破棄された後も、そのテクスチャが使用していた VRAM が GPU ドライバーに解放されない問題を修正しました。<br>
    `d3d12-small-texture-tiles-per-heap` ブート設定パラメータを使用して、小規模テクスチャのヒープサイズを調整できるようになり、VRAMの回収とヒープ割り当てのオーバーヘッドのバランスを調整できるようになりました。
    ([UUM-142284](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142284))

- `エディター`: Windows版エディターに同梱されていた、ウイルス対策ソフトによってブロックされることがあった署名なしの実行ファイル数件に、デジタル署名を追加しました。
    (UUM-147382)

- `Graphics`: `Resolution` および `RefreshRate` に `IEquatable<T>`、`GetHashCode`、および等価演算子を追加し、これらを比較したり、Dictionary のキーとして使用したりする際の GC による割り当てを回避しました。
    (UUM-146197)

- `Graphics`: オーバーレイ UI テクスチャの MSAA サンプル数が URP で混在する問題を修正しました。

- `Graphics`: グラフィック設定 - 「現在のシーンからインポート」アクションが元に戻すリストに追加されない問題を修正しました。
    ([UUM-148881](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148881))

- `iOS`: Apple GPUファミリー1～3において、MSAA深度を持つレンダーパスのマージが時折失敗する問題を修正しました。
    ([UUM-147831](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147831))

- `iOS`: 旧型デバイス（AppleFamily3 以前）におけるシェーダーのウォームアップ問題を修正しました。
    ([UUM-147933](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147933))

- `iOS`: 2019年以降に発売されたiPadでApple Pencilを使用する際に発生していた警告を修正しました。
    ([UUM-147481](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147481))

- `ライセンス`: 指名ユーザーライセンスファイルをインポートした際に、手動でのライセンス有効化に失敗する問題を修正しました。

- `マルチプレイヤー`: GPU Resident Drawer が有効になっている状態で、クローンされたオブジェクトのレンダリングコンポーネントが専用サーバーロールによって削除された際に、エディタがクラッシュする問題を修正しました。
    ([UUM-147692](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147692))

- `Networking`: Webリクエストが突然切断された際に、無効なテクスチャポインタが参照される問題。
    ([UUM-144540](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144540))

- `Networking`: 多くのドメイン再読み込みを伴う長時間のエディターセッションにおいて、UnityWebRequestでカスタム証明書ハンドラーを使用した場合に、エディターのみで発生する可能性のあるクラッシュを修正しました。
    ([UUM-147347](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147347))

- `QNX`: 起動時のタイミングにより、報告されたユーザー時間がオーバーフローする可能性がありました。
    (UUM-148079)

- `シリアライゼーション`: メインスレッド外で WeakReference が破棄されていたため、WeakReference はメインスレッドからのみ解放されるという Mon の GC の前提と競合し、クラッシュが発生する問題を修正しました。これにより、ガベージコレクタ内部で発生していたクラッシュが解消されました。
    (UUM-143324)

- `SRP Core`: サンプルごとのシェーディングをサポートしていない OpenGL ES 3.1 デバイスで MSAA テクスチャをコピーする際に発生していたシェーダーエラーを修正しました。これらのデバイスでは、通常のブリット処理にフォールバックするようになりました。
    (UUM-147215)

- `URP`: 品質レベルが変更された際に、Metal および OpenGL のバックバッファが古い MSAA サンプル数を保持していた問題を修正しました。これにより、「Attachment 0 は N サンプルで作成されましたが、M サンプルが要求されました」というレンダリングパスエラーが記録されることがありました。
    (UUM-140492)

- `WebGL`: 複数のレイヤーとミップマップを持つ ASTC 圧縮テクスチャのテクスチャデータが正しくアップロードされない問題を修正しました。
    (UUM-145086)




## 6000.0.82f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.collab-proxy`: [2.12.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.12//changelog/CHANGELOG.html) から [2.13.6](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.13//changelog/CHANGELOG.html) へ

- `com.unity.formats.alembic`: [2.4.5](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) から [2.4.7](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) へ

- `com.unity.recorder`: [5.1.6](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) から [5.1.7](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) へ

- `com.unity.multiplayer.tools`: [2.2.9](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) から [2.2.10](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) へ

- `com.unity.ai.navigation`: [2.0.13](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) から [2.0.14](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) へ

- `com.unity.services.deployment`: [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.3//changelog/CHANGELOG.html) から [1.7.2](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.7//changelog/CHANGELOG.html) へ