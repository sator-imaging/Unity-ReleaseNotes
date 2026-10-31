# Unity 6000.3.27f2 LTS
公開日時：2026年10月30日（金）16:57:42 GMT  
https://unity.com/releases/editor/whats-new/6000.3.27f2

# 6000.3.27f2 の既知の問題

- `Android`: 「バックグラウンドで実行」と「予測バック機能のサポート」が有効になっている場合、バックグラウンドから復帰した後に「戻る」ジェスチャーまたはボタンを押すとアプリが終了してしまう
    ([UUM-159613](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159613))

- `オーディオオーサリング`: USBオーディオ出力デバイスが切断された後に再接続され、メインスレッドが再開されると、複数のスタックトレースを伴うクラッシュが発生する
    ([UUM-158166](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158166))

- `エディタインストーラ`: [macOS] プレーヤライブラリが、特注の権限でコード署名されている
    ([UUM-156884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156884))

- `ネイティブエディタアプリケーションのライフサイクル`: [WinEditor] ポーリングレートが高い状態でマウスカーソルを動かすと、再生モードのフレームレートが大幅に低下する
    ([UUM-142550](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142550))

- `スクリプティングのビルド時`: `bee_backend`が複数実行されている際に、`mono_log_write_logfile`の呼び出しでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

- `シェーダーシステム`: SceneManager.LoadSceneAsync を使用してシーンを繰り返し切り替えると、プレイヤーが永久に応答しなくなる
    ([UUM-156125](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156125))

- `SRP Foundation`: デバイスを物理的に回転させた際、LogcatおよびコンソールにRenderPass関連のAndroidエラーが記録される
    ([UUM-157974](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157974))



# 6000.3.27f2 リリースノート

## 改善点

- `アセットのインポート`: バンドルされている Autodesk FBX SDK を 2020.3.11 に更新し、FBX ファイルの解析における 2 つのバッファオーバーフローの脆弱性に対処することで、モデルインポートのセキュリティを向上させました。
    (UUM-155199)



## APIの変更

- `Graphics`: 追加: Graphics.disableDepthAndStencilBuffers を追加しました。これは、Player Settings で「深度およびステンシルバッファを無効にする」が有効になっているかどうかを返す読み取り専用プロパティです。



## 変更点

- `Physics 2D`: 「PhysicsComposer.AddLayer」、「PhysicsComposer.ToPolygons"、"CircleGeometry.ToPolygons"、および "CapsuleGeometry.ToPolygons" は、ジオメトリが指定されていない場合、頂点が3つ未満の場合、または無効な "curveStride" が指定された場合に、以前は "ArgumentOutOfRangeException" をスローしていましたが、これらは標準の検証警告をログに出力するようになりました。
    ([UUM-156367](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156367))



## 修正点

- `2D`: 2D レンダラーでオーバーレイカメラを使用する際の ArgumentException を修正しました。
    ([UUM-148111](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148111))

- `2D`: レンダーパスから要求された際、中間テクスチャが作成されない問題を修正しました。
    ([UUM-145892](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145892))

- `2D`: URP 2D エディタ専用のアイコンがプレイヤービルドに含まれてしまう問題を修正しました。
    (UUM-144935)

- `2D`: ゲームオブジェクトの有効化を切り替えた際に、LineRenderer が正しく初期化されない問題を修正しました。
    ([UUM-147747](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147747))

- `Android`: UaaL モードで unload 直後に GameActivity を再起動した際に発生するフリーズを修正しました。
    (UUM-149857)

- `Animation`: null の clip または referenceClip を引数として `AnimationUtility.SetAdditiveReferencePose` を呼び出した際に発生するクラッシュを修正しました。
    ([UUM-150816](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150816))

- `アセットパイプライン`: ディレクトリ監視が変更されたファイルに関する期待通りの通知を受け取らない場合、起動時にフリーズする問題を修正しました。
    ([UUM-149019](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149019))

- `Audio`: macOS において、システムがマイクを使用している際にオーディオの再生速度が低下する不具合を修正しました
    ([UUM-149880](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149880))

- `Audio`: 再生モード中にUnity Audioのオン/オフを切り替えた際に、クリップが読み込まれていたAudioSourceを再生した後、再生モードを終了する際に記録されていたアサーション \(m_ModifiedClips.empty\(\)\) を修正しました。
    ([UUM-148749](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148749))

- `Core`: `EnabledWithStackTrace` から `Enabled` に切り替えた後の最初のドメイン再読み込み時に、リーク検出が誤ったリークを報告する問題を修正しました。
    ([UUM-108870](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-108870))

- `DX12`: Direct3D12 グラフィックス API を使用する際、GPU バッファの解放時に発生する「use-after-free」が原因で、Windows 上でランダムにクラッシュする問題を修正しました。
    ([UUM-150682](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150682))

- `エディタ`: AssetBundles または Entities コンテンツアーカイブをアンロードする際の TMP_FontAsset のメモリリークを修正しました
    (UUM-145538)

