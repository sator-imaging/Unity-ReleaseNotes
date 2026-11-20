# Unity 6000.3.29f1 LTS
公開日時：2026年11月19日（木）10:35:33 GMT  
https://unity.com/releases/editor/whats-new/6000.3.29f1

# 6000.3.29f1 の既知の問題

- `Android`: 「バックグラウンドで実行」と「予測バック機能のサポート」が有効になっている場合、バックグラウンドから復帰した後に「戻る」ジェスチャーまたはボタンを押すとアプリが終了してしまう
    ([UUM-159613](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159613))

- `エディタインストーラ`: [macOS] プレイヤーライブラリは、特注の権限でコード署名されている
    ([UUM-156884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156884))

- `Mecanim アニメーション`: レガシーな Animation コンポーネントによってアニメーション化されたオブジェクトに対し、AddClip が呼び出された後に、そのオブジェクトを破棄する際に Animation::AnimationObjectDeletionCallback でクラッシュする
    ([UUM-161463](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-161463))

- `Mecanim Animation`: プロパティ名が空の Transform カーブを持つ AnimationClip をサンプリングした際、UnityEngine::Animation::SetBoundCurveFloatValue の実行中にクラッシュする
    ([UUM-161382](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-161382))

- `マルチプレイヤー FPS/サードパーソン テンプレート`: マルチプレイヤー FPS テンプレートを使用したプロジェクトでプレイモードに入ると、memcpy 実行時にクラッシュする
    ([UUM-151778](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151778))

- `検索`: ドメインの再読み込み後に SearchService.Request を呼び出すと、検索データベースがリークする
    ([UUM-161715](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-161715))

- `SRP Foundation`: デバイスを物理的に回転させた際、RenderPass に関連する Android エラーが Logcat およびコンソールに記録される
    ([UUM-157974](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157974))



# 6000.3.29f1 リリースノート

## 改善点

- `Graphics`: 非同期アップロードバッファが破損した場合にレンダリングスレッドがフリーズするのを防ぎ、その場合はリリースビルドでもエラーをログに記録するようにしました。
    (UUM-150567)

- `uGUI`: スクリプト定義シンボル `DISABLE_UGUI_UITK_SUPPORT` を追加しました。これにより、uGUI と UI Toolkit の統合が除外され、UI Toolkit がエディタ内でのみ使用される場合、プレイヤービルドで UI Toolkit モジュールを削除できるようになりました。
    (UUM-159610)

- `URP`: Forward+ および Deferred+ レンダリングパスは、遠方平面の向こう側、または正射影カメラの近方平面の手前にある領域にのみ到達するライトやリフレクションプローブを、処理しなくなりました。



## 変更点

- `Profiler`: Android において、「App Committed Memory」カウンターが、常駐メモリとスワップされたメモリの合計値を返すように変更されました。
    (UUM-155041)

- `Text`: FreeType をバージョン 2.15.0 に更新しました。これにより、macOS での Apple Color Emoji グリフのミラーリングがサポートされ、「Hinted Smooth」および「OS Default」フォントレンダリングモードでのテキストのレンダリング方法が若干変更されました。



## 修正

- `2D`: 「Mask Interaction」が「None」に設定された LineRenderer または TrailRenderer が、同じマテリアルを使用し「Mask Interaction」が有効になっている別の LineRenderer または TrailRenderer によって、スプライトマスクによってクリップされてしまう問題を修正しました。
    ([UUM-158602](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158602))

- `2D`: SpriteShapeUtility.Generate に、2 つの制御点が一致する閉じた形状が渡された際に、「pqInit」でクラッシュする問題を修正しました。<br>
    なお、この API は旧バージョンの Spriteshape パッケージ固有のものであり、今後のバージョンで非推奨となる予定です。 今後、Triangulation を使用する場合は、Spriteshape パッケージ内の SpriteShapeGenerator.cs を参照してください。
    ([UUM-156213](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156213))

