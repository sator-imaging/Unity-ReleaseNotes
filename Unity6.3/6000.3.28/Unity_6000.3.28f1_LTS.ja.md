# Unity 6000.3.28f1 LTS
公開日時：2026年11月3日（火）16:15:25 GMT  
https://unity.com/releases/editor/whats-new/6000.3.28f1

# 6000.3.28f1 の既知の問題

- `Android`: 「バックグラウンドで実行」および「予測バック機能のサポート」が有効になっている場合、バックグラウンドから復帰した後にバックジェスチャまたはバックボタンを押すとアプリが終了してしまう
    ([UUM-159613](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159613))

- `オーディオオーサリング`: USBオーディオ出力デバイスが切断され、再接続された後にメインスレッドが再開されると、複数のスタックトレースを伴うクラッシュが発生する
    ([UUM-158166](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158166))

- `エディタインストーラ`: [macOS] プレーヤーライブラリが、特注の権限でコード署名されている
    ([UUM-156884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156884))

- `ネイティブエディタアプリケーションのライフサイクル`: [WinEditor] ポーリングレートが高い状態でマウスカーソルを動かすと、再生モードのフレームレートが大幅に低下する
    ([UUM-142550](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142550))

- `シェーダーシステム`: SceneManager.LoadSceneAsync を使用してシーンを繰り返し切り替えると、プレイヤーが永久に応答しなくなる
    ([UUM-156125](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156125))

- `SRP Foundation`: デバイスを物理的に回転させた際、Logcat およびコンソールに RenderPass に関連する Android エラーが記録される
    ([UUM-157974](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157974))



# 6000.3.28f1 リリースノート

## 改善点

- `License`: ライセンスクライアントを v1.19.0 に更新し、起動速度が向上しました。



## APIの変更

- `iOS`: 追加: iPhone 18 Pro、iPhone 18 Pro Max、およびiPhone Duoのデバイス世代列挙型と画面カットアウトを追加しました。



## 修正

- `2D`: プレイモードでシャドウキャスターの2D形状編集を元に戻したりやり直したりした際に表示される「ShadowCasterPath用のスクリプトアセットがありません」という警告を修正しました。
    ([UUM-152935](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152935))

- `2D`: スクリプトから作成されたLight 2Dを、シェイプパスなしでFreeformに設定した際に発生していたNullReferenceExceptionを修正しました。
    ([UUM-154810](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154810))

- `2D`: Unity 6.0 または 6.3 で保存されたプロジェクトを新しいバージョンで開いた際、Point Light 2D のクッキースプライトが失われる問題を修正しました。
    ([UUM-156931](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156931))

- `2D`: コライダー 2D（例：タイルマップ コライダー 2D）を投影源として使用するシャドウキャスター 2D の影が、シーンビューおよびゲームビューでちらつく問題を修正しました。
    ([UUM-147033](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147033))

- `Android`: Android向けに最適化されたフレームペーシング（\(Swappy\)）に関するクラッシュ修正をバックポートしました。
    (UUM-153366)

- `Android`: null の MonoScript を引数として `AnimatorController.CreateNewStateMachineBehaviour` を呼び出した際に発生していたクラッシュを修正しました。現在は代わりに `ArgumentNullException` がスローされるようになりました。
    ([UUM-150813](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150813))

- `Android`: OpenGL において、Unity のレンダースレッドが 1 フレーム内で JVM に複数回アタッチ/デタッチし、不要なメモリ割り当てが発生していた問題を修正しました。
    (UUM-155309)

- `Android`: AndroidネイティブライブラリのGNU_RELROセグメントが16 KBにアラインされていなかった問題を修正しました。`libc++_shared.so`は、次回のNDKアップデートまでアラインされないままとなります。
    ([UUM-156603](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156603))

- `Android`: 例えば分割画面モードなどで、アプリがフォーカスを回復した後や、別のアプリがカメラを解放した後、WebCamTextureの再開に数秒かかる問題を修正しました。
    (UUM-155066)

- `Animation`: 範囲外のボーンインデックスが渡された際に、HumanTrait.GetParentBone および HumanTrait.RequiredBone で発生していたクラッシュを修正しました。これらのメソッドは、代わりに ArgumentOutOfRangeException をスローするようになりました。
    ([UUM-150938](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150938))

- `Animation`: 無効またはデフォルトの `AnimationPlayableOutput` に対して `AnimationPlayableOutput.SetSortingOrder` を呼び出した際に発生していたクラッシュを修正しました。これらは、代わりに `NullReferenceException` をスローするようになりました。
    ([UUM-150941](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150941))

