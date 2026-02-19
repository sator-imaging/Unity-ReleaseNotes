# Unity 6000.0.68f1 LTS
公開日時: Wed, 18 Feb 2026 14:49:24 GMT
https://unity.com/releases/editor/whats-new/6000.0.68f1

# 6000.0.68f1 の既知の問題

- `6000.0.55f1,6000.3.0a4`: UI を切り替えながらマルチプレイヤールームを作成すると RaiseException でクラッシュする
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `6000.0.65f1,6000.5.0a4,6000.3.3f1,6000.4.0b2`: 地形ツールが既に元に戻されている場合に、前の地形曲率に従うようになりました。
    ([uum-134053](https://issuetracker.unity3d.com/issues/the-terrain-tools-follow-the-previous-terrain-curvature-when-it-was-already-undone))

- `6000.2.0a7,6000.0.48f1`: [URP] デカール・レンダラー・テクニックが "自動 "に設定されている場合、バッチモードでビルドしたとき、またはエディターでシーン/ゲーム・ビューをレンダリングせずにビルドしたときに、すべてのマテリアルが黒くレンダリングされる。
    ([uum-134298](https://issuetracker.unity3d.com/issues/urp-all-materials-render-black-when-building-via-batchmode-or-without-rendering-scene-slash-game-view-in-editor-if-decal-renderer-technique-is-set-to-automatic))

- `6000.3.0a4,6000.0.62f1`: [iOS] ソフトキーボードで「キャンセル」ボタンを使用すると、テキスト入力フィールドが変更を受け付けなくなる
    ([uum-133751](https://issuetracker.unity3d.com/issues/ios-text-input-field-stops-receiving-changes-when-the-cancel-button-is-used-on-the-soft-keyboard))

- `6000.5.0a5`: Screen.SetResolution() でディスプレイの解像度を変更すると、DX12プレーヤーの明るさが変わる
    ([uum-134064](https://issuetracker.unity3d.com/issues/dx12-player-brightness-changes-when-changing-display-resolution-with-screen-dot-setresolution))

- `IL2CPP`: [iOS] [Android] IL2CPP ビルド時に外部ライブラリのジェネリックに失敗する
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- `メタル`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `Platform Audio`: [Windows] エディターで様々なアクションを実行すると AudioManager::InitFMOD でクラッシュする。
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))

- テキスト (TextMeshPro)：TMPro Font Asset CreatorでマルチスレッドのFont Atlasを生成するときにUNITY_FT_Load_Glyphでクラッシュする
    ([uum-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

空白のURPプロジェクトでプレイモードに入ったり終了したりすると、エディタのメモリリークが発生する
    ([uum-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))

DirectX 12の排他的フルスクリーンモードでフォーカスを切り替えるとプレイヤーがクラッシュする問題
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))



# 6000.0.68f1 リリースノート

## 改良点

- `Shadergraph`: ノードを折りたたんだ時の UV ノードのチャンネルドロップダウンの見た目を改善。
    ([uum-115034](https://issuetracker.unity3d.com/issues/uv-nodes-label-is-cut-off-when-preview-is-collapsed))



## 変更点

- `編集`: targetVelocity が設定された Prismatic Articulation Joint タイプを変更し、Target Velocity を正の値に設定すると、シミュレーション中に正の直線速度が発生するようにしました。同様に、Target Velocity を負の値に設定すると、直線速度は負になります。
    ([uum-113920](https://issuetracker.unity3d.com/issues/prismatic-articulationbody-moves-in-opposite-direction-when-using-targetvelocity))

- `Graphics`: テクスチャのインポートが https://docs.unity3d.com/Documentation/Manual/ImportingTextures.html でサポートされているフォーマットに厳密に従うようになりました。画像ファイルの拡張子を変更することでこれを回避することはできなくなりました。画像ファイルのフォーマットが必要な場合は、機能要求を提出してください。



## 修正

- `2D`: スプライトエディタウィンドウの情報ボックスがモジュールのUIに邪魔されるのを修正。
    ([uum-131899](https://issuetracker.unity3d.com/issues/inactive-skinning-editor-toolbar-overlaps-the-help-box-in-the-sprite-editor-when-asset-is-not-editable))

- `Android`: Android ライブラリドキュメントの余分なスペースを削除。
    (UUM-133945)

- `アニメーション`: AnimationWindowEvent インスペクタの壊れたドキュメントリンクを修正。
    ([UUM-131593](https://issuetracker.unity3d.com/issues/animation-event-is-missing-documentation-link))

- `アセットバンドル`: AssetBundleUnloadOperation` のアロケーションが予想以上に長く持続し、次の `GC.collect()` までクリアされない問題を修正しました。
    (UUM-132703)

- `バグレポーター`: Unity プロジェクトディレクトリにオフラインレポートをエクスポートする際の Bug Reporter のクラッシュを修正しました。
    ([UUM-129604](https://issuetracker.unity3d.com/issues/bug-reporter-crashes-when-exporting-offline-report-into-a-unity-project-directory))

- `DX12`: D3D12使用時にエディターでmaxQueuedFramesが1の時のデッドロックを修正。
    ([uum-131962](https://issuetracker.unity3d.com/issues/editor-freezes-when-qualitysettings-dot-maxqueuedframes-is-set-to-1-and-dx12-is-used))

- `エディター`: Profilerモジュール紹介にデフォルトのProfilerモジュールリストを追加。

- `エディター`: GameObjectインスペクタが無効化されたときにインスペクタから投げられるNullRefExceptionを修正。
    ([uum-130843](https://issuetracker.unity3d.com/issues/endlayoutgroup-beginlayoutgroup-must-be-called-first-error-is-thrown-when-manually-saving-a-complex-ui-prefab-asset))

- `Editor`: 外部ツールにおいて、署名チームIDとiOS/tvOSプロファイルIDの間に一貫性のないID値があったのを修正しました。
    ([uum-132053](https://issuetracker.unity3d.com/issues/inconsistent-id-values-between-signing-team-id-and-ios-slash-tvos-profile-id-in-external-tools))

- `エディター`: Androidのパブリッシング設定の「ビルド」セクションが、Androidのグローバル設定からのみ編集可能になった。
    ([uum-126778](https://issuetracker.unity3d.com/issues/publishing-settings-are-shared-across-different-custom-build-profiles-when-modifying-build-options))

- `エディター`: ProjectSettings で AssetPipeline の設定を行う際に RefreshSettings を行うようにしました。
    (UUM-129185)

- `Editor`: プレインGameObjectをプレハブに再接続する際に、子インスタンスを保持するようにしました。
    ([UUM-102262](https://issuetracker.unity3d.com/issues/child-prefab-instance-connection-lost-when-reconnecting-parent-prefab))

- `エディター`: Windows：バックグラウンドで実行するアプリケーションで、ユーザーがウィンドウのタイトルバーを右クリックしたときにゲームループを更新するようにしました。
    ([uum-124735](https://issuetracker.unity3d.com/issues/main-thread-freezes-when-right-clicking-on-the-title-bar-of-a-windowed-player-on-windows))

- `Graphics`: AssetBundlesからリソース(典型的にはTextures)をロードする時、まれに AsyncResourceUploadBlocking(◆)でデッドロックが発生するのを修正した。
    ([uum-126066](https://issuetracker.unity3d.com/issues/android-the-application-freezes-during-the-assetbundle-loading))

- `iOS`: UAaLセットアップでunityビューのリサイズがレンダリングを壊すかクラッシュするのを修正。
    ([uum-130881](https://issuetracker.unity3d.com/issues/ios-rendering-freezes-and-unitygfxdeviceworker-crash-when-show-splash-screen-is-enabled-and-project-is-built-using-unity-as-a-library))

- `iOS`: キーボードのUIをリキッドグラスによりフィットするように調整。
    (UUM-133464)

- `カーネル`: すべてのトランスフォームオプションの TransformAccess の同期を更新。
    (UUM-126050)

- `パッケージマネージャー`: Unity が空のコンソールタイトルでコマンドプロンプトから起動された場合に、Unity Package Manager が起動時にクラッシュすることがある Windows の問題を修正しました。
    (PAK-8605)

- `物理`: シーンのリロードが無効な状態でクロスコンポーネントをオーサリングするとクラッシュする問題を修正しました。オーサリングの直後に Playmode に入ると、Cloth インスタンスが "オーサリングのみ" の状態に保たれます。
    ([uum-110845](https://issuetracker.unity3d.com/issues/crash-on-clothscene-processcomponentupdates-when-entering-play-mode-after-editing-cloth-collision-points))

- `Shadergraph`: スウィズルノードマスクの大文字小文字が不適切な結果になることがある問題を追加しました。
    ([uum-132879](https://issuetracker.unity3d.com/issues/expected-color-is-changed-to-black-when-using-swizzle-node))

- `Shadergraph`: コピーペーストや複製後にノードが適切に選択されるようになりました。
    ([uum-110841](https://issuetracker.unity3d.com/issues/nodes-in-shader-graph-are-not-selected-when-they-are-duplicated))

- `UIツールキット`: UI ドキュメントがライブリロードを実行し、スクリプトが添付されていない場合に NULL 参照例外がスローされる問題を修正しました。
    ([uum-129344](https://issuetracker.unity3d.com/issues/nullreferenceexception-thrown-when-modifying-a-ui-document-while-a-scene-containing-a-gameobject-with-any-ui-document-and-a-missing-script-component-is-open))

- `UIツールキット`: 要素を削除した後にビルダーをドッキングするとNullReferenceExceptionがスローされる。
    ([uum-128717](https://issuetracker.unity3d.com/issues/docked-ui-builder-corrupts-when-the-domain-isnt-reloaded-after-deleting-an-element))

- `VFX Graph`: カーブやグラデーションの分岐で、GPUへのリベイクやアップロードが無意味になっていた問題を修正。
    (UUM-129743)

- `Web`: レガシー入力システムで、タッチ・イベントによるマウス位置のシミュレーションを修正しました。
    ([UUM-130369](https://issuetracker.unity3d.com/issues/input-dot-mouseposition-stops-syncing-to-touch-input-when-using-downloadhandlertexture-in-webgl-build))

- `WebGL`: WebGPU: シェーダーにバインドされたテクスチャを読み込みと書き込みの両方で自動的に処理。
    ([uum-131864](https://issuetracker.unity3d.com/issues/webgpu-cant-bind-compute-rwtexture-for-read-and-write))

- `WebGL`: WebGPU: シェーダーで RWTexture2D テクスチャを使用するパイプラインエラーを修正し、unorm RWTextures の使用を簡素化しました。
    ([uum-131863](https://issuetracker.unity3d.com/issues/webgpu-errors-with-unorm-and-half4-rwtexture))

- `WebGL`: WebGPU: ShaderVariantCollectionのウォームアップでコンソールのCreateRenderPipelineエラーを解決。
    ([uum-131262](https://issuetracker.unity3d.com/issues/webgpu-createrenderpipeline-errors-with-shadervariantcollection-warmup))




## 6000.0.68f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.addressables`: [2.8.0](https://docs.unity3d.com/Packages/com.unity.addressables@2.8//changelog/CHANGELOG.html) から [2.8.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.8//changelog/CHANGELOG.html) へ。

- `com.unity.burst`: [1.8.27](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) から [1.8.28](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.formats.alembic`: [2.4.2](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) から [2.4.4](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) へ。

- `com.unity.ide.visualstudio`: [2.0.26](https://docs.unity3d.com/Packages/com.unity.ide.visualstudio@2.0//changelog/CHANGELOG.html)から[2.0.27](https://docs.unity3d.com/Packages/com.unity.ide.visualstudio@2.0//changelog/CHANGELOG.html)

- `com.unity.mobile.notifications`: [2.4.2](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html)から[2.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: [2.5.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.5//changelog/CHANGELOG.html) から [2.5.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.5//changelog/CHANGELOG.html) へ。

- `com.autodesk.fbx`: 5.1.1 から 5.1.3

- `com.unity.memoryprofiler`: [1.1.9](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) から [1.1.11](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- `com.unity.multiplayer.tools`: [2.2.7](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) から [2.2.8](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) へ。

- `com.unity.dt.app-ui`: [1.3.1](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.3//changelog/CHANGELOG.html) から [1.3.5](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.3//changelog/CHANGELOG.html) に変更。

- `com.unity.ai.inference`: [2.4.1](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.4//changelog/CHANGELOG.html) から [2.5.0](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.5//changelog/CHANGELOG.html)