# Unity 6000.0.86f1 LTS
公開日時：2026年11月12日（木）09:43:45 GMT  
https://unity.com/releases/editor/whats-new/6000.0.86f1

# 6000.0.86f1 の既知の問題

- `Android`: 「バックグラウンドで実行」および 「予測バック機能」が有効になっている場合、バックジェスチャーやバックボタンでアプリが終了してしまう
    ([UUM-159613](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159613))

- `エディターインストーラー`: [macOS] プレイヤーライブラリが、特注の権限でコード署名されている
    ([UUM-156884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156884))

- `シェーダーシステム`: SceneManager.LoadSceneAsync を使用してシーンを繰り返し切り替えると、Player が永久に応答しなくなる
    ([UUM-156125](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156125))

- `Video`: 特定の .mp4 動画ファイルを含むプロジェクトを開いた際、BitmapDataToImageReference の処理中にクラッシュする
    ([UUM-160889](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-160889))



# 6000.0.86f1 リリースノート

## 改善点

- `アセットのインポート`: バンドルされている Autodesk FBX SDK を 2020.3.11 に更新し、FBX ファイルの解析における 2 つのバッファオーバーフローの脆弱性を修正することで、モデルのインポート時のセキュリティを向上させました。
    (UUM-155199)

- `ライセンス`: ライセンスクライアントを v1.19.0 に更新し、起動速度を向上させました。



## API の変更

- `iOS`: 追加: iPhone 18 Pro、iPhone 18 Pro Max、および iPhone Duo のデバイス世代列挙型と画面カットアウトを追加しました。



## 修正

- `2D`: プレイモードでシャドウキャスターの 2D シェイプ編集を元に戻したりやり直したりした際に表示される「ShadowCasterPath のスクリプトアセットがありません」という警告を修正しました。
    ([UUM-152935](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152935))

- `2D`: スクリプトから作成されたLight 2Dを、シェイプパスなしでFreeformに設定した際に発生していたNullReferenceExceptionを修正しました。
    ([UUM-154810](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154810))

- `2D`: 実行時に Tilemap Collider 2D のタイルが削除された後、Shadow Caster 2D が以前の影を残してしまう問題を修正しました。
    ([UUM-149925](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149925))

- `2D`: 「Mask Interaction」が「None」に設定されている LineRenderer または TrailRenderer が、同じマテリアルを使用し「Mask Interaction」が有効になっている別の LineRenderer または TrailRenderer によって、スプライトマスクによってクリップされてしまう問題を修正しました。
    ([UUM-158602](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158602))

- `2D`: Unity 6.0 または 6.3 で保存されたプロジェクトを新しいバージョンで開いた際、Point Light 2D のクッキースプライトが失われる問題を修正しました。
    ([UUM-156931](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156931))

- `2D`: コライダー 2D（例：タイルマップ コライダー 2D）を投影源として使用するシャドウキャスター 2D の影が、シーンビューおよびゲームビューでちらつく問題を修正しました。
    ([UUM-147033](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147033))

- `2D`: 2D レンダラーの「深度/ステンシルバッファ」設定が無効になっている場合、一部の OpenGL ES デバイスでスプライトや UI がレンダリングされない問題を修正しました。
    ([UUM-159093](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159093))

- `2D`: URP 2D エディタ専用のアイコンがプレイヤービルドに含まれてしまう問題を修正しました。
    (UUM-144935)

- `Android`: Android 向けに最適化されたフレームペーシング \(Swappy\) に関するクラッシュ修正をバックポートしました。
    (UUM-153366)

- `Android`: OpenGL において、Unity のレンダースレッドが 1 フレーム内で JVM に複数回アタッチ/デタッチし、不要な割り当てが発生していた問題を修正しました。
    (UUM-155309)

- `Android`: AndroidネイティブライブラリのGNU_RELROセグメントが16 KBにアラインされていなかった問題を修正しました。`libc++_shared.so`は、次回のNDKアップデートまでアラインされないままとなります。
    ([UUM-156603](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156603))

- `Android`: カーソルがロックされている状態でマウスを動かすと、スクロール値が発生する問題を修正しました。
    ([UUM-156720](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156720))

