# Unity 6000.0.69f1 LTS
公開日時: Wed, 04 Mar 2026 09:50:56 GMT
https://unity.com/releases/editor/whats-new/6000.0.69f1

# 6000.0.69f1 の既知の問題点

- `6000.1.0a2,6000.0.64f1`: シングルパスステレオレンダリングでプレイモードに入るとSkyboxしか表示されない
    ([uum-132342](https://issuetracker.unity3d.com/issues/single-pass-stereo-rendering-shows-only-skybox-when-entering-play-mode))

- `6000.2.0a2,6000.0.38f1`: [Android][IL2CPP][ARMv7] 値が大きな構造体を持つジェネリックデリゲートを呼び出すと、構造体フィールドの値が破損する
    ([uum-134192](https://issuetracker.unity3d.com/issues/android-il2cpp-armv7-struct-field-value-corrupts-when-invoking-a-generic-delegate-with-a-large-struct-by-value))

- `6000.3.0a4,6000.0.62f1`: 前の入力がキャンセルされた後に同じ入力フィールドを選択しても、入力フィールドが更新されない
    ([uum-133712](https://issuetracker.unity3d.com/issues/input-field-does-not-update-when-selecting-the-same-input-field-after-previous-input-was-canceled))

- `6000.5.0a3,6000.4.0b8,6000.3.8f1,6000.0.68f1`: [iOS] Info.plistにUIApplicationSceneManifestを追加しても、アプリの実行中にApplication.deepLinkActivatedが起動されない。
    ([uum-135497](https://issuetracker.unity3d.com/issues/ios-application-dot-deeplinkactivated-does-not-get-invoked-while-app-is-running-when-uiapplicationscenemanifest-is-added-in-info-dot-plist))

- `IL2CPP`: [iOS] [Android] IL2CPPビルド中に外部ライブラリのジェネリックに失敗する
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- `メタル`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `Windows`: バックグラウンドで実行" が有効でアクティブウィンドウが切り替わるとプレイヤーがハングする
    ([uum-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))

DirectX 12の排他的フルスクリーンモードでフォーカスを切り替えるとプレイヤーがクラッシュする
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))

[Silicon] Razer Synapseアプリを開いているときにプロジェクトを開くとos_unfair_recursive_lock_with_optionsでクラッシュする
    ([uum-135043](https://issuetracker.unity3d.com/issues/silicon-crash-on-os-unfair-recursive-lock-lock-with-options-when-opening-a-project-while-the-razer-synapse-app-is-open))



# 6000.0.69f1 リリースノート

## 改良点

- `インストーラー`: Windows システム上の .NET 3.5 のアクティベーションを削除。インストーラーを直接使用する場合のインストール時間を大幅に短縮。
    (UUM-133360)



## 修正

- `Android`: カスタム Gradle テンプレートに `compileSdkVersion` 属性がある場合に `GradleTemplateUpdater` からのダイアログが表示される問題を修正した。
    ([uum-134142](https://issuetracker.unity3d.com/issues/android-gradle-compilesdkversion-is-incorrectly-deprecated-on-6-dot-0-6-dot-4))

- `Android`: UI Toolkit入力フィールドのキャレット位置がTouchScreenKeyboardでテキスト選択を変更したときに更新されない問題を修正しました。
    ([uum-128088](https://issuetracker.unity3d.com/issues/android-soft-keyboards-arrows-and-select-tools-do-not-have-visual-feedback-when-hide-mobile-input-is-enabled))

- `Android`: Android `GameActivity` を使用しているときに `OnApplicationQuit` が一貫して呼び出されない問題を修正しました。
    (UUM-131090)

- `Android`: Device Simulator のデバイス定義を更新し、古いデバイスの特定のモデル名ではなく、一般的な特性ベースの名前を使用するようにしました。
    (UUM-134051)

- `DX12`: DXC シェーダー・コンパイラーを使用する際のクラスター・ライティングの問題を修正。
    (UUM-134785)

- `DX12`: 最終アップスケールパスの間、プロキシバッファの srv フォーマットを swapchain rtv のフォーマットと一致。
    ([UUM-134064](https://issuetracker.unity3d.com/issues/dx12-player-brightness-changes-when-changing-display-resolution-with-screen-dot-setresolution))

- `Editor`: Hub インストールと Hub ドキュメントへのリンクを追加。

- `エディター`: Burst SharedStaticメモリがエディターのシャットダウン前にクリアされるようになり、シャットダウン中にジョブがスケジュールされた場合にクラッシュすることがあった問題を修正。
    ([uum-133804](https://issuetracker.unity3d.com/issues/crash-on-extracthandles-when-shutting-down-the-editor-in-a-specific-scene-while-burst-jobs-are-in-progress))

- `エディター`: playmodeでRender Pipeline Converterウィンドウを開こうとすると、関係のないウィンドウが開いてしまうバグを修正しました。
    ([uum-132083](https://issuetracker.unity3d.com/issues/the-sprite-importer-window-is-opened-instead-of-the-render-pipeline-converter-window-when-opening-it-in-play-mode))

- `Editor`: EditorUtility.CompressTexture/EditorUtility.CompressCubemapTextureが、符号付きEACフォーマットへの圧縮を処理のあまりに遅い段階で中断し、テクスチャを壊れた状態のままにしてしまう問題を修正しました。符号付きEACフォーマットは圧縮のためにサポートされていないことに注意してください。

- `Editor`: Ubuntuのパッケージマネージャーでパッケージのエクスポートダイアログを開くとハングアップしたりウィンドウが文字化けする問題を修正しました。
    ([uum-131283](https://issuetracker.unity3d.com/issues/ubuntu-package-managers-export-package-window-is-rendered-with-artifacts-when-editor-is-running-on-opengl))

- `エディター`: スクリプトのコンパイルが Windows と Linux で異なる結果となり、複数のプラットフォームで作業しているチームにとって不必要なアセットファイルの変更を引き起こしていた問題を修正しました。
    (UUM-133554)

- `エディター`: EditorUtility.CompressTexture/EditorUtility.CompressCubemapTextureで、NPOTミップマップされたテクスチャをサポートされていないターゲット形式に圧縮しようとする可能性があった問題を修正しました。この件に関する追加の詳細が API ドキュメントに追加されました。
    ([uum-129605](https://issuetracker.unity3d.com/issues/corrupted-mipmaps-are-generated-when-using-editorutility-dot-compresstexture-with-npot-textures))

- `エディター`: プレイヤー設定のスクリプト定義リスト項目を追加・削除する際に、不要な適用ポップアップが表示されるのを修正しました。
    ([uum-121033](https://issuetracker.unity3d.com/issues/do-you-want-to-apply-changes-warning-pop-up-appears-when-adding-and-removing-list-items-in-player-settings))

- `エディター`: アトラスがエディターフォントに対して大きくなりすぎる場合のDebug.Assert警告を修正。
    ([uum-85059](https://issuetracker.unity3d.com/issues/assert-error-is-thrown-when-the-editor-language-is-set-to-one-of-the-experimental-ones-in-an-hdrp-project))

- `エディター`: スクリプト可能なレンダーパスを持つプロジェクトで、ビルドプロファイルを切り替えたときに、一時的なアタッチメントに関するコンソールエラーがエディターで投げられることがありました。これは修正されました。
    ([uum-97475](https://issuetracker.unity3d.com/issues/gbuffer-slash-render-deferred-lighting-and-render-pass-related-errors-constantly-thrown-after-switching-a-build-profile))

- `Graphics`: カメラプレビュー - パイプラインを変更する際に、レンダーターゲットテクスチャが再作成されず、無効なレンダーテクスチャオプションが作られていました。
    ([uum-133293](https://issuetracker.unity3d.com/issues/after-converting-a-built-in-project-to-urp-render-texture-setting-error-message-is-spammed))

- `Graphics`: メタル(Metal)使用時にステンシルのアタッチメントが正しく設定されず、メタル(Metal)の検証エラーが発生する問題を修正しました。
    (UUM-133783)

- `Graphics`: TexturesD3D11Base::SetTexture`のDX11クラッシュを修正しました。
    ([UUM-134071](https://issuetracker.unity3d.com/issues/crash-on-texturesd3d11base-settexture-when-using-directx11))

- `Graphics`: WebGPU で複数のレンダーターゲットをクリアする際の問題を修正しました。
    ([uum-133743](https://issuetracker.unity3d.com/issues/webgpu-urp-rendergraph-renderpass-doesnt-clear-textures))

- `IL2CPP`: デバッグ c++ 設定で WebRequests を使用すると Switch プラットフォームでクラッシュする問題を修正。
    (UUM-127898)

- `IL2CPP`: 汎用パラメータ型の内部ハッシュ関数を改良して起動時間を短縮した。
    (UUM-133424)

- `Input`: 入力システムのスクロールデルタの動作が常に正規化されるというリグレッションが発生。これは修正されました。
    (UUM-134566)

- `入力システム`: 入力デバイスがメインスレッド以外のスレッドで検出されるプラットフォームで Unity のクラッシュや未定義の動作につながる可能性のある同期プリミティブの不正な使用を修正しました。
    (UUM-134537)

- `macOS`: シーンロード中にキーボード入力がリセットされる問題を修正しました。
    ([UUM-132112](https://issuetracker.unity3d.com/issues/keyboard-state-is-reset-when-automatically-loading-a-scene-via-script))

- `macOS`: macOSで多くのファイルを開いている時にネットワーク要求が失敗する問題を修正しました。
    (UUM-134087)

- `Mono`: インクリメンタル GC マーキングとルート登録解除の間の競合状態を修正。
    (UUM-131742)

- `パッケージマネージャ`: パッケージマネージャ：パッケージマネージャ：upm パッケージを使用した Url のディープリンクで、検出可能であれば選択されたパッケージを表示します。また、バージョンが指定されている場合、またはパッケージが検出可能でない場合、Add ポップアップを表示します。
    (PAK-8687)

- `物理`: 内部コリジョンメッシュにレイキャストが発射されないためにブラシが表示されないという問題を修正しました。
    ([uum-61756](https://issuetracker.unity3d.com/issues/paintable-area-is-offset-from-the-mesh-when-editing-cloth-constraints))

- `Player`: Video Playerがパスにスペースが含まれるファイルを開いた際に発生したURLパースの問題を修正。
    ([uum-125789](https://issuetracker.unity3d.com/issues/video-does-not-play-in-macos-build-when-built-app-is-placed-in-a-path-with-a-space-in-it-on-a-specific-project))

- `シーン/ゲームビュー`: アクティブな選択範囲にフォーカスすると、シーンビューでオーバーレイの内容が編集されてしまう問題を修正しました。
    ([uum-134399](https://issuetracker.unity3d.com/issues/overlays-are-focused-when-using-the-frame-selected-in-window-under-cursor-shortcut-just-after-editing-overlay-fields))

- `Shadergraph`: 一部のプラットフォームでビルトインレンダーパイプラインのシェーダーグラフをコンパイルする際、"fixed "が再定義される警告を修正。
    (UUM-126357)

- `シェーダー`: 計算中の RWTexture2D への書き込みを修正。
    (UUM-127198)

- `テキストメッシュプロ`: href "部分が欠落している不適切な書式の&lt;a&gt;タグの処理を改善。正しくフォーマットされたタグは &lt;a href="リンクID"&gt;ハイライトされるテキスト&lt;/a&gt; となります。
    ([uum-130554](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-occurs-when-entering-tags-in-a-textmeshpro-ui-field))

- `uGUI`: 非常に大きなrectトランスフォームの境界がある場合に発生するクラッシュを修正。
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `uGUI`: 非常に大きなrectトランスフォーム境界を持つことによって引き起こされるクラッシュの根本原因を修正。影響を受けるシーンのGameObjectにリンクする警告を追加しました。
    (UUM-134019)

- `UIツールキット`: コレクションがソートされた時に、正しくないインデックスがMultiColumnTreeViewとMultiColumnListViewのデータソースパスに適用されていた問題を修正しました。
    ([uum-133865](https://issuetracker.unity3d.com/issues/multicolumnlistview-does-not-visually-sort-the-column-when-bindingsourceselection-is-set-to-auto-assign))

- `UIツールキット`: PanelSettings.renderMode がパブリック API になりました。
    (UUM-119486)

- `取り消しシステム`: ルートGameObjectsの複数選択でTransformタイプを置き換えるアンドゥ／リドゥを行う際、ルートGameObjectsが階層順序を変更するのを修正。
    ([uum-133391](https://issuetracker.unity3d.com/issues/gameobjects-change-hierarchy-order-when-undoing-adding-component-to-multiple-gameobjectsgameobjects-change-hierarchy-order-when-undoing-adding-component-to-multiple-gameobjects))

- `Web`: タッチキャンセルイベントを処理する際に発生していたバグを修正。
    ([uum-132183](https://issuetracker.unity3d.com/issues/mouse-postion-can-become-max-value-or-infinity-when-using-touch-input-with-legacy-input-module))

- `WebGL`: AudioSource.SetScheduledEndTimeのバグを修正しました。SetScheduledEndTimeが呼ばれた時に、起動時にAudioSourceの再生要求が保留されていた場合。
    ([uum-117576](https://issuetracker.unity3d.com/issues/setscheduled-end-time-does-not-work-on-webgl))

- `WebGL`: \WebGPU]CoreCopyシェーダによるMSAAテクスチャのRenderGraphエラーを修正しました。
    ([uum-133838](https://issuetracker.unity3d.com/issues/webgpu-errors-when-corecopy-shader-is-used-to-copy-an-msaa-texture))




## 6000.0.69f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.addressables`: [2.8.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.8//changelog/CHANGELOG.html) から [2.9.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.9//changelog/CHANGELOG.html) へ。

- `com.unity.inputsystem`: [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html) から [1.19.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.19//changelog/CHANGELOG.html)

- `com.unity.probuilder`: [6.0.8](https://docs.unity3d.com/Packages/com.unity.probuilder@6.0//changelog/CHANGELOG.html) から [6.0.9](https://docs.unity3d.com/Packages/com.unity.probuilder@6.0//changelog/CHANGELOG.html)

- `com.unity.recorder`: [5.1.4](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) から [5.1.5](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) に変更。

- `com.unity.scriptablebuildpipeline`: [2.5.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.5//changelog/CHANGELOG.html) から [2.6.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html) に変更。

- `com.unity.services.wire`: [1.4.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html)から[1.4.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html)

- `com.unity.splines`: [2.8.2](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html) から [2.8.3](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html) へ。

- `com.unity.xr.management`: [4.5.3](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html) から [4.5.4](https://docs.unity3d.com/Packages/com.unity.xr.management@4.5//changelog/CHANGELOG.html) へ。

- `com.unity.xr.oculus`: [4.5.2](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html) から [4.5.4](https://docs.unity3d.com/Packages/com.unity.xr.oculus@4.5//changelog/CHANGELOG.html) に変更。

- `com.unity.terrain-tools`: [5.3.1](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html) から [5.3.2](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html) に変更。

- `com.unity.ai.navigation`: [2.0.10](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)から[2.0.11](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.addressables.android`: [1.0.9](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html)から[1.0.10](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk`: [1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.4//changelog/CHANGELOG.html) から [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html) に変更。

- `com.unity.microsoft.gdk.tools`: [1.4.4](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.4//changelog/CHANGELOG.html) から [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html) まで。

- `com.unity.microsoft.gdk.discovery`: [1.1.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.1//changelog/CHANGELOG.html) から [1.2.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html) まで