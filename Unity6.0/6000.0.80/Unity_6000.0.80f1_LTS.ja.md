# Unity 6000.0.80f1 LTS
公開日時：2026年7月22日（水）11:25:57 GMT  
https://unity.com/releases/editor/whats-new/6000.0.80f1

# 6000.0.80f1 の既知の問題

- `6000.0.23f1`: アニメーターの評価中に RigBuilder が再バインドを行った後、プレイモードを終了する際に Animator::OnPlayableUnbind でクラッシュする
    ([UUM-146750](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146750))

- `6000.0.67f1`: [iOS] iOSのコントロールセンターにアクセスすると、音声が途切れる
    ([UUM-145522](https://issuetracker.unity3d.com/issues/ios-audio-is-cut-out-when-accessing-ios-control-center))

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true) および UseTexture を指定して AddComputePass を使用した場合、D3D12SwapChain::Present の実行時にクラッシュする
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `アセットインポーター`: プレイモードに入ると、「(Unity) WriteObjectToVector」の処理中にエディターがクラッシュする
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: コマンドバッファのタイムアウトエラー発生後にゲームがフリーズする
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

bee_backendが複数実行されている際にmono_log_write_logfileでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

フォントアトラスの生成時に複数のスタックトレースが発生し、クラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.0.80f1 リリースノート

## 改善点

- `アセットパイプライン`: 説明の詳細を追加しました



## 修正点

- `2D`: ライトバッチングデバッガーでレイヤー名の並べ替えが反映されない問題を修正しました。
    ([UUM-136214](https://issuetracker.unity3d.com/issues/layer-names-in-the-light-batching-debugger-window-do-no-update-unless-the-window-is-restarted-or-a-new-layer-is-added-when-renaming-existing-layers))

- `2D`: 「2D パッケージをインストール」ボタンが、本来無効になるべきでない状況で無効になっていた問題を修正しました。
    ([UUM-143583](https://issuetracker.unity3d.com/issues/sprite-renderer内の「2Dスプライトパッケージをインストール」ボタンが、スプライトが割り当てられていない場合に無効化され、ヘルプテキストの内容と矛盾していた問題))

- `アクセシビリティ`: Android における `AccessibilityRole.Toggle` ノードのステータス通知が二重に表示される問題を修正しました。
    ([UUM-146950](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146950))

- `アセットのインポート`: 古いリソースにアクセスしたために発生していた、キーワード::LocalSpace::Find でのエディタのクラッシュを修正しました。
    ([UUM-133882](https://issuetracker.unity3d.com/issues/crash-on-keywords-localspace-find-when-reimporting-specific-assets))

- `アセットパイプライン`: 参照されているテクスチャが削除され、同じ GUID で復元された後、アセットのプレビューが白いままである問題を修正しました。
    ([UUM-138622](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-138622))

- `ドキュメント`: コンポーネントの使用方法に関する情報を追加しました。

- `エディタ`: `[SerializeReference]` フィールドを使用している異なる MonoBehaviour スクリプトを持つ GameObject を複数選択した際、`SerializableManagedRef::CallMethod` で発生していたクラッシュを修正しました。
    ([UUM-142019](https://issuetracker.unity3d.com/issues/crash-on-serializablemanagedref-callmethod-when-performing-various-unity-operations))

- `エディタ`: プラットフォームを選択して「ビルドプロファイルを追加」をクリックしても、プラットフォームブラウザダイアログでそのプラットフォームが選択されないという動作を修正しました。
    (UUM-130650)

- `Graphics`: レイトレーシング使用時の DirectX12 分割グラフィックスジョブにおけるクラッシュを修正しました。
    (UUM-145956)

- `iOS`: アプリがバックグラウンドに移行した際に iOS で発生していた誤った「Touch was already deallocated」エラーを修正しました。
    ([UUM-145381](https://issuetracker.unity3d.com/issues/ios-when-application-is-sent-to-background-with-active-touch-error-message-is-printed))

- `ネットワーク`: UnityWebRequest からの Curl エラーが適切にログに記録されず、問題のデバッグが困難になる状況を修正しました。なお、この状況下でも、エラーは呼び出し元コードに対して正しく報告されていました。このバグはログ記録にのみ影響していました。
    ([UUM-145433](https://issuetracker.unity3d.com/issues/unitywebrequest-can-lose-error-messages-from-curl))

- `URP`: 「Dirt Texture」が有効になっているが値が null の場合、Bloom のランタイムシェーダーバリアントが誤って選択される問題を修正しました。
    ([UUM-141980](https://issuetracker.unity3d.com/issues/bloom-post-processing-effect-in-urp-is-missing-in-a-build-when-dirt-texture-is-enabled-in-the-bloom-override-of-a-global-volume))

- `WebGL`: WebGPU: float32-blendable WebGPU 拡張機能の欠如に起因する、一部のモバイルデバイスでのエラーを修正しました。
    ([UUM-145735](https://issuetracker.unity3d.com/issues/webgpu-urp-errors-when-float32-blendable-isnt-available))

- `Windows`: Windows 環境で New Input System を使用し、`<Pointer>/position` バインディングを適用した際、ゲームビュー内でペンの位置が限られた領域に制限されて表示される問題を修正しました。
    ([UUM-142269](https://issuetracker.unity3d.com/issues/pen-position-gets-constrained-to-a-limited-area-when-using-a-stylus-in-game-view-or-player))




## 6000.0.80f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.services.authentication`: [3.6.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.6//changelog/CHANGELOG.html) から [3.7.3](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html) へ

- `com.unity.services.qos`: [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.qos@1.3//changelog/CHANGELOG.html) から [1.4.1](https://docs.unity3d.com/Packages/com.unity.services.qos@1.4//changelog/CHANGELOG.html) へ