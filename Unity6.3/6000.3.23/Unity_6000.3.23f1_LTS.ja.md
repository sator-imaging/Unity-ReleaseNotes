# Unity 6000.3.23f1 LTS
公開日時：2026年8月26日（水）14:35:12 GMT  
https://unity.com/releases/editor/whats-new/6000.3.23f1

# 6000.3.23f1 の既知の問題

- `2021.3.34f1`: 再生モードで音量を変更すると、オーディオミキサーからクリック音がする
    ([UUM-150250](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150250))

- `6000.6.0a3,6000.5.0b8,6000.3.16f1`: D3D12において、ShaderWarmup.WarmupShaderFromCollection() の直後にシェーダーをアンロードすると、use-after-free によりプレーヤーがクラッシュする
    ([UUM-149781](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149781))

- テキスト (TextMeshPro): TMPro Font Asset Creator でマルチスレッドのフォントアトラスを生成する際、UNITY_FT_Load_Glyph の処理中にクラッシュする
 ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

bee_backend が複数実行されている場合に mono_log_write_logfile でクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

Font Atlasの生成時に、複数のスタックトレースが発生してクラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.3.23f1 リリースノート

## 改善点

- `ドキュメント`: MonoBehaviour.OnValidate のスクリプトリファレンスにおいて、OnValidate によって設定された値がいつ保存され、いつメモリ上にのみ存在するのかを明確化しました。
    ([UUM-134473](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134473))



## 変更点

- `インストーラー`: Windows エディターのインストーラーに、`-CPULightmapper=no` コマンドラインスイッチを追加しました。これにより、CPU プログレッシブ・ライトマッパーのみが必要とするコンポーネント（現在はサポート終了済みの Microsoft Visual C++ 2010 ランタイム）のインストールをスキップできるようになりました。
    (UUM-149122)

- `Mono`: ToFileDescriptor からアサーションを削除しました
    ([UUM-145761](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145761))



## 修正

- `2D`: 3D エディタモードにおいて、SpriteSprite Generation としてインポートされたテクスチャがスプライトサブアセットを生成しないケースを修正しました。
    ([UUM-142920](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142920))

- `2D`: スプライトエディタウィンドウの変更中に高速再生モードに入ると表示されていたエラーメッセージを修正しました。
    ([UUM-146790](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146790))

- `アクセシビリティ`: Narrator（Windowsに組み込まれているスクリーンリーダー）で `AssistiveSupport.screenReaderStatusChanged` がサポートされていなかった問題を修正しました。
    ([UUM-147175](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147175))

- `AI`: サポートされていない設定の結果、NavMeshAgentが任意の方向にジャンプして、自身のNavMeshObstacleコンポーネントから離れようとしていました。現在、エージェントは安定した一方向へ移動するようになりました。
    (UUM-141803)

- `AI`: ボックス型の NavMeshObstacle 内に生成またはテレポートされた NavMeshAgent は、その障害物から移動できなくなっていました。
    ([UUM-146477](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146477))

- `Android`: Androidの「外部ツール」設定パネルにおける配置の問題を修正しました。
    (UUM-148378)

- `アセットパイプライン`: プレイモードに入った際に発生する可能性があった、`WriteObjectToVector` / `CreateOrReloadInspectorCopy` におけるエディタのクラッシュを修正しました。
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `ビルドパイプライン`: メモリ設定 \(メインアロケータ &gt; その他のアロケーター > リマッパーの初期容量\)で、PersistentManager.Remapperの容量を予約できるようになりました。
    (UUM-136275)

- `DX12`: Windows上でDirect3D12グラフィックスAPIを使用する際、小さなテクスチャが破棄された後も、そのテクスチャが使用していたVRAMがGPUドライバーに解放されない問題を修正しました。<br>
    `d3d12-small-texture-tiles-per-heap` ブート設定パラメータを使用して、小規模テクスチャのヒープサイズを調整できるようになり、VRAMの回収とヒープ割り当てのオーバーヘッドのバランスを調整できるようになりました。
    ([UUM-142284](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142284))

