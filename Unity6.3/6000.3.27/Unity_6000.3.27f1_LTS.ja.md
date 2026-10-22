# Unity 6000.3.27f1 LTS
公開日時: 2026年10月20日(火) 13:42:16 GMT  
https://unity.com/releases/editor/whats-new/6000.3.27f1

# 6000.3.27f1 の既知の問題

- `コンテンツのビルド`: SceneManager.LoadSceneAsync を使用してシーンを繰り返し切り替えると、プレイヤーが永久に応答しなくなる
    ([UUM-156125](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156125))

- `エディタインストーラ`: [macOS] プレイヤーライブラリが、特注の権限でコード署名されている
    ([UUM-156884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156884))

- `ネイティブエディタアプリケーションのライフサイクル`: [WinEditor] ポーリングレートが高い状態でマウスカーソルを動かすと、再生モードのフレームレートが大幅に低下する
    ([UUM-142550](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142550))

- `スクリプティングのビルド時間`: `bee_backend`が複数実行されている際に、`mono_log_write_logfile`の呼び出しでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

- `SRP Foundation`: デバイスを物理的に回転させた際、RenderPass に関連する Android エラーが Logcat およびコンソールに記録される
    ([UUM-157974](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157974))



# 6000.3.27f1 リリースノート

## 改善点

- `アセットのインポート`: バンドルされている Autodesk FBX SDK を 2020.3.11 に更新し、FBX ファイルの解析における 2 つのバッファオーバーフローの脆弱性に対処することで、モデルインポートのセキュリティを強化しました。
    (UUM-155199)



## API の変更

- `Graphics`: 追加: `Graphics.disableDepthAndStencilBuffers` を追加しました。これは、Player Settings で「深度およびステンシルバッファを無効にする」が有効になっているかどうかを返す読み取り専用プロパティです。



## 変更点

- `Physics 2D`: 「PhysicsComposer.AddLayer」、 「PhysicsComposer.ToPolygons」、「CircleGeometry.ToPolygons」、および「CapsuleGeometry.ToPolygons」は、ジオメトリが指定されていない場合、頂点が3つ未満の場合、または無効な「curveStride」が指定された場合に、「ArgumentOutOfRangeException」をスローする代わりに、標準の検証警告をログに出力するようになりました。
    ([UUM-156367](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156367))



## 修正点

- `2D`: 2D レンダラーでオーバーレイカメラを使用する際の ArgumentException を修正しました。
    ([UUM-148111](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148111))

- `2D`: レンダーパスで要求された際、中間テクスチャが作成されない問題を修正しました。
    ([UUM-145892](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145892))

- `2D`: URP 2D エディタ専用のアイコンがプレイヤービルドに含まれてしまう問題を修正しました。
    (UUM-144935)

- `2D`: ゲームオブジェクトの有効化を切り替えた際に、LineRenderer が正しく初期化されない問題を修正しました。
    ([UUM-147747](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147747))

- `Android`: UaaL モードで GameActivity をアンロードした直後に再起動するとフリーズする問題を修正しました。
    (UUM-149857)

