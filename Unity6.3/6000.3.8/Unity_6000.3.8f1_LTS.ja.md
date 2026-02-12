# Unity 6000.3.8f1 LTS
公開日時 Wed, 11 Feb 2026 10:40:25 GMT
https://unity.com/releases/editor/whats-new/6000.3.8f1

# 6000.3.8f1 の既知の問題

- `6000.0.55f1,6000.3.0a4`: UI を切り替えながらマルチプレイヤールームを作成すると RaiseException でクラッシュする
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `6000.0.65f1,6000.5.0a4,6000.3.3f1,6000.4.0b2`: 地形ツールが既に元に戻されている場合に、前の地形曲率に従うようになりました。
    ([uum-134053](https://issuetracker.unity3d.com/issues/the-terrain-tools-follow-the-previous-terrain-curvature-when-it-was-already-undone))

- `6000.1.0a2,6000.0.64f1`: シングルパスステレオレンダリングでプレイモードに入るとスカイボックスだけが表示される
    ([uum-132342](https://issuetracker.unity3d.com/issues/single-pass-stereo-rendering-shows-only-skybox-when-entering-play-mode))

- `6000.3.0a1`: PhysicsCommands::PhysX::GetShapeGeometryHolderで、無効化されたオブジェクトのメソッドを呼び出すとクラッシュする。
    ([uum-134161](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-getshapegeometryholder-when-calling-a-method-on-a-disabled-object))

- `6000.3.0b1,6000.0.65f1`: QualitySettings.maxQueuedFramesを1に設定し、DX12を使用するとエディターがフリーズする。
    ([uum-131962](https://issuetracker.unity3d.com/issues/editor-freezes-when-qualitysettings-dot-maxqueuedframes-is-set-to-1-and-dx12-is-used))

- `6000.3.5f1`: カービングを有効にしてNavMesh Obstaclesを移動するとCPU使用率が増加する
    ([uum-133911](https://issuetracker.unity3d.com/issues/increased-cpu-usage-when-moving-navmesh-obstacles-with-carving-enabled))

- `6000.5.0a1,6000.3.2f1`: 特定のシーンでシーンビューを移動すると CheckDeviceStatus でクラッシュする。
    ([uum-131824](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-moving-in-the-scene-view-on-a-specific-scene))

- `6000.5.0a1,6000.3.2f1`: DX12 を使用し、すべてのスプラインノットを選択すると、複数のスタックトレースでクラッシュする
    ([uum-131707](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-using-dx12-and-selecting-all-spline-knots))

- `6000.5.0a5`: Screen.SetResolution() でディスプレイの解像度を変更すると DX12 プレーヤーの明るさが変わる
    ([uum-134064](https://issuetracker.unity3d.com/issues/dx12-player-brightness-changes-when-changing-display-resolution-with-screen-dot-setresolution))

- `メタル`: コマンドバッファのタイムアウトエラーの後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: [iOS] iOS のスプラッシュ画面の後に画面が点滅する
    ([uum-121453](https://issuetracker.unity3d.com/issues/ios-screen-flashing-after-the-ios-splash-screen))

- `Platform Audio`: [Windows] エディターで様々なアクションを実行すると AudioManager::InitFMOD でクラッシュする
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))

空のURPプロジェクトでプレイモードに入ったり出たりするときにエディタのメモリリーク
    ([uum-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))



# 6000.3.8f1 リリースノート

## 改良点

- `資産パイプライン`: シンボリックリンク検出のパフォーマンスを改善。
    (UUM-132708)

- `Shadergraph`: ノードが折りたたまれたときのUVノードのチャンネルドロップダウンの外観を改善。
    ([UUM-115034](https://issuetracker.unity3d.com/issues/uv-nodes-label-is-cut-off-when-preview-is-collapsed))



## 変更点

- `Graphics`: テクスチャのインポートは https://docs.unity3d.com/Documentation/Manual/ImportingTextures.html でサポートされているフォーマットに厳密に従うようになりました。画像ファイルの拡張子を変更することでこれを回避することはもはやできません。もし画像ファイルのフォーマットが必要であれば、機能要求を出してください。



## 修正

- `2D`: スプライトエディターウィンドウのカスタムピボットフィールドのオーバーフローを修正。
    ([uum-133168](https://issuetracker.unity3d.com/issues/sprite-editors-custom-pivot-fields-get-pushed-out-of-their-bounds-when-entering-a-lot-of-numbers-in-the-property-field))

- `2D`: ユーザが任意の位置で空のブラシでペイントし、∕(0, 0, 0)でタイルをクリアする問題を修正。
    ([uum-128709](https://issuetracker.unity3d.com/issues/painting-on-a-tilemap-erases-random-tile-when-an-empty-tile-was-selected-in-the-tilemap-palette))

- `アニメーション`: OnFocus`コールバック中にアニメーションウィンドウが最後に選択されたオブジェクトに戻る問題を修正しました。Animationウィンドウがフォーカスを得たとき、現在の選択オブジェクトを保持するようになりました。
    ([uum-131198](https://issuetracker.unity3d.com/issues/last-selected-asset-before-docking-animation-window-gets-selected-when-a-domain-reload-occurs))

- `アニメーション`: AnimationWindowEvent インスペクタの壊れたドキュメントリンクを修正。
    ([uum-131593](https://issuetracker.unity3d.com/issues/animation-event-is-missing-documentation-link))

- `バグレポーター`: Unity プロジェクトディレクトリにオフラインレポートをエクスポートする際の Bug Reporter のクラッシュを修正しました。
    ([uum-129604](https://issuetracker.unity3d.com/issues/bug-reporter-crashes-when-exporting-offline-report-into-a-unity-project-directory))

- `バグレポーター`: フォーカスされたドロップダウンフィールドにカーソルを置いたままスクロールすると値が変化するのを修正。
    (SUS-5725)

- `エディター`: Profilerモジュール紹介にデフォルトのProfilerモジュールリストを追加。

- `エディター`: あるUnityインスタンスのWinEditor SplashScreenを閉じると他のインスタンスも閉じるように修正。
    ([uum-124686](https://issuetracker.unity3d.com/issues/the-project-launching-process-moves-to-the-background-when-another-project-is-closed))

- `Editor`: Advanced Object Selectorを使用中にDefault Render Pipelineを変更する際に二重の確認ダイアログが表示されるのを修正しました。
    ([uum-132296](https://issuetracker.unity3d.com/issues/a-second-prompt-asking-users-to-confirm-is-opened-when-cancelling-the-switch-of-the-graphics-default-render-pipeline-while-using-the-advanced-object-selector))

- `Editor`: 別のディスプレイで再度開いたユーティリティ・ウィンドウのWinEditorの誤ったDPIスケーリングを修正しました。
    (UUM-131238)

- `エディター`: いくつかのシナリオでモーダルDialogBoxが表示されている時に、WinEditorが無反応になるのを修正。
    ([UUM-132303](https://issuetracker.unity3d.com/issues/the-editor-freezes-and-leaks-memory-when-cancelling-the-switch-of-the-default-render-pipeline-while-using-the-advanced-object-selector))

- `エディター`: SceneProviderがt:behaviorを持つエントリーを見つけられるようになりました。
    ([uum-114607](https://issuetracker.unity3d.com/issues/hierarchy-search-in-searchwindow-filtering-by-exact-type-monobehaviour))

- `Editor`: プレーンなGameObjectをプレハブに再接続する場合、子インスタンスを保持します。
    ([uum-102262](https://issuetracker.unity3d.com/issues/child-prefab-instance-connection-lost-when-reconnecting-parent-prefab))

- `Graphics`: MSAA メモリレスデプスバッファを解決する際の Metal Validation エラーによるクラッシュを修正。
    (UUM-125478)

- `Graphics`: AssetBundlesからリソース(典型的にはTextures)をロードする時、 AsyncResourceUploadBlocking(◆)で稀にデッドロックが発生するのを修正。
    ([uum-126066](https://issuetracker.unity3d.com/issues/android-the-application-freezes-during-the-assetbundle-loading))

- `物理2D`: 「PhysicsShapeDefinition.moverData" プロパティが、Unity エディタのインスペクタで編集可能になりました。
    (UUM-133265)

- `物理 2D`: PhysicsWorld.CastMover" がトリガーシェイプを検出しないように。
    (UUM-133265)

- `物理 2D`: PhysicsTransform と PhysicsRotate コンストラクタが Burst と互換性があることを確認。
    (UUM-133265)

- `物理 2D`: PhysicsShape.definition に "PhysicsShapeDefinition.startMassUpdate" と "PhysicsShapeDefinition.startStaticContacts" プロパティの読み取りが追加されました。
    (UUM-133265)

- `スクリプト`: 削除されるべきでないアセンブリ参照を削除することによって、AssemblyUpdaterがアセンブリを破損するのを修正しました。
    ([UUM-132084](https://issuetracker.unity3d.com/issues/api-updater-strips-unity-owned-custom-attribute-references-within-precompiled-dlls))

- `スクリプト`: いくつかのシナリオで ScriptUpdater のスタックオーバーフローを修正。
    ([uum-130076](https://issuetracker.unity3d.com/issues/script-updater-for-dot-dot-dot-failed-with-exitcode-dot-dot-dot-and-stdout-stack-overflow-dot-errors-thrown-in-console-when-a-project-using-obsolete-api-is-opened))

- `Shadergraph`: スウィズルノードマスクの大文字小文字が不適切な結果になることがある問題を追加。
    ([uum-132879](https://issuetracker.unity3d.com/issues/expected-color-is-changed-to-black-when-using-swizzle-node))

- `シェーダー`: スキップされたバリアントキーワードが定義されていないことによるシェーダーのコンパイルエラーを修正。
    ([uum-98633](https://issuetracker.unity3d.com/issues/number-pragma-skip-variants-fog-linear-does-not-remove-fog-linear-keyword-declared-keyword))

- `シェーダー`: ShaderUtil.IsGrahicsAPISupported が exclude_renderers で正しく動作するようになりました。
    (UUM-133092)

- `テキスト`: vOffset`タグのサポートを追加。
    (UUM-132638)

- `uGUI`: \仮想キーボードのステータスがDoneに設定された状態で`OnSubmit`がトリガーされたときに、入力フィールドが適切に非アクティブになるように、入力フィールドの問題を修正しました。
    ([UUM-130350](https://issuetracker.unity3d.com/issues/ios-android-onsubmit-event-is-triggered-indefinitely-on-ugui-input-field-after-dismissing-keyboard-on-mobile))

- `UIツールキット`: レンダリング中にメッシュを解放するハンドリングを修正。
    ([uum-126665](https://issuetracker.unity3d.com/issues/rendering-artifacts-appear-in-ui-builder-when-applying-high-blur-value-filter-for-mask64-or-toggle-elements))

- `UIツールキット`: エディターとXRでScrollViewのドラッグを可能に。
    (UUM-117166)

- `UIツールキット`: UIドキュメントがライブリロードを実行し、スクリプトがアタッチされていない場合にNULL参照例外がスローされる問題を修正しました。
    ([UUM-129344](https://issuetracker.unity3d.com/issues/nullreferenceexception-thrown-when-modifying-a-ui-document-while-a-scene-containing-a-gameobject-with-any-ui-document-and-a-missing-script-component-is-open))

- `UIツールキット`: UIデバッガを通して`-unity-material`スタイルにマテリアルを割り当てようとした際のエラーを修正しました。
    ([uum-114133](https://issuetracker.unity3d.com/issues/ui-debugger-invalid-value-for-property-unity-material))

- `UIツールキット`: スタイルシートから継承されたマテリアルのプロパティがUIビルダーで適切にオーバーライドされない問題を修正しました。
    ([uum-130880](https://issuetracker.unity3d.com/issues/inherited-material-reference-in-the-ui-builder-disappears-after-adding-a-material-property-override-for-a-child-visual-element))

- `UI Toolkit`: 一部のSVGアセットをインポートする際のサイレントクラッシュを修正しました。
    ([uum-132415](https://issuetracker.unity3d.com/issues/silent-crash-when-importing-svg-files))

- `UI Toolkit`: Unity 6.3へのアップグレード時にSVGインポーターの設定が失われたのを修正。
    ([uum-133203](https://issuetracker.unity3d.com/issues/svg-importer-settings-are-lost-when-upgrading-to-unity-6-dot-3))

- `UI Toolkit`: 大きなSVGアセットの塗りつぶしでSVGテッセレーションの問題が修正されました。
    ([uum-133144](https://issuetracker.unity3d.com/issues/svg-importer-fill-errors-with-large-svg-asset))

- `バージョン管理`: バージョン管理プロジェクトの設定フィールドがウィンドウのタイトルと一致していなかった問題を修正しました。
    ([uum-127155](https://issuetracker.unity3d.com/issues/version-control-information-does-not-align-with-window-title-1))

- `Web`: レガシー入力システムで、タッチイベントによるマウス位置のシミュレーションを修正した(Input.mousePosition)。
    ([uum-130369](https://issuetracker.unity3d.com/issues/input-dot-mouseposition-stops-syncing-to-touch-input-when-using-downloadhandlertexture-in-webgl-build))

- `WebGL`: WebGPU: ShaderVariantCollectionのウォームアップでコンソールのCreateRenderPipelineエラーを解決。
    ([uum-131262](https://issuetracker.unity3d.com/issues/webgpu-createrenderpipeline-errors-with-shadervariantcollection-warmup))




## 6000.3.8f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.addressables`: [2.8.0](https://docs.unity3d.com/Packages/com.unity.addressables@2.8//changelog/CHANGELOG.html) から [2.8.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.8//changelog/CHANGELOG.html) へ。

- `com.unity.formats.alembic`: [2.4.2](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) から [2.4.4](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) に変更。

- `com.unity.scriptablebuildpipeline`: [2.5.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.5//changelog/CHANGELOG.html) から [2.5.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.5//changelog/CHANGELOG.html) へ。

- `com.autodesk.fbx`: 5.1.2 から 5.1.3

- `com.unity.ai.navigation`: [2.0.9](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) -> [2.0.10](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.ai.inference`: [2.4.1](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.4//changelog/CHANGELOG.html)から[2.5.0](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.5//changelog/CHANGELOG.html)