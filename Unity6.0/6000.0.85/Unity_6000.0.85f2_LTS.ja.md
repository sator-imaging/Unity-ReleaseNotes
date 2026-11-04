# Unity 6000.0.85f2 LTS
公開日時：2026年11月3日（火）16:15:34 GMT  
https://unity.com/releases/editor/whats-new/6000.0.85f2

# 6000.0.85f2 の既知の問題

- `Android`: 「バックグラウンドで実行」および「予測バック機能のサポート」が有効になっている場合、バックグラウンドから復帰した後に「戻る」ジェスチャーまたはボタンを押すとアプリが終了してしまう
    ([UUM-159613](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159613))

- `DirectX12`: [RenderGraph][D3D12] EnableAsyncCompute(true) および UseTexture を指定して AddComputePass を使用した場合、D3D12SwapChain::Present でクラッシュする
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `エディターインストーラー`: [macOS] プレイヤーライブラリは、特注の権限でコード署名されています
    ([UUM-156884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156884))

- `スクリプティングのビルド時`: `bee_backend`が複数実行されている際に、`mono_log_write_logfile`の呼び出しでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

- `シェーダーシステム`: SceneManager.LoadSceneAsync を使用してシーンを繰り返し切り替えると、プレイヤーが永久に応答しなくなる
    ([UUM-156125](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156125))



# 6000.0.85f2 リリースノート

## 改善点

- `ビルドシステム`: 同梱の 7-Zip をバージョン 26.03 に更新しました。



## APIの変更

- `Graphics`: 追加: Graphics.disableDepthAndStencilBuffers を追加しました。これは、Player Settings で「深度およびステンシルバッファを無効にする」が有効になっているかどうかを返す読み取り専用プロパティです。



## 変更点

- `Android`: Android Gradle Plugin (AGP) のバージョンを 9.0.0 から 9.1.1 に更新しました。



## 修正

- `2D`: 2Dレンダラーでオーバーレイカメラを使用する際のArgumentExceptionを修正しました。
    ([UUM-148111](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148111))

- `2D`: スプライトエディタウィンドウの変更中に高速再生モードに入ると表示されるエラーメッセージを修正しました。
    ([UUM-146790](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146790))

- `2D`: レンダリングパスで要求された際、中間テクスチャが生成されない問題を修正しました。
    ([UUM-145892](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145892))

- `2D`: ゲームオブジェクトの有効/無効を切り替えた際に、LineRendererが正しく初期化されない問題を修正しました。
    ([UUM-147747](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147747))

- `2D`: 2D Rendererの「Render Scale」設定によって、カメラのソートレイヤーのテクスチャ解像度が影響を受けていた問題を修正しました。
    ([UUM-151723](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151723))

- `Android`: ターゲットAPIレベル37が選択された際に発生していた「ハッシュ文字列 android-37 のターゲットが見つかりませんでした」というエラーを修正しました。
    ([UUM-150216](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150216))

