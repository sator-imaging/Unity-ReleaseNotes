# Unity 6000.3.9f1 LTS
公開日時: Wed, 18 Feb 2026 11:29:51 GMT
https://unity.com/releases/editor/whats-new/6000.3.9f1

# 6000.3.9f1 の既知の問題

- `6000.0.55f1,6000.3.0a4`: UI を切り替えながらマルチプレイヤールームを作成すると RaiseException でクラッシュする
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `6000.0.65f1,6000.5.0a4,6000.3.3f1,6000.4.0b2`: 地形ツールが既に元に戻されている場合に、前の地形曲率に従うようになりました。
    ([uum-134053](https://issuetracker.unity3d.com/issues/the-terrain-tools-follow-the-previous-terrain-curvature-when-it-was-already-undone))

- `6000.2.0a7,6000.0.48f1`: [URP] デカール・レンダラー・テクニックが "自動 "に設定されている場合、バッチモードでビルドしたとき、またはエディターでシーン/ゲーム・ビューをレンダリングせずにビルドしたときに、すべてのマテリアルが黒くレンダリングされる。
    ([uum-134298](https://issuetracker.unity3d.com/issues/urp-all-materials-render-black-when-building-via-batchmode-or-without-rendering-scene-slash-game-view-in-editor-if-decal-renderer-technique-is-set-to-automatic))

- `6000.3.0a1`: PhysicsCommands::PhysX::GetShapeGeometryHolderで、無効化されたオブジェクトのメソッドを呼び出すとクラッシュする。
    ([uum-134161](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-getshapegeometryholder-when-calling-a-method-on-a-disabled-object))

- `6000.3.0a4,6000.0.62f1`: [iOS] ソフトキーボードで「キャンセル」ボタンを使用すると、テキスト入力フィールドが変更を受け付けなくなる
    ([uum-133751](https://issuetracker.unity3d.com/issues/ios-text-input-field-stops-receiving-changes-when-the-cancel-button-is-used-on-the-soft-keyboard))

- `6000.3.5f1`: NavMeshの障害物をカービングを有効にして移動するとCPU使用率が増加する
    ([uum-133911](https://issuetracker.unity3d.com/issues/increased-cpu-usage-when-moving-navmesh-obstacles-with-carving-enabled))

- `6000.5.0a5`: Screen.SetResolution() でディスプレイの解像度を変更すると DX12 プレイヤーの明るさが変わる
    ([uum-134064](https://issuetracker.unity3d.com/issues/dx12-player-brightness-changes-when-changing-display-resolution-with-screen-dot-setresolution))

- `6000.5.0a5,6000.3.6f1,6000.4.0b6`: [LinuxEditor] エディタ外でファイルを編集しているときに、スクリプトの変更を再インポートしてコンパイルする際に自動更新に失敗する
    ([uum-133944](https://issuetracker.unity3d.com/issues/linux-auto-refresh-fails-to-reimport-and-compile-script-changes-when-editing-files-outside-the-editor))

- `メタル`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `プラットフォームオーディオ`: [Windows] エディターで様々なアクションを実行するとAudioManager::InitFMODでクラッシュする
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))

- テキスト (TextMeshPro)：TMPro Font Asset CreatorでマルチスレッドのFont Atlasを生成すると、UNITY_FT_Load_Glyphでクラッシュする
    ([uum-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

リモートドライブパス（OneDrive、Dropboxなど）の下にあるプロジェクトでUnityのさまざまな操作を実行すると、mdb_txn_renew0でクラッシュする
    ([uum-134234](https://issuetracker.unity3d.com/issues/crash-on-mdb-txn-renew0-when-performing-various-unity-operations-in-a-project-thats-located-under-a-remote-drive-path-onedrive-dropbox-etc))

空白のURPプロジェクトでプレイモードに入ったり出たりするときにエディタのメモリリークが発生する
    ([uum-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))

DirectX 12の排他的フルスクリーンモードでフォーカスを切り替えるとプレイヤーがクラッシュする問題
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))



# 6000.3.9f1 リリースノート

# # 変更点

- `エディター`: targetVelocity が設定された Prismatic Articulation Joint タイプを変更し、Target Velocity を正の値に設定すると、シミュレーション中に正の直線速度になるようにしました。同様に、Target Velocity を負の値に設定すると、直線速度は負になります。
    ([uum-113920](https://issuetracker.unity3d.com/issues/prismatic-articulationbody-moves-in-opposite-direction-when-using-targetvelocity))



# # 修正

- `2D`: タイルパレットの警告アイコンの画像を高解像度のものに変更。
    ([uum-129885](https://issuetracker.unity3d.com/issues/help-box-icon-in-tile-palette-window-is-blurry-in-both-unity-themes))

- `2D`: 長いパレット名やブラシ名がタイルパレットの他のUI要素を隠してしまう問題を修正。
    ([uum-130336](https://issuetracker.unity3d.com/issues/long-tile-palette-name-breaks-window-ui))

- `2D`: 異なる長さの名前を持つ他のパレットやブラシに切り替えると、パレットやブラシのドロップダウンのサイズが変わる問題を修正。
    ([uum-132618](https://issuetracker.unity3d.com/issues/tile-palette-dropdown-expands-when-palette-name-is-longer-in-tile-palette-window))

- `2D`: そのスウィズルがXY/YX以外の値に設定されている間にズームインまたはズームアウトされた場合に、タイル・パレットが前方軸に移動する問題を修正しました。
    (UUM-133308)

- `2D`: タイルパレットウィンドウが最初に表示されたときに、分割ビューのラインがボトムビューと整列していない問題を修正しました。
    ([UUM-129883](https://issuetracker.unity3d.com/issues/drop-down-component-is-overlapped-with-the-default-tile-palette-layout-line))

- `2D`: スプライトエディターウィンドウの情報ボックスがモジュールのUIに邪魔されるのを修正。
    ([uum-131899](https://issuetracker.unity3d.com/issues/inactive-skinning-editor-toolbar-overlaps-the-help-box-in-the-sprite-editor-when-asset-is-not-editable))

- `2D`: ターゲット、パレット、ブラシのドロップダウンで、長いターゲット名、パレット名、ブラシ名を切り捨て。
    ([uum-132825](https://issuetracker.unity3d.com/issues/tile-palette-dropdown-menu-doesnt-truncate-longer-tilemap-names-in-tile-palette-window))

- `2D`: TilemapによるUIで使用されるテキストをSceneViewからScene Viewに更新。
    ([uum-130251](https://issuetracker.unity3d.com/issues/tile-palette-sceneroot-and-sceneview-are-not-rendered-with-correct-ui-spacing))

- `Android`: Linux/Macで表示される警告のgdbパスを修正。
    (UUM-133333)

- `Android`: Android ライブラリドキュメントの余分なスペースを削除。
    (UUM-133945)

- `アセットバンドル`: AssetBundleUnloadOperation` のアロケーションが予想以上に長く持続し、次の `GC.collect()` までクリアされない問題を修正しました。
    (UUM-132703)

- `DX12`: レンダーパスの内部で非同期のコンピュートフェンス待ちを許可することで修正されました。
    ([UUM-105302](https://issuetracker.unity3d.com/issues/dx12-crash-on-d3d12rendersubpassinfo-begin-when-changing-property-value-on-custom-render-pass-feature))

- `DX12`: スクラッチメモリ割り当てに関連するクラッシュを修正。
    ([uum-131707](https://issuetracker.unity3d.com/issues/crash-with-multiple-stack-traces-when-using-dx12-and-selecting-all-spline-knots))

- `DX12`: スクラッチメモリ割り当てに関するクラッシュを修正。
    ([uum-131824](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-moving-in-the-scene-view-on-a-specific-scene))

- `DX12`: D3D12使用時にエディターでmaxQueuedFramesが1の時のデッドロックを修正。
    ([uum-131962](https://issuetracker.unity3d.com/issues/editor-freezes-when-qualitysettings-dot-maxqueuedframes-is-set-to-1-and-dx12-is-used))

- `エディター`: 保存されたエディターレイアウトに戻ると、ドッキングされたマルチプレイヤーモードウィンドウが消える。
    ([uum-133602](https://issuetracker.unity3d.com/issues/docked-multiplayer-play-mode-window-disappears-when-switching-back-to-a-saved-editor-layout))

- `エディター`: アドバンスド・テキスト・ジェネレーターで、省略記号グリフがプライマリー・フォントにない場合にクラッシュする問題を修正しました。
    ([uum-133551](https://issuetracker.unity3d.com/issues/crash-on-textlayoutservice-computeglyphoverflow-when-opening-a-specific-uxml))

- `エディター`: NULLテキスト生成情報の例外を修正しました。
    ([uum-133791](https://issuetracker.unity3d.com/issues/textgenerationinfo-pointer-is-null-errors-are-logged-when-hovering-over-inspected-element-in-the-ui-debugger))

- `エディター`: ドメイン再読み込み時にファイルが削除された場合、エディター環境設定タブが開いていると発生するエラーを修正。
    ([uum-133958](https://issuetracker.unity3d.com/issues/nullreferenceexception-error-is-thrown-during-addressables-cleanup-when-the-project-settings-window-is-open))

- `エディター`: プロジェクト内の水のサンプルでプレーヤーをビルドするとエラーが発生する問題を修正しました。
    (UUM-133713)

- `Editor`: (UUM-133713): EditorUtility.CompressTexture / EditorUtility.CompressCubemapTexture が符号付き EAC フォーマットへの圧縮を途中で中断し、テクスチャが壊れた状態になる問題を修正しました。符号付きEACフォーマットは圧縮のためにサポートされていないことに注意してください。

- `エディター`: Windowsでモーダルダイアログボックスが表示されたときにエディターが反応しなくなる問題を修正しました。
    ([uum-132303](https://issuetracker.unity3d.com/issues/the-editor-freezes-and-leaks-memory-when-cancelling-the-switch-of-the-default-render-pipeline-while-using-the-advanced-object-selector))

- `エディター`: iOSのビルドダイアログで「置換」ボタンと「キャンセル」ボタンの位置が入れ替わっていた問題を修正しました。
    ([uum-133660](https://issuetracker.unity3d.com/issues/clean-build-replace-button-does-nothing-when-pressed-and-building-a-project-for-the-ios-platform))

- `エディター`: EditorUtility.CompressTexture/EditorUtility.CompressCubemapTextureで、NPOTミップマップされたテクスチャをサポートされていないターゲットフォーマットに圧縮しようとする可能性がある問題を修正しました。この件に関する追加の詳細が API ドキュメントに追加されました。
    ([uum-129605](https://issuetracker.unity3d.com/issues/corrupted-mipmaps-are-generated-when-using-editorutility-dot-compresstexture-with-npot-textures))

- `エディター`: adp profile name foldoutのラベルテキストをクリックしても展開されない問題を修正。
    ([uum-133311](https://issuetracker.unity3d.com/issues/adaptive-performance-scaler-profile-foldouts-dont-open-when-clicked-on-the-foldout-title))

- `エディター`: searchpropositionsの置換マッチの方法を修正。
    ([uum-132679](https://issuetracker.unity3d.com/issues/vfx-graph-template-windows-search-filter-returns-no-results-for-any-category-when-a-template-category-contains-special-characters))

- `Editor`: 外部ツールの署名チーム ID と iOS/tvOS プロファイル ID の間の ID 値の不一致を修正した。
    ([uum-132053](https://issuetracker.unity3d.com/issues/inconsistent-id-values-between-signing-team-id-and-ios-slash-tvos-profile-id-in-external-tools))

- `エディター`: ATGを使用した段落選択に関する問題を修正しました。
    ([uum-133353](https://issuetracker.unity3d.com/issues/text-selection-slash-highlighting-is-not-rendered-properly-when-selecting-slash-highlighting-package-description-that-has-multiple-lines-in-the-package-manager-window))

- `エディター`: ダイアログボックスに長すぎるメッセージが含まれている場合に、コンソールに表示されるエラーメッセージを修正しました。このメッセージはエディターのログで見ることができます。
    (UUM-121610)

- `エディター`: WinEditorのSplashScreenイメージが、異なるDPIスケールのディスプレイ間でドラッグされた場合に破損するのを修正しました。
    ([UUM-124825](https://issuetracker.unity3d.com/issues/windows-the-launch-screen-does-not-redraw-correctly-when-moved-to-a-display-of-a-different-scale))

- `エディター`: Android用のパブリッシング設定「ビルド」セクションが、グローバルAndroid設定からのみ編集可能になりました。
    ([uum-126778](https://issuetracker.unity3d.com/issues/publishing-settings-are-shared-across-different-custom-build-profiles-when-modifying-build-options))

- `エディター`: ProjectSettings で AssetPipeline の設定を行う際に RefreshSettings を行うようにしました。
    (UUM-129185)

- `エディター`: マルチプレイヤーモードツールがプレイモードシナリオのリストを表示しない。
    ([UUM-133716](https://issuetracker.unity3d.com/issues/the-multiplayer-play-mode-tool-doesnt-see-the-list-of-play-mode-scenarios-when-using-6000-dot-3-x))

- `Graphics`: イミディエイトモードの描画が大量のメモリを消費していたのを修正。
    ([uum-132332](https://issuetracker.unity3d.com/issues/100-percent-crash-rate-when-loading-two-profiler-captures-in-the-profile-analyzer-compare-tool))

- `iOS`: キーボードのUIをリキッドグラスに合うように調整。
    (UUM-133464)

- `パッケージマネージャー`: Unityが空のコンソールタイトルでコマンドプロンプトから起動された場合、Unityパッケージマネージャが起動時にクラッシュするWindowsの問題を修正しました。
    (PAK-8605)

- `物理`: Rigidbody.SweepTestとRigidbody.SweepTestAllで、RigidbodyのColliderコンポーネントが子GameObjectに配置されている場合にコリジョンレイヤーの設定が変更される問題を修正しました。
    ([uum-91192](https://issuetracker.unity3d.com/issues/the-gameobjects-layer-which-contains-the-rigidbody-is-used-for-rigidbody-dot-sweeptest-when-retrieving-a-collider-from-a-child-gameobject-with-a-non-collide-able-layer))

- `物理`: クロス検査ツールのペイントツールで、内部のコリジョンメッシュにレイキャストが発射されないためにブラシが表示されない問題を修正しました。
    ([uum-61756](https://issuetracker.unity3d.com/issues/paintable-area-is-offset-from-the-mesh-when-editing-cloth-constraints))

- `物理 2D`: 複数のカメラに対するデバッグレンダリングの問題を修正し、カスタム描画要素の正確な寿命を確保し、早期のクリアを止めました。さらに、カスタム描画要素は常に自動シーン描画の後に描画されるようになりました。
    (UUM-133990)

- `物理 2D`: デバッグ SDF シェーダのプロパティ "drawThickness" と "drawPointScale" の問題を修正しました。PhysicsWorldDefinition "をデフォルトにリセットするか、"drawThickness "のデフォルトである1と "drawPointScale "のデフォルトである0.5を使用することをお勧めします。  これを行わないと、アウトラインのレンダリングが以前よりもわずかに太くなっていることに気づくでしょう。
    (UUM-133990)

- `物理 2D`: PhysicsRotate」プロパティのドロワーで、インスペクタに「Angle（角度）」と「Direction（方向）」の両方が表示される問題を修正しました。これは混乱しやすいので、「Rotation（回転）」という単一のフィールドに簡素化されました。
    (UUM-133990)

- `Profiler`: キャプチャリストのツールチップ、およびミニハイライトバーに表示される「フレームオーバーターゲット」のパーセンテージが、メインウィンドウのハイライト表示と同期しなくなることがある問題を修正しました。
    ([uum-120289](https://issuetracker.unity3d.com/issues/profiler-saving-whilst-profiling-is-recording-can-result-in-highlights-data-not-matching))

- `Profiler`: Win32プラットフォーム上でメタデータを含むサンプルを追加する際に、Profilerがバッファオーバーランしてクラッシュする可能性を修正しました。
    (UUM-129792)

- `Profiler`: プロファイラがデータ処理中にメモリ不足になった場合に Out-Of-Memory 致命的なエラーを発生させるようにしました。
    ([UUM-130676](https://issuetracker.unity3d.com/issues/profiler-crash-on-dynamicheapallocator-getblockpointer))

- `プロジェクトブラウザ`: 不変アセットを削除しようとすると、コンソールに重複した警告が投げられる問題を修正しました。
    ([uum-121159](https://issuetracker.unity3d.com/issues/two-warnings-appear-for-every-soft-delete-operation-when-deleting-sub-assets-in-the-project-browser))

- `テキスト`: nobr タグの ATG サポートを追加。
    (UUM-133007)

- `UIツールキット`: フィルターが DPI を考慮していなかったのを修正。
    ([UUM-122745](https://issuetracker.unity3d.com/issues/filters-do-not-take-dpi-into-account))

- `UIツールキット`: バインディングが変更され、要素が階層内で移動された場合に、不正なバインディングが使用されるのを修正。
    ([uum-133584](https://issuetracker.unity3d.com/issues/script-enum-fields-show-none-when-expanding-nested-inspector-elements))

- `UIツールキット`: Vulkan defineの再定義エラーを解決しました。
    ([uum-132686](https://issuetracker.unity3d.com/issues/ui-shader-graph-throws-unitydisplayorientationpretransform-error-when-android-is-the-selected-platform))

- `UIツールキット`: UI Toolkit：極端なアスペクト比の図形でPainter2D Fillがレンダリングされないのを修正した。

- `URP`: \URP Graphics設定に地形シェーダーを含める設定を追加しました。チェックを外すと、地形詳細シェーダがビルドに追加されなくなります。
    ([uum-109540](https://issuetracker.unity3d.com/issues/urp-terrain-shaders-are-always-included-when-building-on-any-target-platform))

- `VFX Graph`: カーブやグラデーションの分岐が、リベイクやGPUへのアップロードに失敗する問題を修正。
    (UUM-129743)

- `WebGL`: WebGPU: シェーダーにバインドされたテクスチャーを読み込みと書き込みの両方で自動的に処理。
    ([UUM-131864](https://issuetracker.unity3d.com/issues/webgpu-cant-bind-compute-rwtexture-for-read-and-write))

- `WebGL`: WebGPU: シェーダーで RWTexture2D テクスチャを使用するパイプラインエラーを修正し、unorm RWTextures の使用を簡素化しました。
    ([uum-131863](https://issuetracker.unity3d.com/issues/webgpu-errors-with-unorm-and-half4-rwtexture))




# # 6000.3.9f1 におけるパッケージの変更

# # 更新されたパッケージ

- `com.unity.burst`: [1.8.27](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) から [1.8.28](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) へ。

- `com.unity.mobile.notifications`: [2.4.2](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html) から [2.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html) に変更。

- `com.unity.ui.test-framework`: [1.0.0](https://docs.unity3d.com/Packages/com.unity.ui.test-framework@1.0//changelog/CHANGELOG.html)から[6.3.0](https://docs.unity3d.com/Packages/com.unity.ui.test-framework@6.3//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: [1.1.9](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) から [1.1.11](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: [2.8.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.8//changelog/CHANGELOG.html) から [2.9.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.9//changelog/CHANGELOG.html)

- `com.unity.multiplayer.tools`: [2.2.7](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)から[2.2.8](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html)

- `com.unity.services.multiplayer`: [2.0.0](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.0//changelog/CHANGELOG.html)から[2.1.1](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.1//changelog/CHANGELOG.html)