- `2D`: 2D レンダラーの深度/ステンシルバッファ設定が無効になっている場合、一部の OpenGL ES デバイスでスプライトや UI がレンダリングされない問題を修正しました。
    ([UUM-159093](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159093))

- `アクセシビリティ`: UI Automation クライアント（例：スクリーンリーダー）が実行されている際に、Windows プレイヤーが終了時にクラッシュする問題を修正しました。
    ([UUM-157903](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157903))

- `Android`: Bouncy Castle を \(1.70 から 1.86 へ\) アップグレードしました。Keystore Manager によって作成される新しい署名鍵では、2048 ビット RSA および SHA1withRSA の代わりに、4096 ビット RSA および SHA256withRSA 証明書が使用されます。 既存の鍵は変更されません。
    (UUM-156925)

- `Android`: 「デフォルトの向き」が「自動回転」に設定され、「自動回転の動作」が「ユーザー」に設定されている場合、ユーザーが画面をロックした向きにアプリケーションが回転しない問題を修正しました。
    (UUM-158455)

- `Android`: カーソルがロックされている状態でマウスを動かすとスクロール値が生成される問題を修正しました。
    ([UUM-156720](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156720))

- `Android`: 入力デバイスからタッチパッドの入力ソースが報告されていない場合、タッチパッド入力が無視され、エラーがログに記録される問題を修正しました。
    (UUM-159337)

- `Android`: eMudhraの中間証明書のセキュリティ上の脆弱性を修正するため、OpenJDKを17.0.18+8から17.0.21+9に更新しました。
    ([UUM-158390](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158390))

- `Android`: バンドルされている Android SDK の cmdline-tools を 21.0 に更新し、その avdmanager を使用して作成された Android 17 (API 37.0) 向けエミュレータが正しく起動するようにしました。
    (UUM-157110)

- `アセットのインポート`: アセットの再インポート時に、まだ読み込まれたままのオブジェクトがアンロードされた場合、エディタの「トランスフォーム」でクラッシュする問題を修正しました。
    (UUM-126651)

- `アセットパイプライン`: macOS の exFAT ドライブ上でプロジェクトを作成したりフォルダを複製したりした際に、「ファイルが存在します」というエラーが表示される問題を修正しました。
    ([UUM-150634](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150634))

- `オーディオ`: クワッドスピーカーモードで、2チャンネル以上が出力されないバグを修正しました。
    ([UUM-146928](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146928))

- `Audio`: Unityがオーディオ出力の再開に失敗した後、オーディオ出力デバイスが再接続された際にエディターで発生していた致命的なエラーを修正しました。
    ([UUM-158166](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158166))

- `DX12`: Direct3D12 をサポートしていないプラットフォームにおいて、Player Settings に使用できない D3D12 デバイスフィルタリング設定が表示される問題を修正しました。
    (UUM-149251)

- `エディター`: Unityエディターのソフトウェア利用規約に同意しておらず、利用規約ファイルが存在しない、空である、 読み取れない場合に発生するクラッシュを修正しました。
    ([UUM-154911](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154911))

- `エディタ`: 複雑なジェネリック型で `EditorApplication.delayCall` コールバックが宣言されているプロジェクトにおいて、[ヘルプ] > [バグを報告] を開くか、エディタを終了した際に発生していたクラッシュを修正しました。
    ([UUM-122928](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-122928))

- `エディタ`: ツールコンテキストのオーバーレイが表示されているが折りたたまれている状態で、階層ビューで GameObject を選択した際に NullReferenceException が発生する問題を修正しました。
    ([UUM-141529](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141529))

- `エディタ`: macOS でエディタを終了する際に断続的に発生していたクラッシュを修正しました。
    ([UUM-160348](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-160348))

- `エディタ`: Android XR などのパッケージをインストールするビルドプロファイルを作成する際、パッケージのインポートが完了する前にプロファイルが設定され、その結果、品質レベルにレンダリングパイプラインアセットが設定されない問題を修正しました。
    (UUM-156303)