- `DX12`: 解像度切り替え時に、ダイナミックスケールレンダリングターゲットが共有配置ヒープを再エイリアシングしても、HDRPのハードウェア動的解像度機能による明るいピクセルのアーティファクトやD3D12検証エラー1422が発生しなくなりました。
    ([UUM-108671](https://issuetracker.unity3d.com/issues/visual-artifacts-appear-when-the-hd-dynamic-resolution-component-changes-the-resolution-scale))

- `エディタ`: 「ソースフォントファイル」が存在しないフォールバックを使用した場合に、ATG で発生していたクラッシュを修正しました。
    (UUM-148158)

- `エディタ`: `services-gateway` フォールバック URL のタイプミスを修正しました。これにより、リモート設定 CDN に接続できない場合、Hub 経由で起動されたエディタでサインインやクラウドサービスの利用に失敗する問題が解消されました。
    (UUM-149207)

- `Editor`: コピー操作中に存在しないアセットを削除しようとする問題を修正しました。
    ([UUM-144993](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144993))

- `Editor`: ビルド中にアクセラレータとの接続が切断された際に発生するクラッシュを修正しました。
    ([UUM-148391](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148391))

- `エディタ`: コンテキストモードで継承されたスタイルシートを表示する際、スタイルシートと所有するドキュメント名の間にスペースが入っていなかった問題を修正しました。
    ([UUM-147743](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147743))

- `エディタ`: 「トリミング」および「オフセット」を設定した動画をインポートまたはトランスコードした際に、Windows版エディタがクラッシュする問題を修正しました。
    ([UUM-146426](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146426))

- `エディタ`: Hubモードのサービス設定処理の内部的な堅牢化を行いました。ユーザーに目に見える動作の変更はありません。
    (UUM-149208)

- `Editor`: ScreenCapture.CaptureScreenshotAsTexture\(\) によるスクリーンキャプチャに枠が表示される。
    ([UUM-130878](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-130878))

- `エディタ`: URP および HDRP テンプレートで GRD を無効化しました。
    ([UUM-143179](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143179))

- `エディタ`: MPPM クローンがアクティブな状態でパッケージを更新すると、クローンがクラッシュする。
    (UUM-148292)

- `EmbeddedLinux`: システムに `wl_seat` が存在しない場合のクラッシュを修正しました。
    (UUM-148754)

- `GI`: 広大な地形を含むシーンで、ライティング可視化オーバーレイの「ライティングデータ」を「プレビュー」に切り替えた際に発生するクラッシュおよびパッキング時間の長さを修正しました。
    ([UUM-149471](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149471))

- `GI`: 複数のライトマッピングインスタンスに分割されるほど大規模な地形を含むシーンで、インタラクティブなライティングプレビューを使用する際のエディタのクラッシュを修正しました。
    (UUM-148850)

- `GI`: StreamingAssets内に配置されたシーンのライティングをベイクする際に発生していたクラッシュを修正しました。
    ([UUM-149240](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149240))

- `GI`: 有効なライトマップ UV を持たないオブジェクトが、警告「メッシュの UV レイアウト内のすべての三角形の面積がゼロです」とともに、ベイクされたライティングから削除される問題を修正しました。
    ([UUM-148666](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148666))

- `GI`: Microsoft Visual C++ 2010 ランタイムがインストールされていない場合に Windows エディタが起動しない問題を修正しました。代わりに、CPU プログレッシブ・ライトマッパーは利用不可であることを報告するようになりました。
    (UUM-149122)

- `Graphics`: `Resolution` および `RefreshRate` に `IEquatable<T>`、`GetHashCode`、および等価演算子を追加し、これらを比較したり辞書のキーとして使用したりする際のガベージコレクションによる割り当てを回避しました。
    (UUM-146197)

- `Graphics`: 「On Tile Post Processing」機能を、Universal Rendererでのみ利用可能にしました。
    ([UUM-148038](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148038))

- `Graphics`: GRD が有効な場合、staticShadowCaster への変更が正しく反映されるようになりました。
    ([UUM-140724](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140724))

- `Graphics`: 「Unityの『画面』サイズを最小化」という最適化設定でXRを使用する際、ミップマップレベルの計算が不正確になる問題を修正しました。<br>
    XRにおけるカメラ矩形は、SRPにおいてステレオの合計寸法ではなく、片目の寸法を正しく返すようになりました。これは、ミップマップストリーミングや解像度依存のUI/テキストレンダリングなど、解像度依存の計算にカメラ矩形を利用するすべてのシステムに影響します。必要に応じて、ミップマップストリーミングの設定やUIのスケーリングを調整してください。
    ([UUM-47681](https://issuetracker.unity3d.com/issues/calculated-mipmap-level-does-not-taking-xr-resolution-into-account))

- `Graphics`: グラフィック設定 - 「現在のシーンからインポート」アクションがアンドゥリストに追加されません。
    ([UUM-148881](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148881))

- `Graphics`: URP コアパッケージから unifiedraytracing アセットバンドルが削除されました。
    ([UUM-135643](https://issuetracker.unity3d.com/issues/newly-created-project-contains-a-unifiedraytracing-assetbundle-when-universal-or-high-definition-templates-are-used))

- `Input System`: Windows において、ベンダー定義のレポート数が大きい HID デバイス（例: `ReportCount=1024`）で使用される場合、重複した記述子要素が出力されることにより、デバイスの `capabilities` 文字列が極端に長くなるバグを修正しました。 これにより、記述子のサイズは適正になり、デバイスの実際の操作機能には影響がありません。
    (UUM-144506)

- `ライセンス`: 指名ユーザーライセンスファイルをインポートした際に、手動でのライセンス有効化に失敗する問題を修正しました。

- `Multiplayer`: GPU Resident Drawer が有効な状態で、クローンされたオブジェクトのレンダリングコンポーネントが Dedicated Server ロールによって削除された際に、エディタがクラッシュする問題を修正しました。
    ([UUM-147692](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147692))

- `Networking`: Webリクエストが突然切断された際に、無効なテクスチャポインタが参照される問題を修正しました。
    ([UUM-144540](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144540))

- `Networking`: 多くのドメイン再読み込みを伴う長時間のエディターセッションにおいて、UnityWebRequestでカスタム証明書ハンドラーを使用する際、エディターのみがクラッシュする可能性があった問題を修正しました。
    ([UUM-147347](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147347))

- `パッケージマネージャー`: 複数のアセットが選択されている場合、または選択されたアセットがUPMパッケージでない場合、「UPMパッケージをエクスポート」オプションを無効化しました。
    ([UUM-135090](https://issuetracker.unity3d.com/issues/multi-select-is-not-handled-correctly-when-exporting-packages-in-the-project-window))

- `Shadergraph`: カスタムノードの色を選択するためのカラーピッカーの不具合を修正しました。
    ([UUM-114854](https://issuetracker.unity3d.com/issues/could-not-invoke-color-picker-for-shadergraph-warning-is-thrown-when-changing-the-node-color-in-the-user-defined-color-mode))

- `SRP Core`: AMDUnityPluginが静的リンクされたCRTを使用するように修正しました。
    (UUM-147060)

- `uGUI`: インスペクター内の UGUI/TMP クラスに関するドキュメントリンクを修正しました。
    ([UUM-144450](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144450))

- `UI Toolkit`: 内部の描画範囲リストが部分的に埋まっている状態でさらに拡大した際、ワールド空間でのUIレンダリング中にArgumentExceptionが発生する問題を修正しました。
    (UUM-149611)

- `UI Toolkit`: ボタンが 8 つ以上存在する場合に発生していた ToggleButtonGroup の値のラップ問題を修正しました。
    ([UUM-149531](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149531))

- `UI Toolkit`: `Painter2D` および SVG のストロークにおいて、長さ 0 のダッシュパターンの指定時にレンダリングされずエラーが発生する問題を修正し、長さ 0 の丸みのあるダッシュをドットとしてレンダリングするようにしました。
    ([UUM-135766](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-135766))

- `バージョン管理`: アセットのインポート後に Perforce からファイルを取得する際、変更されていないファイルが変更リストに自動的に追加されてしまう問題を修正しました。
    ([UUM-49713](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-49713))




## 6000.3.23f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.2d.animation`: [13.0.5](https://docs.unity3d.com/Packages/com.unity.2d.animation@13.0//changelog/CHANGELOG.html) から [13.0.6](https://docs.unity3d.com/Packages/com.unity.2d.animation@13.0//changelog/CHANGELOG.html) へ

- `com.unity.2d.common`: [12.0.3](https://docs.unity3d.com/Packages/com.unity.2d.common@12.0//changelog/CHANGELOG.html) から [12.0.4](https://docs.unity3d.com/Packages/com.unity.2d.common@12.0//changelog/CHANGELOG.html) へ

- `com.unity.2d.tilemap.extras`: [6.0.2](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@6.0//changelog/CHANGELOG.html) から [6.0.3](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@6.0//changelog/CHANGELOG.html) へ

- `com.unity.2d.tooling`: [1.0.3](https://docs.unity3d.com/Packages/com.unity.2d.tooling@1.0//changelog/CHANGELOG.html) から [1.0.4](https://docs.unity3d.com/Packages/com.unity.2d.tooling@1.0//changelog/CHANGELOG.html) へ

- `com.unity.collab-proxy`: [2.12.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.12//changelog/CHANGELOG.html) から [2.13.6](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.13//changelog/CHANGELOG.html) へ

- `com.unity.services.authentication`: [3.7.3](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html) から [3.7.4](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html)

- `com.unity.timeline`: [1.8.12](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) から [1.8.13](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)

- `com.unity.xr.management`: [4.5.4](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html) から [4.6.1](https://docs.unity3d.com/Packages/com.unity.xr.management@4.6//changelog/CHANGELOG.html)