- `Animation`: `AnimationPlayableOutputExtensions.SetAnimationStreamSource` にデフォルトまたは無効な `AnimationPlayableOutput` を指定した際に発生していたクラッシュを修正しました。
    ([UUM-150939](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150939))

- `アセットバンドル`: Addressables または Scriptable Build Pipeline を使用している場合、変更されていないコンテンツのビルド間で AssetBundle のコンテンツハッシュが変更され、プレイヤーが変更されていないバンドルを再ダウンロードしてしまう問題を修正しました。影響を受けるバンドルは、アップグレード後の最初のビルドで新しいハッシュが割り当てられます。
    ([UUM-148841](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148841))

- `アセットのインポート`: SVGImporter などの組み込みモジュールが提供するインポーターのデフォルトプリセットが、プロジェクトの再起動後に適用されなくなる問題を修正しました。
    ([UUM-146265](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146265))

- `アセットのインポート`: crunchで圧縮されたテクスチャをインポート中に、Linux版エディタが時折終了し、ログに「crn_threading_pthreads.cpp\(194\): Failure: semaphore: sem_wait\(\) or sem_timedwait\(\) failed」と表示される問題を修正しました。 crunch コンプレッサーは、中断された待機を致命的なエラーとして扱っていましたが、現在は待機を再試行するようになりました。
    ([UUM-150055](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150055))

- `ビルドシステム`: Bee_backend の古い出力の削除処理において、同じファイルを無期限に再チェックしないようにしました。
    (UUM-158568)

- `ビルドシステム`: 以前の bee_backend がまだ実行中の場合、エディタがハングしないようにしました。
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

- `DX12`: 1フレーム内で、大きなダイナミックフォントアトラスなどの大容量テクスチャが何度も更新された際に、DirectX 12で発生していたクラッシュを修正しました。
    ([UUM-140070](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140070))

- `DX12`: IUnityGraphicsD3D12::GetNextFrameFenceValue\(\)が、グラフィックスジョブが有効な状態で、ネイティブプラグインがUnityの現在のコマンドリストに記録したコマンドよりも先に完了する可能性のあるフェンス値を返す問題を修正しました。
    (UUM-156768)

- `DX12`: 1回の再描画でフレームごとの描画量が極端に多いシーンをレンダリングした場合、エディタがメモリ不足エラーやGPUデバイスのリセットによりクラッシュしなくなりました。 Direct3D 12 では、アップロード用スクラッチメモリが 1 GiB 以上蓄積されると、フレームの途中で GPU 処理を再度送信するようになりました。この閾値は変更可能であり、d3d12-scratch-flush-threshold ブート設定パラメータを使用して、このしきい値を変更したり、0に設定して無効にしたりできます。フレーム途中のフラッシュが初めて実行されると、エディタまたはプレイヤーのログにそのパラメータ名が表示されます。
    (UUM-93272)

- `エディタ`: Macエディタで「強制終了」操作を実行した際に `NativeWindowManager` で発生していたクラッシュを修正しました。
    ([UUM-157869](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157869))

- `エディタ`: ATG小節の高さが制限されていない場合に発生するクラッシュを修正しました。
    ([UUM-155956](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-155956))

- `エディタ`: 隣接するリンク間を移動した際にホバーイベントが発火しない問題を修正しました。
    (UUM-156714)

- `エディタ`: Android用Unity Render Serviceのビルドプロファイルにある「モジュールをインストール」ボタンが、Androidモジュールがインストールされていない場合に、破損したダウンロードリンクを開いてしまう問題を修正しました。
    (UUM-154168)

- `エディタ`: TrueTypeFontImporter の [ヘルプ] ボタンのリンクを修正しました。
    ([UUM-144647](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144647))

- `エディタ`: マルチプレイヤー: 「プレイモードのシナリオ」ウィンドウを大きなサイズで再表示した際、選択範囲のハイライトがリストの区切り線を越えて表示される問題を修正しました。
    ([UUM-137539](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-137539))

- `エディタ`: Windows: エディタがバッチモードで実行され、メインウィンドウを作成できなかった際に発生していたクラッシュを修正しました。
    ([UUM-153339](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153339))

- `エディタ`: \[Android\] Unity 6.3でのAPKインストール中にデバイスがオフラインになった理由をユーザーに通知するエラーメッセージを表示するようにしました。
    (UUM-151550)

- `GI`: AMD GPU上でVulkanを使用してベイクを行う際、Adaptive Probe Volumesが、シーンにジオメトリが存在しないかのようにプローブを配置してしまう問題を修正しました。
    ([UUM-137732](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-137732))