- `エディタ`: ドメインのリロード中にメニュー項目を再構築する際の再入可能性（reentrancy）が原因で発生していた、Linux 限定のエディタのクラッシュを修正しました。
    (UUM-149839)

- `エディタ`: 未保存の変更があるウィンドウが開いている状態で、保存済みのエディタレイアウトに切り替えようとすると、レイアウトの変更をキャンセルできなくなるバグを修正しました。
    ([UUM-150448](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150448))

- `エディタ`: UITKの「標準テキスト」における同時アクセスに関する問題を修正しました
    ([UUM-151887](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151887))

- `エディタ`: 「高度なテキスト」で、同じ文字列内に複数のスクリプトが使用される問題を修正しました。
    ([UUM-150208](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150208))

- `GI`: レイトレーシングのアクセラレーション構造体に追加された地形が、メッシュとそのGPUバッファをリークしなくなりました。
    (UUM-151903)

- `Graphics`: コンピュートシェーダーが、グラフィックスパイプラインがサポートする範囲を超えるスレッドグループを要求した場合（例：一部の Intel GPU での「High Quality Line Rendering」）、Metal 上で GPU がハングする問題を修正しました。
    (UUM-147457)

- `Graphics`: シングルパス XR をメモリレステクスチャ配列にレンダリングする際、Metal 上でエディタが「Metal: メモリレステクスチャには 2D テクスチャが必要です。」というアサートを出力していた問題を修正しました。
    (UUM-154442)

- `Graphics`: Graphicsジョブが有効な状態で、MeshTopology.Quadsを使用した場合にGraphics.RenderPrimitivesおよびGraphics.DrawProceduralがクラッシュする問題を修正しました。
    ([UUM-141117](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141117))

- `HDRP`: MSAA および雲レイヤーが有効な場合、空を背景にしたジオメトリの周囲に暗い輪郭線が表示される問題を修正しました。
    ([UUM-150911](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150911))

- `IL2CPP`: `Thread.VolatileWrite(ref object, object)` における GC 書き込みバリアの欠落を修正しました。
    (UUM-155582)

- `IL2CPP`: System.IO.Compression.BrotliStream および BrotliDecoder で、信頼できないデータのデコードによりリモートコード実行が可能となる可能性があったセキュリティ上の脆弱性 \(CVE-2026-111497\) を修正しました。

- `IL2CPP`: スレッドオブジェクトのメモリが、スレッドの終了後も GC によって保持され続ける問題を修正しました
    ([UUM-149541](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149541))

- `IL2CPP`: ref構造体型の静的フィールドおよびThreadStaticフィールドにおいて、増分GCの書き込みバリアが欠落していた問題を修正しました。
    ([UUM-153622](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153622))

- `Input System`: WindowsのXbox Game BarおよびmacOSのオーバーレイ（Spotlightなど）の不具合を修正しました。 Windows では、Steam/Discord/NVIDIA のオーバーレイは従来通り動作します。
    ([UUM-150045](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150045))

- `iOS`: Unityの初期化前に `application:openURL` または `application:continueUserActivity` が呼び出された際に発生していたクラッシュを修正しました。
    ([UUM-151801](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151801))

- `Kernel`: 32 ビット整数のオーバーフローによって引き起こされていた NativeSlice でのクラッシュを修正しました。
    (UUM-154594)

- `macOS`: 最新の macOS バージョンで、X.509 証明書をインポートする際に発生する可能性があったクラッシュを修正しました。
    (UUM-154511)

- `macOS`: macOS 上で、バッチモードや自動テストの実行中に、ウィンドウのいずれかがフォーカスを失った際にエディタの動作が遅くなる問題を修正しました。

- `Mono`: System.IO.Compression.BrotliStream および BrotliDecoder で使用される Brotli デコーダーに存在したセキュリティ脆弱性 \(CVE-2026-111497\) を修正しました。この脆弱性により、信頼できないデータをデコードした際に、リモートでコードが実行される可能性がありました。

- `Mono`: デフォルトの GCHandle を使用する際のクラッシュを解消しました
    ([UUM-153835](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153835))

- `Multiplayer`: Vulkan グラフィックス API を使用する際、追加のエディタインスタンスを含むプレイモードシナリオが「デプロイ中」の状態から抜け出せなくなる問題を修正しました。
    ([UUM-154645](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154645))

- `Networking`: 改ざんされた eMudhra 証明書を使用しているサーバーへの TLS 接続を拒否するようにしました。
    (UUM-158231)

- `Networking`: Unity Transport: TLS/DTLS セッションの作成時に発生していた軽微なメモリリークを修正しました。
    ([UUM-151755](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151755))

- `パッケージマネージャー`: パッケージマネージャーで使用される Node.js ランタイムを v24.22.1 に更新することで、リモートコード実行を可能にするセキュリティ脆弱性 \(CVE-2026-111497\) を修正しました。

