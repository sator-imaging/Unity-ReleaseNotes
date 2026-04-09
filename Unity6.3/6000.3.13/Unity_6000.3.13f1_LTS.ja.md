# Unity 6000.3.13f1 LTS
公開日時: Wed, 08 Apr 2026 09:59:17 GMT
https://unity.com/releases/editor/whats-new/6000.3.13f1

# 6000.3.13f1 の既知の問題

- `6000.0.17f1`: DX12使用時にシーンビューでGameObjectを選択するとCheckDeviceStatusでクラッシュする。
    ([uum-138597](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-selecting-gameobjects-in-the-scene-view-while-using-dx12))

- `6000.2.0a10`: プロジェクトを初めて開いた時に TexturesD3D12::CreateTextureInternal() でクラッシュする。
    ([uum-135024](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-opening-a-project-for-the-first-time))

- `6000.2.0b1`: DisableTypeTreeを使用したAsset BundleからVFXオブジェクトをロードする際、"CachedReader::OutOfBoundsError "でクラッシュする。
    ([uum-137538](https://issuetracker.unity3d.com/issues/crash-on-cachedreader-outofboundserror-when-loading-vfx-object-from-an-asset-bundle-with-disabletypetree))

- `6000.3.0a3`: Umbra::QueryExt::queryStaticShadowCasters で、Near Clipping Planes の最小値でカスタム Reflection Probe をベイクするとクラッシュする。
    ([uum-137250](https://issuetracker.unity3d.com/issues/crash-on-umbra-queryext-querystaticshadowcasters-when-baking-a-custom-reflection-probe-with-the-minimum-near-clipping-planes-value))

- `6000.5.0a4,6000.0.66f1,6000.3.4f1,6000.4.0b4`: ShaderVariantCollection.variantCountとShaderVariantCollection.shaderCountがBuildsで0を返す
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- `6000.5.0a8,6000.6.0a1,6000.4.0b12,6000.3.12f1`: 特定のシーンで照明をビルドすると複数のスタックトレースでクラッシュする問題
    ([uum-138494](https://issuetracker.unity3d.com/issues/crash-with-multiple-stacktraces-when-building-lighting-in-a-specific-scene))

- `6000.6.0a1,6000.3.11f1`: UIドキュメントでDrawText()を使用して動的テキストを作成すると、Colorパラメータが無視される
    ([uum-137907](https://issuetracker.unity3d.com/issues/color-parameter-is-ignored-when-creating-dynamic-text-in-a-ui-document-with-drawtext))

- `6000.6.0a1,6000.5.0a9,6000.3.12f1,6000.4.0f1`: プラットフォームを切り替えるとシェーダ関連の警告が発生する (TraceTransparentRays)
    ([uum-139001](https://issuetracker.unity3d.com/issues/switching-platforms-will-trigger-shader-related-warnings-tracetransparentrays))

- `メタル`: コマンドバッファのタイムアウトエラーの後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

vk::OnscreenSwapChain::AcquireNextImage でのクラッシュ
    ([uum-138508](https://issuetracker.unity3d.com/issues/crash-in-vk-onscreenswapchain-acquirenextimage))

ConstraintProjectionTree::projectionTreeBuildStep で、ConfigurableJoint が JointProjectionMode.PositionAndRotation を使用し、接続された Rigidbody がキネマティックから非キネマティックに切り替わったときにクラッシュする。
    ([uum-135394](https://issuetracker.unity3d.com/issues/crash-on-constraintprojectiontree-projectiontreebuildstep-when-configurablejoint-uses-jointprojectionmode-dot-positionandrotation-and-connected-rigidbody-switches-from-kinematic-to-non-kinematic))

空白のURPプロジェクトで再コンパイルすると、VisualElementのエディタ・メモリ・リークが発生する
    ([uum-138000](https://issuetracker.unity3d.com/issues/editor-memory-leak-in-visualelement-when-recompiling-in-a-blank-urp-project))

新しいリリースが最新のURPおよびHDRPテンプレートバージョンなしで出荷される
    ([uum-137426](https://issuetracker.unity3d.com/issues/new-releases-are-shipped-without-the-newest-urp-and-hdrp-template-versions))

DirectX 12の排他的フルスクリーンモードでフォーカスを切り替えるとプレイヤーがクラッシュする問題
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))



# 6000.3.13f1 リリースノート

## 機能

- `バージョン管理`: プロジェクトブラウザとインスペクタから、フォルダーの "ソースコントロールに追加" と "変更を元に戻す" アクションを追加。

- `バージョン管理`: ブランチを視覚化し、ナビゲートするための新しいブランチエクスプローラーを追加。

- `バージョン管理`: ウィンドウの再読み込みやセッションをまたがるすべてのスプリッターの位置の永続性を追加。

- `バージョン管理`: マージビューでシェルブを部分的に適用できるようにした。

- `バージョン管理`: F2キーボードショートカットでブランチやラベルの名前を変更できるようにした。



## 改良点

- `検索`: Deep Indexing" が有効な大規模プロジェクトの Search Index アーチファクトをマージする際のパフォーマンスが向上。
    (UUM-133013)



## API の変更

- `オーディオ`: 追加: ScriptableAudioPipeline ControlContext に API を追加し、システムがいつ設定されているかを発見しやすくした。
    ([uum-133107](https://issuetracker.unity3d.com/issues/configure-is-not-working-for-nested-generators))



## 変更点

- `Android`: GameActivity ライブラリを 3.0.5 から 4.4.0 に更新。

- `ドキュメント`: クイックスタートのハイパーリンクを ECS Feature Set Unity Documentation ページに変更。

- `バージョン管理`: ステータスバーにチェンジセットとラベルのアイコンを追加。

- `バージョン管理`: Unity Hub からプロジェクトを開くときにワークスペースの作成を遅延。

- `バージョン管理`: より一貫したキーボードワークフローのために、ダイアログ間のテキストフィールドのフォーカス動作を改善。

- `バージョン管理`: 変更待ちビューの空の状態を改善。

- `バージョン管理`: プロジェクトを誤って別の組織に接続しないようにした。

- `バージョン管理`: 新規プロジェクトの初期化を更新し、完全な初期チェックを行うようにした。

- `バージョン管理`: macOS の非表示ショートカットを Cmd+Shift+H に更新。



## 修正

- `2D`: 2D レンダラーで RSUV がサポートされない問題を修正。2D レンダラー用の ShaderUserVariable サポートを追加。
    (UUM-131692)

- `適応パフォーマンス`: gc の割り当てを修正。
    (UUM-136604)

- `AI`: Linux上で、NavMeshAgentインスペクタのAgent Typeプロパティの "Open Agent Settings... "オプションがエラーを発行し、__Navigation__ウィンドウを開かなかった問題を修正しました。
    ([uum-131690](https://issuetracker.unity3d.com/issues/opening-agent-settings-window-when-choosing-agent-type-throws-invalidoperationexception-error-in-the-console-window))

- `Android`: カーソルがロックされている時のマウス入力を修正しました。
    (UUM-91677)

- `Android`: タッチスクリーンのキーボードをスワイプしても、入力フィールドに単語がスパムされないようにした ୧(๑⃙⃘⁼̴̀꒳⁼̴́๑⃙⃘)
    ([UUM-116283](https://issuetracker.unity3d.com/issues/android-ui-toolkit-gameactivity-swipe-typed-word-overrides-a-last-entry-with-an-inputfield-with-a-large-amount-of-characters))

- `Android`: `AndroidApplication.onConfigurationChanged` がGameActivityの言語/国の変更を正しく反映するようになった。

- `アセットインポート`: keywords::LocalSpace::Findで、古いリソースにアクセスしたためにエディタがクラッシュする問題を修正。
    ([uum-133882](https://issuetracker.unity3d.com/issues/crash-on-keywords-localspace-find-when-reimporting-specific-assets))

- `エディター`: 品質レベルリストの表示を他の並べ替え可能リストと一致するように調整。
    ([uum-136310](https://issuetracker.unity3d.com/issues/reorderable-list-containing-quality-levels-in-the-build-profiles-window-uses-different-padding-sizes-compared-with-the-player-settings-graphics-api-reorderable-list))

- `エディター`: パブリッシング設定/WebAssembly言語機能のメモリ設定が0以下にならないようにクランプ。
    ([uum-134687](https://issuetracker.unity3d.com/issues/memory-related-fields-in-the-webassembly-language-features-can-be-set-to-the-negative-numbers))

- `エディター`: LinuxEditorでMemoryProfiler使用時に発生する誤検出のTLSエラーを修正。
    ([uum-136317](https://issuetracker.unity3d.com/issues/linux-tls-allocator-alloc-temp-tls-underlying-allocator-alloc-temp-main-has-unfreed-allocations-dot-dot-dot-error-and-warnings-are-thrown-when-selecting-a-snapshot-in-memory-profiler))

- `Editor`: プロファイラのスクリーンショットキャプチャに使用されたRenderTextureオブジェクトが適切に破棄されないメモリリークを修正しました。
    ([uum-137789](https://issuetracker.unity3d.com/issues/rendertarget-memory-usage-is-cumulative-and-is-creating-a-memory-leak-when-changing-scenes))

- `Editor`: QualitySettingsEditorがUpdateを呼び出すたびにプロジェクト内のすべてのビルド・プロファイルを読み込む際のパフォーマンスの問題を修正しました。
    (UUM-136760)

- `Editor`: カスタマイズ可能なツールバーの IMGUI 要素のエラーを修正しました。
    (UUM-135117)

- `エディター`: Win64プラグインの古いメタファイルをアップグレードするとプラグインが無効になる問題を修正。
    ([UUM-137610](https://issuetracker.unity3d.com/issues/win64-cpu-is-set-to-none-when-applying-changes-to-plugin-where-the-meta-has-the-serializedversion-2))

- `Editor`: 検索命題のアセットストア生成を修正。
    ([uum-133640](https://issuetracker.unity3d.com/issues/pressing-plus-button-in-search-field-in-asset-store-search-window-throws-formatexception-error-in-the-console-window))

- `エディター`: 資産ストアのクイッククリックナビゲーションを修正。
    ([uum-133625](https://issuetracker.unity3d.com/issues/nullreferenceexception-errors-thrown-in-the-console-when-holding-arrow-key-down-to-navigate-through-not-fully-loaded-assets-in-search-asset-store-window))

- `Editor`: インポートワーカープロセスの準備中にフォールバックシェーダーを検索するとクラッシュする問題を修正。
    ([uum-107712](https://issuetracker.unity3d.com/issues/assetimportworkers-crash-when-changing-shader-precision-model))

- `Editor`: ビルド自動化モーダルがビルドプロファイルの更新を追加しない問題を修正。
    (UUM-136372)

- `エディター`: プレビューモードが複数のアニメーションウィンドウ間で同時に同期される問題を修正。
    (UUM-136817)

- `エディター`: プレーヤー設定のラベルの切り捨てを修正。
    ([UUM-136316](https://issuetracker.unity3d.com/issues/the-use-dxgi-flip-model-swapchain-for-d3d11-settings-label-is-not-truncated-when-viewing-player-settings-in-a-build-profile))

- `エディター`: WinEditorのDragDrop操作中にmouseOverWindowが更新されない問題を修正。
    ([uum-137200](https://issuetracker.unity3d.com/issues/gameobject-deletion-fails-when-deleting-gameobject-after-dragging-prefab-into-scene-view))

- `エディター`: ObjectFieldにオブジェクトがないのに "Properties "と表示される問題を修正。
    ([uum-136445](https://issuetracker.unity3d.com/issues/scaler-profile-new-element-has-a-properties-button-in-the-context-menu-that-does-nothing-when-pressed))

- `エディター`: コンパイラの最適化バグに起因する、ウィンドウ起動時に稀に発生するWindowsEditorのクラッシュを修正。
    ([uum-137226](https://issuetracker.unity3d.com/issues/crash-on-containerwindow-doactivateandbringtofront-when-performing-various-actions-in-the-editor))

- `Editor`: Shader Build Settings(シェーダービルド設定)を使用している場合、各プロジェクトロード時にシェーダーグラフアセットが再インポートされないように修正。
    ([uum-134390](https://issuetracker.unity3d.com/issues/shader-graphs-are-re-imported-every-time-the-project-is-opened-when-dynamic-branching-for-fog-is-enabled))

- `Editor`: いくつかのパフォーマンスマーカー関数をスレッドセーフに修正。
    (UUM-129081)

- `エディター`: スクリプティング定義とコンパイラの追加引数の適用ボタンと元に戻すボタンを有効または無効にするロジックを修正。
    ([UUM-126488](https://issuetracker.unity3d.com/issues/empty-lists-can-be-applied-in-additional-compiler-argument-list-in-project-settings))

- `エディター`: WebGLの入力フィールドが入力後にフォーカスアウトしてしまう問題を修正。
    ([uum-137597](https://issuetracker.unity3d.com/issues/input-fields-do-not-maintain-focus-when-they-are-selected-in-a-web-build))

- `エディター`: ビルドプロファイルウィンドウの適切な動作を保証するために、buildprofilecontext.asset をロードできない場合に再作成するようにしました。
    ([uum-136377](https://issuetracker.unity3d.com/issues/nullreferenceexception-and-empty-build-profiles-window-when-buildprofilecontext-dot-asset-contains-invalid-script-reference))

- `エディター`: ビルドプロファイルの「品質設定」ドロップダウンで、すべての項目が追加された後の冗長な分離行を削除。
    ([uum-136313](https://issuetracker.unity3d.com/issues/an-unused-separation-line-is-present-in-the-quality-settings-lists-dropdown-menu-when-there-is-only-one-option-to-choose-from-in-the-build-profiles-window))

- `エディター`: Ubuntu 25.10以降で`libxml2`の名前が変更される問題を解決しました。Ubuntu 24.04はエディタがサポートする最高バージョンのままです。
    (UUM-137582)

- `GI`: URPReflectionProbeSettings 関連のアップグレードエラーを修正。
    (UUM-126607)

- `Graphics`: 無効なキーワードでシリアライズされたシェーダーバリアントを含む GraphicsStateCollection に対して GetVariants API を呼び出すと警告が表示されるようになりました。
    (UUM-136009)

- `Graphics`: GraphicsStateCollection API を使用した Pipeline State Object ｟PSO ｠のウォームアップで、トレースされた PSO がレンダー パスの外で記録された場合に、Metal で不正なキャッシュミスが発生する問題を修正しました。
    (UUM-135455)

- `Graphics`: DirectX11 でレンダーテクスチャの代わりに camera.SetTargetBuffers\(￤) でセットアップされた場合に、GrabPass が正しく rect サイズをセットしない問題を修正しました。
    ([uum-135889](https://issuetracker.unity3d.com/issues/grabpass-does-not-correctly-set-the-rect-size-when-set-up-with-a-camera-dot-settargetbuffers-instead-of-a-render-texture-in-directx11))

- `Graphics`: 特定の ShaderVariants をクエリするいくつかの GraphicsStateCollection API は、Unity 6000.3 と 6000.4 の特定の古いバージョンで、ロードされたコレクションアセットが以前にシリアライズされていた場合、正しいバリアントを見つけることができませんでした。
    (UUM-136008)

- `Graphics`: \同じレンダーパス・サブパスで深度読み込みとステンシル書き込み操作でレンダリング するとき、Mali GPU（非Midgard）でビジュアルアーチファクトを修正した。回避策は、この問題が存在するバージョン 41.0.0 より前のドライバに適用されます。
    (UUM-31270)

- `HDRP`: サンプルの説明中の不正なアセット参照を修正しました。
    ([UUM-137827](https://issuetracker.unity3d.com/issues/asset-sg-eye-dot-shadergraph-could-not-be-found-error-thrown-in-the-console-when-clicking-shader-graph-link-in-inspector-window-eye-samples-showcase))

- `カーネル`: -.
    (UUM-113356)

- N/A \(internal)：GeometryUtility.CalculateFrustumPlanes平面の方向を明確にしました。

- `N/A ｟GeometryUility.CalculateFrustumPlanes plane direction`: 誤ったリンクを修正。

- N/A \(internal)：スペルミスを修正。

- `Physics`: RigidbodyコンポーネントのAPIが、プレハブコンテキストから実行された場合に完全に保護されない問題を修正しました。
    ([uum-137716](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodygetflags-when-changing-rigidbody-interpolation-value-through-api-for-prefab-objects))

- `物理`: インスペクタがCenter/Radius/Height/SizeのようなColliderコンポーネントのデータを+/-Infinityに設定できる問題を修正しました。
    ([uum-136447](https://issuetracker.unity3d.com/issues/invalid-aabb-aabb-errors-are-spammed-when-infinity-value-is-entered-in-collider-component-fields))

- `Physics`: Rigidbody.centerOfMassに設定された値がシリアライズされない問題を修正しました。
    ([uum-137716](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodygetflags-when-changing-rigidbody-interpolation-value-through-api-for-prefab-objects))

- `物理`: Rigidbody.constraintsがプレハブアセット上で呼び出された時に、設定された値をシリアライズしない問題を修正しました。
    ([uum-137716](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodygetflags-when-changing-rigidbody-interpolation-value-through-api-for-prefab-objects))

- `物理 2D`: "PhysicsBody "と "PhysicsBodyDefinition "に "collisionThreshold "へのアクセスを追加し、CCDを使用する場合の設定を可能にしました。
    (UUM-137696)

- `Physics 2D`: 既存のゲッターを補足するために、"mass"、"rotationalInertia"、"localCentrOfMass "のPhysicsBody用の不足していたセッターを追加。
    ([uum-137414](https://issuetracker.unity3d.com/issues/massconfiguration-issues-with-physicsbody))

- `物理 2D`: PhysicsHingeJointを "unpinned "できるようになりました。これにより、点間拘束でのみ回転拘束が可能になり、効果的に回転のみの拘束を適用したままPhysicsBodyを動かせるようになりました。
    (UUM-137810)

- `物理 2D`: Box2Dが更新され、様々なバグ修正と改良が行われました。特に、シミュレーション中の接触のパフォーマンスを向上させるための接触のリサイクル機能が追加されました。
    (UUM-137810)

- `物理 2D`: 無効化された "PhysicsShapeDefinition.startMassUpdate "でPhysicsShapeを追加する場合、"PhysicsBody.ApplyMassFromShapes "または "PhysicsBody.massConfiguration "のいずれかを呼び出すことで、PhysicsBodyの衝突検出が正しく設定されるようにしました。
    ([uum-137414](https://issuetracker.unity3d.com/issues/massconfiguration-issues-with-physicsbody))

- `Profiler`: Profiler(プロファイラー)ウィンドウのキャプチャリストとタイムラインビューの境界で、レンダリングのアーティファクトを修正しました。
    ([uum-116890](https://issuetracker.unity3d.com/issues/rendering-artefacts-visible-in-the-profiler-window-modules-section-when-capture-list-is-open))

- `Shadergraph`: カスタムライティングサンプルの誤った追加ライトのインデックスを修正。
    ([uum-137007](https://issuetracker.unity3d.com/issues/2-lights-are-rendered-when-8-lights-exist-and-using-custom-lighting-shader-graph-with-forward-or-deferred-rendering))

- `シェーダー`: シェーダー保存時にクラッシュすることがあったのを修正。
    ([uum-133627](https://issuetracker.unity3d.com/issues/crash-on-enumeratedisabledkeywordsinvariantsarray-or-unity-xxh32-when-rapidly-saving-shadergraph-or-vfxgraph-changes))

- `SRP Core`: Volume Profile Inspector ウィンドウのパフォーマンスを改善。
    (UUM-136456)

- `UI Toolkit`: 長時間の高負荷時に発生するレイアウトキャッシュのメモリリークを修正しました。
    (UUM-137552)

- `UIツールキット`: グラフ検証後にバッジが正しく表示されない問題を修正。
    (UUM-137317)

- `UIツールキット`: 開始色が透明の場合、ボーダーの色遷移が機能しないのを修正。
    ([UUM-136876](https://issuetracker.unity3d.com/issues/border-is-not-rendered-when-transition-duration-is-set-and-border-color-is-transparent))

- `UIツールキット`: プレイモードに入った後、フィルターが折りたたまれるのを修正。
    ([uum-137614](https://issuetracker.unity3d.com/issues/ui-builder-filter-foldout-collapses-when-entering-play-mode-or-docking-the-window))

- `UIツールキット`: UIビルダーのプロジェクトタブで、libraryPathが指定されている場合に重複したグループをレンダリングする問題を修正。
    ([uum-137536](https://issuetracker.unity3d.com/issues/duplicated-groups-and-incorrect-grouping-in-ui-builder-when-using-uxmlelementattribute-librarypath))

- `UIツールキット`: DynamicColorヒントを持つタイトメッシュ・スプライトの背景色が更新されないのを修正。
    ([uum-136987](https://issuetracker.unity3d.com/issues/button-with-dynamiccolor-doesnt-update-its-unity-background-image-tint-color))

- `URP`: Bloomテクスチャで、無効なテクスチャハンドルが実行パスにまたがって再利用され、Render Graphの実行エラーにつながる問題を修正しました。
    ([uum-137390](https://issuetracker.unity3d.com/issues/crash-in-rendergraph-bloom-following-upgrade-to-unity-6-dot-3-6))

- `バージョン管理`: サイドバーの「保留中の変更」を右クリックした時のレイアウト例外を修正しました。

- `バージョン管理`: ブランチ差分から履歴を開く際に NullReferenceException が発生する問題を修正。

- `バージョン管理`: チェンジセットごとの diff パネルで NullReferenceException が発生する可能性があったのを修正。

- `バージョン管理`: チェックインダイアログの進行状況ラベルを修正し、ローカライズした。

- `バージョン管理`: Explore Repositories ウィンドウのぼやけたアイコンを修正。

- `バージョン管理`: バージョン管理ウィンドウのボタンの大文字と小文字をUnityの標準に合わせて修正。

- `バージョン管理`: ブランチビューからのチェンジセットごとの差分の問題を修正。

- `バージョン管理`: テーブルが空の時にブランチのコンテキストメニューが開かない問題を修正。

- `バージョン管理`: チェックインダイアログでコメント欄がオートフォーカスされないのを修正。

- `バージョン管理`: テーブルが空の時にラベルのコンテキストメニューが開かないのを修正。

- `バージョン管理`: 現在の選択範囲がチェンジセットやラベルの場合に、新規ブランチボタンが失敗するのを修正。

- `バージョン管理`: 再生モードを終了した後、ステータスバーが灰色になるのを修正。

- `バージョン管理`: ワークスペースの作成中にUnityのバージョン管理ウィンドウがマウスの移動を必要とせずに更新されるように修正。

- `バージョン管理`: Unity バージョン管理ウィンドウの検証メッセージの配置を修正。

- `WebGL`: WebGPUとWebGLで地形詳細メッシュを使用する際に発生するレンダリングエラーを修正しました。
    ([uum-91734](https://issuetracker.unity3d.com/issues/webgl-player-fails-to-render-scene-when-terrain-with-detail-mesh-is-added-and-webgpu-graphics-api-is-used))

- `WebGL`: \GPU Resident Drawer Instancingが無効なバインディングダイナミックオフセットで失敗することがありました。
    ([uum-135867](https://issuetracker.unity3d.com/issues/webgpu-error-with-fantasy-kingdom-and-gpu-resident-drawer))

- `WebGL`: \RG8UNorm のようないくつかのテクスチャフォーマットは、texture_formats_tier1 拡張が利用可能な場合でも、計算シェーダーの書き込み可能なテクスチャとして使用すると失敗します。
    ([uum-136007](https://issuetracker.unity3d.com/issues/webgpu-rg8unorm-texture-says-it-doesnt-support-random-writes))

- `XR`: テクスチャ圧縮ターゲティングを有効にして Meta Quest アプリケーションをビルドして実行する際の問題を修正しました。
    ([uum-131974](https://issuetracker.unity3d.com/issues/meta-quest-player-stuck-at-splashscreen-when-build-app-bundle-and-split-application-binary-are-enabled-with-multiple-texture-compression-formats))




## 6000.3.13f1 におけるパッケージの変更

## 更新されたパッケージ

- `com.unity.burst`: [1.8.28](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) から [1.8.29](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) へ。

- `com.unity.collab-proxy`: [2.11.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) から [2.12.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.12//changelog/CHANGELOG.html)

- `com.unity.purchasing`: [4.14.2](https://docs.unity3d.com/Packages/com.unity.purchasing@4.14//changelog/CHANGELOG.html) から [4.15.0](https://docs.unity3d.com/Packages/com.unity.purchasing@4.15//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: [3.6.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.6//changelog/CHANGELOG.html) から [3.6.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.6//changelog/CHANGELOG.html) に変更。

- `com.unity.services.vivox`: [16.9.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.9//changelog/CHANGELOG.html) から [16.10.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.10//changelog/CHANGELOG.html)

- `com.unity.test-framework.performance`: [3.2.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.2//changelog/CHANGELOG.html)から[3.4.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.4//changelog/CHANGELOG.html)

- `com.unity.timeline`: [1.8.11](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)から[1.8.12](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)

- `com.unity.xr.arcore`: [6.3.3](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.3//changelog/CHANGELOG.html) から [6.3.4](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.3//changelog/CHANGELOG.html) に変更。

- `com.unity.xr.arfoundation`: [6.3.3](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.3//changelog/CHANGELOG.html)から[6.3.4](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.arkit`: [6.3.3](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.3//changelog/CHANGELOG.html)から[6.3.4](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.compositionlayers`: [2.3.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.3//changelog/CHANGELOG.html)から[2.4.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.4//changelog/CHANGELOG.html)

- `com.unity.xr.meta-openxr`: [2.3.0](https://docs.unity3d.com/Packages/com.unity.xr.meta-openxr@2.3//changelog/CHANGELOG.html)から[2.3.1](https://docs.unity3d.com/Packages/com.unity.xr.meta-openxr@2.3//changelog/CHANGELOG.html)

- `com.unity.transport`: [2.7.1](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html) から [2.7.2](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html) に変更。

- `com.unity.netcode.gameobjects`: [2.10.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.10//changelog/CHANGELOG.html)から[2.11.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.11//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: [2.0.11](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)から[2.0.12](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.polyspatial`: [3.1.1](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.1//changelog/CHANGELOG.html) から [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.1//changelog/CHANGELOG.html) へ。

- `com.unity.polyspatial.visionos`: [3.1.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.1//changelog/CHANGELOG.html) から [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.1//changelog/CHANGELOG.html) まで。

- `com.unity.polyspatial.xr`: [3.1.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.1//changelog/CHANGELOG.html) から [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.1//changelog/CHANGELOG.html) まで。

- `com.unity.polyspatial.extensions`: [3.1.1](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.1//changelog/CHANGELOG.html)から[3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.1//changelog/CHANGELOG.html)

- `com.unity.xr.visionos`: [3.1.1](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.1//changelog/CHANGELOG.html) から [3.1.4](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.1//changelog/CHANGELOG.html) まで。

- `com.unity.ai.inference`: [2.5.0](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.5//changelog/CHANGELOG.html) から [2.6.0](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.6//changelog/CHANGELOG.html)