- `Android`: 例えば分割画面モードなどで、アプリがフォーカスを回復した後や、別のアプリがカメラを解放した後、WebCamTextureの再開に数秒かかる問題を修正しました。
    (UUM-155066)

- `Android`: バンドルされている Android SDK のコマンドラインツールを 21.0 に更新し、その avdmanager で作成された Android 17 (API 37.0) 向けエミュレータが正しく起動するようにしました。
    (UUM-157110)

- `Animation`: `AnimationUtility.SetAdditiveReferencePose` を、null の clip または referenceClip を引数として呼び出した際にクラッシュする。
    ([UUM-150816](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150816))

- `アセットバンドル`: Addressables または Scriptable Build Pipeline を使用している場合、変更されていないコンテンツのビルド間で AssetBundle のコンテンツハッシュが変更され、プレイヤーが変更されていないバンドルを再ダウンロードしてしまう問題を修正しました。影響を受けるバンドルは、アップグレード後の最初のビルドで新しいハッシュが割り当てられます。
    ([UUM-148841](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148841))

- `アセットのインポート`: Linux版エディタで、crunch圧縮されたテクスチャをインポート中に「crn_threading_pthreads.cpp\(194\): Failure: semaphore: sem_wait\(\) または sem_timedwait\(\) が失敗しました」というエラーメッセージがログに記録される問題を修正しました。Crunchコンプレッサーは、中断された待機を致命的なエラーとして扱っていましたが、現在は待機を再試行するようになりました。
    ([UUM-150055](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150055))

- `アセットパイプライン`: アセットパイプライン: ディレクトリ監視が変更されたファイルに関する期待通りの通知を受け取れない場合に発生していた、起動時のハングを修正しました。
    ([UUM-149019](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149019))

- `Audio`: 再生モード中にUnity Audioのオン/オフを切り替えた際に、クリップが読み込まれていたAudioSourceを再生した後、再生モードを終了する際にログに出力されていたアサーション \(m_ModifiedClips.empty\(\)\) を修正しました。
    ([UUM-148749](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148749))

- `ビルドシステム`: dotnet を呼び出す際に使用される他のメソッドに MSBUILDDEBUGPATH を追加しました。

- `ビルドシステム`: Bee_backend による古い出力の削除処理において、同じファイルを無限に再チェックし続けることがないようにしました。
    (UUM-158568)

- `ビルドシステム`: 以前の `bee_backend` がまだ実行中の場合でも、エディタがハングアップしないようにしました。
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

- `DX12`: EnableAsyncCompute\(true\) を指定して AddComputePass を使用する際、D3D12SwapChain::Present でのクラッシュを修正した。
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `DX12`: グラフィックスジョブが有効な状態で、ネイティブプラグインがUnityの現在のコマンドリストに記録したコマンドよりも先に完了する可能性のあるフェンス値を、IUnityGraphicsD3D12::GetNextFrameFenceValue\(\)が返す問題を修正しました。
    (UUM-156768)

- `エディタ`: 未保存の変更があるウィンドウが開いている状態で、保存済みのエディタレイアウトに切り替えようとすると、レイアウトの変更をキャンセルできなくなるバグを修正しました。
    ([UUM-150448](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150448))

- `エディター`: `Instantiate` では親トランスフォームのスケールが考慮されるのに対し、`InstantiateAsync` では考慮されないというバグを修正しました。
    ([UUM-154591](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154591))