- `エディタ`: `Instantiate` では親トランスフォームのスケールが考慮されるのに対し、`InstantiateAsync` では考慮されなかったバグを修正しました。
    ([UUM-154591](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154591))

- `エディター`: スクリプトで `UnityEngine.Device.SystemInfo.processorModel、processorManufacturer、または supportsMachineLearning を使用しているスクリプトで、プレイヤービルドがエラー CS0117 で失敗する問題を修正しました。
    ([UUM-154729](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154729))

- `エディタ`: 「自動保存」が有効な状態で名前フィールドを選択した後、プレハブのフィールドが部分的にしか保存されない問題を修正しました。
    ([UUM-157667](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157667))

- `エディタ`: レンダリンググラフが有効な状態で、キューブマップを宛先とするレンダリングリクエストで何も表示されない問題を修正しました。
    (UUM-147726)

- `エディタ`: ドメインのリロード中に、CloudJob ワーカースレッドの ujob_execute_job でエディタがクラッシュし、次のドメインリロード時にハングアップすることがある問題を修正しました。ドメインリロード中に Analytics が再起動し、その最初にキューに入れられたジョブが、再起動前のジョブに依存している可能性があるためです。
    ([UUM-158326](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158326))

- `Editor`: 高ポーリングのマウスを使用している際に、WinEditorのPlayModeで発生するFPSの遅延を軽減する。
    ([UUM-142550](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142550))

- `エディタ`: Windowsエディタ向けに、同梱のVCRedistをバージョン14.51.36247に更新しました。
    (UUM-156578)

- `エディタ`: グラフィックスジョブが有効な場合、エディタはフレーム中にコンパイルされたシェーダーバリアントを持つレンダラーを描画するようになりました。 以前はシェーダーの欠落により空白となっていたアセットのプレビューやワンショットレンダリングが、SRPバッチャーによるフォールバックパスを通じて期待通りに描画されるようになりました。
    (UUM-147205)

- `エンジン診断`: ANRレポートは、応答を停止したプロセスの最後のセッションに紐付けられるようになりました。
    (UUM-157717)

- `エンジン診断`: リモート設定の前にキャプチャされたクラッシュ、例外、およびANRレポートは、発生したセッションを含む重要な属性を保持するようになりました。
    (UUM-159169)

- `Engine Diagnostics`: Engine Diagnostics の設定が適用されている最中に、ワーカースレッドからクラッシュレポートが記録された際に発生する可能性があったクラッシュを修正しました。
    (UUM-158113)

- `Engine Diagnostics`: Android アプリが起動時に余分なセッションを報告し、その結果、最初のセッションが無効なタイムスタンプで終了してしまう問題を修正しました。
    (UUM-157715)

- `GI`: APV を使用し、L2 球面調和関数が無効になっている場合に、混合光が完全に遮蔽されて表示されるバグを修正しました。
    ([UUM-156430](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156430))

- `GI`: URP固有の設定のみを変更した場合、ライティングのベイク処理時にリフレクションプローブが再ベイクされないことがある不具合を修正しました。
    ([UUM-133949](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-133949))

- `GI`: Unity Compute ライトベーカーを使用する際、macOS 上でプローブのオクルージョンが正しくベイクされない問題を修正しました。
    ([UUM-160178](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-160178))

- `Graphics`: GraphicsStateCollection.WarmUpProgressively を使用してパイプライン状態オブジェクトをプリウォームする際、Vulkan で発生していたクラッシュを修正しました。
    (UUM-154071)

- `Graphics`: Crunch圧縮されたキューブマップが半解像度以下でストリーミングされる際、シーンの読み込み中に発生する可能性のあるフリーズまたはクラッシュを修正しました。
    (UUM-150567)

- `Graphics`: 有効なアタッチメント形式がまだ設定されていないスワップチェーンに直接レンダリング中にシェーダーパスが適用された際に発生する可能性のあるVulkanのクラッシュを修正しました。
    ([UUM-134018](https://issuetracker.unity3d.com/issues/crash-on-nvoglv64-vkgetinstanceprocaddr-when-starting-the-project-with-vulkan-and-test-framework-performance))

- `Graphics`: Direct3D 12 グラフィックス API を使用してエディタで RenderDoc を読み込んだ際に、コンソールにアサーションエラーが記録される問題を修正しました。
    (UUM-115796)

- `Graphics`: `-batchmode -quit` オプションを指定してプロジェクトをインポートした際、URP および HDRP でマテリアルがアップグレードされない問題を修正しました。
    ([UUM-153768](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153768))

- `Graphics`: GPU がそのフォーマットをサポートしていない場合や、ミップレベルが 4x4 未満、あるいは 4 の倍数でない場合など、BC 圧縮されたテクスチャが CPU 上で解凍される際に発生するメモリ破損を修正しました。
    (UUM-154799)

- `Graphics`: Graphics: GraphicsState.SetMeshData を使用して作成されたスキン付きメッシュの GraphicsStateCollection をウォームアップすると、描画と一致しないパイプラインが生成され、Vulkan での最初の描画時にもそのパイプラインが作成されてしまう問題を修正しました。
    (UUM-156721)

- `Graphics`: Vulkan スワップチェーンにおける予期しない失敗が、正しくログに記録されるようになりました。
    ([UUM-153744](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153744))

- `Graphics`: Vulkan: グラフィックスジョブが有効な状態でシェーダーをアンロードおよびリロードした際、無効なシェーダーモジュールによって引き起こされていたランダムなクラッシュを修正しました。
    (UUM-136086)

- `ライセンス`: Unity ライセンス クライアントに接続できない場合、エディタがライセンスなしで動作を継続し、バッチモードでコード 0 を返して終了してしまう問題を修正しました。
    ([UUM-151817](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151817))

- `Linux`: プロジェクトの読み込み中にウィンドウマネージャーがエディタの起動画面を閉じた際に、Linuxでクラッシュする問題を修正しました。
    ([UUM-132175](https://issuetracker.unity3d.com/issues/linux-crash-on-editorlaunchscreen-platformeditorlaunchscreen-setprogress-when-opening-a-project))

- `Linux`: ツールチェーンが DWARF v5 (Clang 15 以降) を出力する際、Linux 上で il2cpp.usymが、ツールチェーンがDWARF v5（Clang 15以上）を出力する際、Linux上で使用可能なソースパスなしで生成される問題を修正しました。
    (UUM-150040)

- `ネットワーク`: デフォルトの乱数シードデバイスを `/dev/random` から `/dev/urandom` に変更しました。

- `Player`: 高ポーリングのマウスを使用している際の、Window Standalone プレイヤーにおける FPS ラグを軽減しました。
    ([UUM-147395](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147395))

- `プロファイラ`: プロファイラレコーダーの容量を超過してラップした際、`ProfilerRecorder.ToArray` がレコーダーが保持しているサンプル数よりも少ないサンプル数を返す問題を修正しました。
    ([UUM-159078](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159078))

- `スクリプティング`: `Object.Instantiate` の `InstantiateParameters` 引数で永続的な親オブジェクトが渡される問題を修正しました。現在はエラーをログに記録し、他の `Instantiate` オーバーロードと同様に、親オブジェクトなしでオブジェクトを作成します。
    (UUM-150465)

- `スクリプティング`: ハッシュコードが異なるプレーンに対して `Plane.Equals` が `true` を返す問題を修正しました。これにより、HashSet および Dictionary での検索が失敗していました。
    ([UUM-157345](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157345))

- `スクリプティング`: ScriptUpdaterの実行時にエディタが長時間フリーズする可能性があった問題を修正しました。
    (UUM-154695)

- `シリアライゼーション`: Playerで読み込まれた、またはAssetBundleから読み込まれたプレハブの下にシーンのGameObjectが配置され、Resources.UnloadUnusedAssetsによってそのプレハブがアンロードされた際に発生していたクラッシュを修正しました。
    (UUM-150465)

- `シリアライゼーション`: 同じ名前でエディタ用とプレイヤー用の別々のバリアントを持つプリコンパイル済みアセンブリを使用するシーンを読み込んだ際に、プレイヤーがクラッシュする問題を修正しました。
    ([UUM-157381](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-157381))

- `シェーダー`: エディターでのキーワードのオーバーライドを防ぐよう、マテリアルプロパティを調整しました。
    ([UUM-133561](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-133561))

- `Shaders`: エディタでのキーワードのオーバーライドを防ぐため、マテリアルプロパティを修正しました。
    ([UUM-76775](https://issuetracker.unity3d.com/issues/material-dot-enablekeyword-method-has-手動でインスタンス化されたマテリアルで呼び出した際にマテリアルに影響がない場合))

- `Shaders`: プリロードされた ShaderVariantCollection を使用してシーンを繰り返し切り替えた際に、プレイヤーがフリーズする問題を修正しました。
    ([UUM-156125](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156125))

- `Shaders`: バックグラウンドでシェーダーバリアントがコンパイルされている最中にシェーダーメッセージが読み込まれた際、エディタがクラッシュする可能性があった問題を修正しました。
    (UUM-154510)

- `Shaders`: グラフィック設定およびビルドプロファイル内の「最初のシーン表示後にシェーダーをプリロードする」オプションが、チェックを入れた後に自動的にチェックが外れ、「1フレームあたりのプリロード時間制限 \(ms\)」 が -1 と表示される問題を修正しました。
    ([UUM-151773](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151773))

- `シェーダー`: `#line` ディレクティブで終わるシェーダーファイルをインポートした際にエディタがクラッシュする問題を修正しました。
    (UUM-159786)

