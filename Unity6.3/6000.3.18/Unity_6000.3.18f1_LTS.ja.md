# Unity 6000.3.18f1 LTS
公開日時：2026年6月17日（水）08:57:11 GMT  
https://unity.com/releases/editor/whats-new/6000.3.18f1

# 6000.3.18f1 の既知の問題

- `6000.0.11f1`: 特定のアセットを含むプロジェクトを閉じる際に、ProfilerMutexLock でクラッシュする
    ([UUM-144371](https://issuetracker.unity3d.com/issues/crash-on-profilermutexlock-when-closing-a-project-with-specific-assets))

- `6000.5.0a6`: 特定のプロジェクトでプレイモードに入ると、PhysicsCommands::PhysX::BodySetPose でクラッシュする
    ([UUM-143658](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodysetpose-when-entering-特定のプロジェクトでプレイモードに入る際))

- `アセットインポーター`: プレイモードに入る際、「(Unity) WriteObjectToVector」でエディターがクラッシュする
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- テキスト (TextMeshPro): TMPro フォントアセットクリエーターでマルチスレッドのフォントアトラスを生成中に UNITY_FT_Load_Glyph でクラッシュする
 ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

エディタでさまざまな操作を実行した際に mdb_cursor_sibling でクラッシュする
    ([UUM-141720](https://issuetracker.unity3d.com/issues/crash-on-mdb-cursor-sibling-when-performing-various-actions-in-the-editor))

bee_backendが複数実行されている際にmono_log_write_logfileでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

フォントアトラスの生成時に複数のスタックトレースが発生し、クラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.3.18f1 リリースノート

## 新機能

- `ドキュメント`: UDP ドキュメントパイプラインに、エンジンドキュメント内の外部参照リンクを解決するためのステップが追加されました。



## 改善点

- `Multiplayer`: Perforce が接続された状態で MPPM プレイヤータグを作成する際、「VirtualProjectSettings.json」に関する書き込みアクセスエラーを修正
    (UUM-144074)



## 変更点

- `エディタ`: macOS 用の Rosetta 2 インストールヘルパーアプリは不要となったため、削除されました。



## 修正

- `2D`: すべての領域でパディングが完全に適用されない問題（\(Case IN-139653\)）を修正しました。
    ([UUM-139518](https://issuetracker.unity3d.com/issues/sprite-packer-does-not-obey-padding-when-allow-rotation-is-enabled))

- `2D`: グリッドモードにおいて、ブラシピックが開いた際に、最後に選択された項目ではなくグリッドの末尾までスクロールしてしまう問題を修正しました。
    (UUM-138222)

- `2D`: Lens Flare コンポーネントを追加した際に発生していたエラーを修正し、正射影カメラのサポートを追加しました。
    ([UUM-141781](https://issuetracker.unity3d.com/issues/render-graph-execution-and-argumentexception-errors-are-spammed-when-adding-lens-flare-srp-component-in-a-2d-urp-project))

- `2D`: タイルパレットのブラシ選択画面において、GridViewの一番下までスクロールした後に空白領域が表示される問題を修正しました。
    ([UUM-142144](https://issuetracker.unity3d.com/issues/empty-scrollable-space-appears-and-scrollbar-shrinks-when-scrolling-down-in-the-tile-palette-brush-picks-overlay-window-and-list-view-selected-with-many-saved-brushes))

- `2D`: Light2D および Shadow Caster 2D コンポーネントが、インスペクターで誤ったアイコンを表示する問題を修正しました。
    ([UUM-132563](https://issuetracker.unity3d.com/issues/not-clear-abbreviation-ld-on-the-2d-light-overlay))

- `2D`: ShaderGraph マテリアルを使用しているスプライトで、スケールが負の値の場合のピック操作を修正しました。
    ([UUM-141627](https://issuetracker.unity3d.com/issues/sprite-renderer-is-not-selectable-in-scene-view-when-using-a-sprite-shader-graph-material-on-a-negatively-scaled-object))

- `2D`: スプライトエディタウィンドウが、プレビューテクスチャを参照してしまうことがある問題を修正しました。
    ([UUM-140054](https://issuetracker.unity3d.com/issues/selected-object-is-sprite-window-is-shown-and-sprite-becomes-non-editable-when-reopening-sprite-editor-with-preview-enabled))

- `Adaptive Performance`: パフォーマンスアクションの遅延およびサーマルアクションの遅延に負の値が設定されないようにしました。
    (UUM-135803)

- `AI`: NavMesh データを読み込む際、NavMeshSurface の読み込み中は、そのサーフェスのすべてのタイルが読み込まれるまで既存の NavMeshLinks の処理を回避するようになり、オーバーヘッドが軽減されました。
    ([UUM-126707](https://issuetracker.unity3d.com/issues/navmeshmanager-dot-loaddata-takes-a-long-time-and-causes-performance-spikes-when-enabling-a-navmeshsurface-with-already-instantiated-navmeshlinks))

- `Android`: `RunWithoutFocus` が有効な状態で Android アプリをバックグラウンドに移行した際に発生していた Vulkan のクラッシュを修正しました。
    (UUM-141888)

- `Audio`: 通常のオーディオプロセッサの破棄中に発生していた、誤検知によるエラーの連発（「Cannot access the processor - handle is stale...」）および「nested processor had to be forcefully updated」という誤った警告を修正しました。
    (UUM-142099)

- `DX12`: アクティブなコマンドバッファの制限を超えた場合、GPUの処理完了を待たないようにしました。
    (UUM-139697)

- `DX12`: `EnableAsyncCompute(true)` を指定して `AddComputePass` を使用する際、`D3D12SwapChain::Present` でのクラッシュを修正しました。
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `DX12`: Sentis ポーズサンプルにおける DirectML のクラッシュを修正しました。
    (UUM-143597)

- `DX12`: シェーダーの非同期コンパイル中に、Meta パスの CommandBuffer.DrawMesh\(\)がシェーダーの非同期コンパイル中に無視される問題を修正しました。
    (UUM-139294)

- `エディタ`: エディタのクラッシュ時に、未保存の状態を反映していない SceneBackup ファイルが不要な復元ダイアログを表示するのを防ぐため、これらのファイルを削除するようにしました。
    (UUM-142761)

- `エディター`: 保存されていない追加内容を元に戻した後、[プロジェクト設定] > [グラフィックス] > [シェーダー] でキーワード宣言のオーバーライドを削除しても、エディターが `ArgumentOutOfRangeException` をスローしなくなりました。
    ([UUM-143037](https://issuetracker.unity3d.com/issues/argumentoutofrangeexception-is-thrown-removing-a-keyword-declaration-overrides-after-adding-and-reverting-one-of-them))

- `エディター`: 専用サーバーのビルドプロファイルを追加した後、ウィンドウを再表示するまで「**プロファイルの切り替え**」ボタンが「ビルドプロファイル」ウィンドウに表示されない問題を修正しました。
    ([UUM-143216](https://issuetracker.unity3d.com/issues/the-switch-profile-button-does-専用サーバーのビルドプロファイルが追加された際、ビルドプロファイルウィンドウを再表示するまで**Switch Profile**ボタンが表示されない問題))

- `エディタ`: ビルドプロファイルウィンドウを開いた際、Player Settingsアセットがインポートされていないとクラッシュする問題を修正しました。
    ([UUM-116727](https://issuetracker.unity3d.com/issues/crash-on-std-1-tree-const-iterator-when-opening-特定のプロジェクトにおけるビルドプロファイルウィンドウ))

- `エディタ`: モーションブラーのタイルパスにおいて、特定のオブジェクト速度の場合にタイルごとの最小速度が初期化されないままになるというエッジケースを修正しました。
    ([UUM-142360](https://issuetracker.unity3d.com/issues/invalid-blue-value-in-motionblurmergetilepass-when-objects-move-at-certain-speeds))

- `エディタ`: フォントアセットクリエーターで作成した RASTER_HINTED フォントアトラスが破損する問題を修正しました。
    ([UUM-142852](https://issuetracker.unity3d.com/issues/some-glyphs-are-skewed-in-rendered-textmeshpro-font-asset-when-using-raster-hinted-render-mode))

- `エディタ`: 例外ログ出力時に発生する一部のケースでのクラッシュを修正しました。
    ([UUM-141434](https://issuetracker.unity3d.com/issues/crash-on-scripting-logexception-when-async-http-callback-executes-after-scripting-domain-teardown))

- `Editor`: ハイパーリンクの使用時に発生していたクラッシュを修正しました。
    ([UUM-142829](https://issuetracker.unity3d.com/issues/editor-crashes-in-textlib-findintersectinglink-when-hovering-uitk-labels-with-tags-rendered-via-atg))

- `エディタ`: -nographics スイッチを指定してバッチモードで、カスタム DefaultCursor が設定されたプロジェクトを開いた際に Linux エディタがクラッシュする問題を修正しました。
    ([UUM-142569](https://issuetracker.unity3d.com/issues/linuxeditor-crash-on-xaddextension-when-opening-the-unity-editor-on-linux-with-batchmode-and-nographics-on-a-project-with-a-custom-default-cursor))

- `エディタ`: プレイモード中にインスペクタのプレビューで再生すると、レンダリングテクスチャおよび生テクスチャのプレビューがカクつく。
    ([UUM-140017](https://issuetracker.unity3d.com/issues/video-player-preview-stutters-slash-lags-when-played-in-the-inspector-preview-during-play-mode))

- `エディター`: \[Android\] 「属性の競合」エラーウィンドウ内で、存在しない「Gradle トラブルシューティング」ページへのリンクを、Unity 6.3 用の正常に機能する「Gradle for Android」リンクに置き換えました。
    ([UUM-142945](https://issuetracker.unity3d.com/issues/colliding-attributes-error-opens-a-missing-page-when-pressing-the-troubleshoot-button))

- `GI`: Rosetta 2 がインストールされていない MacOS ARM ビルドでライトのベイクを行うと発生していたクラッシュを修正しました。
    (UUM-142663)

- `GI`: Rosetta が利用できない場合、MacOS ARM ビルドでの CPU ライトのベイクを無効にしました。
    (UUM-142173)

- `Graphics`: パフォーマンスの急上昇を防ぐため、テクスチャストリーミングにおけるレンダラーの追加を遅延させるようにしました。
    (UUM-140042)

- `Graphics`: 回転を適用した際にリフレクションプローブで発生していたアーティファクトを修正しました。
    ([UUM-137813](https://issuetracker.unity3d.com/issues/shadow-cast-by-rotated-reflection-probe-has-corners-culled-when-using-forward-plus-or-deferred-plus-rendering-path))

- `Graphics`: Vulkan グラフィックス API を使用している際に、ウィンドウのサイズ変更時のエディタのパフォーマンスを改善しました。
    (UUM-141307)

- `Graphics`: まだ読み込まれていない親オブジェクトを設定しても、マテリアルプロパティが失われなくなりました。
    ([UUM-113050](https://issuetracker.unity3d.com/issues/material-properties-are-lost-when-setting-a-parent-that-hasnt-been-loaded-yet))

- `Graphics`: \[OpenGLES\] Windows版のOpenGLES3スタンドアロンプレーヤーで、Alt+Enterキーでフルスクリーンモードを切り替えた後に発生していたレンダリングエラーおよびOpenGL検証エラーを修正しました。
    ([UUM-109464](https://issuetracker.unity3d.com/issues/rendering-errors-are-thrown-when-canceling-full-screen-on-opengl-api-windows-build))

- `HDRP`: ビルドターゲットを切り替えた後、`ReAllocateOffscreenUIColorBufferIfNeeded` で発生していた NullReferenceException を修正しました。
    ([UUM-143038](https://issuetracker.unity3d.com/issues/nullreferenceexception-object-reference-not-set-to-an-instance-of-an-object-error-is-thrown-after-switching-to-the-default-build-profile-in-high-definition-3d-template))

- `HDRP`: パストレーシングが有効な際に、HDR UI オーバーレイが表示されない問題を修正しました。
    ([UUM-142884](https://issuetracker.unity3d.com/issues/hdrp-game-view-is-rendered-black-when-using-pathtracing-on-a-hdr-display))

- `HDRP`: リフレッシュが行われるまで、HDRPのポストプロセス・ボリュームのオーバーライドが更新されない問題を修正しました。
    ([UUM-142661](https://issuetracker.unity3d.com/issues/some-post-processing-volume-overrides-only-update-after-a-refresh-when-using-hdrp))

- `IL2CPP`: メソッド、ファイル、行番号を表示するオプションを選択した際、ログのコールスタックに誤ったメソッドが表示されることがある問題を修正しました。
    ([UUM-138416](https://issuetracker.unity3d.com/issues/build-stack-trace-contains-invalid-lines-when-building-with-il2cpp-using-scripts-with-delegates-containing-generic-types-in-the-signature))

- `IMGUI`: IMGUI の選択に関する問題を修正しました。
    ([UUM-137875](https://issuetracker.unity3d.com/issues/all-of-the-logs-テキストの一部のみを選択しようとした際に、テキスト全体が選択されてしまう問題))

- `パッケージマネージャー`: Windows でのパッケージインストール中に断続的に発生していた `EPERM: 操作が許可されていません、名前変更` エラーを修正しました。
    ([UUM-142421](https://issuetracker.unity3d.com/issues/package-installation-fails-non-deterministically-with-errors-eperm-operation-not-permitted-when-installing-packages))

- `パッケージマネージャー`: 複数のインスペクタで同じ `package.json` を選択した際、エラーが発生しないように修正しました。
    (UUM-142468)

- `Physics`: Articulation Body のジョイント制限が、Physics SDK で定義された範囲内に収まるようになりました。
    ([UUM-91742](https://issuetracker.unity3d.com/issues/articulation-body-with-revolute-joint-type-has-erratic-behavior-when-upper-limit-is-set-to-above-360))

- `Physics`: 布同士の衝突を計算する際、NvClothの内部処理による過剰なメモリ割り当てが原因で発生していたメモリ破損を修正しました。
    ([UUM-64185](https://issuetracker.unity3d.com/issues/crash-on-collideparticles-when-entering-play-mode))

- `Physics`: 参照しているメッシュアセットのファイルを上書きすると、MeshCollider が機能しなくなる問題を修正しました。
    ([UUM-141284](https://issuetracker.unity3d.com/issues/meshcollider-preview-gizmo-disappears-from-the-scene-view-when-overriding-the-mesh-asset-using-any-3d-editing-tool))

- `Physics`: カプセルコライダーのデバッグ用可視化機能を修正し、スケールが適用された際にもカプセルの先端が曲率を維持するようにしました。
    ([UUM-142483](https://issuetracker.unity3d.com/issues/colliders-are-rendered-deformed-when-viewed-through-physics-debugger-in-scene-view))

- `Physics`: NvCloth ソルバーカーネル内で、SIMD 演算の結果として NaN 値が生じるいくつかのケースを修正しました。
    ([UUM-64185](https://issuetracker.unity3d.com/issues/crash-on-collideparticles-when-entering-play-mode))

- `Physics 2D`: 「PhysicsAABB.Normalized\(\)」が「PhysicsAABB.Normalize\(\)」に変更されました。
    (UUM-143279)

- `Physics 2D`: スクリプト関連のドキュメントにおける不整合、スペルミス、および型参照の誤りを修正しました。
    (UUM-143279)

- `Physics 2D`: 複数のスレッドから `PhysicsCore2D` システムを使用する際の安定性を向上させ、ワールドやオブジェクトの破棄中にクラッシュを引き起こす可能性のある、まれなレースコンディションを修正しました。
    (UUM-143564)

- `Prefabs`: 破損した `PrefabInstance` をクリーンアップする際、追加されたオブジェクトが削除されなくなりました。
    ([UUM-142338](https://issuetracker.unity3d.com/issues/crash-on-mergeobjectcollection-when-repeatedly-selecting-a-prefab-asset-in-the-project-browser))

- `Profiler`: スタンドアロン・プロファイラーウィンドウの「AI Assistant」ボタンを無効化しました。
    ([UUM-142961](https://issuetracker.unity3d.com/issues/ask-assistant-button-remains-in-standalone-profiler-after-ai-assistant-package-is-removed-via-package-manager-causing-errors-in-the-console-when-clicked))

- `Profiler`: プロファイラーがアタッチされている状態でクラッシュしたプロセスの最終フレームにおける、CPU タイムラインのレンダリングを修正しました。
    ([UUM-71728](https://issuetracker.unity3d.com/issues/フレームが画面幅を超えている場合、プロファイラーのタイムラインのスクロールバーでフレーム全体を表示できない問題))

- `Scene Manager`: 複数のシーンが読み込まれた状態でプレイモードを終了する際、ユーザースクリプトが `EditorSceneManager.sceneClosed` をサブスクライブし、ハンドラ内で開いているシーンを列挙すると発生していたクラッシュを修正しました。
    ([UUM-131346](https://issuetracker.unity3d.com/issues/crash-on-scene-custom-getpathinternal-when-exiting-play-mode-while-listening-to-editorscenemanager-dot-sceneclosed-and-printing-open-scenes))

- `Shaders`: シェーダーインスペクターの「コンパイルしてコードを表示」ドロップダウンが、要素の重なりを防ぐために幅広くなりました。
    ([UUM-143195](https://issuetracker.unity3d.com/issues/shader-inspector-compile-and-show-code-popup-clips-menu-item-text-and-overlaps-the-show-button-with-the-variants-included-label))

- `Text`: Advanced Text Generator (ATG) のテキストシェーピングにおけるパフォーマンスのボトルネックを修正しました。
    (UUM-139797)

- `TextMeshPro`: TMP シェーダーが、シェーダーで設定されたカラーモードに合わせる代わりに、常に HDR カラーピッカーを使用してしまう問題を修正しました。
    ([UUM-141742](https://issuetracker.unity3d.com/issues/ゲームビューからTMPテキストオブジェクトの面やアウトラインの色をサンプリングする際、スポイトツールが誤った値を選択する問題))

- `UI Toolkit`: パネル内のいずれかの要素が毎フレームスタイルを更新している場合、ScrollView.ScrollTo が呼び出された後、毎フレーム手動のスクロール入力が上書きされてしまう問題を修正しました。
    ([UUM-142486](https://issuetracker.unity3d.com/issues/scrollview-snaps-back-to-the-target-after-scrollto-when-the-ui-updates-every-frame))

- `UI Toolkit`: フィルター使用時に GroupTransform で発生していた問題の修正。
    ([UUM-142586](https://issuetracker.unity3d.com/issues/scrollview-clips-content-when-under-an-ancestor-that-has-a-filter-set))

- `UI Toolkit`: ダイナミック高さのコレクションビューで、垂直スクロール時に水平スクロール値が 0 にリセットされる問題を修正しました。
    ([UUM-142573](https://issuetracker.unity3d.com/issues/multi-column-list-view-horizontal-scroll-resets-to-left-most-position-when-scrolling-vertically))

- `UI Toolkit`: アクティブなスタイルシートが別のスタイルシートの下に再配置された際、UI Builder が新しいセレクタを誤った USS ファイルに追加してしまう問題を修正しました。
    ([UUM-143744](https://issuetracker.unity3d.com/issues/new-selector-is-added-to-the-top-most-stylesheet-instead-of-the-active-uss-when-using-add-new-selector-in-ui-builder))

- `UI Toolkit`: ベーステンプレートが編集された UXML インスタンスを再度開いた後、UI Builder インスペクタで `<AttributeOverrides>` のリスト値が古いまま表示される問題を修正しました。
    ([UUM-141060](https://issuetracker.unity3d.com/issues/a-uxml-instance-with-an-shows-stale-list-state-in-ui-builder-inspector-when-editing-its-base-template-and-reopening-the-instance))

- `UI Toolkit`: UI Builderでデータソースタイプが割り当てられていたビジュアル要素を削除した際に、コンソールで`ObjectDisposedException`がスローされる問題を修正しました。
    ([UUM-129925](https://issuetracker.unity3d.com/issues/deleting-a-visual-element-in-ui-builder-throws-objectdisposedexception-if-it-had-data-source-type-assigned))

- `バージョン管理`: UnityYAMLMerge では、マージ後に空の配列に値が設定されると、無効なプレハブ YAML が生成されることがありました。場合によっては、これによりプレハブの解析に失敗し、使用できなくなることがありました。
    ([UUM-131530](https://issuetracker.unity3d.com/issues/prefabs-are-corrupted-due-to-inline-styled-yaml-when-unityyamlmerge-is-used-to-merge-prefabs))




## 6000.3.18f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.netcode`: [1.13.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html) から [1.13.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html) へ

- `com.unity.formats.alembic`: [2.4.4](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) から [2.4.5](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) へ

- `com.unity.performance.profile-analyzer`: [1.3.4](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) から [1.4.0](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.4//changelog/CHANGELOG.html)

- `com.unity.purchasing`: [4.15.0](https://docs.unity3d.com/Packages/com.unity.purchasing@4.15//changelog/CHANGELOG.html) から [4.15.1](https://docs.unity3d.com/Packages/com.unity.purchasing@4.15//changelog/CHANGELOG.html) へ

- `com.unity.services.core`: [1.17.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.17//changelog/CHANGELOG.html) から [1.18.0](https://docs.unity3d.com/Packages/com.unity.services.core@1.18//changelog/CHANGELOG.html) へ

- `com.unity.xr.arcore`: [6.3.4](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.3//changelog/CHANGELOG.html) から [6.3.5](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.arfoundation`: [6.3.4](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.3//changelog/CHANGELOG.html) から [6.3.5](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.arkit`: [6.3.4](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.3//changelog/CHANGELOG.html) から [6.3.5](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.3//changelog/CHANGELOG.html) へ

- `com.unity.xr.interaction.toolkit`: [3.3.1](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@3.3//changelog/CHANGELOG.html) から [3.3.2](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@3.3//changelog/CHANGELOG.html) へ

- `com.unity.formats.fbx`: [5.1.4](https://docs.unity3d.com/Packages/com.unity.formats.fbx@5.1//changelog/CHANGELOG.html) から [5.1.6](https://docs.unity3d.com/Packages/com.unity.formats.fbx@5.1//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: [2.11.2](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.11//changelog/CHANGELOG.html) から [2.12.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.12//changelog/CHANGELOG.html) へ

- `com.unity.ai.navigation`: [2.0.12](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) から [2.0.13](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.addressables.android`: [1.0.10](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html) から [1.1.0](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.1//changelog/CHANGELOG.html) へ

- `com.unity.sharp-zip-lib`: [1.4.1](https://docs.unity3d.com/Packages/com.unity.sharp-zip-lib@1.4//changelog/CHANGELOG.html) から [1.4.2](https://docs.unity3d.com/Packages/com.unity.sharp-zip-lib@1.4//changelog/CHANGELOG.html)

- `com.unity.services.multiplayer`: [2.1.3](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.1//changelog/CHANGELOG.html) から [2.2.3](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.2//changelog/CHANGELOG.html) へ

- `com.unity.platformtoolkit.steam`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.steam@1.0//changelog/CHANGELOG.html) から [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.steam@1.1//changelog/CHANGELOG.html) へ

- `com.unity.platformtoolkit.playgamesservices`: [1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.playgamesservices@1.0//changelog/CHANGELOG.html) から [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.playgamesservices@1.1//changelog/CHANGELOG.html)

- `com.unity.platformtoolkit.gdk`: [1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gdk@1.0//changelog/CHANGELOG.html) から [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gdk@1.1//changelog/CHANGELOG.html) へ

- `com.unity.platformtoolkit.gamekit`: [1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gamekit@1.0//changelog/CHANGELOG.html) から [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gamekit@1.1//changelog/CHANGELOG.html) へ

- `com.unity.platformtoolkit`: [1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit@1.0//changelog/CHANGELOG.html) から [1.1.0](https://docs.unity3d.com/Packages/com.unity.platformtoolkit@1.1//changelog/CHANGELOG.html) へ