- `Animation`: null の clip または referenceClip を引数として AnimationUtility.SetAdditiveReferencePose` を呼び出した際にクラッシュする問題を修正しました。
    ([UUM-150816](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150816))

- `アセットパイプライン`: ディレクトリ監視が変更されたファイルに関する期待通りの通知を受け取れない場合、起動時にフリーズする問題を修正しました。
    ([UUM-149019](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149019))

- `Audio`: macOS において、システムがマイクを使用している際にオーディオの再生速度が低下する不具合を修正しました
    ([UUM-149880](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149880))

- `Audio`: プレイモード終了時に、Unity Audioがオフからオンに切り替わる間にクリップが読み込まれたAudioSourceを再生した後、ログに記録されていたアサーション \(m_ModifiedClips.empty\(\)\) が記録される問題を修正しました。この問題は、再生モード中にUnity Audioのオン/オフを切り替えた際に、クリップが読み込まれたAudioSourceを再生した後、再生モードを終了する際に発生していました。
    ([UUM-148749](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148749))

- `Core`: `EnabledWithStackTrace` から `Enabled` に切り替えた後の最初のドメイン再読み込み時に、リーク検出が誤ったリークを報告する問題を修正しました。
    ([UUM-108870](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-108870))

- `DX12`: Direct3D12 グラフィックス API を使用する際、GPU バッファの解放時に発生する「use-after-free」が原因で、Windows 上でランダムにクラッシュする問題を修正しました。
    ([UUM-150682](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150682))

- `エディタ`: AssetBundles または Entities のコンテンツアーカイブをアンロードする際の TMP_FontAsset のメモリリークを修正しました
    (UUM-145538)

- `エディタ`: ドメインのリロード中にメニュー項目を再構築する際の再入可能性（reentrancy）が原因で発生していた、Linux 限定のエディタのクラッシュを修正しました。
    (UUM-149839)

- `エディタ`: 未保存の変更があるウィンドウが開いている状態で、保存済みのエディタレイアウトに切り替えようとすると、レイアウトの変更をキャンセルできなくなるバグを修正しました。
    ([UUM-150448](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150448))

- `エディタ`: UITKの「標準テキスト」における同時アクセスに関する問題を修正しました。
    ([UUM-151887](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151887))

- `エディタ`: 「高度なテキスト」で、同じ文字列内で複数のスクリプトが使用される問題を修正しました。
    ([UUM-150208](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150208))

- `GI`: レイトレーシングのアクセラレーション構造体に追加された地形について、メッシュとそのGPUバッファがリークしなくなりました。
    (UUM-151903)

- `Graphics`: コンピュートシェーダーが、グラフィックスパイプラインがサポートする範囲を超えるスレッドグループを要求した場合（例：一部の Intel GPU での「High Quality Line Rendering」）、Metal 上で GPU がハングアップする問題を修正しました。
    (UUM-147457)

- `Graphics`: シングルパス XR をメモリレステクスチャ配列にレンダリングする際、Metal 上でエディタが「Metal: メモリレステクスチャには 2D テクスチャが必要です。」というアサートを出力していた問題を修正しました。
    (UUM-154442)

- `Graphics`: Graphics.RenderPrimitives および Graphics.DrawProcedural が、MeshTopology.Quads を使用している際にクラッシュする問題を修正しました。
    ([UUM-141117](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141117))

- `HDRP`: MSAA と雲レイヤーが有効な場合、空を背景にしたジオメトリの周囲に暗い輪郭線が表示される問題を修正しました。
    ([UUM-150911](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150911))

- `IL2CPP`: `Thread.VolatileWrite(ref object, object)` における GC 書き込みバリアの欠落を修正しました。
    (UUM-155582)

- `IL2CPP`: スレッドオブジェクトのメモリが、スレッドの終了後もGCによって保持され続ける問題を修正しました
    ([UUM-149541](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149541))

- `Input System`: WindowsのXbox Game BarおよびmacOSのオーバーレイ（Spotlightなど）に関する問題を修正しました。Windowsでは、Steam/Discord/NVIDIAのオーバーレイは従来通り動作します。
    ([UUM-150045](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150045))

- `iOS`: Unityの初期化前に `application:openURL` または `application:continueUserActivity` が呼び出された際に発生していたクラッシュを修正しました。
    ([UUM-151801](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151801))

- `Kernel`: 32 ビット整数のオーバーフローによって引き起こされていた NativeSlice でのクラッシュを修正しました。
    (UUM-154594)

- `macOS`: 最新の macOS バージョンで、X.509 証明書をインポートする際に発生する可能性があったクラッシュを修正しました。
    (UUM-154511)

- `macOS`: macOS 上で、バッチモードや自動テストの実行中にウィンドウのフォーカスが外れた際にエディタの動作が遅くなる問題を修正しました。

- `Mono`: デフォルトの GCHandle を使用する際のクラッシュを解消しました
    ([UUM-153835](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153835))

- `マルチプレイヤー`: Vulkan グラフィックス API を使用する際、追加のエディターインスタンスを含むプレイモードのシナリオが「デプロイ中」の状態のままになる問題を修正しました。
    ([UUM-154645](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154645))

- `ネットワーク`: Unity Transport: TLS/DTLS セッションの作成時に発生していた軽微なメモリリークを修正しました。
    ([UUM-151755](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151755))

- `Physics`: Rigidbody.mass が NaN 値を受け入れてしまい、その結果、リジッドボディがすべてのコライダーを通り抜けてしまう問題を修正しました。
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

- `Text`: TextMesh またはレガシー UI Text の文字列が、終了タグのないリッチテキストタグで終わっている場合に発生していた、メモリ範囲外読み取りの不具合を修正しました。
    (UUM-153128)

- `TextMeshPro`: 「TextMeshPro 入力フィールドでバリアント文字を使用した場合、最初のバックスペース入力時に文字が削除されない」という不具合を修正しました
    ([UUM-140383](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140383))

- `TextMeshPro`: 「Content Size Fitter」が設定された TextMeshPro テキストに、狭い幅でスペースに続くハイフンが含まれている場合にエディターがフリーズする問題を修正しました。
    ([UUM-152921](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152921))

- `uGUI`: RectMask2Dの「ソフトネス」が0の場合に、クリップされたコンテンツのエッジがぼやけてしまう問題を修正しました
    ([UUM-150815](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150815))

- `UI Toolkit`: パネルのスケールが整数でない場合、ドロップシャドウなどのフィルターが適用された要素内のテキストやコンテンツがぼやけてしまう問題を修正しました。
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

- `URP`: 互換モードが有効で、オーバーレイカメラがそのベースカメラとは異なるレンダラーを使用している場合、DX11で「CommandBuffer: 実行中に一時的なレンダリングテクスチャが見つかりませんでした」という警告が表示される問題を修正しました。
    ([UUM-117369](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-117369))

- `URP`: プレイヤー設定で「深度およびステンシルバッファを無効にする」が有効になっている場合、2D レンダラーがプレイヤーに深度バッファとステンシルバッファを作成してしまう問題を修正しました。
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

- `Web`: メモリプロファイラで使用される WASM_SIZE および wasmFileSize の不具合を修正しました
    (UUM-149075)

- `WebGL`: WebGPU: ユニフォームバッファおよび動的頂点バッファのメモリ使用量を改善しました
    (UUM-152972)




## 6000.3.27f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.collections`: [2.6.8](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) から [2.7.1](https://docs.unity3d.com/Packages/com.unity.collections@2.7//changelog/CHANGELOG.html) へ

- `com.unity.entities`: [1.4.8](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) から [1.5.0](https://docs.unity3d.com/Packages/com.unity.entities@1.5//changelog/CHANGELOG.html) へ

- `com.unity.physics`: [1.4.7](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) から [1.5.0](https://docs.unity3d.com/Packages/com.unity.physics@1.5//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: [1.4.21](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) から [1.5.0](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.5//changelog/CHANGELOG.html)

- `com.unity.burst`: [1.8.30](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) から [1.8.31](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) へ

- `com.unity.ide.rider`: [3.0.40](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) から [3.1.0](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.1//changelog/CHANGELOG.html) へ

- `com.unity.inputsystem`: [1.20.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.20//changelog/CHANGELOG.html) から [1.20.1](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.20//changelog/CHANGELOG.html) へ

- `com.unity.performance.profile-analyzer`: [1.4.0](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.4//changelog/CHANGELOG.html) から [1.4.2](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.4//changelog/CHANGELOG.html)

- `com.unity.probuilder`: [6.1.2](https://docs.unity3d.com/Packages/com.unity.probuilder@6.1//changelog/CHANGELOG.html) から [6.1.3](https://docs.unity3d.com/Packages/com.unity.probuilder@6.1//changelog/CHANGELOG.html) へ

- `com.unity.services.cloudsave`: [3.4.0](https://docs.unity3d.com/Packages/com.unity.services.cloudsave@3.4//changelog/CHANGELOG.html) から [3.4.2](https://docs.unity3d.com/Packages/com.unity.services.cloudsave@3.4//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: [2.0.15](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) から [2.0.16](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.polyspatial`: [3.2.2](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.2//changelog/CHANGELOG.html) から [3.3.1](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.3//changelog/CHANGELOG.html) へ

- `com.unity.polyspatial.visionos`: [3.2.2](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.2//changelog/CHANGELOG.html) から [3.3.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.3//changelog/CHANGELOG.html)

- `com.unity.polyspatial.xr`: [3.2.2](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.2//changelog/CHANGELOG.html) から [3.3.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.3//changelog/CHANGELOG.html) へ

- `com.unity.polyspatial.extensions`: [3.2.2](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.2//changelog/CHANGELOG.html) から [3.3.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.3//changelog/CHANGELOG.html) へ

- `com.unity.xr.visionos`: [3.2.2](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.2//changelog/CHANGELOG.html) から [3.3.1](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.3//changelog/CHANGELOG.html) へ

- `com.unity.ext.flatsharp`: [1.1.4](https://docs.unity3d.com/Packages/com.unity.ext.flatsharp@1.1//changelog/CHANGELOG.html) から [2.0.1](https://docs.unity3d.com/Packages/com.unity.ext.flatsharp@2.0//changelog/CHANGELOG.html)

- `com.unity.services.multiplayer`: [2.3.3](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.3//changelog/CHANGELOG.html) から [2.4.0](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.4//changelog/CHANGELOG.html) へ

- `com.unity.web.stripping-tool`: [1.3.0](https://docs.unity3d.com/Packages/com.unity.web.stripping-tool@1.3//changelog/CHANGELOG.html) から [1.4.0](https://docs.unity3d.com/Packages/com.unity.web.stripping-tool@1.4//changelog/CHANGELOG.html) へ

- `com.unity.cloud.draco`: [5.4.3](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html) から [5.5.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.5//changelog/CHANGELOG.html) へ

- `com.unity.cloud.ktx`: [3.6.3](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html) から [3.7.1](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.7//changelog/CHANGELOG.html)

- `com.unity.platformtoolkit.steam`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.steam@1.1//changelog/CHANGELOG.html) から [1.2.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.steam@1.2//changelog/CHANGELOG.html)

- `com.unity.platformtoolkit.playgamesservices`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.playgamesservices@1.1//changelog/CHANGELOG.html) から [1.2.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.playgamesservices@1.2//changelog/CHANGELOG.html)

- `com.unity.platformtoolkit.gdk`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gdk@1.1//changelog/CHANGELOG.html) から [1.2.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gdk@1.2//changelog/CHANGELOG.html) へ

- `com.unity.platformtoolkit.gamekit`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gamekit@1.1//changelog/CHANGELOG.html) から [1.2.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gamekit@1.2//changelog/CHANGELOG.html) へ

- `com.unity.platformtoolkit`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit@1.1//changelog/CHANGELOG.html) から [1.2.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit@1.2//changelog/CHANGELOG.html)