- `GI`: APV による斑点や白いスポットが発生する問題を修正しました。
    ([UUM-133626](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-133626))

- `Graphics`: マルチディスプレイ使用時のバックバッファの寸法が正しく設定されるようにしました。
    (UUM-134688)

- `Graphics`: Universal Windows Platform上でDirectX 12を使用したグラフィックジョブの分割処理を行っているプレイヤーにおいて、終了時に発生していたクラッシュを修正しました。
    (UUM-152563)

- `Graphics`: 2Dスプライトマテリアルを使用するLine RendererまたはTrail Rendererが、アニメーションウィンドウで「プレビュー」をオフにした後、または`SetPropertyBlock`を呼び出した後に表示されなくなる問題を修正しました。SetPropertyBlock。
    ([UUM-156620](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156620))

- `Graphics`: アセットのインポートがトリガーされ、かつ `Camera.SetTargetBuffers` を使用して設定されていた場合に発生するクラッシュを修正しました。
    ([UUM-148003](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148003))

- `Graphics`: 特定のレンダーパス／サブパスの構成において、Mali GPU上で発生していたVulkanレンダリングのアーティファクトを修正しました。
    ([UUM-147578](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147578))

- `Graphics`: <br>
    シングルコアを搭載し、並列PSO作成を有効にしているAndroidデバイスにおいて、`SystemInfo.supportsParallelPSOCreation`が正しく`true`を返すようになりました。
    (UUM-153032)

- `HDRP`: 一部の Enum マテリアルプロパティに「Default」が追加される問題を修正しました。
    ([UUM-134256](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134256))

- `HDRP`: デフォルトの品質レベルが「Performant」に設定されていたため、ボリュームフォグが無効な状態でHDテンプレートが開く問題を修正しました。
    (UUM-149134)

- `License`: 同じバージョンのエディタ 2 台で、互換性のないライセンスクライアントのバージョンが要求された場合、ライセンスエラーダイアログが「再試行」と「閉じる」を繰り返し、ループしてしまう問題を修正しました。
    (UUM-153121)

- `Linux`: `-nographics` オプションを指定したバッチモードや、ディスプレイがない場合など、ビデオサブシステムが初期化されていない状態で実行した際に Linux で発生していたクラッシュを修正しました。
    ([UUM-156559](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156559))

- `Linux`: -nographics オプションを指定して -batchmode オプションを指定せずにエディタを起動した際に発生していたクラッシュを修正しました。エディタは現在、無効な引数を報告し、コード 1 で終了します。
    ([UUM-154576](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154576))

- `macOS`: `Screen.sleepTimeout` が `SleepTimeout.SystemSetting` に設定されており、かつシステム設定が `Never` でない場合、システムがスリープ状態になるようにしました。
    ([UUM-150222](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150222))

- `Mono`: TLS 1.3 のみをサポートするサーバーへの WebSocket 接続に関する問題を修正しました。
    (UUM-158461)

- `Mono`: ランタイム統計が無効になっている場合、JIT フェーズのタイミング測定をスキップすることで、JIT コンパイルのオーバーヘッドを低減しました。
    (UUM-158476)

- `Physics`: スケールされた Sphere と Convex Mesh Collider 間の ComputePenetration が、正しい結果を返すようになりました。
    (UUM-139615)

- `Physics`: ジョイントコンポーネントが、新しく接続されたリジッドボディコンポーネントの接触再評価を引き起こさない問題を修正しました。これにより、「enable collisions」などのフラグが有効になるようになりました。
    ([UUM-156450](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156450))

- `Physics 2D`: 「maxFraction」が 1 未満の場合に「PhysicsAABB.CastRay」が誤った分数を返す不具合、および「PhysicsAABB.center」と「PhysicsAABB.extents」の警告で誤ったメンバ名が指定されていた不具合を修正しました。
    ([UUM-156920](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156920))

- `Physics 2D`: 「PhysicsLayers」を修正し、「GetLayerMask」が同じ名前を持つすべてのレイヤーを含めるようにしました。また、「GetLayerName」は名前のないレイヤーの場合、空の文字列を返すようにし、null または範囲外の引数が渡された場合は、正しいパラメータ名を指定した例外をスローするようにしました。
    ([UUM-156920](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156920))

- `Physics 2D`: 「PhysicsMask」を修正し、レイヤー 31 を含む「LayerMask」が上位 32 ビットを設定しなくなるようにした。 空のマスクに対して「AreBitsSet」が false を返すようになり、デフォルトの「ResetBitIterator」にはビット 0 が含まれるようになり、0 から 63 以外のシフトカウントでは例外がスローされるようになりました。
    ([UUM-156920](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156920))

