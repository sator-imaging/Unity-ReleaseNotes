# Unity 6000.0.85f1 LTS
公開日時：2026年10月15日（木）11:57:40 GMT  
https://unity.com/releases/editor/whats-new/6000.0.85f1

# 6000.0.85f1 の既知の問題

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true) および UseTexture を指定して AddComputePass を使用した場合、D3D12SwapChain::Present でクラッシュする
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.0.75f1`: SceneManager.LoadSceneAsync を使用してシーンを繰り返し切り替えると、プレイヤーが永久に応答しなくなる
    ([UUM-156125](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156125))

bee_backendが複数実行されている際にmono_log_write_logfileでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))



# 6000.0.85f1 リリースノート

## 改善点

- `ビルドシステム`: 同梱の 7-Zip をバージョン 26.03 に更新しました。



## APIの変更

- `Graphics`: 追加: Graphics.disableDepthAndStencilBuffers を追加しました。これは、Player Settings で「深度およびステンシルバッファを無効にする」が有効になっているかどうかを返す読み取り専用プロパティです。



## 変更点

- `Android`: Android Gradle Plugin (AGP) のバージョンを 9.0.0 から 9.1.1 に更新しました。



## 修正

- `2D`: 2D レンダラーでオーバーレイカメラを使用する際に発生していた ArgumentException を修正しました。
    ([UUM-148111](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148111))

- `2D`: スプライトエディタウィンドウの変更中に高速再生モードに入ると表示されるエラーメッセージを修正しました。
    ([UUM-146790](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146790))

- `2D`: レンダーパスで要求された際、中間テクスチャが生成されない問題を修正しました。
    ([UUM-145892](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145892))

- `2D`: ゲームオブジェクトの有効化を切り替えた際に、LineRenderer が正しく初期化されない問題を修正しました。
    ([UUM-147747](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147747))

- `2D`: 2D Renderer の「Render Scale」設定によって、カメラのソートレイヤーのテクスチャ解像度が影響を受けていた問題を修正しました。
    ([UUM-151723](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151723))

- `Android`: ターゲットAPIレベル37が選択された際に発生していた「ハッシュ文字列 android-37 を持つターゲットが見つかりませんでした」というエラーを修正しました。
    ([UUM-150216](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150216))

- `Android`: 入力中にカーソルがテキストの末尾に戻ってしまう問題を修正しました。
    ([UUM-121294](https://issuetracker.unity3d.com/issues/android-ios-the-input-field-caret-moves-back-to-the-end-of-the-text-when-typing))

- `Android`: 仮想キーボードとUGUIテキストフィールド間の双方向同期に関する問題を修正しました。
    (UUM-133870)

- `Android`: `editText`の`setText`呼び出しにより、`EditText`の選択範囲に関係なく、IMEの内部カーソルがテキストの末尾にリセットされる問題を修正しました。
    (UUM-142513)

- `Android`: UaaL モードで `GameActivity` をアンロード直後に再起動した際にフリーズする問題を修正しました。
    (UUM-149857)

- `Android`: `TouchScreenKeyboard.selection.length` が常に `0` を返す問題を修正しました。
    ([UUM-125821](https://issuetracker.unity3d.com/issues/android-touchscreenkeyboard-dot-selection-dot-length-always-returns-0-when-any-length-text-is-selected))

- `アセットバンドル`: 別のアセットバンドル内のプレハブの子オブジェクトへの参照を経由してアクセスしたアセットバンドルからプレハブをインスタンス化した際に、プレイヤーがクラッシュする問題を修正しました。
    (UUM-141605)

- `オーディオ`: macOS において、システムがマイクを使用している際にオーディオの再生速度が低下する不具合を修正しました。
    ([UUM-149880](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149880))

- `エディタ`: Linux版エディタで、「ヘルプ」および「ウィンドウ」メニューがメインメニューバーの末尾に配置されていなかった不具合を修正しました。
    (UUM-113169)

- `エディタ`: Direct3D12 上で非同期シェーダーコンパイルがまだ進行中の状態でプレイモードを終了した際に発生していたデッドロックを修正しました。
    ([UUM-152966](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152966))

- `エディタ`: オーバーレイのコンテナの `rootVisualElement` にアクセスすると、再帰的な呼び出しが発生し、エディタがクラッシュする問題を修正しました。
    ([UUM-149209](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149209))

- `エディタ`: 「シーンが変更されました」ダイアログが表示されている状態で Cmd+Q を複数回押すとエディタがクラッシュする問題を修正しました。<br>
    変更を保存せずにプレイモードでエディタを終了した際に、「シーンが変更されました」ダイアログが 2 つ表示される問題を修正しました。
    ([UUM-149668](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149668))

- `Graphics`: Graphicsジョブが有効な状態で、MeshTopology.Quadsを使用するとGraphics.RenderPrimitivesおよびGraphics.DrawProceduralがクラッシュする問題を修正しました。
    ([UUM-141117](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141117))

- `macOS`: 最新の macOS バージョンで、X.509 証明書をインポートする際に発生する可能性があったクラッシュを修正しました。
    (UUM-154511)

- `マルチプレイヤー`: Unity Transport: DTLS または TLS を使用して接続を閉じる際のメモリリークを修正しました。
    ([UUM-151755](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151755))

- `Networking`: 同一ホストへの高速な同時リクエストによって新しいクッキーが設定された後、低速なリクエストが完了した際に、UnityWebRequestのクッキーが時折古い値に戻ってしまう問題を修正しました。
    ([UUM-150958](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150958))

- `ネットワーク`: UnityWebRequest: 進行中のリクエストが、応答しない、または応答が遅い DNS サーバーに対して DNS 解決を行っている最中に、スタンドアロン プレイヤーを終了するとフリーズする問題を修正しました。
    ([UUM-151643](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151643))

- `パーティクル`: 「カメラフェードオフ」と「ソフトパーティクルオン」を組み合わせた際に、一部のデバイスでパーティクルが消えてしまう問題を修正しました。
    ([UUM-146249](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146249))

- `Player`: 開発用プレイヤービルドでデバッグアサートが発生するのを防ぐためのガードを追加しました。
    (UUM-152365)

- `Player`: 実行時に Shader.globalMaximumLOD が変更された後、GameObject が正しい影を落とすようになりました。
    ([UUM-150226](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150226))

- `Profiler`: Profiler の「接続の問題のトラブルシューティング」ボタンが、接続のトラブルシューティングとは無関係なドキュメントページにリンクしていた問題を修正しました。
    ([UUM-153354](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153354))

- `Shaders`: シェーダーのグローバルプロパティ API に範囲外の値が渡されたことにより発生していたクラッシュを修正しました。
    ([UUM-150856](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150856))

- `ソースコードのビルド`: トルコ語の地域形式を使用しているマシンで、エディタのソースコードのビルドが失敗する問題を修正しました。
    (UUM-154501)

- `Terrain`: ハイトマップの解像度がデバイスの最大レンダリングテクスチャサイズを超える地形（例：4096に制限されているデバイスで4097のハイトマップ）を読み込んだ際に発生するクラッシュを修正しました。
    ([UUM-150551](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150551))

- `Text`: TextMesh またはレガシー UI Text の文字列が、終了タグのない quad タグパラメータで終わっている場合に発生していた、メモリ範囲外読み取りの不具合を修正しました。
    (UUM-153129)

- `Text`: TextMesh またはレガシー UI Text の文字列が、終了タグのないリッチテキストタグで終わっている場合に発生する、メモリ範囲外読み取りの不具合を修正しました。
    (UUM-153128)

- `UI Toolkit`: macOS上で実行されるWebビルドにおいて、複数列のリストおよびツリービューで、複数の列で並べ替える際にCmd+クリックではなくCtrl+クリックが必要になる問題を修正しました。

- `UI Toolkit`: macOS上で実行されるWebビルドにおいて、ポインタ、マウス、キーボード、およびナビゲーションイベントのアクションキーがCmdではなくCtrlになっていた問題を修正しました。
    ([UUM-153940](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153940))

- `Universal Windows Platform`: Xbox において、画面上のキーボードを確認すると、入力したテキストが保持されず、テキストフィールドがクリアされてしまう問題を修正しました。
    (UUM-154127)

- `Universal Windows Platform`: Xbox において、B ボタンを押して画面キーボードを閉じると、以前の値に戻る代わりに、入力したテキストが残ってしまう問題を修正しました。
    (UUM-149423)

- `URP`: シーンをリロードすると、特定の `Blitter` 関数が動作しなくなるバグを修正しました。
    (UUM-153092)

- `URP`: 半精度 \(mobile\) のプラットフォームで、ボックス投影反射プローブに継ぎ目が現れるバグを修正しました。
    ([UUM-141981](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141981))

- `URP`: 特定の Android Vulkan デバイスで `RenderTexture.Create` が失敗する問題を修正しました。
    ([UUM-91313](https://issuetracker.unity3d.com/issues/android-vulkan-error-rendertexture-dot-create-failed-format-unsupported-for-random-writes-r16-sfloat-45-dot-logged-when-during-launch-on-an-project-with-urp-2d-renderer))

- `URP`: UV4 入力のセマンティックの違いによる ShaderGraph のコンパイル失敗を修正しました。
    ([UUM-143884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143884))

- `URP`: 「プレイヤー設定」で「深度およびステンシルバッファを無効にする」が有効になっている場合、2D レンダラーがプレイヤーに深度バッファとステンシルバッファを作成してしまう問題を修正しました。
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

- `URP`: `ScriptableRendererData.TryGetRendererFeature` が `NullReferenceException` をスローしていた問題を修正しました。
    ([UUM-150772](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150772))

- `VFX Graph`: 特定のボクセル数で `MeshToSDFBaker` を使用する際に発生していた範囲外アクセスが修正されました。
    ([UUM-151674](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151674))

- `Web`: メモリプロファイラで使用される `WASM_SIZE` および `wasmFileSize` を修正しました。
    (UUM-149075)

- `Web`: 出力アセットのサイズが 2 GB を超える場合の Web プラットフォームのビルド、および出力アセットのサイズが 4 GB を超える場合（非対応）のビルドエラーメッセージを修正しました。
    ([UUM-112909](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-112909))




## 6000.0.85f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.collections`: [2.6.8](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) から [2.7.1](https://docs.unity3d.com/Packages/com.unity.collections@2.7//changelog/CHANGELOG.html) へ

- `com.unity.entities`: [1.4.8](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) から [1.5.0](https://docs.unity3d.com/Packages/com.unity.entities@1.5//changelog/CHANGELOG.html) へ

- `com.unity.netcode`: [1.14.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html) から [1.14.3](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html)

- `com.unity.physics`: [1.4.7](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) から [1.5.0](https://docs.unity3d.com/Packages/com.unity.physics@1.5//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: [1.4.21](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) から [1.5.0](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.5//changelog/CHANGELOG.html) へ

- `com.unity.mobile.notifications`: [2.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html) から [2.5.0](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.5//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: [3.7.4](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html) から [3.8.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.8//changelog/CHANGELOG.html) へ

- `com.unity.services.friends`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.1//changelog/CHANGELOG.html) から [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.3//changelog/CHANGELOG.html) へ

- `com.unity.services.wire`: [1.5.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.5//changelog/CHANGELOG.html) から [1.6.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.6//changelog/CHANGELOG.html) へ

- `com.unity.splines`: [2.8.4](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html) から [2.9.1](https://docs.unity3d.com/Packages/com.unity.splines@2.9//changelog/CHANGELOG.html) へ

- `com.unity.xr.management`: [4.5.4](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html) から [4.6.1](https://docs.unity3d.com/Packages/com.unity.xr.management@4.6//changelog/CHANGELOG.html) へ

- `com.unity.profiling.systemmetrics.mali`: [1.1.1](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) から [1.1.4](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) へ

- `com.unity.multiplayer.tools`: [2.2.10](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) から [2.2.12](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) へ

- `com.unity.ai.navigation`: [2.0.14](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) から [2.0.15](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) へ

- `com.unity.asset-manager-for-unity`: [1.11.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.11//changelog/CHANGELOG.html) から [1.12.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.12//changelog/CHANGELOG.html) へ

- `com.unity.cloud.draco`: [5.4.3](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html) から [5.5.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.5//changelog/CHANGELOG.html)

- `com.unity.cloud.ktx`: [3.6.3](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html) から [3.7.1](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.7//changelog/CHANGELOG.html)

- `com.unity.xr.compositionlayers`: [2.5.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.5//changelog/CHANGELOG.html) から [2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.6//changelog/CHANGELOG.html) へ