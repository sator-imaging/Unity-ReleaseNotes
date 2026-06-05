# Unity 6000.3.17f1 LTS
公開日時: 2026年6月4日(木) 13:42:33 GMT  
https://unity.com/releases/editor/whats-new/6000.3.17f1

# 6000.3.17f1 の既知の問題

- `6000.0.61f1`: SDF16 または SDF32 を使用してフォントアトラスを生成する際、tlsf_free でクラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true) および UseTexture を指定して AddComputePass を使用する際、D3D12SwapChain::Present でクラッシュする
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.2.0a8`: スクリプティング ドメインのテアダウン後に非同期 HTTP コールバックが実行されると、Scripting::LogException でクラッシュする
    ([UUM-141434](https://issuetracker.unity3d.com/issues/crash-on-scripting-logexception-when-async-http-callback-executes-after-scripting-domain-teardown))

- `6000.3.15f1`: [Windows] パッケージのインストール時に「EPERM: operation not permitted」エラーが発生し、非決定的に失敗する
    ([UUM-142421](https://issuetracker.unity3d.com/issues/package-installation-fails-パッケージのインストール時に「EPERM: operation not permitted」エラーが発生し、非決定的に失敗する))

- `6000.5.0a6`: 特定のプロジェクトでプレイモードに入ると、PhysicsCommands::PhysX::BodySetPose でクラッシュする
    ([UUM-143658](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodysetpose-when-entering-play-mode-in-a-specific-project))

- `6000.5.0a7,6000.0.69f1,6000.3.11f1,6000.4.0b11`: [Android][GameActivity] アプリがバックグラウンド中にフォアグラウンドサービスが起動した際、アプリを終了した後、再起動に失敗する
    ([UUM-143555](https://issuetracker.unity3d.com/issues/android-gameactivity-app-fails-to-relaunch-after-it-was-closed-when-a-foreground-service-started-while-app-was-backgrounded))

- `アセットインポーター`: プレイモードに入ると、「(Unity) WriteObjectToVector」でエディターがクラッシュする
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- テキスト (TextMeshPro): TMPro Font Asset Creator でマルチスレッドのフォントアトラスを生成する際、UNITY_FT_Load_Glyph でクラッシュする
    ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

エディタでさまざまな操作を実行すると mdb_cursor_sibling でクラッシュする
    ([UUM-141720](https://issuetracker.unity3d.com/issues/crash-on-mdb-cursor-sibling-when-performing-various-actions-in-the-editor))

bee_backend が複数実行されているときに mono_log_write_logfile でクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))



# 6000.3.17f1 リリースノート

## 改善点

- `エディタ`: オーバーレイモードで「法線」または「接線」が有効になっている場合、Canvas コンポーネントの下に表示されていた警告を削除しました。
    ([UUM-137367](https://issuetracker.unity3d.com/issues/additional-shader-channel-keeps-reverting-when-saving-prefab))

- `Shaders`: 変更が未適用な状態でシェーダービルド設定UIから移動した際に表示される「未適用変更」ダイアログを追加しました。



## 変更点

- `Android`: Gradle を 9.1.0 に、AGP を 9.0.0 にアップグレードしました。



## 修正

- `2D`: SpriteSkin を持つスプライトが、Sprite Atlas V2 パッキングを有効にした状態で「SpriteAtlasManager.atlasRequested」経由で Addressables SpriteAtlas をロードしている場合、エディタのプレイモードで表示されない問題を修正しました
    (UUM-137123)

- `2D`: シーンビューまたはタイルパレットウィンドウの外でマウスボタンを離した際、タイルマップ上の「選択」、「ピック」、「ボックス」、「移動」ツールの操作が適切にキャンセルまたは確定されない問題を修正しました。
    ([UUM-139284](https://issuetracker.unity3d.com/issues/drag-selecting-on-tilemap-gameobject-outside-of-scene-view-causes-the-selection-mode-get-stuck-on-mosue))

- `2D`: ブラシ選択リストビューにおいて、ユーザーがリストビューのすべての列を無効にすると、エラーメッセージが表示され、SceneViewが消失する問題を修正しました。
    ([UUM-141552](https://issuetracker.unity3d.com/issues/all-tile-palette-brush-pick-overlays-columns-can-be-disabled-that-leads-to-nullreferenceexception-errors-being-spammed))

- `2D`: Gridにゼロ以外のセル間隔値が設定されている場合、GetCellCenterLocal/Worldからの戻り値に関する問題を修正しました。
    (UUM-137327)

- `Android`: フルスクリーンモードでタッチスクリーンキーボードを閉じた後、ナビゲーションバーが表示されてしまう問題を修正しました。
    ([UUM-142004](https://issuetracker.unity3d.com/issues/android-navigation-bar-does-not-go-away-when-tapping-on-the-screen-to-close-the-keyboard))

- `Android`: カスタム Gradle テンプレートが選択されている場合のソースビルドを修正しました。
    (UUM-138551)

- `Animation`: レガシーアニメーションシステムにおける精度の不一致により、高フレームレート時にアニメーションイベントがスキップされる問題を修正しました。
    ([UUM-138951](https://issuetracker.unity3d.com/issues/the-animation-event-is-not-triggered-when-the-frame-rate-is-set-to-120-on-the-s26-ultra))

- `Animation`: プレイモードへの移行または終了時に、選択範囲に未解決の GameObject 参照が残ってしまう問題を修正しました。
    (UUM-142098)

- `Animation`: ドープシートでトランスフォームとスプライトのキーフレームが混在している箇所を右クリックした際のエラーを修正しました。
    ([UUM-142341](https://issuetracker.unity3d.com/issues/errors-are-thrown-and-contextual-menu-does-not-open-when-right-clicking-multiple-mixed-keyframes-in-dopesheet))

- `Audio`: すべての AudioListener コンポーネントが無効化されているか、その GameObject が無効化されている場合でも、Player ビルドでオーディオの再生が継続されるようになりました。
    ([UUM-127556](https://issuetracker.unity3d.com/issues/audiolisteners-still-listen-to-audio-when-their-components-are-disabled-in-player))

- `Audio`: プレイモード中に `AudioListener` で `OnAudioFilterRead` エフェクトを有効にしても、`MonoBehaviour` が無効な状態で開始された場合、音が出ない問題を修正しました。
    ([UUM-116871](https://issuetracker.unity3d.com/issues/onaudiofilterread-does-not-affect-signal-on-audiolistener-after-enable))

- `ビルドパイプライン`: 初期ハッシュマップサイズを指定する BootConfig キー "remapper-initial-capacity" を使用して、PersistentManager.Remapper の容量を確保する機能を追加しました。
    (UUM-136275)

- `ドキュメント`: 2D コライダーのリファレンスページにおける Vale のエラーを修正しました。

- `DX12`: メモリ負荷の高い操作を実行した際に DX12 で発生するクラッシュを修正しました。
    (UUM-141699)

- `エディタ`: デバッグモードの Terrain Inspector 設定で利用可能な `enableHeightmapLODFrustumCulling` というオプションを追加し、地形フラスタムに基づく LOD カリングを無効にできるようにしました。
    (UUM-141589)

- `エディタ`: カスタムビルドプロファイルでのグラフィックスAPIリストの変更が正しく機能するようになりました。
    (UUM-127416)

- `エディタ`: 入力メッシュに、単一のエッジを共有する重なり合った三角形が多数存在する場合に、メッシュ LOD ジェネレータで発生していたクラッシュを修正しました。
    ([UUM-137244](https://issuetracker.unity3d.com/issues/crash-on-meshlodutils-buildclustermergejobsgeneric-when-generating-mesh-lods-for-a-specific-model))

- `エディタ`: ファイルの破損や外部によるファイルロックにより、curlファイルキャッシュデータベース \(CurlRequestCache.db\) を開くことができない場合、起動時にクラッシュする問題を修正しました。
    ([UUM-140399](https://issuetracker.unity3d.com/issues/crash-on-getdatabase-when-sqlite-database-for-the-curl-file-cache-fails-to-open-or-create))

- `Editor`: アウトラインパスをポリゴンにテッセレーションする際のクラッシュを修正しました。PolygonCollider2D、TilemapCollider2D、およびPhysicsComposerに影響する可能性があります。
    ([UUM-142017](https://issuetracker.unity3d.com/issues/editor-crashes-on-outputpolymesh-when-running-a-specific-scene-in-play-mode-or-player))

- `エディター`: BuildPlayerProcessor.PrepareForBuild コールバックが、ビルド前にアセンブリを含むフォルダーを削除した際に発生していたプレイヤーのクラッシュを修正しました
    ([UUM-137492](https://issuetracker.unity3d.com/issues/player-crashes-upon-launch-when-a-folder-is-deleted-as-a-prebuild-step))

- `エディター`: エディターの言語を日本語に変更した際に、Macエディターで発生する極めて稀なクラッシュを修正しました
    ([UUM-141719](https://issuetracker.unity3d.com/issues/crash-on-platform-strlen-when-the-editors-language-is-changed-to-japanese))

- `Editor`: 「固定時間ステップ」フィールドに Inf または NaN を入力した際に発生していた「無効な二重パラメータ」エラーを修正しました。
    ([UUM-138227](https://issuetracker.unity3d.com/issues/argumentexception-invalid-double-parameter-dot-error-is-thrown-when-infinity-is-typed-into-the-fixed-timestep-field))

- `エディタ`: 「プレイヤー設定」>「プリロードされたアセット」などのインスペクタ配列の「サイズ」フィールドに非常に大きな値（例：24124124）を入力した際に、エディタがフリーズする問題を修正しました。
    ([UUM-139781](https://issuetracker.unity3d.com/issues/the-editor-freezes-indefinitely-when-entering-24124124-into-the-preloaded-assets-size))

- `エディタ`: テクスチャがキューブマップとして、またはミップマップなしでインポートされるように設定されている場合、選択したレベルでこれらのテクスチャにエフェクトが適用されているにもかかわらず、テクスチャインポーターの「Aniso Level」スライダーを操作できない問題を修正しました。
    ([UUM-138249](https://issuetracker.unity3d.com/issues/aniso-level-still-applies-when-generate-mipmap-is-disabled-in-texture-import-settings))

- `エディタ`: プレイモード中にプレハブをインポートする際、MonoBehaviour/ScriptableObjectフィールドに保存された参照が失われることがある問題を修正しました。
    ([UUM-139664](https://issuetracker.unity3d.com/issues/the-reference-to-a-prefab-variant-is-lost-on-instantiation-when-it-is-serialized-in-a-parents-component))

- `エディタ`: macOSおよびLinux版エディタで、エディタの終了後もVBCSCompilerプロセスが残存して実行され続ける問題を修正しました。
    (UUM-142615)

- `エディタ`: 太字を適用した際にテキストがはみ出す問題を修正しました。
    ([UUM-137212](https://issuetracker.unity3d.com/issues/bold-text-unexpectedly-overflows))

- `Editor`: グラフィックス API の設定による再起動条件のチェックを追加し、ビルドプロファイルの切り替え時にエディタの再起動プロンプトが表示される問題を修正しました。
    (UUM-139685)

- `エディタ`: -projectPath 引数でエディタを起動した際、再接続ループによりハブが引き続き開いてしまう問題を修正しました。
    ([UUM-142653](https://issuetracker.unity3d.com/issues/unity-hub-opens-when-launching-the-editor-with-projectpath-argument-v2))

- `エディタ`: 「最小プローブ間隔」を変更した後のプローブ照明が不正確になる問題を修正しました。
    ([UUM-141983](https://issuetracker.unity3d.com/issues/adaptive-probe-volumes-require-a-min-probe-spacing-が-urp-で-変更された際の-正しい-プローブ-ライティング-データ-のための-2回目の-ベイク))

- `Editor`: ビルドプロファイル内で、スケーラープロファイルに空のカスタムスケーラーフィールドが追加され、UIがリセットされた際に発生するNull例外を修正しました。
    ([UUM-140845](https://issuetracker.unity3d.com/issues/argumentnullexception-thrown-when-reseting-adaptive-performance-settings-with-no-reference-set-in-defaultscaler))

- `エディタ`: UI Toolkit \(default\) インスペクターモードを使用している際、インスペクターでプレハブバリアントのプロパティオーバーライドを元に戻した後、OnValidate が呼び出されない問題を修正しました。以前は、トグルやドロップダウンなどのテキスト以外のフィールドにより、プレハブアセットの自動保存されず、ユーザーがフィールドからフォーカスを外すために他の場所をクリックするまで OnValidate がブロックされるという不具合を修正しました。
    ([UUM-134476](https://issuetracker.unity3d.com/issues/the-onvalidate-method-is-not-invoked-when-reverting-changes-on-a-prefab-variant))

- `エディター`: BuildProfilesを切り替えた際にワーカーがクラッシュするのを防ぐため、インポートワーカーにおけるシングルトンの再読み込み順序を修正しました。
    ([UUM-133886](https://issuetracker.unity3d.com/issues/assetimportworker-crash-on-kernelbase-raiseexception-when-switching-between-web-and-uwp-platforms-in-build-profiles))

- `エディタ`: カラースペース設定の変更時にプロジェクトウィンドウのパスが破損する問題を修正しました。
    ([UUM-139519](https://issuetracker.unity3d.com/issues/project-window-path-display-breaks-visually-when-player-settings-color-space-is-changed))

- `エディタ`: シーンにスプライトアトラスが含まれている場合に、マルチプレイヤープレイモードのクローンで発生するスプライトアトラスアセットのインポートエラーを修正しました。
    (UUM-139265)

- `エディタ`: TextCore用のスプライトアセットにおけるUnicode処理を修正しました。
    ([UUM-141521](https://issuetracker.unity3d.com/issues/ui-toolkit-doesnt-render-the-assigned-sprites-when-using-unicode-characters-assigned-to-a-sprite))

- `エディタ`: 地形: 選択した地形のハイトマップを編集する際に発生していたパフォーマンスの低下を修正しました。
    ([UUM-141526](https://issuetracker.unity3d.com/issues/the-editor-start-performing-very-poorly-when-editing-the-terrain-heightmap-with-terraindata))

- `EmbeddedLinux`: `GameWindow.DisposeAsync` の欠落していたドキュメントを追加しました。
    (UUM-141650)

- `Engine Diagnostics`: プレイヤーループが停止した後、非同期クラッシュレポートパイプラインが完了できなかったため、シャットダウン時に重複したマネージド例外のカウントが失われる問題を修正しました。
    ([UUM-141101](https://issuetracker.unity3d.com/issues/combined-log-and-throw-exceptions-function-does-not-show-up-in-diagnostics-cloud-dashboard-when-called-in-player))

- `Engine Diagnostics`: JNIネイティブメソッドが時期尚早に登録解除され、`nativeOnAndroidAppSetIdResult` で `java.lang.UnsatisfiedLinkError` が発生する原因となっていたクラッシュを修正しました。
    (UUM-137662)

- `GI`: `PruneCellIndexList` 内の古いセルインデックスが原因で発生していた APV クラッシュを修正しました。
    ([UUM-142091](https://issuetracker.unity3d.com/issues/crash-on-rendererscene-notifyinvisible-when-gameobjects-are-deleted-from-the-hierarchy-in-a-specific-scene))

- `GI`: 黒い四角形のアーティファクトを修正しました。
    ([UUM-142681](https://issuetracker.unity3d.com/issues/black-square-shadow-artifacts-visible-when-using-screen-space-reflections-without-maximum-smoothing))

- `Graphics`: 利用可能な場合、ブレンドシェイプのみを持つメッシュに GPU スキニングを適用するようにしました。
    ([UUM-137953](https://issuetracker.unity3d.com/issues/low-performance-when-multiple-meshes-using-blendshape-are-rendered-on-screen))

- `Graphics`: バッファのオーバーランが発生した際に `validateCommonDrawErrors` で発生していた Metal Validation アサーションを修正しました。
    ([UUM-138495](https://issuetracker.unity3d.com/issues/mac-metal-failed-assertion-on-validatecommondrawerrors-when-buffer-is-overrun))

- `Graphics`: GPUオクルージョンカリング中に、GPU常駐のドローワーがクワッドトポロジーのメッシュを誤って三角形としてレンダリングする問題を修正しました。
    ([UUM-132444](https://issuetracker.unity3d.com/issues/automatic-lod-fails-and-gpu-occlusion-culling-incompatibility-occurs-when-using-spline-based-quad-topology-meshes))

- `Graphics`: インスペクターの幅が狭い場合に、「プロジェクト設定を開く &gt; Graphics ...」ボタンからテキストがはみ出す問題を修正しました。
    ([UUM-141971](https://issuetracker.unity3d.com/issues/global-settings-asset-open-project-settings-graphics-dot-dot-dot-text-overflows-the-button-bounds-when-inspector-is-narrow))

- `Graphics`: シェーダーパス内の最も近いヒットシェーダーにあるUAVがクラッシュを引き起こす問題を修正しました。これらは現在サポートされておらず、この場合、シェーダーコンパイラは代わりにエラーを報告します。
    ([UUM-137197](https://issuetracker.unity3d.com/issues/crash-on-writehitgrouprecordjob-when-material-closesthit-uses-rwtexture2d-uav))

- `Graphics`: レンダリングコマンドをレンダリングスレッドに渡す際に使用されるメモリ量を削減し、関連する診断機能を改善しました。
    (UUM-127793)

- `IL2CPP`: GameCore用のC++コードをビルドするためのMSVCの最大バージョンを16から17に引き上げた。
    (UUM-109593)

- `IL2CPP`: ランクが18を超える多次元配列に関するIL2CPPのコード生成の問題を修正した。
    ([UUM-138552](https://issuetracker.unity3d.com/issues/build-fails-when-building-a-project-containing-an-18-plus-dimension-array-with-il2cpp))

- `iOS`: il2cpp コマンドによる GameAssembly のビルドに失敗した場合、Xcode プロジェクトのビルドも失敗するようにしました。
    (UUM-141609)

- `ライセンス`: ライセンスクライアントの再接続に関する問題を修正しました。
    ([UUM-142572](https://issuetracker.unity3d.com/issues/floating-license-is-lost-for-concurrent-jobs))

- `Linux`: Linux上で2 GiBを超えるPOSIXファイルの読み込みが失敗する問題を修正しました。
    ([UUM-140520](https://issuetracker.unity3d.com/issues/couldnt-open-file-for-reading-error-occurs-when-running-binary2text-on-a-file-larger-than-2-gib))

- `Particles`: サブエミッターモジュール内でサブエミッターが複数回出現した際に発生していたクラッシュを修正しました。
    ([UUM-142083](https://issuetracker.unity3d.com/issues/crash-on-particlesystemupdatedata-cachesubemitters-particlesystem-and-when-shared-subemitter-referenced-by-multiple-nested-particle-systems))

- `Physics`: 投影モードが有効な ConfigurableJoint において、接続されたボディがキネマティックからダイナミックに変更された際にクラッシュが発生する問題を修正しました
    ([UUM-135394](https://issuetracker.unity3d.com/issues/constraintprojectiontree-projectiontreebuildstep-でのクラッシュ（ConfigurableJointがJointProjectionModeのDot Position and Rotationを使用し、接続されたRigidbodyがキネマティックから非キネマティックに切り替わった場合）))

- `Physics`: Ragdoll Builder ウィンドウ内でアニメーターが null の場合、[Auto-Fill] ボタンをグレーアウトするようにしました。
    (UUM-142958)

- `Physics 2D`: PhysicsCore2D レンダラーがオーバーレイカメラ上でレンダリングを行わないように修正しました。
    ([UUM-142142](https://issuetracker.unity3d.com/issues/physicscore2d-renderer-should-ensure-it-only-renders-to-a-base-camera-in-urp))

- `Prefabs`: 「ExecuteInEditMode」プレハブモードの警告ダイアログに、セッションのオプトアウト機能を追加しました。
    (UUM-139861)

- `QNX`: `GameWindow.DisposeAsync` の欠落していたドキュメントを追加しました。
    (UUM-141650)

- `Shadergraph`: 事前定義されたキーワードのシェーダー入力を使用するシェーダーをエディターで開いた際に、再定義のコンパイルエラーが発生する問題を修正しました。
    ([UUM-142398](https://issuetracker.unity3d.com/issues/redefinition-of-lod-fade-crossfade-shader-errors-thrown-when-opening-speedtree9-urp-dot-shadergraph-in-universal-3d-template))

- `Shaders`: 変更が未適用な状態でシェーダービルド設定 UI から移動した際に表示される「未適用変更」ダイアログを追加しました。
    ([UUM-138992](https://issuetracker.unity3d.com/issues/user-is-グラフィックス設定から別の設定ウィンドウへ移動した際に、変更を適用するか元に戻すかの確認プロンプトが表示されない問題))

- `Shaders`: Material.GetTexturePropertyNameIDs がマテリアルバリアントに対して空を返す問題を修正しました。
    ([UUM-85842](https://issuetracker.unity3d.com/issues/an-empty-list-is-incorrectly-returned-for-material-variant-when-using-material-dot-gettexturepropertynameids))

- `Shaders`: シェーダーのビルド設定にある「キーワード宣言のオーバーライド」セクションで、エラーメッセージが見づらかった問題を修正しました。
    ([UUM-132639](https://issuetracker.unity3d.com/issues/light-editor-theme-the-error-message-keyword-declaration-override-cannot-be-empty-is-poorly-visible-in-the-graphics-settings-window))

- `Shaders`: プロパティを持たないシェーダーに対して、シェーダーインスペクターの「プロパティ」展開パネルが空で表示される問題を修正しました。
    ([UUM-127146](https://issuetracker.unity3d.com/issues/planeocclusionshader-properties-foldout-does-not-display-any-content))

- `Shaders`: 大きなシェーダーで「コンパイル」および「コードを表示」ドロップダウンを使用しても、エディタがフリーズしなくなりました。これは、バリアントの包含数を計算するために、すべてのシェーダーステージのすべてのキーワードを反復処理することを回避したためです。
    ([UUM-141740](https://issuetracker.unity3d.com/issues/compile-and-show-code-dropdown-freezes-the-editor-for-a-long-time))

- `Test Framework`: Unity Test Framework がパブリッシング設定の SCID をデフォルト値で上書きしてしまう問題を修正しました。
    (UUM-138637)

- `uGUI`: 「リッチテキスト編集を許可」が無効な状態で、TMP InputField の先頭でカーソルを左に移動した際に `IndexOutOfRangeException` が発生する問題を修正しました。
    ([UUM-134157](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-thrown-when-moving-caret-left-at-start-of-tmp-input-field-with-rich-text))

- `UI Elements`: UIToolkit.br.Bindings.PerformanceTests の一部のリグレッションを引き起こしていた新しいコードを最適化しました
    (UUM-139531)

- `UI Toolkit`: TreeView 内でアイテムの選択が左側の XR コントローラーでのみ可能だった問題を修正しました。
    ([UUM-141157](https://issuetracker.unity3d.com/issues/tree-view-from-ui-toolkit-will-take-one-xr-controller-as-primary-input-and-ignore-the-secondary-when-the-game-is-unpaused))

- `UI Toolkit`: インスペクターで選択された際に、UIDocumentがルートVisualElementを再生成してしまう問題を修正しました。
    ([UUM-127851](https://issuetracker.unity3d.com/issues/uidocument-generatevisualcontent-callback-is-not-assigned-when-uidocument-is-shown-in-the-inspector))

- `UI Toolkit`: HierarchyでUIドキュメントが選択されている状態でPlayモードに入ると発生する`MissingReferenceException`エラーを修正しました。
    ([UUM-131364](https://issuetracker.unity3d.com/issues/missingreferenceexception-error-is-thrown-when-entering-play-mode-while-ui-document-is-selected-in-hierarchy))

- `URP`: フレームデバッガーのメモリ使用量が過剰になる不具合を修正しました。
    ([UUM-139160](https://issuetracker.unity3d.com/issues/frame-debugger-excessive-memory-usage-regression))

- `URP`: 「テクスチャ」フォルダを展開した際に、フレームデバッガーでテクスチャプレビューアイコンが表示されない問題を修正しました。
    ([UUM-134917](https://issuetracker.unity3d.com/issues/texture-preview-icons-are-missing-in-frame-debugger-when-expanding-textures-foldout))

- `URP`: URP Gbuffer シェーダーで `#pragma rendertarget_format_hint` を指定するように変更し、この情報を必要とするプラットフォームでのレンダリング問題を修正しました。
    (UUM-134506)

- `VFX Graph`: `-nographics` オプションでビルドした際に、VFX Graph の Position \(Depth) が正しく動作しない問題を修正しました。
    ([UUM-141265](https://issuetracker.unity3d.com/issues/building-with-nographics-breaks-vfx-graph-position-depth-as-an-operator))

- `Video`: シーク時に、プラットフォームから報告されるフレームIDと、C#レイヤーに報告するフレームIDの間で発生する可能性のあるレースコンディションを修正しました。
    (UUM-134928)

- `Web`: マルチスレッドのWebビルドでGamepad APIが動作しない問題を修正しました。
    ([UUM-136543](https://issuetracker.unity3d.com/issues/gamepad-input-does-not-work-in-a-web-build-when-native-c-slash-c-plus-plus-multithreading-is-enabled))




## 6000.3.17f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.services.core`: [1.16.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.16//changelog/CHANGELOG.html) から [1.17.0] へ(https://docs.unity3d.com/Packages/com.unity.services.core@1.17//changelog/CHANGELOG.html)

- `com.unity.services.wire`: [1.4.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html) から [1.4.4](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html)

- `com.unity.test-framework.performance`: [3.4.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.4//changelog/CHANGELOG.html) から [3.5.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.5//changelog/CHANGELOG.html) へ