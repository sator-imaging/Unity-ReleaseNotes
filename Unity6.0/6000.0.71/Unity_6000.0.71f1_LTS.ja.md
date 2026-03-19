# Unity 6000.0.71f1 LTS
公開日時: Wed, 18 Mar 2026 07:40:01 GMT
https://unity.com/releases/editor/whats-new/6000.0.71f1

# 6000.0.71f1 の既知の問題点

- `IL2CPP`: [iOS] [Android] IL2CPPのビルド中に外部ライブラリのジェネリックに失敗する
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- `メタル`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

DirectX 12の排他的フルスクリーンモードでフォーカスを切り替えるとプレイヤーがクラッシュする
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))



# 6000.0.71f1 リリースノート

## 修正

- `2D`: タイルパレットを作成する際に、セルサイズプロパティが負の値を受け付ける問題を修正しました。エディターは負の値を0に設定するようになりました。
    ([uum-130884](https://issuetracker.unity3d.com/issues/tile-palette-allows-negative-manual-cell-size-values-causing-asset-corruption-and-assertion-failed-on-expression-errors))

- `2D`: ライトバッチングデバッガーで名前がオーバーフローしないように修正。
    ([uum-132565](https://issuetracker.unity3d.com/issues/long-light-gameobject-names-are-overflowing-the-light-batching-debugger-text-fields))

- `2D`: Light Batching Debugger で名前がリフレッシュされないのを修正。
    ([uum-132573](https://issuetracker.unity3d.com/issues/light-batching-debugger-doesnt-update-light-gameobjects-name-unless-the-window-is-restarted))

- `2D`: TilemapによるUIで使用されるテキストをSceneViewからScene Viewに更新。
    ([uum-130251](https://issuetracker.unity3d.com/issues/tile-palette-sceneroot-and-sceneview-are-not-rendered-with-correct-ui-spacing))

- `DX12`: 検証エラーでカバーされていなかったDirect3D Graphics Infrastructure ｟DXGI｠エラーをユーザーログに追加しました。CheckDeviceStatus(￤)でエラーでないリターンコード￤(例: 087a0001￤)の誤報告を修正しました。
    (UUM-135201)

- `DX12`: ウィンドウのフォーカスを切り替えた後にプレイヤーがハングするのを修正しました。
    ([UUM-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))

- `エディター`: Animator ウィンドウのテキストを読みやすくするため、常に Signed Distance Field ↪SDF78↩ を使用するように変更。
    ([uum-134486](https://issuetracker.unity3d.com/issues/animator-state-labels-are-not-rendered-correctly-when-using-the-bitmap-renderer-as-the-default-editor-text-renderer))

- `エディター`: エディターがプレハブインスタンスから `SerializeReference` に関連する未使用のオーバーライドを正しくクリアするようになりました。
    ([uum-135932](https://issuetracker.unity3d.com/issues/prefabs-remove-unused-overrides-fails-to-clean-up-overrides-when-the-managed-instance-type-in-serializereference-is-changed))

- `エディター`: 特定のケースで発生する4フレームのメモリ確保警告を修正。
    ([uum-86868](https://issuetracker.unity3d.com/issues/a-memory-leak-occurs-when-selecting-the-console-window-and-the-inspector-window-covers-the-game-view-window-when-specific-ui-elements-are-displayed-in-it))

- `Editor`: IsRunningXRMobile' が現在のコンテキストに存在しない問題を修正。
    ([uum-135971](https://issuetracker.unity3d.com/issues/urp-broken-android-project-after-lazy-initialization-for-platformautodetect))

- `Editor`: USSスタイルの検証で、タブが空白であることを認識していなかった問題を修正した。
    ([uum-135915](https://issuetracker.unity3d.com/issues/warning-expected-end-of-value-but-found-is-shown-when-inserting-a-blank-line-between-opacity-and-scale-in-a-uss-file))

- `エディター`: Windows、Mac、Linux*で*Overrideを切り替えた後、Player Settingsのアイコンのサイズと保持が保持されない問題を修正。
    ([uum-131965](https://issuetracker.unity3d.com/issues/icon-override-texture2d-fields-in-the-player-settings-window-are-not-square-and-do-not-retain-data-after-disabling))

- `エディター`: プロジェクト設定ウィンドウで検索フィルターを削除すると、そのセクションのテキストが完全にハイライトされてしまう問題を修正しました。
    ([uum-134769](https://issuetracker.unity3d.com/issues/all-text-in-the-project-settings-window-is-still-tinted-white-after-deleting-text-in-the-search-window))

- `エディター`: Linux エディターで、同じ名前のファイルを上書きするプロンプトが表示されない問題を修正しました。
    ([uum-134937](https://issuetracker.unity3d.com/issues/linux-no-file-already-exists-pop-up-thrown-when-saving-shader-variants-with-an-already-existing-name-from-build-profiles-or-project-settings-window))

- `エディター`: TextCoreの日中韓改行を修正。
    ([uum-135887](https://issuetracker.unity3d.com/issues/cjk-text-goes-outside-of-the-bounds-of-a-label-in-ui-builder-when-wrapping-is-enabled))

- `Editor`: モジュール詳細パネルのコントローラースクリプトの例を修正した。

- `編集`: Hub ドキュメントへのリンクを修復。

- `エンジン診断`: Diagnostics ネイティブクラッシュレポートの誤ったタイムスタンプを修正。
    (UUM-135436)

- `GI`: APVツールチップの小さなタイプミスを修正：Steaming &gt; Streaming。
    ([UUM-134159](https://issuetracker.unity3d.com/issues/streaming-is-misspelled-as-steaming-in-enable-gpu-streaming-and-enable-disk-streaming-tooltpis))

- `Graphics`: Vulkan バックエンドのバッファプールにおけるデータ競合を修正しました。
    (UUM-134547)

- `Graphics`: (UUM-134547) `Graphics`: builtinRP blit copyがfloat4カラーを出力するようにした(fxed4はメタル上では half4に変換されるため、u16やf32データではデータが切り詰められる)。
    ([uum-128591](https://issuetracker.unity3d.com/issues/terrain-heightmap-loses-precision-on-android-and-ios-when-the-heightmap-texture-is-blitted-to-a-rendertexture-using-the-default-blit-shader))

- `Graphics`: \バッチモードでデカールを有効にしてモバイルプラットフォーム用にビルドする と、マテリアルが黒くなる問題を修正しました。
    ([uum-134298](https://issuetracker.unity3d.com/issues/urp-all-materials-render-black-when-building-via-batchmode-or-without-rendering-scene-slash-game-view-in-editor-if-decal-renderer-technique-is-set-to-automatic))

- `Input`: スプラッシュスクリーンが無効でInput Managerのみを使用するプロジェクトで、スタンドアロンプレイヤーウィンドウのサイズを変更する際にリサイズカーソルが表示されない問題を修正しました。
    ([uum-134058](https://issuetracker.unity3d.com/issues/double-sided-arrow-mouse-cursor-does-not-appear-when-resizing-the-player-and-input-backend-is-set-to-input-manager-old))

- `Input`: IOHIDDevice_GetUsage の無効なロングバッファポインタを修正しました。
    ([uum-135043](https://issuetracker.unity3d.com/issues/silicon-crash-on-os-unfair-recursive-lock-lock-with-options-when-opening-a-project-while-the-razer-synapse-app-is-open))

- `インストーラー`: MacOSプラットフォームサポートインストーラーは、異なるバージョンの他のUnity Editorインストールから同じプラットフォームのサポートを削除しなくなりました。
    (UUM-133396)

- `iOS`: アプリが既に実行されている状態でカスタムURLスキームまたはユニバーサルリンク経由でアプリが開かれた場合、またはコールドスタートからディープリンク経由でアプリが起動された一部のケースで、Application.deepLinkActivatedが呼び出されない問題を修正しました。
    ([uum-135497](https://issuetracker.unity3d.com/issues/ios-application-dot-deeplinkactivated-does-not-get-invoked-while-app-is-running-when-uiapplicationscenemanifest-is-added-in-info-dot-plist))

- `iOS`: キーボードレイアウトが変更された場合のみ報告することでパフォーマンスを改善しました。
    ([uum-134845](https://issuetracker.unity3d.com/issues/ios-high-cpu-load-when-device-keyboard-is-open))

- `物理`: 物理のジョイント・コンポーネント・ギズモで、ジョイントがワールド空間の固定点に接続されている場合に、自動設定された接続アンカーがジョイントに追従してしまう問題を修正。
    ([uum-134423](https://issuetracker.unity3d.com/issues/spring-joint-shows-only-one-anchor-gizmo-in-scene-view-when-auto-configure-connected-anchor-is-enabled))

- `物理`: MeshCollider`で`Use Fast Midphase`クッキングオプションを使用してレイキャスティングを行う際に、スタックオーバーフローを防止しました。
    ([uum-110564](https://issuetracker.unity3d.com/issues/silent-crash-when-raycasting-on-a-specific-dense-mesh))

- `Shadergraph`: HDRとマークされたテクスチャ・プロパティに対するテクスチャ・サンプリング操作を修正。
    ([uum-122106](https://issuetracker.unity3d.com/issues/hdr-images-are-compressed-incorrectly-with-default-settings-on-android-platform))

- `テキスト`: 標準テキストでビットマップを使用した場合にハイライトが正しくなかったのを修正。
    ([uum-134691](https://issuetracker.unity3d.com/issues/project-settings-search-highlights-are-misaligned-when-using-the-bitmap-text-rendering-mode))

- `uGUI`: キーボードが閉じたらInputFieldsを非アクティブにする。
    ([uum-133712](https://issuetracker.unity3d.com/issues/input-field-does-not-update-when-selecting-the-same-input-field-after-previous-input-was-canceled))

- `uGUI`: フォント再構築のスコープ中にテキストコンポーネントが追加された場合の例外を修正。
    ([uum-128580](https://issuetracker.unity3d.com/issues/invalidoperationexception-thrown-when-text-legacy-font-is-rebuilt-via-inputfield-legacy-onvaluechanged-callback))

- `UIエレメント`: UnityEventのインスペクタのコピー/ペーストを修正し、CustomEditorを持つコンポーネント(Buttonなど)と持たないコンポーネントの間で動作するようにしました。以前は、コピーしたUnityEventをこれらの2種類のコンポーネント間で貼り付けると、互換性のないクリップボードフォーマットのために静かに失敗していました。
    ([uum-134401](https://issuetracker.unity3d.com/issues/unityevent-does-not-get-pasted-to-a-ugui-component-when-trying-to-copy-it-from-a-script))

- `UIツールキット`: EditorUtility.activePlayModeTint を公開し、カスタムメッシュや Painter2D の色がエディタと一貫して見えるようにしました。
    (UUM-114424)

- `UI ツールキット`: オーバーフローまたはコーナー半径を変更した後に不正なクリッピングを引き起こす可能性のあるバグを修正しました。
    ([UUM-135869](https://issuetracker.unity3d.com/issues/invalid-clip-method))

- `UIツールキット`: 変更後にクリッピング状態の更新が不完全になる可能性のある状態を修正。
    (UUM-108710)

- `UIツールキット`: 2Dベクターグラフィックスでストロークパスを描画する際に、特定の鋭角や退化に近いセグメントで例外が発生することがあったのを修正しました。
    (UUM-135440)

- `UIツールキット`: EditorMonitor の RenderTexture のリークを修正。
    (UUM-104256)

- `UIツールキット`: 以前のフレームでオーバーフローが修正された時に、背景画像として VectorImage がステンシルマスクとして正しく使用されていなかったのを修正。
    ([UUM-110567](https://issuetracker.unity3d.com/issues/text-is-not-masked-when-creating-a-vector-image-and-using-a-mask-inside-a-visualelement))

- `バージョン管理`: Unity 6.4以降の非推奨インスタンスID APIを修正。

- `ビデオ`: Vulkan Graphics API を使用した特定のモバイルデバイスで Video を再生できない問題を修正しました。
    ([uum-133914](https://issuetracker.unity3d.com/issues/video-player-renders-no-video-on-specific-devices-when-using-vulkan))

- `WebGL`: WebGPU：一部のシェーダーがコンパイルに失敗する原因となっていたシェーダーコンパイラのエラーを修正しました。
    ([uum-134978](https://issuetracker.unity3d.com/issues/shader-compiler-and-shader-errors-are-thrown-in-the-console-when-building-web-platform-with-webgpu-experimental-enabled-in-auto-graphics-api))

- `XR`: オーディオ設定を変更した際にエディタがクラッシュすることがあったのを修正。
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))




## 6000.0.71f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.cinemachine`: [2.10.4](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html) から [2.10.6](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html) へ。

- `com.unity.collab-proxy`: [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) から [2.11.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) へ。

- `com.unity.performance.profile-analyzer`: [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) から [1.3.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) に変更。

- `com.unity.remote-config`: [4.2.2](https://docs.unity3d.com/Packages/com.unity.remote-config@4.2//changelog/CHANGELOG.html) から [4.2.5](https://docs.unity3d.com/Packages/com.unity.remote-config@4.2//changelog/CHANGELOG.html) に変更。

- `com.unity.services.analytics`: [6.2.1](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) から [6.3.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.3//changelog/CHANGELOG.html)

- `com.unity.visualscripting`: [1.9.7](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)から[1.9.10](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.9.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html) から [1.10.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.10//changelog/CHANGELOG.html)

- `com.unity.cloud.draco`: [5.4.0](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html) から [5.4.3](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html)

- `com.unity.cloud.ktx`: [3.6.1](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html) から [3.6.3](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html)