- `Physics 2D`: 正規化されていない回転に対して「PhysicsRotate.isNormalized」が警告をログに出していた問題、および「PhysicsRotate.Normalized」の警告で誤ったメソッド名が指定されていた問題を修正しました。
    ([UUM-156920](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156920))

- `Physics 2D`: 「PhysicsTransform」の検証警告で、誤ったメソッド名が指定されていた問題を修正しました。
    ([UUM-156920](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156920))

- `Prefabs`: 並列インポート時に、インプロセスとアウトプロセスでプレハブをインポートした際の挙動が不確定になる問題を修正しました。

- `Project Browser`: コピーしたサブアセットをフォルダに貼り付けた際、同名の既存アセットが上書きされ、それらへの参照が破損する問題を修正しました。
    ([UUM-121005](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-121005))

- `スクリプティング`: フレーム更新中に `Awaitable.NextFrameAsync または Awaitable.EndOfFrameAsync といったアウェイタブルをキャンセルすると、無関係なアウェイタブルがデフォルトの結果で早期に完了してしまう問題を修正しました。
    ([UUM-156357](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156357))

- `検索`: 読み取り専用パッケージ内にあるシーンについて、検索ウィンドウのインスペクターに「シーンを追加」オプションが表示されるバグを修正しました。
    ([UUM-139396](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-139396))

- `シェーダー`: コンピュートシェーダーまたはレイトレーシングシェーダーが null の状態で `RenderingCommandBuffer.SetKeyword` を呼び出した際に発生するクラッシュを修正しました。
    ([UUM-158327](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158327))

- `Shaders`: ヌルまたは破棄されたマテリアルに対して SetKeyword を含む RenderingCommandBuffer を実行した際に発生するクラッシュを修正しました。
    ([UUM-157105](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157105))

- `Shaders`: ビルド実行時にまれに発生していたクラッシュを修正しました。
    ([UUM-148715](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148715))

- `Shaders`: コンパイルされていない、または破損したシェーダーがキャンバス上でレンダリングされた際にエディタで発生するクラッシュを修正しました。
    ([UUM-153265](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153265))

- `Shaders`: デフォルトで作成された `LocalKeyword` および `LocalKeywordSpace` フィールドへのアクセスによりエディタがクラッシュする問題を修正しました。
    ([UUM-156424](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156424))

- `Shaders`: 指定された値が有効な列挙範囲外の場合に、Material.GetPropertyNames がクラッシュする問題を修正しました。
    ([UUM-157945](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157945))

- `Shaders`: メインテクスチャが存在しない場合、Material.mainTexture はコンソールにエラーを記録するのではなく、null を返すようになりました。
    ([UUM-103940](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-103940))

- `SRP Core`: ビルドターゲットがモバイルプラットフォームの場合、TraceVirtualOffset シェーダーにおける型が小さい型への変換に関するシェーダー警告を修正しました。
    ([UUM-157091](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157091))

- `uGUI`: スライス画像、タイル画像、テキストなどの UI 要素が、最初に描画された後にキャンバスの「単位あたりの参照ピクセル数」、「スケール係数」、「ピクセルパーフェクト」、または「レンダリングカメラ」が変更された際に更新されない問題を修正しました。
    ([UUM-151004](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151004))

- `UI Toolkit`: キーの値が非常に大きい場合、保存後に AnimationCurve の UXML 属性の値が失われる問題を修正しました。
    ([UUM-156823](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156823))

- `UI Toolkit`: テキストで、アトラスのパディングが小さく、アウトライン幅がゼロまたは負の値であるフォントアセットを使用した場合、文字の周囲にアーティファクトが発生する問題を修正しました。
    ([UUM-146020](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146020))

- `UI Toolkit`: レイアウト内で「Render Graph Viewer」などのウィンドウが開いた状態でエディタを起動した際に、ログに記録されていたエラーを修正しました。
    ([UUM-150211](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150211))

- `UI Toolkit`: スケールされた要素にフィルターを適用した際に、ぼやけて見える問題を修正しました。
    ([UUM-155303](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-155303))

- `UI Toolkit`: WebGL 2 および一部の OpenGL ES 3.0搭載デバイスで、ベクター画像に保存された際に単色塗りやグラデーション塗りが欠落する問題を修正しました。また、テクスチャ塗りの前に単色塗りやストロークが描画された際に発生していたArgumentOutOfRangeExceptionも修正しました。
    (UUM-155233)

- `UI Toolkit`: バックグラウンドフィルターチェーン内の不透明度処理後や、フィルター処理された要素のアンチエイリアス処理されたエッジなど、半透明のピクセルにおいて、反転およびコントラストフィルターが過度に明るい色を生成する問題を修正しました。
    (UUM-155804)

- `UI Toolkit`: 要素名にスペースが含まれる要素のオーバーライドを編集する際、UI Builder が「Attribute Overrides」に重複した属性を追加し、その結果 UXML ファイルが無効になる問題を修正しました。
    ([UUM-149755](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149755))

- `UI Toolkit`: UIToolkitInteroperabilityBridge が、各 UI Toolkit パネルに対して毎フレーム GC メモリを割り当てていた問題を修正しました。
    ([UUM-158158](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158158))

- `URP`: 一部の Enum マテリアルプロパティに「Default」が追加される問題を修正しました。
    ([UUM-134256](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134256))

- `URP`: 追加のライトシャドウが無効化されているが、シャドウマスクが有効になっている状態でディファードレンダリングを使用する際、URPがストリップドバリアントを使用しようとするバグを修正しました。
    ([UUM-153600](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153600))

- `URP`: 「Render Scale」が 1 に設定されていない状態で「Forward+」レンダリングパスを使用すると、一部の iOS デバイスでクラッシュする問題を修正しました。
    ([UUM-151281](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151281))

- `URP`: Depth/ステンシルバッファが無効になっている2Dレンダラーと併用した場合、URPのRenderGraphサンプル内の「Renderer List」および「Culling」サンプルが毎フレームエラーを記録していた問題を修正しました。
    ([UUM-157948](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157948))

- `URP`: 同じエディターセッション内で、以前に「LODクロスフェードをサポート」が有効なシェーダーグラフがインポートされていたかどうかに応じて、シェーダーグラフが異なるシェーダーコードとしてインポートされたり、アセットバンドルのハッシュ値が異なったりする問題を修正しました。
    (UUM-155529)

- `URP`: 非推奨となっている `LightingPhysicallyBased` のオーバーロードが、表面法線を無視し、スペキュラーハイライトのトグルを視線方向として使用していた問題を修正しました。
    (UUM-149002)

- `VFX Graph`: ビジュアルエフェクト領域内のすべてのネイティブ割り当てにネイティブルートが割り当てられ、メモリリークが発生しないようにしました。
    (UUM-126944)

- `VFX Graph`: ビジュアルエフェクトグラフの出力をソートした際、エフェクトのインスタンスの一部がカメラの視野外にある場合（特に複数のカメラを使用している場合）、GPUがクラッシュしたりレンダリングが破損したりする問題を修正しました。
    (UUM-149758)

- `XR`: サブシステムが破棄された後に `SubsystemWithProvider.Start` を呼び出した際、`ArgumentNullException` が発生せず、破棄されたプロバイダーが再起動してしまう問題を修正しました。
    ([UUM-151411](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151411))




## 6000.3.28f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.collab-proxy`: [2.13.6](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.13//changelog/CHANGELOG.html) から [2.14.0](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.14//changelog/CHANGELOG.html) へ

- `com.unity.probuilder`: [6.1.3](https://docs.unity3d.com/Packages/com.unity.probuilder@6.1//changelog/CHANGELOG.html) から [6.1.4](https://docs.unity3d.com/Packages/com.unity.probuilder@6.1//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: [3.8.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.8//changelog/CHANGELOG.html) から [3.8.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.8//changelog/CHANGELOG.html) へ

- `com.unity.services.cloud-build`: [2.1.0](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.1//changelog/CHANGELOG.html) から [2.1.1](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.1//changelog/CHANGELOG.html) へ

- `com.unity.services.wire`: [1.6.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.6//changelog/CHANGELOG.html) から [1.6.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.6//changelog/CHANGELOG.html)

- `com.unity.xr.compositionlayers`: [2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.6//changelog/CHANGELOG.html) から [2.6.1](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.6//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: [1.1.12](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) から [1.2.0](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.2//changelog/CHANGELOG.html) へ

- `com.unity.services.multiplayer`: [2.4.0](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.4//changelog/CHANGELOG.html) から [2.4.1](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.4//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.12.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.12//changelog/CHANGELOG.html) から [1.12.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.12//changelog/CHANGELOG.html) へ

**追加されたパッケージ**

- [com.unity.steamworks-api@1.0.0](https://docs.unity3d.com/Packages/com.unity.steamworks-api@1.0//changelog/CHANGELOG.html)