- `エディター`: スクリプトで `UnityEngine.Device.SystemInfo.processorModel、processorManufacturer、または supportsMachineLearning を使用しているスクリプトで、プレイヤービルドがエラー CS0117 で失敗する問題を修正しました。
    ([UUM-154729](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154729))

- `エディタ`: 「自動保存」が有効な状態で名前フィールドを選択した後、プレハブのフィールドが部分的にしか保存されない問題を修正しました。
    ([UUM-157667](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157667))

- `エディタ`: TrueTypeFontImporter の [ヘルプ] ボタンのリンクを修正しました。
    ([UUM-144647](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144647))

- `エディタ`: Windows版エディタに同梱されているVCRedistをバージョン14.51.36247に更新しました。
    (UUM-156578)

- `エディタ`: URP: アセットバンドルのビルドを開始する前に、URPアセットを保存するようになりました。
    ([UUM-153206](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153206))

- `エディタ`: グラフィックスジョブが有効な場合、エディタはフレーム中にコンパイルされたシェーダーバリアントを持つレンダラーを描画するようになりました。以前はシェーダーの欠如により空白となっていたアセットのプレビューやワンショットレンダリングは、SRPバッチャーによるフォールバックパスを通じて、期待どおりに描画されるようになりました。
    (UUM-147205)

- `エディター`: \[Android\] Unity 6.0 での APK インストール中にデバイスがオフラインになった理由をユーザーに通知するエラーを表示するようになりました。
    (UUM-151550)

- `Engine Diagnostics`: リモート設定の前にキャプチャされたクラッシュ、例外、および ANR レポートは、発生したセッションを含む重要な属性を保持するようになりました。
    (UUM-159169)

- `Engine Diagnostics`: Engine Diagnostics の設定が適用されている最中に、ワーカースレッドからクラッシュレポートが記録された際に発生する可能性があったクラッシュを修正しました。
    (UUM-158113)

- `GI`: URP固有の設定のみが変更された場合、ライティングのベイク処理時にリフレクションプローブが再ベイクされないことがあるバグを修正しました。
    ([UUM-133949](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-133949))

- `GI`: AMD GPU上でVulkanを使用してベイクを行う際、Adaptive Probe Volumesが、シーンにジオメトリが存在しないかのようにプローブを配置してしまう問題を修正しました。
    ([UUM-137732](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-137732))

- `GI`: APV による斑点や白いスポットが発生する問題を修正しました。
    ([UUM-133626](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-133626))

- `Graphics`: Universal Windows Platform上でDirectX 12を使用したグラフィックスジョブの分割処理を行っているプレイヤーにおいて、終了時のクラッシュを修正しました。
    (UUM-152563)

- `Graphics`: エディタがシングルパス XR をメモリレステクスチャ配列にレンダリングする際、Metal 上で「Metal: メモリレステクスチャには 2D テクスチャが必要です。」というアサートが発生していた問題を修正しました。
    (UUM-154442)

- `Graphics`: 2Dスプライトマテリアルを使用するLine RendererまたはTrail Rendererが、アニメーションウィンドウで「プレビュー」をオフにした後、または`Renderer.SetPropertyBlock`を呼び出した後に表示されなくなる問題を修正しました。
    ([UUM-156620](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156620))

- `Graphics`: Vulkan および GraphicsJobs を使用する際のミップストリーミングに関する問題を修正しました。
    (UUM-137032)

- `Graphics`: GPU がそのフォーマットをサポートしていない場合や、 かつミップレベルが4x4未満、または4の倍数でない場合などに、CPU上でBC圧縮されたテクスチャが展開される際に発生するメモリ破損を修正しました。
    (UUM-154799)

- `Graphics`: <br>において、`SystemInfo.supportsParallelPSOCreation`が正しく`true`を返すようになりました。
    シングルコアのAndroidデバイスにおいて、並列PSO作成を有効にする場合、`SystemInfo.supportsParallelPSOCreation`が正しく`true`を返すようになりました。
    (UUM-153032)

- `HDRP`: 一部のEnumマテリアルプロパティに「Default」が追加される問題を修正しました。
    ([UUM-134256](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134256))

- `HDRP`: MSAAと雲レイヤーが有効な際、空を背景にしたジオメトリの周囲に暗い輪郭線が表示される問題を修正しました。
    ([UUM-150911](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150911))

- `入力システム`: WindowsのXbox Game BarおよびmacOSのオーバーレイ（Spotlightなど）の不具合を修正しました。Windowsでは、Steam/Discord/NVIDIAのオーバーレイは従来通り動作します。
    ([UUM-150045](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150045))

- `iOS`: Unityの初期化前に`application:openURL`または`application:continueUserActivity`が呼び出された際に発生していたクラッシュを修正しました。
    ([UUM-151801](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151801))

- `Kernel`: 32ビット整数のオーバーフローによって引き起こされていた NativeSlice でのクラッシュを修正しました。
    (UUM-154594)

- `License`: Unity Licensing Client に接続できない場合、エディターがライセンスなしで動作を継続し、バッチモードではコード 0 で終了してしまう問題を修正しました。
    ([UUM-151817](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151817))

- `ライセンス`: 同じバージョンの 2 つのエディタで、互換性のないライセンスクライアントのバージョンが要求された場合、ライセンスエラーダイアログが「再試行」と「閉じる」を繰り返し続ける問題を修正しました。
    (UUM-153121)

- `Linux`: -nographics オプションを指定して -batchmode オプションを指定せずにエディタを起動した際に発生していた Linux でのクラッシュを修正しました。エディタは現在、無効な引数を報告し、コード 1 で終了します。
    ([UUM-154576](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154576))

- `macOS`: `Screen.sleepTimeout` が `SleepTimeout.SystemSetting` に設定されており、かつシステム設定が `Never` ではない場合、システムがスリープ状態になるようにしました。
    ([UUM-150222](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150222))

- `macOS`: macOS 上で、バッチモードまたは自動テスト実行中に、エディタのウィンドウのいずれかがフォーカスを失った際にエディタの動作が遅くなる問題を修正しました。

- `ネットワーク`: Unity Transport: TLS/DTLS セッションの作成時に発生していた軽微なメモリリークを修正しました。
    ([UUM-151755](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151755))

- `スクリプティング`: フレーム更新中に `Awaitable.NextFrameAsync` または `Awaitable.EndOfFrameAsync` のアウェイト可能処理をキャンセルすると、無関係なアウェイト可能処理がデフォルトの結果で早期に完了してしまう問題を修正しました。
    ([UUM-156357](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156357))

- `シェーダー`: ヌルのコンピュートシェーダーで `RenderingCommandBuffer.SetKeyword` を呼び出した際に発生するクラッシュを修正しました。
    ([UUM-158327](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158327))

- `Shaders`: ヌルまたは破棄されたマテリアルに対して SetKeyword を含む RenderingCommandBuffer を実行した際に発生していたクラッシュを修正しました。
    ([UUM-157105](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157105))

- `Shaders`: バックグラウンドでシェーダーバリアントがコンパイルされている最中にシェーダーメッセージが読み込まれた際に、エディタがクラッシュする可能性があった問題を修正しました。
    (UUM-154510)

- `Shaders`: コンパイルされていない、または破損したシェーダーがキャンバス上でレンダリングされている際に、エディターがクラッシュする問題を修正しました。
    ([UUM-153265](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153265))

- `Shaders`: 指定された値が有効な列挙範囲外の場合に `Material.GetPropertyNames` がクラッシュする問題を修正しました。
    ([UUM-157945](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157945))

- `SRP Core`: ネイティブパスがオンタイルピクセルストレージの制限を超えていると判定された場合、古い iOS デバイス（Apple GPU ファミリー 3 以前）において、レンダリングパスがマージされず、フレーム全体がレンダリングパスごとに 1 つのネイティブパスにシリアル化される問題を修正しました。
    ([UUM-148865](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148865))

- `SRP Core`: ネイティブサブパスが 8 つ未満の場合でも、8 つのラスタレンダリングパス後にレンダリンググラフがネイティブレンダリングパスを終了してしまう問題を修正しました。これにより、URP UI オーバーレイなどの次のパスが、アタッチメントをメモリから再度読み込む必要がありました。
    ([UUM-158401](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158401))

- `UI Toolkit`: キーの値が非常に大きい場合、保存後に AnimationCurve の UXML 属性の値が失われる問題を修正しました。
    ([UUM-156823](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156823))

- `UI Toolkit`: テキストで、アトラスのパディングが小さく、アウトライン幅がゼロまたは負の値であるフォントアセットを使用した場合、文字の周囲にアーティファクトが発生する問題を修正しました。
    ([UUM-146020](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146020))

- `UI Toolkit`: ドッキングされたウィンドウを最大化・復元した場合や、デバッガーで UI Toolkit ライブリロードを切り替えた場合など、UI Toolkit デバッガーウィンドウが再作成された後に、ダイナミックアトラスビューアーにアトラスが表示されない問題を修正しました。
    ([UUM-150663](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150663))

- `URP`: 互換モードが有効で、オーバーレイカメラがそのベースカメラとは異なるレンダラーを使用している場合、DX11で「CommandBuffer: 実行中に一時的なレンダリングテクスチャが見つかりませんでした」という警告が表示される問題を修正しました。
    ([UUM-117369](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-117369))

- `URP`: 一部のエヌム・マテリアルプロパティに「Default」が追加される問題を修正しました。
    ([UUM-134256](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134256))

- `URP`: 追加のライトシャドウが無効化され、シャドウマスクが有効化された状態でディファードレンダリングを使用する際、URPがストリップドバリアントを使用しようとするバグを修正しました。
    ([UUM-153600](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153600))

- `URP`: 深度/ステンシルバッファが無効になっている 2D レンダラーと併用した場合、URP RenderGraph サンプル内の「Renderer List」および「Culling」サンプルが毎フレームエラーを記録してしまう問題を修正しました。
    ([UUM-157948](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157948))

- `URP`: 同じエディタセッション内で、以前に「LODクロスフェードのサポート」が有効なシェーダーグラフがインポートされていたかどうかに応じて、シェーダーグラフが異なるシェーダーコードとしてインポートされたり、アセットバンドルのハッシュ値が異なったりする問題を修正しました。
    (UUM-155529)

- `XR`: サブシステムが破棄された後に `SubsystemWithProvider.Start` を呼び出した際、`ArgumentNullException` が発生せず、破棄されたプロバイダーが再起動してしまう問題を修正しました。
    ([UUM-151411](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151411))




## 6000.0.86f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.2d.animation`: [10.2.3](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.2//changelog/CHANGELOG.html) から [10.2.4](https://docs.unity3d.com/Packages/com.unity.2d.animation@10.2//changelog/CHANGELOG.html) へ

- `com.unity.2d.psdimporter`: [9.1.2](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.1//changelog/CHANGELOG.html) から [9.1.3](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@9.1//changelog/CHANGELOG.html) へ

- `com.unity.2d.tilemap.extras`: [4.1.1](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@4.1//changelog/CHANGELOG.html) から [4.1.2](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@4.1//changelog/CHANGELOG.html) へ

- `com.unity.burst`: [1.8.30](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) から [1.8.31](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.13.6](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.13//changelog/CHANGELOG.html) から [2.14.0](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.14//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.4.0](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.4//changelog/CHANGELOG.html) から [1.4.2](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.4//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: [3.8.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.8//changelog/CHANGELOG.html) から [3.8.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.8//changelog/CHANGELOG.html)

- `com.unity.services.cloudsave`: [3.4.0](https://docs.unity3d.com/Packages/com.unity.services.cloudsave@3.4//changelog/CHANGELOG.html) から [3.4.2](https://docs.unity3d.com/Packages/com.unity.services.cloudsave@3.4//changelog/CHANGELOG.html) へ

- `com.unity.services.wire`: [1.6.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.6//changelog/CHANGELOG.html) から [1.6.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.6//changelog/CHANGELOG.html) へ

- `com.unity.test-framework.performance`: [3.5.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.5//changelog/CHANGELOG.html) から [3.7.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.7//changelog/CHANGELOG.html) へ

- `com.unity.xr.oculus`: [4.5.4](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html) から [4.5.6](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html) へ

- `com.unity.ai.navigation`: [2.0.15](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) から [2.0.16](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) へ

- `com.unity.asset-manager-for-unity`: [1.12.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.12//changelog/CHANGELOG.html) から [1.12.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.12//changelog/CHANGELOG.html) へ

- `com.unity.cloud.draco`: [5.5.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.5//changelog/CHANGELOG.html) から [5.6.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.6//changelog/CHANGELOG.html)

- `com.unity.cloud.ktx`: [3.7.1](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.7//changelog/CHANGELOG.html) から [3.8.0](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.8//changelog/CHANGELOG.html) へ

- `com.unity.xr.compositionlayers`: [2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.6//changelog/CHANGELOG.html) から [2.6.1](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.6//changelog/CHANGELOG.html)

**追加されたパッケージ**

- [com.unity.steamworks-api@1.0.0](https://docs.unity3d.com/Packages/com.unity.steamworks-api@1.0//changelog/CHANGELOG.html)