- `シェーダー`: ベースマテリアルが変更された後、中間バリアントがそのプロパティをロックしていた場合、マテリアルバリアントが古いプロパティ値を維持してしまう問題を修正しました。
    ([UUM-158581](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158581))

- `SRP Core`: 8つのラスタライズ・レンダリング・パスを超えると、ネイティブ・サブパスが8つ未満の場合でも、レンダリング・グラフがネイティブ・レンダリング・パスを終了してしまう問題を修正しました。これにより、URP UIオーバーレイなどの次のパスが、アタッチメントをメモリから再度読み込む必要がありました。
    ([UUM-158401](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158401))

- `Text`: 不正な形式の可変フォントを読み込んだ際に、範囲外読み取りを引き起こす可能性があった FreeType の脆弱性 \(CVE-2026-23865\) を修正しました。
    ([UUM-140975](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140975))

- `TextMeshPro`: TMP Essential Resources をインポートした後、TMP Importer ウィンドウを閉じると発生する可能性があった「TextMesh Pro Essential Resources are missing」というエラーを修正しました。
    ([UUM-147231](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147231))

- `UI Toolkit`: カラーストップのないグラデーションを含む SVG ファイルをインポートした際に発生していた NullReferenceException を修正しました。
    ([UUM-159742](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159742))

