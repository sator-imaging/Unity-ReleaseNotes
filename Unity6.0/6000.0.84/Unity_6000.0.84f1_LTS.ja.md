# Unity 6000.0.84f1 LTS
公開日時：2026年9月16日（水）08:37:48 GMT  
https://unity.com/releases/editor/whats-new/6000.0.84f1

# 6000.0.84f1 の既知の問題

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true) および UseTexture を指定して AddComputePass を使用する際、D3D12SwapChain::Present でクラッシュする
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.3.0a1,6000.0.51f1`: 2D レンダラーでブルームが有効な場合に黒い画面が表示される
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

bee_backendが複数実行されている際に、mono_log_write_logfileの呼び出しでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

フォントアトラスの生成時に複数のスタックトレースが発生し、クラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

[WinEditor] ポーリングレートが高い状態でマウスカーソルを動かすと、再生モードのフレームレートが大幅に低下する
    ([UUM-142550](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142550))



# 6000.0.84f1 リリースノート

## 変更点

- `Android`: エディタに同梱されている Gradle のバージョンを 9.1.0 から 9.3.1 に更新しました。



## 修正点

- `Android`: Androidのバージョンラベルを、Googleの命名規則に合わせて修正しました。
    (UUM-150412)

- `Android`: 「Run Without Focus」が設定されている際に、AndroidでWebCamTextureが復元されない問題を修正しました。
    (UUM-149681)

- `Android`: Android API レベル 32 未満の場合、SystemInfo.processorModel および SystemInfo.processorManufacturer が警告文字列ではなく「unknown」を返すように修正しました。これにより、他のプラットフォームでの動作と一致するようになりました。
    (UUM-150389)

- `Audio`: 再生モードでのオーディオミキサーのフェーダーのクリック音を修正しました。
    ([UUM-150250](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150250))

- `Audio`: 一定時間の無音後に出力を再開する際、オーディオ出力デバイスの再初期化に失敗しても、エディタがエラーをログに出力しなくなりました。現在は出力が一時停止されたままとなり、警告がログに出力され、次にオーディオが使用される際に再開が再試行されます。また、出力を再開できなかった場合にエディタのシャットダウン時に発生する可能性があったクラッシュも修正されました。
    (UUM-115959)

- `ビルドシステム`: ビルド中にシステムクロックが過去に遡った場合、ビルドが成功したにもかかわらず IL2CPP Analytics ツールが JsonException を発生させて終了してしまう問題を修正しました。
    ([UUM-150019](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150019))

- `エディタ`: アニメーションウィンドウでHDRカラーが正しく記録されない問題を修正しました。
    ([UUM-83771](https://issuetracker.unity3d.com/issues/hdr-colors-are-recorded-in-gamma-compressed-values-instead-of-linear-values-when-using-the-animation-window))

- `EmbeddedLinux`: 最初のタッチ入力が無視される問題を修正しました。
    (UUM-150086)

- `Graphics`: Blit Type が「Auto」に設定されている際に、Midgard Mali GPU でデバイスがフリーズする問題を修正しました。
    (UUM-149414)

- `Graphics`: OpenGL ES 使用時に、マテリアルごとの定数バッファに関連するメモリエラーによって引き起こされるクラッシュを修正しました。
    (UUM-150590)

- `Graphics`: 品質設定 - デフォルトのプラットフォームには「…」が追加され、名称が非常に長い品質レベルには「品質レベルヘッダー」が追加されました。
    ([UUM-148889](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148889))

- `Linux`: 最初のタッチ入力が無視される問題を修正しました。
    (UUM-150086)

- `QNX`: 最初のタッチ入力が失われるケースを修正しました。
    (UUM-150086)

- `uGUI`: フォントに省略記号のグリフがなく、「省略記号のオーバーフローモード」が選択されている場合に、省略記号の改行再帰が発生する問題を修正しました。
    ([UUM-134066](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134066))

- `URP`: タイルマップのグリッド線が表示されない問題を修正しました。 SRP によるレンダリング後、プレビューカメラのレンダリングターゲットが正しいことを確認してください。
    ([UUM-122618](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-122618))

- `バージョン管理`: エディタの起動時に、「UpdateSettings: Unknown version control plugin: XYZ」というバージョン管理エラーを引き起こしていたレースコンディションを修正しました。
    ([UUM-149884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149884))

- `VFX Graph`: 組み込み属性の再分類を防ぐための修正を行いました。
    ([UUM-151058](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151058))

- `Web`: NameFilesAsHashes の機能を修正しました。
    (UUM-148663)

- `WebGL`: シェーダーがキューブテクスチャを期待しているにもかかわらず、テクスチャが明示的にバインドされていなかった場合のエラーを修正しました。
    ([UUM-150746](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150746))

- `XR`: XRプラットフォームにおいて、特にDeferredまたはForward+レンダリングパスで動的解像度を使用している際に発生する可能性のある、ブロック状またはずれたライティングアーティファクトを修正しました。
    (UUM-143709)

- `XR`: 深度テクスチャの送信が有効になっている状態で、実行時に MSAA レベルを変更した際に、XR グラフィックスがフリーズしてしまう問題を修正しました。




## 6000.0.84f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.addressables`: [2.9.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.9//changelog/CHANGELOG.html) から [2.10.3](https://docs.unity3d.com/Packages/com.unity.addressables@2.10//changelog/CHANGELOG.html) へ

- `com.unity.inputsystem`: [1.19.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.19//changelog/CHANGELOG.html) から [1.20.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.20//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: [2.6.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html) から [2.6.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html) へ

- `com.unity.terrain-tools`: [5.3.2](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html) から [5.3.3](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html) へ