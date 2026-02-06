# Unity 6000.3.7f1 LTS
公開日時: Thu, 05 Feb 2026 07:53:48 GMT
https://unity.com/releases/editor/whats-new/6000.3.7f1

# 6000.3.7f1 の既知の問題

- `6000.0.55f1,6000.3.0a4`: UI を切り替えながらマルチプレイヤールームを作成すると RaiseException でクラッシュする
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `6000.1.0a2,6000.0.64f1`: シングルパスステレオレンダリングでプレイモードに入るとスカイボックスだけが表示される
    ([uum-132342](https://issuetracker.unity3d.com/issues/single-pass-stereo-rendering-shows-only-skybox-when-entering-play-mode))

- `6000.3.0a1`: [WinEditor] Search native DialogBox が起動しているときにフォーカスを失うとエディタが "フリーズ" する
    ([uum-132303](https://issuetracker.unity3d.com/issues/the-editor-freezes-and-leaks-memory-when-cancelling-the-switch-of-the-default-render-pipeline-while-using-the-advanced-object-selector))

- `6000.3.0b1,6000.0.65f1`: QualitySettings.maxQueuedFramesを1に設定してDX12を使用するとエディタがフリーズする
    ([uum-131962](https://issuetracker.unity3d.com/issues/editor-freezes-when-qualitysettings-dot-maxqueuedframes-is-set-to-1-and-dx12-is-used))

- `6000.5.0a1,6000.3.2f1`: 特定のシーンでシーンビューを移動するとCheckDeviceStatusでクラッシュする
    ([uum-131824](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-moving-in-the-scene-view-on-a-specific-scene))

- `6000.5.0a1,6000.3.2f1`: DX12 を使用し、すべてのスプラインノットを選択すると、複数のスタックトレースでクラッシュする
    ([uum-131707](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-using-dx12-and-selecting-all-spline-knots))

- `6000.5.0a3,6000.4.0b2`: プロファイルアナライザーの比較ツールで2つのプロファイラーキャプチャをロードすると100%のクラッシュ率
    ([uum-132332](https://issuetracker.unity3d.com/issues/100-percent-crash-rate-when-loading-two-profiler-captures-in-the-profile-analyzer-compare-tool))

- `メタル`: コマンドバッファタイムアウトエラーの後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: [iOS] iOS のスプラッシュ画面の後に画面が点滅する
    ([uum-121453](https://issuetracker.unity3d.com/issues/ios-screen-flashing-after-the-ios-splash-screen))

- `Platform Audio`: [Windows] エディターで様々なアクションを実行すると AudioManager::InitFMOD でクラッシュする
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))

- `特定のプラグインがインストールされたシーンを開くと、複数のスタックトレースでクラッシュする。
    ([uum-133643](https`: //issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-opening-scenes-with-a-certain-plugin-installed))

- `([uum-132677]) `: 空白の URP プロジェクトでプレイモードに入ったり出たりする際のエディタのメモリリーク
    ([uum-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))



# 6000.3.7f1 リリースノート

## 変更点

- `uGUI`: uGUIのプロファイラモジュールの名前を "UI(Canvas) "と "UI Details(Canvas) "に変更した。
    (UUM-132153)



## 修正

- `2D`: SpriteRendererのシリアライズされたプロパティが変更され、MaterialPropertyBlockにちょうど2つのプロパティが設定されている場合に、SpriteRendererのMaterialPropertyBlockがリセットされる問題を修正しました。
    ([uum-127937](https://issuetracker.unity3d.com/issues/materialpropertyblock-of-a-spriterenderer-is-reset-when-it-is-updated-through-the-color-picker))

- `Android`: Application.Unloadを呼び出したときにGameActivityベースのアプリケーションがバックグラウンドにならない問題を修正しました。
    (UUM-129424)

- `アニメーション`: DopeSheetエディターで、曲線メニューが接線に変更を適用しない問題を修正しました。
    ([UUM-132540](https://issuetracker.unity3d.com/issues/animation-keyframes-are-always-set-to-clamped-auto-when-another-option-is-selected))

- `アセットパイプライン`: シーンの保存時に OnWillSaveAssets がアセットパスの空のリストを返すことがある問題を修正しました。
    ([uum-115091](https://issuetracker.unity3d.com/issues/onwillsaveassets-receives-an-empty-paths-array-when-saving-a-new-scene))

- `ドキュメント`: Create a Profiler モジュールページへのリンクを修正しました。

- `DX12`: UWPビルドのレンダーパスパスを有効にした。レンダーパス機能が利用できない場合に、一部のパスのビューポートが正しく設定されない可能性を修正。
    ([uum-89085](https://issuetracker.unity3d.com/issues/d3d12-mainlight-shadowmap-clear-incorrectly-when-using-uwp))

- `DX12`: CPU 側の時間サンプリングで壊れていた `IDXGISwapChain::GetFrameStatistics` を修正。
    (UUM-107892)

- `Editor`: navigation and pathfinding ˶(com.unity.module.ai)によって要求された全てのメモリ割り当てにルートラベルを追加しました。
    (UUM-126905)

- `エディター`: プロジェクトのロード中の潜在的なクラッシュを軽減するためにLinuxエディタにセーフガードを追加。
    ([UUM-132175](https://issuetracker.unity3d.com/issues/linux-crash-on-editorlaunchscreen-platformeditorlaunchscreen-setprogress-when-opening-a-project))

- `エディター`: UnityCrashHandler 実行ファイルにバージョン情報を追加。
    (UUM-132574)

- `エディター`: レイアウト保存時に予期せず警告が投げられるバグを修正。
    ([UUM-131954](https://issuetracker.unity3d.com/issues/a-cannot-save-invalid-window-create-layout-warning-is-thrown-when-any-custom-layout-is-created))

- `Editor`: ビルド時にメタパスが取り除かれないことによるパフォーマンスの低下を修正。
    (UUM-116130)

- `エディター`: SearchWindow からカラムを追加できるように修正。
    ([UUM-132150](https://issuetracker.unity3d.com/issues/add-column-dot-dot-dot-button-does-not-work-in-the-search-window))

- `エディタ`: クラッシュ報告のシンボルアップロード認証で、信頼性の低いLoggedIn(◆)状態チェックの代わりにTryLogin(◆)と直接アクセストークン検証を使うように修正。
    (ULO-8719)

- `Editor`: URPの反射プローブの境界の編集で、ハンドルを使って反対側を独立して編集できない問題を修正。
    ([UUM-132551](https://issuetracker.unity3d.com/issues/two-opposite-sides-of-the-reflection-probe-boundaries-are-moved-when-trying-to-move-only-one-side))

- `Editor`: アセットバンドルのロード/アンロードがテクスチャのストリーミング要求をキャンセルする際のハングを修正。
    ([uum-116419](https://issuetracker.unity3d.com/issues/editor-and-android-player-hangs-slash-freezes-when-repeatedly-loading-slash-unloading-assetbundle-in-vulkan))

- `エディター`: 一貫性のないチェックボックスの位置を修正。
    (UUM-132515)

- `エディター`: uGUI ゲームオブジェクトの作成において、メニューの順番が正しくないために自動リネームに失敗していたのを修正。
    ([UUM-132217](https://issuetracker.unity3d.com/issues/legacy-ui-elements-are-not-entering-auto-renaming-on-creation))

- `エディター`: ビルトインシーンのラベルを修正。
    ([uum-125472](https://issuetracker.unity3d.com/issues/default-scene-dropdown-field-contains-a-spelling-mistake-default-builtin))

- `エディター`: グラフィック設定」セクションのドロップダウンとチェックボックスの位置ずれを修正。
    ([uum-126644](https://issuetracker.unity3d.com/issues/misaligned-dropdowns-and-checkboxes-in-graphics-settings-section))

- `エディター`: shadergraph uGUIサンプルの名前を新しいメニュー名に従うように修正。
    (UUM-132809)

- `Editor`: AssetDatabaseScalability のパフォーマンスのリグレッション問題を修正。
    (UUM-132351)

- `エディター`: Light Editor テーマを使用している場合、Project タブがほとんど表示されない問題を修正。
    ([UUM-132553](https://issuetracker.unity3d.com/issues/plus-button-below-project-tab-is-barely-visible-when-using-light-editor-theme))

- `Editor`: トランスフォームの種類を変更すると、ルートトランスフォームが階層の最後に移動してしまう問題を修正。
    ([uum-132190](https://issuetracker.unity3d.com/issues/gameobject-drops-to-the-last-position-in-the-hierarchy-when-a-recttransform-component-is-added))

- `Editor`: メインツールバーのスライダーのコンテクストメニューに複数のセパレーターが表示されていたのを修正。
    ([uum-131672](https://issuetracker.unity3d.com/issues/an-extra-separator-is-added-to-main-toolbar-context-menu-when-extending-maintoolbarelement-with-populatecontextmenu))

- `エディター`: アンダーラインの折り返しに関する問題を修正。
    ([uum-132463](https://issuetracker.unity3d.com/issues/underline-vertex-left-position-is-greater-than-right-position-errors-when-enabling-advanced-text-generator-auto-size-and-resizing-the-ui-builder-panels))

- `エディタ`: アンダーラインの折り返しに関する問題を修正。
    ([uum-132475](https://issuetracker.unity3d.com/issues/learn-more-underline-doesnt-appear-on-both-words-if-they-get-separated-into-two-lines))

- `エディター`: サンプル水面 VFX グラフ・ノードの水デカール・サンプリングを修正。
    (UUM-132609)

- `編集`: 遠くの風速が速い時の水の高さのサンプリングを修正。
    ([UUM-121090](https://issuetracker.unity3d.com/issues/hdrp-water-surface-water-height-sampling-returns-false-height-when-distant-wind-speed-is-high))

- `エディター`: WorldToGUIPoint` と `OnDrawGizmos` API の動作を改善。

- `EmbeddedLinux`: EmbeddedLinux：RaspiOS vulkan のクラッシュを修正。
    ([uum-129585](https://issuetracker.unity3d.com/issues/embedded-linux-crash-on-application-launch-with-vulkan))

- `Graphics`: ソフトシャドウが有効な場合の点光源シャドウのアーティファクトを修正。
    ([uum-128839](https://issuetracker.unity3d.com/issues/white-lighting-artifact-when-a-point-light-with-a-small-emission-range-and-hard-shadows-touches-an-object-while-a-directional-light-with-soft-shadows-and-another-point-light-are-present))

- `Graphics`: フレームクリーンナップマップを修正し、テクスチャIDを削除せずに無効なテクスチャやメモリレスのテクスチャを削除するように。
    (UUM-129828)

- `iOS`: 数字パッドまたは電話パッド・キーボード・タイプを使用しているときにスクリーン上のキーボードが再オープンしないのを修正。
    (UUM-132968)

- `iOS`: UAaLセットアップでunityビューのリサイズがレンダリングを壊すかクラッシュするのを修正。
    ([UUM-130881](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-and-unitygfxdeviceworker-crash-when-show-splash-screen-is-enabled-and-project-is-built-using-unity-as-a-library))

- `物理`: シーンのリロードを無効にして布コンポーネントをオーサリングするとクラッシュする問題を修正。オーサリングの直後に Playmode に入ると、Cloth インスタンスが "オーサリングのみ" の状態に維持されます。
    ([uum-110845](https://issuetracker.unity3d.com/issues/crash-on-clothscene-processcomponentupdates-when-entering-play-mode-after-editing-cloth-collision-points))

- `物理2D`: 低レベル物理スクリプトのドキュメントのタイプミスと不正なリンクを修正しました。
    (UUM-132991)

- `Profiler`: Path 値が空の Player で MemoryProfiler.TakeSnapshot が呼び出されたとき、正しいフォルダに Memory Captures を送信しない問題を修正。
    (UUM-107629)

- `Profiler`: プロファイラ：プロファイラに使用されるメモリや、MemLabel kMemProfiling/kMemProfilingEditor を使用するメモリのネイティブ・メモリの root 化が、Memory Profiler で Native &gt; Unity Subsystems &gt; Unrooted として表示されるのを修正しました。
    (UUM-128226)

- `シェーダー`: ShaderUtil.GetMaterialProperties`を呼び出すとまれにクラッシュする問題を修正しました。
    ([UUM-130712](https://issuetracker.unity3d.com/issues/crash-on-pptr-operator-shader-star-ptr64-when-opening-a-project-with-specific-assets))

- `シェーダー`: シェーダーのコンパイルログメッセージの数値フォーマットを修正。
    (UUM-132747)

- `SRP Core`: ビルド実行後に空のレンダリングデバッガが表示される問題を修正。
    ([UUM-131802](https://issuetracker.unity3d.com/issues/renderingdebugger-opening-rendering-debugger-after-building-the-player-does-not-register-any-debug-items))

- `SRP Core`: Package Manager ウィンドウを複数回開いたり閉じたりした場合に SampleDependencyImporter から稀に発生するエラーを修正しました。
    ([uum-132472](https://issuetracker.unity3d.com/issues/system-dot-nullreferenceexception-errors-logged-when-opening-the-package-manager-via-button-in-the-toolbar-whilst-packages-are-loading))

- `SRP Core`: MSAAが有効で、URPのDecal Renderer FeatureがAutomaticまたはDBufferに設定されている場合、DepthCopyパスでGizmosレンダリングを処理するRender Graphが失敗するのを修正。
    ([uum-131330](https://issuetracker.unity3d.com/issues/black-game-view-screen-and-exception-mismatch-when-gizmos-are-enabled-in-game-view-with-msaa-enabled-and-the-decal-renderer-feature-set-to-automatic-or-dbuffer-in-urp))

- `テキスト`: line-heightのATGサポートを追加。
    ([uum-132202](https://issuetracker.unity3d.com/issues/paragraph-spacing-and-the-line-height-tag-are-not-working-when-the-advanced-text-generator-is-enabled))

- `テキスト`: ATG にインデントタグのサポートを追加した。
    (UUM-131288)

- `UI ツールキット`: 要素を削除した後にビルダーをドッキングすると NullReferenceException がスローされる。
    ([UUM-128717](https://issuetracker.unity3d.com/issues/docked-ui-builder-corrupts-when-the-domain-isnt-reloaded-after-deleting-an-element))

- `UIツールキット`: VisualElementのマテリアルに互換性がない場合に警告を表示するようにしました。
    ([uum-114770](https://issuetracker.unity3d.com/issues/material-applied-to-label-renders-over-ui-builder-window-when-zoomed-in))

- `バージョン管理`: 2.11.2のWaitForPendingOperations.cs.metaの無効な重複GUIDによるコンパイルエラーを修正。

- `バージョン管理`: Unity 6.3以下のバージョンでエディター内部へ直接アクセスできるように修正。

- `WebGL`: WebGPU: texture_formats_tier2 エクステンションの一貫性のない処理の問題を修正しました。
    (UUM-131865)




6000.3.7f1 における ## パッケージの変更

## 更新されたパッケージ

- `com.unity.2d.animation`: [13.0.2](https://docs.unity3d.com/Packages/com.unity.2d.animation@13.0//changelog/CHANGELOG.html) から [13.0.4](https://docs.unity3d.com/Packages/com.unity.2d.animation@13.0//changelog/CHANGELOG.html) へ。

- `com.unity.2d.common`: [12.0.1](https://docs.unity3d.com/Packages/com.unity.2d.common@12.0//changelog/CHANGELOG.html) から [12.0.2](https://docs.unity3d.com/Packages/com.unity.2d.common@12.0//changelog/CHANGELOG.html) に変更。

- `com.unity.2d.tooling`: [1.0.0](https://docs.unity3d.com/Packages/com.unity.2d.tooling@1.0//changelog/CHANGELOG.html) から [1.0.2](https://docs.unity3d.com/Packages/com.unity.2d.tooling@1.0//changelog/CHANGELOG.html) に変更。

- `com.unity.collab-proxy`: [2.11.2](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html)から [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html)へ。

- `com.unity.ide.rider`: [3.0.38](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) から [3.0.39](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- `com.unity.mobile.android-logcat`: [1.4.6](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) から [1.4.7](https://docs.unity3d.com/Packages/com.unity.mobile.android-logcat@1.4//changelog/CHANGELOG.html) に変更。

- `com.unity.testtools.codecoverage`: [1.2.7](https://docs.unity3d.com/Packages/com.unity.testtools.codecoverage@1.2//changelog/CHANGELOG.html)から[1.3.0](https://docs.unity3d.com/Packages/com.unity.testtools.codecoverage@1.3//changelog/CHANGELOG.html)

- `com.unity.xr.hands`: [1.7.2](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html) から [1.7.3](https://docs.unity3d.com/Packages/com.unity.xr.hands@1.7//changelog/CHANGELOG.html) に変更。

- `com.unity.profiling.systemmetrics.mali`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) から [1.1.1](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) に変更。