- `UI Toolkit`: 別のListView内にネストされたListView内の項目をクリックまたはドラッグすると、親となるListViewの項目も選択またはドラッグされてしまう問題を修正しました。
    ([UUM-140195](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140195))

- `UI Toolkit`: ハッシュコードが異なる行列に対して、`Matrix2D.Equals(Matrix2D)` が true を返す問題を修正しました。
    ([UUM-158175](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158175))

- `UI Toolkit`: クリップ対象の要素にトランスフォームが適用されている場合、objectBoundingBox単位のSVGクリップパスおよびマスクの位置がずれる問題を修正しました。
    ([UUM-159735](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159735))

- `UI Toolkit`: 「アンチエイリアスされた円弧エンコーディング」のテッセレーションモードで「ベクター画像」としてインポートされた SVG ファイルにおいて、objectBoundingBox 単位のクリップパスまたはマスクを使用すると、内容が空として表示される問題を修正しました。
    ([UUM-159735](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159735))

- `UI Toolkit`: 「&lt;radialGradient&gt;」の半径が 0 の場合、SVG インポート時に無効な放射状グラデーションが生成される問題を修正しました。形状は、最後のストップの色で塗りつぶされるようになりました。
    ([UUM-158256](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158256))

- `UI Toolkit`: SVGのインポート時に、そのシェイプまたはグループのターゲットがファイル内の後方で定義されている場合、「&lt;use&gt;」要素が削除されてしまう問題を修正しました。
    ([UUM-158220](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158220))

