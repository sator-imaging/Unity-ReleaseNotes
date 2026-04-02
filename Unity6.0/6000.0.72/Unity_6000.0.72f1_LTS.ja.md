# Unity 6000.0.72f1 LTS
公開日時: Wed, 01 Apr 2026 09:38:47 GMT
https://unity.com/releases/editor/whats-new/6000.0.72f1

# 6000.0.72f1 の既知の問題点

- `6000.5.0a4,6000.0.66f1,6000.3.4f1,6000.4.0b4`: ShaderVariantCollection.variantCountとShaderVariantCollection.shaderCountがBuildsで0を返します。
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- `IL2CPP`: [iOS] [Android] IL2CPPのビルド中に外部ライブラリのジェネリックに失敗する
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- `メタル`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

ConfigurableJoint が JointProjectionMode.PositionAndRotation を使用し、接続された Rigidbody がキネマティックから非キネマティックに切り替わったときに、ConstraintProjectionTree::projectionTreeBuildStep でクラッシュする。
    ([uum-135394](https://issuetracker.unity3d.com/issues/crash-on-constraintprojectiontree-projectiontreebuildstep-when-configurablejoint-uses-jointprojectionmode-dot-positionandrotation-and-connected-rigidbody-switches-from-kinematic-to-non-kinematic))

空白のURPプロジェクトで再コンパイルすると、VisualElementのエディタ・メモリ・リークが発生する
    ([uum-138000](https://issuetracker.unity3d.com/issues/editor-memory-leak-in-visualelement-when-recompiling-in-a-blank-urp-project))

DirectX 12の排他的フルスクリーンモードでフォーカスを切り替えるとプレイヤーがクラッシュする問題
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))



# 6000.0.72f1 リリースノート

## 機能

- `バージョン管理`: プロジェクトブラウザとインスペクタから、フォルダーの "ソースコントロールに追加" と "変更を元に戻す" アクションを追加。

- `バージョン管理`: ブランチを視覚化し、ナビゲートするための新しいブランチエクスプローラーを追加。

- `バージョン管理`: ウィンドウの再読み込みやセッションをまたがるすべてのスプリッターの位置の永続性を追加。

- `バージョン管理`: マージビューでシェルブを部分的に適用できるようにした。

- `バージョン管理`: F2キーボードショートカットでブランチとラベルの名前を変更できるようにした。



## 改良点

- `ドキュメント`: Memory Profiler パッケージへの直接リンクを追加。

- `ドキュメント`: メモリ管理のドキュメントにクリーンページとダーティページの管理に関する情報を追加した。

- `インストーラー`: 圧縮戦略の最適化により、Windows のインストーラーにかかる時間が最大 60% 短縮されました。
    (UUM-136633)



## 変更点

- `バージョン管理`: ステータスバーにチェンジセットとラベルのアイコンを追加。

- `バージョン管理`: Unity Hub からプロジェクトを開くときにワークスペースの作成を遅延。

- `バージョン管理`: より一貫したキーボードワークフローのために、ダイアログ間のテキストフィールドのフォーカス動作を改善。

- `バージョン管理`: 変更待ちビューの空の状態を改善。

- `バージョン管理`: プロジェクトを誤って別の組織に接続しないようにした。

- `バージョン管理`: 新規プロジェクトの初期化を更新し、完全な初期チェックを行うようにした。

- `バージョン管理`: macOS の非表示ショートカットを Cmd+Shift+H に更新。



## 修正

- `2D`: タイルパレットの警告アイコンの画像を高解像度のものに変更。
    ([uum-129885](https://issuetracker.unity3d.com/issues/help-box-icon-in-tile-palette-window-is-blurry-in-both-unity-themes))

- `2D`: タイル・パレットのブラシ・ピック・オーバーレイが拡張されたときに、ブラシ・ピック・リストのアイテムが最小サイズよりも低い高さで初期化される問題を修正しました。
    ([uum-132593](https://issuetracker.unity3d.com/issues/saved-picks-list-items-are-initialised-with-a-lower-height-than-the-minimum-size-when-the-tile-palette-brush-pick-overlay-is-expanded))

- `2D`: ブラシピックリストのアイテムが不正な形になり、スライダーでピックサイズを小さくしたときにリストが切れてしまう問題を修正しました。
    ([uum-132606](https://issuetracker.unity3d.com/issues/saved-tile-palette-brush-list-items-become-malformed-causing-the-list-to-become-cut-off-when-decreasing-the-pick-size-with-the-slider))

- `2D`: ピックのサイズを調整し、表示モードをグリッドに切り替えた後、ブラシピックの名前が消える問題を修正。
    ([uum-132598](https://issuetracker.unity3d.com/issues/saved-tile-palette-brush-names-disappear-after-adjusting-the-size-of-the-picks-and-switching-view-mode-to-grid))

- `2D`: 2つ目のタイルパレットブラシピックアセットを作成する際に、データ損失エラーを回避するためにアセットの破棄が許可されていない問題を修正。
    ([uum-132608](https://issuetracker.unity3d.com/issues/destroying-assets-is-not-permitted-to-avoid-data-loss-error-thrown-when-creating-a-second-tile-palette-brush-pick-asset))

- `2D`: ブラシピックを大量に保存した場合に、ブラシピックリストがスクロールしてしまう問題を修正。
    ([uum-134369](https://issuetracker.unity3d.com/issues/scrolling-in-the-tile-palette-brush-pick-overlay-breaks-when-a-lot-of-brushes-are-saved-and-the-list-view-is-enabled))

- `2D`: シャドウキャスターの2Dカリングを修正。
    ([uum-135640](https://issuetracker.unity3d.com/issues/2d-freeform-light-shadows-disappear-when-light-center-is-offset-from-shape-bounds))

- `DX12`: CommandBuffer.SetRenderTarget`が無効な深度スライスを使用した場合に、レンダーターゲットのバインディング中にクラッシュする問題を修正しました。
    (UUM-130121)

- `DX12`: 以前はコンピュートシェーダーのSRVとしてバインドされていたレンダーターゲットへの描画を再開した後に、リソースバリアが欠落していたのを修正しました。
    (UUM-127520)

- `Editor`: BuildProfileの重複を括弧で区別しました。
    (UUM-130365)

- `Editor`: FormerlySerializedAsが型のフィールドと衝突する場合に、プレハブプロパティの修正を適用するように修正。
    ([UUM-135039](https://issuetracker.unity3d.com/issues/object-reference-is-saved-on-an-incorrect-property-when-formerlyserializedas-is-used-on-an-overridden-prefab-variant-field))

- `エディター`: TextCoreでCJKを使用するとクラッシュする問題を修正。
    ([uum-136683](https://issuetracker.unity3d.com/issues/editor-freezes-when-rendering-wrapped-text-inside-japanese-parentheses-in-too-small-of-a-space))

- `エディター`: 標準テキストで太字スタイルを使用したときにグローバルフォールバックが見つからない問題を修正。
    ([uum-136612](https://issuetracker.unity3d.com/issues/synthetic-bold-applies-to-a-label-instead-of-bold-font-weight-when-using-fallback-font-asset))

- `エディター`: プレーヤー設定のラベルの切り捨てを修正。
    ([uum-136316](https://issuetracker.unity3d.com/issues/the-use-dxgi-flip-model-swapchain-for-d3d11-settings-label-is-not-truncated-when-viewing-player-settings-in-a-build-profile))

- `エディター`: MeshToSDFBakerで、複数のメッシュが提供されている場合にメッシュの破壊が欠けていたのを修正。
    ([uum-128633](https://issuetracker.unity3d.com/issues/memory-leaks-are-caused-when-using-meshtosdfbaker-dot-dispose))

- `GI`: 別プロセスでx64エミュレーションを使用してCPU lightmapperを実行することにより、Apple Silicon EditorとWindows on ARM EditorでCPU lightmapperを有効に。
    (UUM-102347)

- `GI`: AMD の APV 仮想オフセットのベイクを修正。
    ([UUM-114563](https://issuetracker.unity3d.com/issues/look-rotation-viewing-vector-is-zero-messages-are-logged-in-the-console-when-baking-lighting-with-display-probes-setting-enabled-in-rendering-debugger-while-using-the-android-build-profile-on-amd-hardware))

- `Graphics`: GraphicsStateCollection API を使用した Pipeline State Object ｟PSO ｠のウォームアップで、トレースされた PSO がレンダーパスの外で記録された場合に、 Metal 上で不正なキャッシュミスが発生する問題を修正しました。
    (UUM-135455)

- `Graphics`: NVIDIA ドライバの更新後に SystemInfo.supportsInlineRayTracing が false になる問題を修正しました。
    ([UUM-137132](https://issuetracker.unity3d.com/issues/raytracing-updating-nv-graphics-drivers-to-595-dot-79-causes-systeminfo-dot-supportsinlineraytracing-to-become-false))

- `Graphics`: 一部の Android デバイスでインスタンス化を使用した際の地形の継ぎ目を修正しました。
    (UUM-131277)

- `Graphics`: \(UUM-1312) `Graphics`: いくつかのAndroidデバイスで、インスタンス化時に地形の継ぎ目を 修正した。回避策は、この問題が存在するバージョン 41.0.0 より前のドライバに適用されます。
    (UUM-31270)

- `IL2CPP`: ラムダ式の無効な MethodsToPreserve エントリを修正しました。
    ([UUM-124814](https://issuetracker.unity3d.com/issues/unity-cil-linker-fails-on-player-build-when-persistent-listeners-have-and-in-their-xml-attribute-names))

- `UIツールキット`: フラットUI(overlayまたはeditor)におけるZの保存の矛盾を修正した。
    ([uum-115032](https://issuetracker.unity3d.com/issues/dragging-search-query-block-can-remove-its-color))

- `UI Toolkit`: MultiColumnTreeViewで、ソート時にGetIdFromIndexとGetItemDataForIndexから間違ったデータを返す問題を修正しました。
    (UUM-111055)

- `UIツールキット`: プレイモードの色合いが常に適用されない問題を修正。
    (UUM-136707)

- `UIツールキット`: WebGL シェーダーの精度の問題を修正。
    ([UUM-132006](https://issuetracker.unity3d.com/issues/ui-toolkit-text-becomes-visually-distorted-when-the-text-is-not-directly-facing-the-camera))

- `UI Toolkit`: オーバーレイ UI のレンダリング時に invertCulling を false に強制することで、リーク状態に対する安全性を強化。
    (UUM-136734)

- `バージョン管理`: サイドバーの「保留中の変更」を右クリックしたときのレイアウト例外を修正。

- `バージョン管理`: ブランチ差分から履歴を開く際に NullReferenceException が発生する問題を修正。

- `バージョン管理`: チェンジセットごとの diff パネルで NullReferenceException が発生する可能性があったのを修正。

- `バージョン管理`: チェックインダイアログの進行状況ラベルを修正し、ローカライズした。

- `バージョン管理`: Explore Repositories ウィンドウのぼやけたアイコンを修正。

- `バージョン管理`: バージョン管理ウィンドウのボタンの大文字と小文字をUnityの標準に合うように修正。

- `バージョン管理`: ブランチビューからのチェンジセットごとの差分の問題を修正。

- `バージョン管理`: テーブルが空の時にブランチのコンテキストメニューが開かない問題を修正。

- `バージョン管理`: チェックインダイアログでコメント欄がオートフォーカスされないのを修正。

- `バージョン管理`: テーブルが空の時にラベルのコンテキストメニューが開かないのを修正。

- `バージョン管理`: 現在の選択範囲がチェンジセットやラベルの場合に、新規ブランチボタンが失敗するのを修正。

- `バージョン管理`: 再生モードを終了した後、ステータスバーが灰色になるのを修正。

- `バージョン管理`: ワークスペースの作成中にUnityのバージョン管理ウィンドウがマウスの移動を必要とせずに更新されるように修正。

- `バージョン管理`: Unity バージョン管理ウィンドウの検証メッセージの配置を修正。

- `VFX Graph`: ドメイン再読み込みの後、ColorFieldが失われるのを修正。
    (UUM-124799)

- `VFX Graph`: カスタム属性の評価が正しくなく、間違った動作やシェーダの警告につながる。
    ([UUM-135239](https://issuetracker.unity3d.com/issues/vfx-warning-and-simulation-error-when-using-a-specific-custom-attribute-configuration))

- `Video`: WebGLSupport` の fakemod モジュールの `ChannelGroupI::getPitch` の警告を修正。
    ([uum-134014](https://issuetracker.unity3d.com/issues/fmod-returns-error-code-78-message-repeatedly-shown-in-the-console-when-playing-audio-using-an-audio-random-container))




## 6000.0.72f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.collections`: [2.6.2](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) から [2.6.5](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) へ。

- `com.unity.entities`: [1.4.2](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) から [1.4.5](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html)

- `com.unity.physics`: [1.4.2](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) から [1.4.5](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: [1.4.15](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) から [1.4.18](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) まで。

- `com.unity.2d.aseprite`: [1.1.10](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html) から [1.1.11](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html) へ。

- `com.unity.cinemachine`: [2.10.6](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html) から [2.10.7](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.11.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) から [2.12.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.12//changelog/CHANGELOG.html)

- `com.unity.nuget.mono-cecil`: [1.11.5](https://docs.unity3d.com/Packages/com.unity.nuget.mono-cecil@1.11//changelog/CHANGELOG.html) から [1.11.6](https://docs.unity3d.com/Packages/com.unity.nuget.mono-cecil@1.11//changelog/CHANGELOG.html) に変更。

- `com.unity.postprocessing`: [3.5.0](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html)から[3.5.4](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html)

- `com.unity.profiling.core`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.profiling.core@1.0//changelog/CHANGELOG.html) から [1.0.3](https://docs.unity3d.com/Packages/com.unity.profiling.core@1.0//changelog/CHANGELOG.html) へ。

- `com.unity.serialization`: [3.1.2](https://docs.unity3d.com/Packages/com.unity.serialization@3.1//changelog/CHANGELOG.html) から [3.1.5](https://docs.unity3d.com/Packages/com.unity.serialization@3.1//changelog/CHANGELOG.html) に変更。

- `com.unity.services.vivox`: [16.8.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.8//changelog/CHANGELOG.html) から [16.10.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.10//changelog/CHANGELOG.html) に変更。

- `com.unity.splines`: [2.8.3](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html) から [2.8.4](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html) へ。

- `com.unity.test-framework.performance`: [3.2.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.2//changelog/CHANGELOG.html)から[3.3.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.3//changelog/CHANGELOG.html)

- `com.unity.visualscripting`: [1.9.10](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)から[1.9.11](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)

- `com.unity.transport`: [2.6.0](https://docs.unity3d.com/Packages/com.unity.transport@2.6//changelog/CHANGELOG.html)から[2.7.2](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: [1.1.11](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) から [1.1.12](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) へ。

- `com.unity.ai.navigation`: [2.0.11](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) から [2.0.12](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)