- `Physics`: Rigidbody.mass が NaN 値を受け入れてしまい、その結果、ボディがすべてのコライダーを通り抜けてしまう問題を修正しました。
    ([UUM-154143](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154143))

- `Physics 2D`: 各種 Physics Core 2D メソッドにおいて、欠落していたパブリック引数の検証を追加しました。
    ([UUM-156367](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156367))

- `Physics 2D`: 「PhysicsChain.friction」、「PhysicsChain.bounciness」、「PhysicsChain.frictionMixing」、または「PhysicsChain.bouncinessMixing」を設定した後に発生する可能性があったクラッシュまたはメモリ破損を修正しました。

- `Profiler`: ロード処理の進行中にメモリプロファイラのスナップショットを取得した際、PreloadManager で発生していたデッドロックを修正しました。
    (UUM-143493)

- `Shadergraph`: キーワードノードと仮想テクスチャサンプリングの両方を使用しているグラフで発生していたレンダリングエラーを修正しました。
    (UUM-139845)

- `ソースコードのビルド`: トルコ語の地域形式を使用しているマシンで、エディタのソースコードのビルドが失敗する問題を修正しました。
    (UUM-154501)

- `Text`: TextMesh またはレガシー UI Text の文字列が、終了タグのない quad タグパラメータで終わっている場合に発生していた、メモリ範囲外読み取りの不具合を修正しました。
    (UUM-153129)

- `Text`: TextMesh またはレガシー UI Text の文字列が、終了タグのないリッチテキストタグで終わっている場合に発生する、メモリ範囲外読み取りの不具合を修正しました。
    (UUM-153128)

- `TextMeshPro`: 「入力フィールドでバリアント文字を使用している場合、TextMeshPro 入力フィールドの最初のバックスペース操作で文字が削除されない」という不具合を修正しました
    ([UUM-140383](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140383))

- `TextMeshPro`: 「Content Size Fitter」が設定された TextMeshPro テキストに、狭い幅でスペースに続くハイフンが含まれている場合にエディタがフリーズする問題を修正しました。
    ([UUM-152921](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152921))

- `uGUI`: RectMask2Dの「ソフトネス」が0の場合、クリップされたコンテンツのエッジがぼやけてしまう問題を修正しました
    ([UUM-150815](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150815))

- `UI Toolkit`: パネルのスケールが整数でない場合、ドロップシャドウなどのフィルターが適用された要素内のテキストやコンテンツがぼやけて表示される問題を修正しました。
    ([UUM-155009](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-155009))

- `UI Toolkit`: 水平方向にのみスクロール可能な ScrollView やリストビューにおいて、トラックパッドによる水平スクロールがほとんど動かない、または間違った方向へ動いてしまう問題を修正しました。
    (UUM-152573)

- `UI Toolkit`: macOS上で動作するWebビルドにおいて、複数列のリストビューやツリービューで、複数の列で並べ替える際にCmd+クリックではなくCtrl+クリックが必要だった問題を修正しました。

- `UI Toolkit`: macOS上で動作するWebビルドにおいて、ポインタ、マウス、キーボード、およびナビゲーションイベントのアクションキーがCmdではなくCtrlになっていた問題を修正しました。
    ([UUM-153940](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153940))

- `UI Toolkit`: ドッキングされたウィンドウを最大化・元に戻したり、デバッガーで UI Toolkit Live Reload を切り替えたりするなどして UI Toolkit デバッガーウィンドウが再作成された後、Dynamic Atlas Viewer にアトラスが表示されない問題を修正しました。
    ([UUM-150663](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150663))

- `UI Toolkit`: USSのtransition-timing-function宣言で、5pxなどキーワードではない値が使用された場合に、エディタやプレーヤーがフリーズする問題を修正しました。
    ([UUM-155159](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-155159))

- `UI Toolkit`: コンポーネントの異なるプレハブを切り替えた後、2つ目のインスペクタでプレハブを選択しても、「ゲームオブジェクトの選択」ウィンドウがそれを無視してしまう問題を修正しました。
    ([UUM-154149](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154149))

- `URP`: 互換モードが有効で、オーバーレイカメラがそのベースカメラとは異なるレンダラーを使用している場合、DX11で発生していた「CommandBuffer: 実行中に一時的なレンダリングテクスチャが見つかりませんでした」という警告を修正しました。
    ([UUM-117369](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-117369))

- `URP`: プレイヤー設定で「深度およびステンシルバッファを無効にする」が有効になっている場合、2D レンダラーがプレイヤーに深度バッファとステンシルバッファを作成してしまう問題を修正しました。
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

- `Web`: メモリプロファイラで使用される WASM_SIZE および wasmFileSize を修正しました
    (UUM-149075)

- `WebGL`: WebGPU: ユニフォームバッファおよび動的頂点バッファのメモリ使用量を改善
    (UUM-152972)




## 6000.3.27f2 におけるパッケージの変更点