- `Android`: 入力中にカーソルがテキストの末尾に戻ってしまう問題を修正しました。
    ([UUM-121294](https://issuetracker.unity3d.com/issues/android-ios-the-input-field-caret-moves-back-to-the-end-of-the-text-when-typing))

- `Android`: 仮想キーボードとUGUIテキストフィールド間の双方向同期に関する問題を修正しました。
    (UUM-133870)

- `Android`: `editText`の`setText`呼び出しにより、`EditText`の選択範囲に関係なく、IMEの内部カーソルがテキストの末尾にリセットされる問題を修正しました。
    (UUM-142513)

- `Android`: UaaL モードで unload 直後に GameActivity を再起動した際にフリーズする問題を修正しました。
    (UUM-149857)

- `Android`: `TouchScreenKeyboard.selection.length` が常に `0` を返す問題を修正しました。
    ([UUM-125821](https://issuetracker.unity3d.com/issues/android-touchscreenkeyboard-dot-selection-dot-length-always-returns-0-when-any-length-text-is-selected))

- `アセットバンドル`: 別のアセットバンドル内のプレハブの子オブジェクトへの参照を経由してアクセスしたアセットバンドルからプレハブをインスタンス化した際に、プレイヤーがクラッシュする問題を修正しました。
    (UUM-141605)

- `オーディオ`: macOS において、システムがマイクを使用している際にオーディオの再生速度が低下する不具合を修正しました。
    ([UUM-149880](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149880))

- `エディタ`: Linux版エディタで、「ヘルプ」および「ウィンドウ」メニューがメインメニューバーの末尾に配置されていなかったバグを修正しました。
    (UUM-113169)

- `エディタ`: Direct3D12 上で非同期シェーダーコンパイルがまだ進行中の状態でプレイモードを終了した際に発生していたデッドロックを修正しました。
    ([UUM-152966](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152966))

- `エディタ`: オーバーレイのコンテナの `rootVisualElement` にアクセスすると、再帰的な呼び出しが発生し、エディタがクラッシュする問題を修正しました。
    ([UUM-149209](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149209))

- `エディタ`: 「シーンが変更されました」ダイアログが表示されている状態で Cmd+Q を複数回押すとエディタがクラッシュする問題を修正しました。<br>
    未保存の変更がある状態でプレイモードのエディタを終了した際に、「シーンが変更されました」ダイアログが 2 回表示される問題を修正しました。 変更されました」ダイアログが2つ表示される問題を修正しました。
    ([UUM-149668](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149668))

- `Graphics`: Graphicsジョブが有効な状態で、MeshTopology.Quadsを使用するとGraphics.RenderPrimitivesおよびGraphics.DrawProceduralがクラッシュする問題を修正しました。
    ([UUM-141117](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141117))

- `IL2CPP`: `System.IO.Compression.BrotliStream` および `BrotliDecoder` で使用される Brotli デコーダーに存在したセキュリティ脆弱性 \(CVE-2026-111497\) を修正しました。この脆弱性により、信頼できないデータをデコードした際に、リモートでコードが実行される可能性がありました。

- `macOS`: 最近の macOS バージョンにおいて、X.509 証明書をインポートする際に発生する可能性があったクラッシュを修正しました。
    (UUM-154511)

- `Mono`: System.IO.Compression.BrotliStream および BrotliDecoder で使用される Brotli デコーダーに存在したセキュリティ脆弱性 \(CVE-2026-111497\) を修正しました。この脆弱性により、信頼できないデータをデコードした際に、リモートでコードが実行される可能性がありました。

- `マルチプレイヤー`: Unity Transport: DTLS または TLS を使用して接続を閉じる際のメモリリークを修正しました。
    ([UUM-151755](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151755))

- `Networking`: 同一ホストへの高速な同時リクエストによって新しいクッキーが設定された後、低速なリクエストが完了した際に、UnityWebRequestのクッキーが時折古い値に戻ってしまう問題を修正しました。
    ([UUM-150958](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150958))

- `ネットワーク`: 改ざんされた eMudhra 証明書を使用しているサーバーへの TLS 接続を拒否するようにしました。
    (UUM-158231)

- `ネットワーク`: UnityWebRequest: 進行中のリクエストが、応答しない、または応答が遅い DNS サーバーに対して DNS 解決を行っている最中に、スタンドアロン プレイヤーを終了するとフリーズする問題を修正しました。
    ([UUM-151643](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151643))

- `パッケージマネージャー`: パッケージマネージャーで使用されている Node.js ランタイムを v22.23.4 に更新することで、リモートコード実行を可能にするセキュリティ脆弱性 \(CVE-2026-111497\) を修正しました。

- `Particles`: 一部のデバイスにおいて、「カメラフェードオフ」と「ソフトパーティクルオン」を組み合わせた際にパーティクルが消えてしまう問題を修正しました。
    ([UUM-146249](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146249))

- `Player`: 開発用プレイヤービルドでデバッグアサートが発生するのを防ぐためのガードを追加しました。
    (UUM-152365)

- `Player`: 実行時に Shader.globalMaximumLOD を変更した後、GameObject が正しい影を落とすようになりました。
    ([UUM-150226](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150226))

- `Profiler`: プロファイラーの「接続の問題のトラブルシューティング」ボタンが、接続のトラブルシューティングとは無関係なドキュメントページにリンクしていた問題を修正しました。
    ([UUM-153354](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153354))

- `Shaders`: シェーダーのグローバルプロパティ API に範囲外の値が渡されたことにより発生していたクラッシュを修正しました。
    ([UUM-150856](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150856))

- `ソースコードのビルド`: トルコ語の地域形式を使用しているマシンで、エディタのソースコードのビルドが失敗する問題を修正しました。
    (UUM-154501)

- `Terrain`: ハイトマップの解像度がデバイスの最大レンダリングテクスチャサイズを超える地形（例：4096に制限されているデバイスでの4097のハイトマップ）を読み込んだ際に発生するクラッシュを修正しました。
    ([UUM-150551](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150551))

- `Text`: TextMesh またはレガシー UI Text の文字列が、終了タグのない quad タグパラメータで終わっている場合に発生していた、メモリ範囲外読み取りの不具合を修正しました。
    (UUM-153129)

- `Text`: TextMesh またはレガシー UI Text の文字列が、終了タグのないリッチテキストタグで終わっている場合に発生する、メモリ範囲外読み取りの不具合を修正しました。
    (UUM-153128)

- `UI Toolkit`: macOS上で実行されるWebビルドにおいて、複数列のリストおよびツリービューで、複数列による並べ替えを行う際にCmd+クリックではなくCtrl+クリックが必要となっていた問題を修正しました。

- `UI Toolkit`: macOS上で実行されるWebビルドにおいて、ポインタ、マウス、キーボード、およびナビゲーションイベントのアクションキーがCmdではなくCtrlとなっていた問題を修正しました。
    ([UUM-153940](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153940))

- `URP`: シーンを再読み込みすると、特定の `Blitter` 関数が動作しなくなるバグを修正しました。
    (UUM-153092)

- `URP`: 半精度 \(mobile\) のプラットフォームで、ボックス投影リフレクションプローブに継ぎ目が現れるバグを修正しました。
    ([UUM-141981](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141981))

- `URP`: RenderTextureの不具合を修正しました。Createが失敗するバグを修正しました。
    ([UUM-91313](https://issuetracker.unity3d.com/issues/android-vulkan-error-rendertexture-dot-create-failed-format-unsupported-for-random-writes-r16-sfloat-45-dot-logged-when-during-launch-on-an-project-with-urp-2d-renderer))

- `URP`: UV4入力のセマンティックの違いによるシェーダーグラフのコンパイル失敗を修正しました。
    ([UUM-143884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143884))

- `URP`: 「プレイヤー設定」で「深度およびステンシルバッファを無効にする」が有効になっている場合、2D レンダラーがプレイヤーに深度バッファとステンシルバッファを作成してしまう問題を修正しました。
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

- `URP`: `ScriptableRendererData.TryGetRendererFeature` が `NullReferenceException` をスローしていた問題を修正しました。
    ([UUM-150772](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150772))

- `VFX Graph`: 特定のボクセル数で `MeshToSDFBaker` を使用する際に発生していた範囲外アクセスが修正されました。
    ([UUM-151674](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151674))

- `Web`: メモリプロファイラで使用される `WASM_SIZE` および `wasmFileSize` を修正しました。
    (UUM-149075)

- `Web`: 出力アセットのサイズが 2 GB を超える場合の Web プラットフォームのビルド、および出力アセットのサイズが 4 GB を超える場合のビルドエラーメッセージ（\(未対応\)）を修正しました。
    ([UUM-112909](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-112909))




## 6000.0.85f2 におけるパッケージの変更点