- `UI Toolkit`: SVGのインポート時に、グラデーションがファイルの後半で定義されている場合、グラデーションのストロークが省略されてしまう問題を修正しました。
    ([UUM-158255](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158255))

- `UI Toolkit`: SVG インポート時に、半径が 0 の点が 1 つだけ含まれる円弧が省略される問題を修正しました。この円弧は、直線として描画されるようになりました。
    ([UUM-158225](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158225))

- `UI Toolkit`: SVGのインポート時に、後続の「&lt;style&gt;」要素が同じセレクタに対して他のプロパティを設定している場合、先行する「&lt;style&gt;」要素の宣言が削除されてしまう問題を修正しました。
    ([UUM-158217](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158217))

- `UI Toolkit`: SVG インポート時に、「&lt;style&gt;」要素内の「@import」ステートメントの後に続くスタイルルールが削除されてしまう問題を修正しました。
    ([UUM-158228](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158228))

- `UI Toolkit`: SVGのインポート時に、「&lt;style&gt;」要素内の「@media」ブロックの後に続くスタイルルールが削除されてしまう問題を修正しました。
    ([UUM-158229](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158229))

- `UI Toolkit`: 複数の要素がファイルの後半で定義された「&lt;clipPath&gt;」を使用している場合、SVGのインポート時に要素がクリップされない問題を修正しました。
    ([UUM-158251](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158251))

- `UI Toolkit`: SVG インポート時に、ファイル内の「&lt;style&gt;」要素より前にある要素に「&lt;style&gt;」ルールが適用されない問題を修正しました。
    ([UUM-158230](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158230))

- `UI Toolkit`: 「&lt;use&gt;」要素が別の「&lt;use&gt;」要素を参照している場合に、SVGインポートでKeyNotFoundExceptionが発生する問題を修正しました。
    ([UUM-158249](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158249))

- `UI Toolkit`: 「mask」属性が、ファイルの後半で定義された「&lt;mask&"を参照している場合、またはマスクが存在しない場合に、ArgumentNullExceptionが発生する問題を修正しました。
    ([UUM-158239](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158239))

- `UI Toolkit`: 「&lt;polygon&gt;」または「&lt;polyline&gt;」のポイントが「-10-10」のように区切られていない場合に、SVGのインポートでエラーが発生する問題を修正しました。
    ([UUM-158257](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158257))

- `UI Toolkit`: プロパティが「inherit」に設定されている場合に、SVGのインポートでエラーが発生する問題を修正しました。
    ([UUM-158226](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158226))

- `UI Toolkit`: 一部の曲線ベジェセグメントに対して、VectorUtils.Bounds が小さすぎる境界を返す問題を修正しました。
    ([UUM-158205](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158205))

- `UI Toolkit`: 境界が y = 0 から始まらない場合、VectorUtils.FlipVerticesInBounds が、境界が y = 0 から始まらない場合に頂点を境界の外側に移動してしまう問題を修正しました。
    ([UUM-158215](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158215))

- `UI Toolkit`: スイープ角度が 0 の場合に VectorUtils.MakeArc が 4 分の 1 の円を返す問題を修正しました。
    ([UUM-158218](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158218))

- `UI Toolkit`: スイープ角度が円周全体の場合に、VectorUtils.MakeArc が空のパスを返す問題を修正しました。
    ([UUM-158219](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158219))

- `UI Toolkit`: VectorUtils.SceneNodeBounds が、閉じた輪郭の閉曲線を無視してしまう問題を修正しました。
    ([UUM-158209](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158209))

