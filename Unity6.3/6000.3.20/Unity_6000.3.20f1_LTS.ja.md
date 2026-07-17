# Unity 6000.3.20f1 LTS
公開日時：2026年7月16日（木）13:36:03 GMT  
https://unity.com/releases/editor/whats-new/6000.3.20f1

# 6000.3.20f1 の既知の問題

- `6000.0.23f1`: アニメーターの評価中に RigBuilder が再バインドを行った後、プレイモードを終了する際に Animator::OnPlayableUnbind でクラッシュする
    ([UUM-146750](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146750))

- `6000.0.67f1`: [iOS] iOSのコントロールセンターにアクセスすると音声が途切れる
    ([UUM-145522](https://issuetracker.unity3d.com/issues/ios-audio-is-cut-out-when-accessing-ios-control-center))

- `アセットインポーター`: プレイモードに入ると、「(Unity) WriteObjectToVector」の処理中にエディターがクラッシュする
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

bee_backendが複数実行されている際にmono_log_write_logfileでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

フォントアトラスの生成時に複数のスタックトレースが発生し、クラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.3.20f1 リリースノート

## 改善点

- `ビルドシステム`: 同梱の 7-Zip をバージョン 26.02 に更新しました。

- `グラフィックス`: ミップマップストリーミングのマニュアルページを更新し、UnityがメッシュのUVデータとカメラ位置からミップマップレベルをどのように選択するかを説明しました。また、Unityがレベルを計算できないオブジェクト（\(パーティクルシステムなどの手続き的に生成されたジオメトリを含む\)）の挙動を明確化し、`Texture2D.requestedMipmapLevel` のコード例を追加しました。
    ([UUM-131691](https://issuetracker.unity3d.com/issues/texture-rendered-at-different-fidelity-with-particle-system-renderer-when-using-a-different-material-derived-from-the-same-texture-with-identical-settings))

- `Physics`: 「プロジェクト設定」→「Physics」→「設定」→「GameObjects」に、マルチスレッドとシングルスレッドのシミュレーションを切り替えることができるドロップダウンメニューを追加しました。
    (UUM-144574)



## 修正点

- `2D`: インスペクターウィンドウ内の「スプライトアトラスインポーター」ボタンの *参照を開く* が、古いバージョンのマニュアルにリダイレクトされる問題を修正しました。
    ([UUM-133073](https://issuetracker.unity3d.com/issues/open-reference-for-sprite-atlas-importer-button-in-inspector-window-redirects-to-an-outdated-version-of-the-manual))

- `2D`: ライトバッチングデバッガーで、レイヤー名の並べ替えが反映されない問題を修正しました。
    ([UUM-136214](https://issuetracker.unity3d.com/issues/layer-names-in-the-light-batching-debugger-window-do-no-update-ウィンドウを再起動するか、既存のレイヤーをリネームする際に新しいレイヤーを追加しない限り))

- `2D`: プレイヤーをビルドする際、ビルド対象のすべてのシーンに含まれるスプライトアトラスのテクスチャがエディタのメモリに残ってしまう問題を修正しました。
    ([UUM-137607](https://issuetracker.unity3d.com/issues/sprite-atlas-textures-from-all-included-build-scenes-persist-in-editor-memory-when-building-the-player))

- `2D`: 編集用に開かれているタイルパレット上でドラッグ＆ドロップを行った際に、新しいタイルアセットを作成すると例外が発生する問題を修正しました。
    ([UUM-143122](https://issuetracker.unity3d.com/issues/missingreferenceexception-during-image-import-to-tile-palette-when-in-tile-palette-edit-mode))

- `2D`: Light2Dのシリアライゼーションに関する競合を修正しました。
    (UUM-141743)

- `2D`: チャンクモードで `TilemapRenderer` を使用する際、反転したタイルの法線マップに関する問題を修正しました。
    ([UUM-143429](https://issuetracker.unity3d.com/issues/flipped-tiles-with-normal-maps-are-inverted-with-tilemaprenderer-with-chunk-mode))

- `2D`: タイルパレットから選択ツールを使用した後、ペイントなどの別のツールに切り替えた際に、シーンが「変更済み」と表示される問題を修正しました。
    ([UUM-141736](https://issuetracker.unity3d.com/issues/scene-becomes-dirty-when-selecting-a-tile-palette-cell-and-then-switching-to-the-paint-tool))

- `2D`: GridSelectionToolの「スケール」を変更して負の値に拡大縮小した際、タイルがちらつく問題を修正しました。
    ([UUM-141782](https://issuetracker.unity3d.com/issues/tile-sprite-flickers-when-scaled-to-negative-values))

- `2D`: Delete キーまたは Backspace キーを使用して GridSelection を削除する際、編集用にタイルパレットのロックを解除するようにしました。
    ([UUM-141744](https://issuetracker.unity3d.com/issues/unable-to-delete-tiles-from-tile-palette-permanently-with-the-delete-key))

- `アクセシビリティ`: Android 環境で `AccessibilityRole.Slider`、`AccessibilityRole.TextField`、および `AccessibilityRole.SearchField` のアクセシビリティノードがハードウェアキーボードからの入力を受け取るために、開発者が実行すべき手順を文書化しました。
    ([UUM-126557](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-126557))

- `Android`: 使用されていない Tools 26.1.1 のダウンロードファイルを空のフォルダに置き換えました。
    (UUM-141878)

- `Audio`: 非同期でのサウンド読み込み中に発生するデータ競合が原因で、`Sound.getOpenState` でまれに発生していたクラッシュを修正しました。
    ([UUM-145498](https://issuetracker.unity3d.com/issues/crash-in-fmod-when-using-load-in-background))

- `ビルドシステム`: `dotnet` を呼び出す際に使用される他のメソッドに `MSBUILDDEBUGPATH` を追加しました。

- `コア`: GameObject をクローンする際、`Transform` のシリアライズされた値が正しく初期化されない問題を修正しました。
    ([UUM-131305](https://issuetracker.unity3d.com/issues/transform-corruption-and-slash-or-crash-on-physx-createcharactercontroller-when-spawning-physics-objects-into-prefab-stages))

- `ドキュメント`: コンポーネントの使用方法に関する情報を追加しました。

- `ドキュメント`: UITK ポップアップのサンプルコードと手順に、背景情報や詳細を追加しました。

- `ドキュメント`: VFX オペレーター Reciprocal の誤った 'out' プロパティを修正しました。
    (UUM-144446)

- `エディタ`: オーディオ: 破損したオーディオミキサーアセットを含むプロジェクトを開いた際にエディタがクラッシュする問題を修正しました。
    ([UUM-143706](https://issuetracker.unity3d.com/issues/crash-on-audiomixercontroller-removeinvalidsendlevelguidsrecursive-when-opening-a-project-with-specific-audio-files-for-the-first-time))

- `エディター`: エディターのシャットダウン中に、マネージドの `DomainUnload` ハンドラーが `UnityEngine.Object` の null チェックを実行した際に発生していたクラッシュ（`ProfilerMutexLock / assertion gPersistentManager \!= NULL`）を修正しました。
    ([UUM-144371](https://issuetracker.unity3d.com/issues/crash-on-profilermutexlock-when-closing-a-project-with-specific-assets))

- `エディター`: シーンファイルに、追加コンポーネントのリストが不正な形式のプレハブインスタンスが含まれている場合に発生していたクラッシュを修正しました。
    ([UUM-145507](https://issuetracker.unity3d.com/issues/crash-on-deleteprefabinstanceobjectsformissingprefabs-when-opening-a-specific-scene))

- `エディタ`: 検索ウィンドウをドッキングした際に、QueryTree ハンドラが正しく設定されない問題を修正しました。
    ([UUM-132981](https://issuetracker.unity3d.com/issues/nullreferenceexception-errors-are-thrown-in-the-console-when-clicking-on-saved-built-in-reports-in-docked-search-window))

- `エディタ`: Wayland上で実行中に、ファイルをエディタにドラッグした際に発生していたLinuxエディタのエラーを修正しました。
    ([UUM-111593](https://issuetracker.unity3d.com/issues/linux-the-error-releasebutton-expects-buttonid-is-thrown-when-trying-to-add-file-using-drag-and-hold-in-the-project-window))

- `エディタ`: 同じフォントを指す 2 つの異なる FontAsset を使用した場合に ATG で発生していたフォントの表示異常を修正しました。
    (UUM-133996)

- `エディタ`: 「CreateEmptyParent」メニュー項目を使用した後、元に戻す/やり直し操作でデフォルトの親オブジェクトがクリアされてしまう問題を修正しました。
    ([UUM-115213](https://issuetracker.unity3d.com/issues/performing-redo-create-empty-parent-object-action-resets-default-parent-object-in-the-scene))

- `エディタ`: プラットフォームを選択して「ビルドプロファイルの追加」をクリックしても、プラットフォームブラウザダイアログでそのプラットフォームが選択されないという動作を修正しました。
    (UUM-130650)

- `エディタ`: 選択時にネイティブのモーダルダイアログが開いた際、オブジェクトセレクタがフリーズするのを防ぎました。
    ([UUM-139847](https://issuetracker.unity3d.com/issues/object-selector-becomes-unresponsive-when-selecting-root-ui-document-as-data-source-for-add-binding-in-ui-builder))

- `エディタ`: LMDBの軽微なメモリリークを修正しました。
    (UUM-138144)

- `エディタ`: 型不一致を防ぐため、エディタはプレイヤーデータを書き込む前に参照のサニタイズを行うようになりました。
    ([UUM-143556](https://issuetracker.unity3d.com/issues/crash-in-player-when-calling-setactive-on-a-gameobject-with-a-type-mismatched-reference))

- `エディタ`: `QuaternionEulerField` の入力検証を強化し、NaN および無限大が有効な入力として受け入れられなくなりました。
    ([UUM-142032](https://issuetracker.unity3d.com/issues/game-object-brush-orientation-value-fields-に-NaN-または-無限大-の-値-を入力すると-コンソールに-クォータニオン関連のエラーが-大量に-表示され-タイル-パレット-ウィンドウで-値を-元に戻さない限り-エラーが-解消されない-問題))

- `GI`: 「ライティング」＞「アダプティブ・プローブ・ボリューム」＞「現在のベイクセット」プロパティで、現在設定されているAPVベイクセットを選択できない不具合を修正しました。
    ([UUM-145389](https://issuetracker.unity3d.com/issues/apv-data-becomes-incorrect-when-reselecting-the-currently-active-baking-set))

- `Graphics`: レイトレーシング使用時の DirectX12 スプリット・グラフィックス・ジョブにおけるクラッシュを修正しました。
    (UUM-145956)

- `Graphics`: Windows 環境で Vulkan を使用し、Split Graphics Jobs を実行する際、キャッシュに null が挿入され、その結果、DrawCalls が閉じられたコマンドバッファへの描画を試み、クラッシュを引き起こす問題を解決しました。
    (UUM-132307)

- `IL2CPP`: Linux 環境で空の .usym ファイルが生成される問題を修正しました。
    ([UUM-142527](https://issuetracker.unity3d.com/issues/linux-stack-trace-file-path-and-line-number-information-is-missing-when-il2cpp-stacktrace-information-is-set-to-method-name-file-name-and-line-number))

- `カーネル`: 多数の外部スレッドおよび手動ジョブが関与するジョブシステムにおける潜在的なデッドロックを修正しました。
    (UUM-143073)

- `Networking`: UnityWebRequest から発生する Curl エラーが適切にログに記録されず、問題のデバッグが困難になる状況を修正しました。なお、この状況下でも、失敗は呼び出し元コードに対して正しく報告されていました。このバグはログ記録にのみ影響していました。
    ([UUM-145433](https://issuetracker.unity3d.com/issues/unitywebrequest-can-lose-error-messages-from-curl))

- `ネットワーク`: UnityWebRequestにおいて、アップロードリクエストを再開した際に、エラー 26 または 65（「必要なデータの巻き戻しができませんでした」）がログに記録されることがある問題を修正しました。
    ([UUM-144767](https://issuetracker.unity3d.com/issues/webrequest-missing-curlopt-seekfunction-causes-curl-error-26-on-post-retry-with-reused-connections))

- `パッケージマネージャー`: Unityの起動時に、一部のパッケージの署名アイコンが正しく表示されない問題を修正しました。
    ([UUM-143201](https://issuetracker.unity3d.com/issues/signed-registry-packages-show-green-shield-icon-when-show-pre-release-package-versions-is-toggled-on))

- `プロファイラー`: macOS でプロファイリングデータを直接読み込んだ際、関連するファイルタイプ（.data、.raw）がフィルタリングされなかった問題を修正しました。
    ([UUM-139554](https://issuetracker.unity3d.com/issues/profiler-data-stream-has-invalid-signature-errors-are-thrown-when-loading-a-highlights-file-in-the-profiler))

- `Search`: ドメインの再読み込み時にバックグラウンドスレッドが適切にキャンセルされず、Search LMDB がクラッシュする問題を修正しました。
    ([UUM-141720](https://issuetracker.unity3d.com/issues/crash-on-mdb-cursor-sibling-when-performing-various-actions-in-the-editor))

- `Search`: ドメインの再読み込み中に、一部のバックグラウンドスレッドが孤立して停止できなくなり、Search LMDB がクラッシュする問題を修正しました。
    ([UUM-143640](https://issuetracker.unity3d.com/issues/crash-on-mdb-database-getmapsize-when-domain-reloads-while-background-search-indexing-is-active))

- `SRP Core`: HDR出力レンダリング中に、.NETがフレーム間でプールされた配列バッファを解放した際に断続的に発生していた、まれなマネージド割り当てを削除しました。
    (UUM-145447)

- `Text`: FT_Done_Face でのエディタの終了時のクラッシュを修正しました。
    ([UUM-144575](https://issuetracker.unity3d.com/issues/clash-on-unity-ft-done-face-when-closing-the-editor-after-rendering-text-with-the-advanced-text-generator-using-a-runtime-created-font-asset))

- `UI Toolkit`: SVGのインポートに失敗する代わりに、無効な`stroke-miterlimit`値をクリップするようにしました。
    ([UUM-120825](https://issuetracker.unity3d.com/issues/svg-fails-to-import-when-stroke-miterlimit-is-less-than-1))

- `UI Toolkit`: カスタムシェーダーを使用して固定色を出力する際、楕円形が長方形として表示される問題を修正しました。
    ([UUM-145855](https://issuetracker.unity3d.com/issues/arc-aa-isnt-applied-when-using-a-custom-shader-that-outputs-a-constant))

- `UI Toolkit`: デバッグインスペクタでリストの要素を追加または削除する際に `ObjectDisposedException` が発生する問題を修正しました。
    ([UUM-143676](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143676))

- `URP`: URPスタンドアロンプレイヤービルドにおいて、プレイヤーログにリーク警告が発生していたメモリリークの問題を修正しました。
    ([UUM-115886](https://issuetracker.unity3d.com/issues/jobtempalloc-memory-leak-warning-is-thrown-when-the-player-is-shut-down))

- `URP`: ダートテクスチャが有効になっているが値が null の場合、ブルームのランタイムシェーダーバリアントが誤って選択される問題を修正しました。
    ([UUM-141980](https://issuetracker.unity3d.com/issues/bloom-post-processing-effect-in-urp-is-missing-in-a-build-when-dirt-texture-is-enabled-in-the-bloom-override-of-a-global-volume))

- `Web`: Player Graphics API が WebGPU に設定されている場合、再生中に VideoPlayer.frameReady が 1 回しか発火しない問題を修正しました。
    ([UUM-141418](https://issuetracker.unity3d.com/issues/web-videoplayer-dot-frameready-event-fires-only-once-in-a-video-when-the-player-graphics-api-is-set-to-webgpu))

- `WebGL`: WebGPU: float32-blendable WebGPU 拡張機能がないために一部のモバイルデバイスで発生していたエラーを修正しました。
    ([UUM-145735](https://issuetracker.unity3d.com/issues/webgpu-urp-errors-when-float32-blendable-isnt-available))

- `WebGL`: \[WebGPU\] シェーダーの破棄および作成時に発生する可能性のあるクラッシュを修正しました。
    ([UUM-145390](https://issuetracker.unity3d.com/issues/type-error-is-thrown-when-a-new-computeshader-is-instantiated-after-destroying-previous-computeshader))

- `Windows`: WindowsでNew Input Systemを使用し、`<Pointer>/position`バインディングを適用した際、Game View内でペンの位置が限られた領域に制限されてしまう問題を修正しました。
    ([UUM-142269](https://issuetracker.unity3d.com/issues/pen-position-gets-constrained-to-a-limited-area-when-using-a-stylus-in-game-view-or-player))




## 6000.3.20f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.ads`: [4.16.4](https://docs.unity3d.com/Packages/com.unity.ads@4.16//changelog/CHANGELOG.html) から [4.19.0](https://docs.unity3d.com/Packages/com.unity.ads@4.19//changelog/CHANGELOG.html) へ

- `com.unity.services.cloudcode`: [2.10.2](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.10//changelog/CHANGELOG.html) から [2.10.3](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.10//changelog/CHANGELOG.html)

- `com.unity.services.vivox`: [16.10.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.10//changelog/CHANGELOG.html) から [16.11.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.11//changelog/CHANGELOG.html)

- `com.unity.xr.compositionlayers`: [2.4.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.4//changelog/CHANGELOG.html) から [2.5.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.5//changelog/CHANGELOG.html) へ

- `com.unity.services.multiplayer`: [2.2.3](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.2//changelog/CHANGELOG.html) から [2.2.4](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.2//changelog/CHANGELOG.html) へ