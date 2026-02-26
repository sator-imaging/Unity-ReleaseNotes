# Unity 6000.3.10f1 LTS
公開日時: Wed, 25 Feb 2026 14:01:36 GMT
https://unity.com/releases/editor/whats-new/6000.3.10f1

# 6000.3.10f1 の既知の問題

- `6000.0.55f1,6000.3.0a4`: UI を切り替えながらマルチプレイヤールームを作成すると RaiseException でクラッシュする
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `6000.0.66f1,6000.3.4f1,6000.4.0b4,6000.5.0a5`: Screen.SetResolution() でディスプレイの解像度を変更すると、DX12 プレーヤーの明るさが変わる
    ([uum-134064](https://issuetracker.unity3d.com/issues/dx12-player-brightness-changes-when-changing-display-resolution-with-screen-dot-setresolution))

- `6000.1.0a2,6000.0.64f1`: シングルパスステレオレンダリングでプレイモードに入るとスカイボックスだけが表示される
    ([uum-132342](https://issuetracker.unity3d.com/issues/single-pass-stereo-rendering-shows-only-skybox-when-entering-play-mode))

- `6000.2.0a10`: プロジェクトを初めて開いた時に TexturesD3D12::CreateTextureInternal() でクラッシュする。
    ([uum-135024](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-opening-a-project-for-the-first-time))

- `6000.2.0a7,6000.0.48f1`: [URP] デカール・レンダラー・テクニックが "自動 "に設定されている場合、バッチモードでビルドしたとき、またはエディターでシーン/ゲーム・ビューをレンダリングせずにビルドしたときに、すべてのマテリアルが黒くレンダリングされる。
    ([uum-134298](https://issuetracker.unity3d.com/issues/urp-all-materials-render-black-when-building-via-batchmode-or-without-rendering-scene-slash-game-view-in-editor-if-decal-renderer-technique-is-set-to-automatic))

- `6000.3.0a4,6000.0.62f1`: 前の入力をキャンセルした後で同じ入力フィールドを選択すると、入力フィールドが更新されない
    ([uum-133712](https://issuetracker.unity3d.com/issues/input-field-does-not-update-when-selecting-the-same-input-field-after-previous-input-was-canceled))

- `6000.3.5f1`: カービングを有効にしてNavMeshの障害物を移動するとCPU使用率が増加する
    ([uum-133911](https://issuetracker.unity3d.com/issues/increased-cpu-usage-when-moving-navmesh-obstacles-with-carving-enabled))

- `6000.3.7f1,6000.4.0b7`: PrefabでRigidbodyコンポーネントの設定を編集する際に、PhysicsCommands::PhysX::BodySetPoseでクラッシュする問題が修正されました。
    ([uum-135381](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodysetpose-when-editing-rigidbody-component-settings-on-a-prefab))

- `6000.5.0a7,6000.3.8f1,6000.4.0b9`: [Android][iOS] UI Toolkit ListViewのタッチパンスクロールが動作しない
    ([uum-135398](https://issuetracker.unity3d.com/issues/android-ios-ui-toolkit-listview-touch-pan-scrolling-does-not-work))

- `コアランタイム`: Entities ContentManagementのGUIDが不安定で、Playerが異なるディレクトリにビルドされるたびに異なる値になる
    ([uum-129944](https://issuetracker.unity3d.com/issues/entities-contentmanagement-guids-are-unstable-and-become-different-each-time-a-player-is-built-to-a-different-directory))

- `DirectX12`: 新しい "Get Started With Unity" プロジェクトを作成する際、D3D12DeviceState::ApplyRenderTargets でクラッシュする。
    ([uum-105801](https://issuetracker.unity3d.com/issues/crash-on-d3d12devicestate-applyrendertargets-when-creating-a-new-get-started-with-unity-project))

- `メタル`: コマンドバッファタイムアウトエラーの後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `Windows`: バックグラウンドで実行" が有効でアクティブウィンドウが切り替わるとプレイヤーがハングする
    ([uum-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))

空の URP プロジェクトでプレイモードに入ったり出たりするときにエディタのメモリリークが発生する
    ([uum-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))

DirectX 12 の排他的フルスクリーンモードでフォーカスを切り替えるとプレイヤーがクラッシュする問題
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))

[Silicon] Razer Synapseアプリを開いているときにプロジェクトを開くとos_unfair_recursive_lock_with_optionsでクラッシュする
    ([uum-135043](https://issuetracker.unity3d.com/issues/silicon-crash-on-os-unfair-recursive-lock-lock-with-options-when-opening-a-project-while-the-razer-synapse-app-is-open))



# 6000.3.10f1 リリースノート

## API の変更点

- `スクリプト`: 追加: `Random` API に単位円周上のランダムな点を Vector2 として返す `onUnitCircle` プロパティを追加。
    (UUM-133714)



## 変更点

- `エディター`: Unity Hub ページにインストールリンクと Hub ドキュメントサイトへのリンクを追加。



## 修正

- `Android`: カスタム Gradle テンプレートに `compileSdkVersion` 属性がある場合に `GradleTemplateUpdater` からのダイアログが表示される問題を修正した。
    ([uum-134142](https://issuetracker.unity3d.com/issues/android-gradle-compilesdkversion-is-incorrectly-deprecated-on-6-dot-0-6-dot-4))

- `アニメーション`: AnimationWindowのAddCurvesから作成されるクォータニオン・キーフレームの誤りを修正しました。
    ([uum-133953](https://issuetracker.unity3d.com/issues/assertion-failed-on-expression-compareapproximately-error-thrown-when-keyframes-are-added-for-rotation-animation))

- `エディター`: シェーダーのビルド設定(*Shader Build Settings*)下の文字列に切り捨てを追加。
    ([uum-133326](https://issuetracker.unity3d.com/issues/selected-keywords-string-under-shader-build-settings-is-cut-off-not-truncated-in-minimized-build-profiles-window))

- `エディター`: フレームデバッガでのメモリリークを避けるため、シェーディングレートLUTを廃棄。
    (UUM-131230)

- `Editor`: デバッグモードでインスペクタを使用するとコンソールにエラーが表示されるバグを修正。
    ([UUM-133467](https://issuetracker.unity3d.com/issues/selecting-multiple-visual-elements-in-the-hierarchy-with-enabled-debug-mode-results-in-malformed-inspector-window-with-thrown-notimplementedexception-and-unityeditor-dot-guiview-processevent-errors))

- `Editor`: Ubuntuのパッケージマネージャでパッケージのエクスポートダイアログを開くとハングアップしたりウィンドウが文字化けする問題を修正しました。
    ([uum-131283](https://issuetracker.unity3d.com/issues/ubuntu-package-managers-export-package-window-is-rendered-with-artifacts-when-editor-is-running-on-opengl))

- `エディタ`: Playerの設定でスクリプト定義リストの項目を追加したり削除したりする際に、不必要な適用ポップアップが表示されるのを修正しました。
    ([uum-121033](https://issuetracker.unity3d.com/issues/do-you-want-to-apply-changes-warning-pop-up-appears-when-adding-and-removing-list-items-in-player-settings))

- `Editor`: D3D12 Device Filter Lists のアセット情報ボックスの余分な空白を修正しました。
    ([uum-123221](https://issuetracker.unity3d.com/issues/d3d12-device-filter-lists-asset-information-box-has-too-much-empty-space))

- `エディター`: 他のアプリから切り替えた時に、LinuxEditorがスクリプトの再コンパイルに失敗する問題を修正。
    ([uum-133944](https://issuetracker.unity3d.com/issues/linux-auto-refresh-fails-to-reimport-and-compile-script-changes-when-editing-files-outside-the-editor))

- `Editor`: Build Profilesウィンドウのローディングスピナーアイコンの視認性を改善。
    ([uum-132018](https://issuetracker.unity3d.com/issues/progress-indicator-in-meta-quest-build-profile-configuration-is-barely-visible))

- `エディター`: スクリプト可能なレンダーパスを持つプロジェクトで、ビルドプロファイルの切り替え時にエディターで一時的なアタッチメントに関するコンソールエラーが投げられることがありました。これは修正されました。
    ([uum-97475](https://issuetracker.unity3d.com/issues/gbuffer-slash-render-deferred-lighting-and-render-pass-related-errors-constantly-thrown-after-switching-a-build-profile))

- `GI`: APVのツールチップの小さなタイプミスを修正しました：Steaming &gt; Streaming。
    ([uum-134159](https://issuetracker.unity3d.com/issues/streaming-is-misspelled-as-steaming-in-enable-gpu-streaming-and-enable-disk-streaming-tooltpis))

- `Graphics`: TexturesD3D11Base::SetTexture`のDX11クラッシュを修正。
    ([uum-134071](https://issuetracker.unity3d.com/issues/crash-on-texturesd3d11base-settexture-when-using-directx11))

- `IL2CPP`: デバッグ c++ 設定で WebRequests を使用すると Switch プラットフォームでクラッシュする問題を修正。
    (UUM-127898)

- `IL2CPP`: 汎用パラメータ型の内部ハッシュ関数を改良して起動時間を短縮した。
    (UUM-133424)

- `macOS`: シーンロード中にキーボード入力がリセットされる問題を修正。
    ([UUM-132112](https://issuetracker.unity3d.com/issues/keyboard-state-is-reset-when-automatically-loading-a-scene-via-script))

- `macOS`: macOSで多くのファイルを開いている時にネットワーク要求が失敗する問題を修正しました。
    (UUM-134087)

- `Mono`: インクリメンタル GC マーキングとルート登録解除の間の競合状態を修正。
    (UUM-131742)

- `物理`: 無効化されたColliderでCollider.GetGeometry&lt;T&gt; \を呼び出すとクラッシュする問題を修正しました。
    ([UUM-134161](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-getshapegeometryholder-when-calling-a-method-on-a-disabled-object))

- `物理`: 物理のジョイント コンポーネント ギズモで、ジョイントがワールド空間の固定点に接続されている場合に、自動設定された接続アンカーがジョイントに追従してしまう問題を修正しました。
    ([uum-134423](https://issuetracker.unity3d.com/issues/spring-joint-shows-only-one-anchor-gizmo-in-scene-view-when-auto-configure-connected-anchor-is-enabled))

- `物理 2D`: (UUM-134580):エディターで、一時停止してシングルステップしている時、補間モー ドを使用している "PhysicsBody "が、どのようなトランスフォーム書き込みとも同 期しないため、レンダラが視覚的に同期しない問題を修正しました。
    (UUM-134580)

- `Profiler`: 複数のクリックによってプロファイル・キャプチャが何度も開き直される問題を修正しました。
    ([UUM-133429](https://issuetracker.unity3d.com/issues/profiler-capture-loading-process-is-deferred-until-the-final-click-is-released-when-selecting-a-capture-in-the-profiler-list-multiple-times-consecutively))

- `Shadergraph`: 一部のプラットフォームでビルトインレンダーパイプラインのシェーダーグラフをコンパイルする際、"fixed "が再定義される警告を修正。
    (UUM-126357)

- `テキスト`: 非常に長い ATG テキストが適切にレンダリングされるように。
    ([UUM-133940](https://issuetracker.unity3d.com/issues/ui-toolkit-label-stops-rendering-text-in-a-custom-editor-window-when-using-advanced-text-generation))

- `UIツールキット`: ビルダーでの選択に関するパフォーマンスのリグレッションを修正。
    (UUM-132445)

- `UIツールキット`: コレクションがソートされた時に、MultiColumnTreeViewとMultiColumnListViewのデータソースパスに不正なインデックスが適用されていた問題を修正しました。
    ([uum-133865](https://issuetracker.unity3d.com/issues/multicolumnlistview-does-not-visually-sort-the-column-when-bindingsourceselection-is-set-to-auto-assign))

- `Undo System`: ルートGameObjectの複数選択でTransformタイプの置き換えを元に戻す/やり直すと、ルートGameObjectの階層順序が変わるのを修正。
    ([uum-133391](https://issuetracker.unity3d.com/issues/gameobjects-change-hierarchy-order-when-undoing-adding-component-to-multiple-gameobjectsgameobjects-change-hierarchy-order-when-undoing-adding-component-to-multiple-gameobjects))

- `WebGL`: AudioSource.SetScheduledEndTimeのバグを修正しました。SetScheduledEndTimeが呼ばれた時、起動時にAudioSourceの再生要求が保留されている場合。
    ([uum-117576](https://issuetracker.unity3d.com/issues/setscheduled-end-time-does-not-work-on-webgl))




## 6000.3.10f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.addressables`: [2.8.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.8//changelog/CHANGELOG.html) から [2.9.0](https://docs.unity3d.com/Packages/com.unity.addressables@2.9//changelog/CHANGELOG.html) へ。

- `com.unity.probuilder`: [6.0.8](https://docs.unity3d.com/Packages/com.unity.probuilder@6.0//changelog/CHANGELOG.html)から[6.0.9](https://docs.unity3d.com/Packages/com.unity.probuilder@6.0//changelog/CHANGELOG.html)

- `com.unity.recorder`: [5.1.4](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) から [5.1.5](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) に変更。

- `com.unity.scriptablebuildpipeline`: [2.5.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.5//changelog/CHANGELOG.html) から [2.6.0](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html) に変更。

- `com.unity.splines`: [2.8.2](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html)から [2.8.3](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html)へ。

- `com.unity.xr.arcore`: [6.3.2](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.3//changelog/CHANGELOG.html) から [6.3.3](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.3//changelog/CHANGELOG.html) へ。

- `com.unity.xr.arfoundation`: [6.3.2](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.3//changelog/CHANGELOG.html)から[6.3.3](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.arkit`: [6.3.2](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.3//changelog/CHANGELOG.html)から[6.3.3](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.3//changelog/CHANGELOG.html)

- `com.unity.xr.management`: [4.5.3](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html) から [4.5.4](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html) に変更。

- `com.unity.microsoft.gdk`: [1.4.5](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.4//changelog/CHANGELOG.html) から [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html) に変更。

- `com.unity.microsoft.gdk.tools`: [1.4.5](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.4//changelog/CHANGELOG.html) から [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html) に変更。

- `com.unity.microsoft.gdk.discovery`: [1.1.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.1//changelog/CHANGELOG.html) から [1.2.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html) に変更。

- `com.unity.services.multiplayer`: [2.1.1](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.1//changelog/CHANGELOG.html) から [2.1.2](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.1//changelog/CHANGELOG.html) に変更。