- `UI Toolkit`: VectorUtils.SegmentsLength が、閉じたパスの閉曲線を直線として計測してしまう問題を修正しました。
    ([UUM-158208](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158208))

- `URP`: DX11バックエンドで動作するChromium上でWebGLを使用する際、ライトが誤った形状でレンダリングされるバグを修正しました。
    ([UUM-142771](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142771))

- `URP`: レンダーパイプラインコンバーターがプレハブを「変換済み」と報告したものの、開いていないシーン内のオブジェクトも同時に変換した際に、プレハブの変更内容が失われる問題を修正しました。
    ([UUM-160400](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-160400))

- `URP`: ライトがカメラにアタッチされている場合、Forward+ および Deferred+ モードにおいて、スポットライトの端にブロック状の隙間が生じる問題を修正しました。
    ([UUM-154016](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154016))

- `URP`: 特定のスポットライトの向きや、カメラのニアプレーンに近いスポットライトにおいて、Forward+ または Deferred+ レンダリングパスを使用している際に、画面の一部でライトが表示されない問題を修正しました。

- `URP`: Forward+ および Deferred+ において、画面の端やカメラのニアプレーン付近でポイントライトやスポットライトが消えてしまう問題を修正しました。
    ([UUM-146356](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146356))

- `URP`: ボーンが動いていない状態でスプライトが反転された際、スプライトスキンの「Shadow Caster 2D」が反転されていない影を維持してしまう問題を修正しました。
    ([UUM-158409](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158409))

- `URP`: Forward+ または Deferred+ レンダリングパスを使用する際、カメラ後方のスポットライトの照らされる領域の上部が失われる問題を修正しました。
    ([UUM-159132](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-159132))

- `URP`: スタンドアロン版の URP 2D/3D アプリケーションにおけるマルチディスプレイ対応を修正しました。
    (UUM-155833)

- `VFX Graph`: URP 用のパイプラインタグを追加しました。
    ([UUM-160198](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-160198))

- `VFX Graph`: HLSL ソースが空白で始まる場合、カスタム HLSL ブロックおよび演算子が無効なシェーダーコードを生成する問題を修正しました。
    ([UUM-158603](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-158603))

- `XR`: XRの深度スワップチェーンに、誤ったスケールで深度が送信される問題を修正しました。
    ([UUM-149514](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149514))




## 6000.3.29f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.ads.ios-support`: [1.0.1](https://docs.unity3d.com/Packages/com.unity.ads.ios-support@1.0//changelog/CHANGELOG.html) から [1.3.0](https://docs.unity3d.com/Packages/com.unity.ads.ios-support@1.3//changelog/CHANGELOG.html)

- `com.unity.services.friends`: [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.3//changelog/CHANGELOG.html) から [1.4.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.4//changelog/CHANGELOG.html) へ

- `com.unity.splines`: [2.9.1](https://docs.unity3d.com/Packages/com.unity.splines@2.9//changelog/CHANGELOG.html) から [2.9.2](https://docs.unity3d.com/Packages/com.unity.splines@2.9//changelog/CHANGELOG.html)

- `com.unity.test-framework.performance`: [3.5.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.5//changelog/CHANGELOG.html) から [3.7.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.7//changelog/CHANGELOG.html) へ

- `com.unity.visualscripting`: [1.9.12](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) から [1.9.13](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) へ

- `com.unity.xr.oculus`: [4.5.2](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html) から [4.5.6](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html) へ

- `com.unity.netcode.gameobjects`: [2.13.3](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html) から [2.14.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.14//changelog/CHANGELOG.html)

- `com.unity.dt.app-ui`: [2.2.4](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@2.2//changelog/CHANGELOG.html) から [2.3.1](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@2.3//changelog/CHANGELOG.html)

- `com.unity.cloud.draco`: [5.5.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.5//changelog/CHANGELOG.html) から [5.6.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.6//changelog/CHANGELOG.html) へ

- `com.unity.cloud.ktx`: [3.7.1](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.7//changelog/CHANGELOG.html) から [3.8.0](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.8//changelog/CHANGELOG.html) へ