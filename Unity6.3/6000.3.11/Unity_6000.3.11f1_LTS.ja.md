# Unity 6000.3.11f1 LTS
公開日時: Wed, 11 Mar 2026 14:52:35 GMT
https://unity.com/releases/editor/whats-new/6000.3.11f1

# 6000.3.11f1 の既知の問題

- `6000.2.0a10`: プロジェクトを初めて開いたときに TexturesD3D12::CreateTextureInternal() でクラッシュする。
    ([uum-135024](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-opening-a-project-for-the-first-time))

- `6000.3.5f1`: カービングを有効にしてNavMesh Obstaclesを移動するとCPU使用率が増加する
    ([uum-133911](https://issuetracker.unity3d.com/issues/increased-cpu-usage-when-moving-navmesh-obstacles-with-carving-enabled))

- `6000.5.0a3,6000.4.0b8,6000.3.8f1,6000.0.68f1`: [iOS] Info.plistにUIApplicationSceneManifestが追加されている場合、アプリの実行中にApplication.deepLinkActivatedが呼び出されない
    ([uum-135497](https://issuetracker.unity3d.com/issues/ios-application-dot-deeplinkactivated-does-not-get-invoked-while-app-is-running-when-uiapplicationscenemanifest-is-added-in-info-dot-plist))

- `コアランタイム`: Entities ContentManagement GUIDが不安定で、Playerが異なるディレクトリにビルドされるたびに異なるものになる
    ([uum-129944](https://issuetracker.unity3d.com/issues/entities-contentmanagement-guids-are-unstable-and-become-different-each-time-a-player-is-built-to-a-different-directory))

- `メタル`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

DirectX 12の排他的フルスクリーンモードでフォーカスを切り替えるとプレイヤーがクラッシュする
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))

[Silicon] Razer Synapseアプリを開いているときにプロジェクトを開くとos_unfair_recursive_lock_with_optionsでクラッシュする
    ([uum-135043](https://issuetracker.unity3d.com/issues/silicon-crash-on-os-unfair-recursive-lock-lock-with-options-when-opening-a-project-while-the-razer-synapse-app-is-open))



# 6000.3.11f1 リリースノート

## 機能

- `ライセンス`: Kerberos プロキシ認証のサポート。

- `macOS`: Mac Playerで`CAMetalDisplayLink`のサポートを追加しました。
    デフォルトでは無効になっており、プレーヤーの設定で「Use MetalDisplayLink \(Mac Player only)」を切り替えることで有効にできます。また、環境変数 `UNITY_USE_METAL_DISPLAY_LINK=1` を使用することもできます。
    CAMetalDisplayLink`を使用すると、スタッタリングが減少し、フレームペーシングが改善されます。また、`Time.deltaTime`がより安定します。



## 改善点

- `Android`: AndroidPlayer の初期化処理にプロファイリングマーカーを追加。
    ([uum-135048](https://issuetracker.unity3d.com/issues/android-fix-profiling-during-early-application-startup-to-match-other-platforms))

- `ビルドシステム`: エディタにバンドルされている 7-Zip を 26.00 に更新。

- `インストーラー`: Windowsシステム上で.NET 3.5のアクティベーションを削除。インストーラーを直接使用した場合のインストール時間を大幅に短縮。
    (UUM-133360)

- `物理 2D`: PhysicsComposerがIDisposableインターフェイスを実装し、パブリックIDisposable.Disposeメソッドが単に "PhysicsComposer.Destroy(￤)を呼び出すようになりました。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `プラグイン`: DLSS Super ResolutionにプリセットLとMを追加するなど、DLSS SDKをv310.4.0からv310.5.0にアップグレード。

- `SRP Core`: VolumeManager` が `VolumeComponent` タイプを収集する方法を改善し、Player 起動時の遅い反映オーバーヘッドを回避。
    (UUM-134911)



## API の変更

- `Physics 2D`: 追加: "objectValue "プロパティに使用されるEntityIDを公開するために、"PhysicsUserData.objectValueId "プロパティを追加しました。  このプロパティは、EntityId、Object Name、Typeをツールチップとして表示します。Entityがない場合は "None"、EntityIDが有効なオブジェクトを表していない場合は "Invalid Object Id "と表示されます。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `Physics 2D`: 追加: "PhysicsUserData.objectValueId "プロパティを追加し、"objectValue "プロパティに使用されるEntityIDを公開しました。  このプロパティは、EntityId、Object Name、Typeをツールチップとして表示し、Entityがない場合は "None"、EntityIDが有効なオブジェクトを表していない場合は "Invalid Object Id "を表示します。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `物理 2D`: 追加: PhysicsComposerが、"PhysicsComposer.GetComposers\(˶‾‾) "メソッドと "PhysicsComposer.DestroyAll(˶‾‾) "メソッドを使用して、すべてのコンポーザーを取得または破棄できるようになりました。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `Physics 2D`: 追加: PhysicsComposerが、"PhysicsComposer.GetComposers
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `Physics 2D`: 追加: PhysicsComposerのスタティックメソッド "PhysicsComposer.ToPolygons(˶) "で、"CircleGeometry "と "CapsuleGeometry "の両方を "PolygonGeometry "に変換できるようになりました。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `物理 2D`: 追加: PhysicsComposerのスタティックメソッド "PhysicsComposer.ToPolygons(˶) "で、"CircleGeometry "と "CapsuleGeometry "の両方を "PolygonGeometry "に変換できるようになりました。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `物理2D`: PhysicsWorld、PhysicsBody、PhysicsShape、PhysicsJointで、所有者専用のPhysicsUserDataを "SetOwnerUserData(˶) "で設定し、".ownerUserData "で取得できるようになりました。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `物理2D`: 追加: PhysicsWorld、PhysicsBody、PhysicsShape、PhysicsJointで、所有者専用のPhysicsUserDataを "SetOwnerUserData(˶‾‾) "で設定し、".ownerUserData "で取得できるようになりました。
    ([uum-134952](https://issuetracker.unity3d.com/issues/fix-for-6000-dot-6-x-fix-some-api-issues-from-user-feedback))

- `SRP Core`: 追加: 構造体TextureHandleに新しい演算子==と!=を追加。



## 変更点

- `Shadergraph`: コード生成中のプロファイリングを無効にした。
    ([uum-117133](https://issuetracker.unity3d.com/issues/switching-platform-while-profiling-in-edit-mode-throws-non-matching-profiler-dot-endsample-warnings))

- `uGUI`: UI Canvas モジュールのプロファイラーアイコンを更新。
    (UUM-135623)



## 修正

- `2D`: Light Batching Debugger で名前がオーバーフローしないように修正。
    ([uum-132565](https://issuetracker.unity3d.com/issues/long-light-gameobject-names-are-overflowing-the-light-batching-debugger-text-fields))

- `2D`: Light Batching Debugger で名前がリフレッシュされないのを修正。
    ([uum-132573](https://issuetracker.unity3d.com/issues/light-batching-debugger-doesnt-update-light-gameobjects-name-unless-the-window-is-restarted))

- `適応パフォーマンス`: アダプティブ・パフォーマンス・プロファイラのデータが表示されないのを修正。
    (UUM-134873)

- `Android`: バッチモード: Android サポートがインストールされている場合、エディター起動時の Android デバイスの自動スキャンを削除。
    ([UUM-133593](https://issuetracker.unity3d.com/issues/batchmode-the-editor-executes-code-that-is-not-relevant-to-the-target-build-platform-when-a-buildtarget-is-defined-in-batchmode))

- `Android`: UI Toolkitの入力フィールドのキャレット位置が、AndroidでTouchScreenKeyboardがテキスト選択を変更したときに更新されない問題を修正しました。
    ([uum-128088](https://issuetracker.unity3d.com/issues/android-soft-keyboards-arrows-and-select-tools-do-not-have-visual-feedback-when-hide-mobile-input-is-enabled))

- `Android`: Android `GameActivity` を使用しているときに `OnApplicationQuit` が一貫して呼び出されない問題を修正しました。
    (UUM-131090)

- `Android`: 古い入力システムを使用している場合に、マウスを動かさずに負の方向にスクロールすると Android のマウススクロールホイールが機能しない問題を修正しました。
    ([UUM-134074](https://issuetracker.unity3d.com/issues/android-the-y-value-of-input-dot-mousescrolldelta-is-positive-when-scrolling-in-both-directions-in-the-player))

- `Android`: デバイスシミュレータのデバイス定義を更新し、古いデバイスの特定のモデル名ではなく、一般的な特性ベースの名前を使用するようにしました。
    (UUM-134051)

- `オーディオ`: スタンドアロンのプレーヤーを終了する際に、スクリプト可能なジェネレーターに関連するクラッシュを修正しました。
    ([UUM-133608](https://issuetracker.unity3d.com/issues/scriptable-generator-crashes-player-on-exit))

- `ビルド・パイプライン`: パッケージに保存されたシーンをビルドしようとすると、ビルドに失敗する問題を修正しました。
    ([uum-133786](https://issuetracker.unity3d.com/issues/player-build-fails-with-failed-to-open-error-when-scene-is-located-in-a-package))

- `ビルド・パイプライン`: ビルドレポートのビルド時間計算が壊れていたのを修正。
    ([uum-126318](https://issuetracker.unity3d.com/issues/project-auditor-build-time-calculation-can-get-broken))

- `DX12`: 検証エラーでカバーされなかったDirect3D Graphics Infrastructureのエラーをユーザーログに追加した。CheckDeviceStatus(￤)で、エラーでないリターンコード￤（例：087a0001￤）の誤報告を修正しました。
    (UUM-135201)

- `DX12`: ウィンドウのフォーカスを切り替えた後にプレイヤーがハングするのを修正しました。
    ([UUM-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))

- `DX12`: DXC シェーダー・コンパイラーを使用した時のクラスター化したライティングの問題を修正。
    (UUM-134785)

- `DX12`: テクスチャの読み込みが遅くなる問題を修正。
    (UUM-133332)

- `DX12`: 最終アップスケールパスの間、プロキシバッファの srv フォーマットを swapchain rtv のフォーマットと一致。
    ([UUM-134064](https://issuetracker.unity3d.com/issues/dx12-player-brightness-changes-when-changing-display-resolution-with-screen-dot-setresolution))

- `Editor`: UITKにhideSoftkeyboardオプションを追加し、物理キーボードとタッチスクリーンキーボードを同時にアクティブにするオプションを追加。
    (UUM-122340)

- `エディター`: Advanced Text Generator で、合成太字とイタリック体の角度をカスタマイズできるように。
    (UUM-114774)

- エディター`(`Editor`)メッシュLODジェネレーターを変更し、選択カーブが負の場合にLODを出力しないようにしました。
    ([UUM-121461](https://issuetracker.unity3d.com/issues/meshlod-selection-is-inverted-when-importing-a-model-with-unknown-settings))

- `エディター`: プレイモードでレンダー・パイプライン・コンバーター(Render Pipeline Converter)ウィンドウを開こうとすると、関係のないウィンドウが開いてしまうバグを修正しました。
    ([uum-132083](https://issuetracker.unity3d.com/issues/the-sprite-importer-window-is-opened-instead-of-the-render-pipeline-converter-window-when-opening-it-in-play-mode))

- `エディター`: D3D12 Device Filter Lists アセットのヘルプドキュメントのリンクが抜けていたのを修正しました。
    ([uum-123217](https://issuetracker.unity3d.com/issues/d3d12-device-filter-lists-asset-link-to-the-documentation-isnt-working))

- `Editor`: IsRunningXRMobile' が現在のコンテキストに存在しない問題を修正しました。
    ([uum-135971](https://issuetracker.unity3d.com/issues/urp-broken-android-project-after-lazy-initialization-for-platformautodetect))

- `エディター`: Mac Editorのダイアログボックスが特定のキーボード操作に反応しない問題を修正しました。
    ([uum-134031](https://issuetracker.unity3d.com/issues/characters-cannot-be-deleted-when-pressing-delete-button-in-project-build-save-as-pop-up))

- `エディター`: スクリプトのコンパイルが Windows と Linux で異なる結果となり、複数のプラットフォームで作業しているチームにとって不必要なアセットファイルの変更を引き起こしていた問題を修正しました。
    (UUM-133554)

- `Editor`: ATG 使用時の AutoSize 警告ロギングを修正。
    ([UUM-134814](https://issuetracker.unity3d.com/issues/textautosize-is-not-supported-with-the-standard-textgenerator-warning-is-shown-when-enabling-auto-size-in-ui-builder-while-enable-editor-extension-authoring-by-default-is-enabled))

- `Editor`: アーティファクトの前処理の途中でキャンセルした場合、多すぎるアーティファクトをマージするとLMDBがクラッシュするバグを修正。
    ([uum-133590](https://issuetracker.unity3d.com/issues/crash-on-readwritelock-writelock-when-performing-various-unity-operations))

- `エディター`: 物理キーボードの言語切り替えが正しく動作しない問題を修正。
    ([uum-130105](https://issuetracker.unity3d.com/issues/android-legacy-tmp-and-ui-toolkit-input-field-language-toggle-to-some-non-latin-alphabet-languages-does-not-work-with-external-keyboard))

- `エディター`: スケーラーUIの変更がローカルアセットを正しく更新しない問題を修正。
    (UUM-135019)

- `エディター`: スプライトアセットが ATG で正しく表示されないのを修正。
    ([UUM-134941](https://issuetracker.unity3d.com/issues/icons-are-not-displayed-when-font-is-applied-via-style-sheets))

- `エディター`: IMGUIデバッガーのスタイルピッカーUIがマウスドラッグ中にビューをハイライトするように修正。
    ([uum-133941](https://issuetracker.unity3d.com/issues/pick-style-only-responds-to-elements-on-the-first-hovered-window-when-using-the-imgui-debugger))

- `エディター`: リペイントのドットのサイズを修正し、スケーリングファクターで正しくスケールするように。
    (UUM-135511)

- `エディター`: ハブのドキュメントへのリンクを修復。

- `GI`: APVスカイオクルージョンがVulkanでベイクする際に若干明るすぎるのを修正。
    (UUM-101700)

- `Graphics`: カメラプレビュー - パイプラインを変更した際に、レンダーターゲットテクスチャが再作成されず、レンダーテクスチャオプションが無効になっていました。
    ([UUM-133293](https://issuetracker.unity3d.com/issues/after-converting-a-built-in-project-to-urp-render-texture-setting-error-message-is-spammed))

- `Graphics`: メタル(Metal)使用時にステンシルのアタッチメントが正しく設定されず、メタル(Metal)の検証エラーが発生する問題を修正しました。
    (UUM-133783)

- `Graphics`: Vulkan バックエンドのバッファプールにおけるデータ競合を修正しました。
    (UUM-134547)

- `Graphics`: WebGPU で複数のレンダーターゲットをクリアする際の問題を修正しました。
    ([UUM-133743](https://issuetracker.unity3d.com/issues/webgpu-urp-rendergraph-renderpass-doesnt-clear-textures))

- `Graphics`: シェーダーのコンパイルエラー 'tex3D' の呼び出しがあいまい" を修正。
    ([uum-133088](https://issuetracker.unity3d.com/issues/error-shader-error-in-yscloudcover-call-to-tex3d-is-ambiguous-at-assets-slash-yscloudcovertext-dot-shader-606-on-d3d11-is-present-when-compiling-tex3d-shader-with-dxc))

- `Graphics`: \バッチモードでデカールを有効にしてモバイルプラットフォーム用にビルドすると、マテリアルが黒くなる問題を修正しました。
    ([uum-134298](https://issuetracker.unity3d.com/issues/urp-all-materials-render-black-when-building-via-batchmode-or-without-rendering-scene-slash-game-view-in-editor-if-decal-renderer-technique-is-set-to-automatic))

- `HDRP`: デカールプロジェクターとローカルボリューメトリックフォグにアイコンギズモがありません。水のデカールコンポーネントはライトテーマで暗いアイコンが欠落していました。
    ([uum-132819](https://issuetracker.unity3d.com/issues/hdrp-decal-projector-and-local-volumetric-fog-are-missing-their-icon-gizmos-hdrp-decal-projector-and-local-volumetric-fog-are-missing-their-icon-gizmos))

- `IL2CPP`: ラムダ式の無効なMethodsToPreserveエントリを修正。
    ([uum-124814](https://issuetracker.unity3d.com/issues/unity-cil-linker-fails-on-player-build-when-persistent-listeners-have-and-in-their-xml-attribute-names))

- `入力`: スプラッシュスクリーンが無効で Input Manager だけを使用するプロジェクトで、スタンドアロンプレイヤーウィンドウのサイズ変更時にリサイズカーソルが表示されない問題を修正しました。
    ([uum-134058](https://issuetracker.unity3d.com/issues/double-sided-arrow-mouse-cursor-does-not-appear-when-resizing-the-player-and-input-backend-is-set-to-input-manager-old))

- `入力システム`: 入力デバイスがメインスレッド以外のスレッドで検出されるプラットフォームで、Unityのクラッシュや未定義の動作につながる可能性のある同期プリミティブの不正な使用を修正しました。
    (UUM-134537)

- `インストーラー`: MacOS プラットフォームサポートインストーラーは、異なるバージョンの他の Unity エディターインストールから同じプラットフォームのサポートを削除しなくなりました。
    (UUM-133396)

- `ライセンス`: シンボリックリンクされた ULF への書き込みが禁止されました。
    (UUM-121827)

- `macOS`: 新しい `CAMetalDisplayLink` を使用する際、Mac Player でスタッタリングが発生する問題を修正しました。この問題は、プレイヤーの設定で "Use MetalDisplayLink \(Mac Player only)" を切り替えることで有効にできます。
    ([uum-112011](https://issuetracker.unity3d.com/issues/built-project-stutters-intermittently-when-vsync-is-enabled))

- `パッケージマネージャー`: すべてのエラーの場所を「適用」ボタンの下ではなく、各フィールドの下に変更。
    ([uum-112552](https://issuetracker.unity3d.com/issues/validation-messages-in-inspector-window-are-displayed-too-low-during-package-editing-process))

- `パッケージマネージャー`: 依存関係のバージョンがNULL値を持たないように検証を修正。
    ([uum-113308](https://issuetracker.unity3d.com/issues/editing-package-manifest-allows-adding-a-dependency-with-a-null-version))

- `パッケージマネージャー`: 技術的な名前がプロジェクト内の既存の名前と一致しないようにバリデーションを修正。
    ([uum-113396](https://issuetracker.unity3d.com/issues/while-editing-package-manifest-via-inspector-the-package-name-can-be-set-to-an-already-existing-packages-name))

- `パッケージマネージャー`: .unitypackage をインポートすると、内容が2倍抽出されます。
    (PAK-8613)

- `パッケージマネージャ`: パッケージマネージャ：インスペクタウィンドウの Package.json の変更 UI の問題を修正。
    (UUM-133647)

- `パッケージマネージャ`: パッケージマネージャ：upm パッケージを使用した URL のディープリンクで、発見可能な場合に選択されたパッケージを表示。また、バージョンが指定されている場合、またはパッケージが検出可能でない場合、Add ポップアップを表示します。
    (PAK-8687)

- `物理`: プレハブ上のリジッドボディ・コンポーネントが内部物理オブジェクトを生成してしまう問題を修正しました。これは意図されたものではなく、最近の安全性の変更によって表面化したものです。
    ([uum-135381](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodysetpose-when-editing-rigidbody-component-settings-on-a-prefab))

- `物理 2D`: (uum-135381]())`Physics 2D`: "PolygonGeometry.ClosestPoint
    ([uum-134804](https://issuetracker.unity3d.com/issues/polygongeometry-dot-closestpoint-not-returning-perimeter-point-when-overlapped))

- `物理2D`: 物理デバッグ・レンダラーが深度テストを誤って使用していた問題を修正しました。
    (UUM-135992)

- `物理 2D`: (UUM-135939)："PhysicsComposer.GetGeometryIslands\(eRA) "がリードロックされておらず、潜在的な同時実行の問題につながっていた問題を修正しました。
    (UUM-135939)

- `物理 2D`: 編集中のコンポーネントを削除する際の HingeJoint2D ツールハンドルの描画に関する問題を修正しました。
    ([UUM-134276](https://issuetracker.unity3d.com/issues/missingreferenceexception-and-gui-error-errors-thrown-when-deleting-a-sprite-with-box-collider-2d-and-hinge-joint-2d-components))

- `物理 2D`: デフォルトの "PolygonGeometry "コンストラクタが無効なエッジ法線を生成していたのを修正しました。
    ([uum-134804](https://issuetracker.unity3d.com/issues/polygongeometry-dot-closestpoint-not-returning-perimeter-point-when-overlapped))

- `Player`: Video Player がパスにスペースが含まれるファイルを開いたときに発生する URL パース問題を修正。
    ([uum-125789](https://issuetracker.unity3d.com/issues/video-does-not-play-in-macos-build-when-built-app-is-placed-in-a-path-with-a-space-in-it-on-a-specific-project))

- `Profiler`: 不完全なフレームがハイライトビューのサマリーデータに影響する問題を修正しました。
    (UUM-125642)

- `プロファイラー`: プロファイリングデータを記録した後、最大キャプチャフレーム数を減らした場合、保存時にプロファイラーのキャプチャメタデータが作成される問題を修正しました。
    ([UUM-134348](https://issuetracker.unity3d.com/issues/failed-to-read-highlights-data-from-file-dot-dot-dot-unable-to-read-beyond-the-end-of-the-stream-dot-error-is-thrown-after-saving-profiler-capture))

- `Profiler`: kDontCaptureEditor または kRecordTimestamp が異なる場合に、誤った共有 ProfilerRecorder の再利用を防止。
    (UUM-133664)

- `シーン/ゲームビュー`: アクティブな選択範囲にフォーカスすることで、シーンビューのオーバーレイの内容が編集できてしまう問題を修正しました。
    ([UUM-134399](https://issuetracker.unity3d.com/issues/overlays-are-focused-when-using-the-frame-selected-in-window-under-cursor-shortcut-just-after-editing-overlay-fields))

- `スクリプト`: プレイヤービルドにおけるUnityEventのメモリリークを修正しました。
    ([uum-131348](https://issuetracker.unity3d.com/issues/unityeventbase-dot-s-unityevents-memory-leak-occurs-when-loading-and-unloading-scenes-with-ugui-components))

- `Shadergraph`: マスキングを使用しない場合のキャンバスシェーダーの uv1 チャンネルの初期化を修正。
    (UUM-133826)

- `Shadergraph`: ShaderGraph CustomLighting サンプルからの Material Overrides デバッグが機能しないのを修正。
    ([UUM-134440](https://issuetracker.unity3d.com/issues/some-material-overrides-are-viewed-as-broken-when-using-the-shadergraph-customlighting-package-sample))

- `Shadergraph`: HDRとマークされたテクスチャプロパティに対するテクスチャサンプリング操作を修正。
    ([uum-122106](https://issuetracker.unity3d.com/issues/hdr-images-are-compressed-incorrectly-with-default-settings-on-android-platform))

- `Shadergraph`: UGUI ShadersサンプルのFancy Loadingサブグラフを修正。
    (UUM-134638)

- `Shadergraph`: キーワード列挙フィールドの名前の変更とキーワード列挙に対するその他の変更が正しく伝搬するようになりました。
    ([UUM-134292](https://issuetracker.unity3d.com/issues/shadergraph-enum-node-labels-are-not-updated-when-a-new-entry-name-is-set))

- `Shadergraph`: Swizzleノードがアンドゥ/リドゥ後に正しく更新されるようになりました。
    ([uum-134112](https://issuetracker.unity3d.com/issues/shader-graph-swizzle-node-data-updates-incorrectly-after-undo-action))

- `シェーダー`: 計算中の RWTexture2D への書き込みを修正。
    (UUM-127198)

- `テキスト`: PanelTextSettings と FontAsset のアイコンを追加。
    (UUM-134700)

- `テキスト`: ドメインのリロード後に OSFallback が適切に保存されるようにすることで、メモリリークを修正。
    ([UUM-132677](https://issuetracker.unity3d.com/issues/editor-memory-leak-when-entering-and-exiting-play-mode-in-a-blank-urp-project))

- `テキスト`: RichTextTagParser の不完全なタグ解析を修正。
    (UUM-134299)

- `テキストメッシュプロ`: 不適切な書式の &lt;a&gt; タグで "href" 部分が欠落している場合の処理を改善。正しくフォーマットされたタグは &lt;a href="リンクID"&gt;ハイライトされるテキスト&lt;/a&gt; となるはずです。
    ([uum-130554](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-occurs-when-entering-tags-in-a-textmeshpro-ui-field))

- `uGUI`: キーボードが閉じたらInputFieldsを非アクティブにする。
    ([uum-133712](https://issuetracker.unity3d.com/issues/input-field-does-not-update-when-selecting-the-same-input-field-after-previous-input-was-canceled))

- `uGUI`: 矩形変換の境界が非常に大きい場合に発生するクラッシュを修正。
    ([uum-132182](https://issuetracker.unity3d.com/issues/crash-on-raiseexception-when-creating-a-multiplayer-room-while-toggling-ui))

- `uGUI`: 非常に大きなrectトランスフォーム境界を持つことによって引き起こされるクラッシュの根本原因を修正。影響を受けるシーンのGameObjectにリンクする警告を追加しました。
    (UUM-134019)

- `UIツールキット`: 不足していたゲッターAPIを `Painter2D` に追加。
    ([UUM-128715](https://issuetracker.unity3d.com/issues/certain-painter2d-properties-are-missing-the-get-accessors))

- `UIツールキット`: UI Builderのタイプミスを修正。
    ([uum-131438](https://issuetracker.unity3d.com/issues/misspelled-label-custorm-when-editing-aspect-ratio-in-ui-builder-inlined-styles))

- `UIツールキット`: 2Dベクターグラフィックスでストロークパスを描画する際に発生する例外を修正しました。
    (UUM-135440)

- `UIツールキット`: SampleTextureElement ノードを複数回使用できないコード生成のバグを修正しました。
    ([UUM-115301](https://issuetracker.unity3d.com/issues/cant-add-and-use-sample-element-texture-node-twice-in-a-graph))

- `UIツールキット`: コレクションビューコントロールのドラッグ時のスクロールがモバイルデバイスで機能していなかったのを修正。
    ([uum-135398](https://issuetracker.unity3d.com/issues/android-ios-ui-toolkit-listview-touch-pan-scrolling-does-not-work))

- `UIツールキット`: UIE_NOINTERPOLATION の再定義で警告が発生する問題を修正。
    ([uum-134991](https://issuetracker.unity3d.com/issues/uie-nointerpolation-macro-redefinition-warnings-are-thrown-on-vfx-graph-when-changing-the-shader-precision-model-on-web-platform))

- `UIツールキット`: 以前のフレームでオーバーフローが修正された場合に、背景画像として VectorImage がステンシルマスクとして正しく使用されていなかったのを修正。
    ([uum-110567](https://issuetracker.unity3d.com/issues/text-is-not-masked-when-creating-a-vector-image-and-using-a-mask-inside-a-visualelement))

- `UIツールキット`: ダイナミックカラーヒントが使用されている場合に、VectorImagesが均一な色で表示される問題を修正。
    ([uum-126859](https://issuetracker.unity3d.com/issues/svg-pictures-turn-white-on-hover-when-transition-animation-is-added-in-ui-builder))

- `UIツールキット`: SVGをスプライトとしてインポートする際に使用されるマテリアルが間違っていたのを修正。
    ([uum-134795](https://issuetracker.unity3d.com/issues/svg-asset-sprite-materials-are-lost-when-upgrading-the-project-to-a-different-unity-editor-version))

- `UIツールキット`: PanelSettings.renderMode がパブリック API になりました。
    (UUM-119486)

- `URP`: デカールプロジェクターのライトテーマが黒く表示されるようになりました。
    ([UUM-132819](https://issuetracker.unity3d.com/issues/hdrp-decal-projector-and-local-volumetric-fog-are-missing-their-icon-gizmos-hdrp-decal-projector-and-local-volumetric-fog-are-missing-their-icon-gizmos))

- `URP`: 反射プローブの回転がプレイヤーで無効になっていたのを修正。
    (UUM-134244)

- `バージョン管理`: Unity 6.4 以降で非推奨の instanceID API の使用方法を修正。

- `ビデオ`: Vulkan Graphics API を使用した特定のモバイルデバイスで Video を再生できない問題を修正しました。
    ([uum-133914](https://issuetracker.unity3d.com/issues/video-player-renders-no-video-on-specific-devices-when-using-vulkan))

- `Video`: テストを安定させた。
    (UUM-71794)

- `Web`: touchcancel イベントを処理する際に発生していたバグを修正。
    ([UUM-132183](https://issuetracker.unity3d.com/issues/mouse-postion-can-become-max-value-or-infinity-when-using-touch-input-with-legacy-input-module))

- `XR`: オーディオ設定を変更した際にエディタがクラッシュすることがあったのを修正。
    ([uum-126803](https://issuetracker.unity3d.com/issues/crash-on-audiomanager-initfmod-when-performing-various-actions-in-the-editor))




## 6000.3.11f1 におけるパッケージの変更

## 更新されたパッケージ

- `com.unity.addressables`: [2.9.0](https://docs.unity3d.com/Packages/com.unity.addressables@2.9//changelog/CHANGELOG.html) から [2.9.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.9//changelog/CHANGELOG.html) へ。

- `com.unity.cinemachine`: [2.10.5](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html) から [2.10.6](https://docs.unity3d.com/Packages/com.unity.cinemachine@2.10//changelog/CHANGELOG.html) へ。

- `com.unity.collab-proxy`: [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) から [2.11.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html)

- `com.unity.inputsystem`: [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html) から [1.19.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.19//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) から [1.3.2](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) に変更。

- `com.unity.remote-config`: [4.2.4](https://docs.unity3d.com/Packages/com.unity.remote-config@4.2//changelog/CHANGELOG.html) から [4.2.5](https://docs.unity3d.com/Packages/com.unity.remote-config@4.2//changelog/CHANGELOG.html) に変更。

- `com.unity.scriptablebuildpipeline`: [2.6.0](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html) から [2.6.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html) に変更。

- `com.unity.services.analytics`: [6.2.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) から [6.2.2](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) に変更。

- `com.unity.services.wire`: [1.4.1](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html) から [1.4.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html) に変更。

- `com.unity.timeline`: [1.8.10](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) から [1.8.11](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) へ。

- `com.unity.visualscripting`: [1.9.9](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)から[1.9.10](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)

- `com.unity.learn.iet-framework`: [5.0.2](https://docs.unity3d.com/Packages/com.unity.learn.iet-framework@5.0//changelog/CHANGELOG.html) から [5.0.3](https://docs.unity3d.com/Packages/com.unity.learn.iet-framework@5.0//changelog/CHANGELOG.html) に変更。

- `com.unity.learn.iet-framework.authoring`: [1.5.2](https://docs.unity3d.com/Packages/com.unity.learn.iet-framework.authoring@1.5//changelog/CHANGELOG.html)から[1.5.3](https://docs.unity3d.com/Packages/com.unity.learn.iet-framework.authoring@1.5//changelog/CHANGELOG.html)

- `com.unity.terrain-tools`: [5.3.1](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html) から [5.3.2](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html) に変更。

- `com.unity.ai.navigation`: [2.0.10](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)から[2.0.11](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.services.deployment`: [1.6.2](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.6//changelog/CHANGELOG.html)から[1.7.1](https://docs.unity3d.com/Packages/com.unity.services.deployment@1.7//changelog/CHANGELOG.html)

- `com.unity.services.tooling`: [1.4.0](https://docs.unity3d.com/Packages/com.unity.services.tooling@1.4//changelog/CHANGELOG.html)から[1.4.1](https://docs.unity3d.com/Packages/com.unity.services.tooling@1.4//changelog/CHANGELOG.html)

- `com.unity.addressables.android`: [1.0.9](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html)から[1.0.10](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html)

- `com.unity.polyspatial`: [3.0.5](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.0//changelog/CHANGELOG.html)から[3.1.0](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.1//changelog/CHANGELOG.html)

- `com.unity.polyspatial.visionos`: [3.0.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.0//changelog/CHANGELOG.html) から [3.1.0](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.1//changelog/CHANGELOG.html) に変更。

- `com.unity.polyspatial.xr`: [3.0.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.0//changelog/CHANGELOG.html) から [3.1.0](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.1//changelog/CHANGELOG.html) に変更。

- `com.unity.polyspatial.extensions`: [3.0.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.0//changelog/CHANGELOG.html) から [3.1.0](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.1//changelog/CHANGELOG.html) まで。

- `com.unity.xr.visionos`: [3.0.5](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.0//changelog/CHANGELOG.html)から[3.1.0](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.1//changelog/CHANGELOG.html)

- `com.unity.services.multiplayer`: [2.1.2](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.1//changelog/CHANGELOG.html)から[2.1.3](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.1//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.9.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html) から [1.9.2](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html) に変更。

- `com.unity.web.stripping-tool`: [1.2.0](https://docs.unity3d.com/Packages/com.unity.web.stripping-tool@1.2//changelog/CHANGELOG.html) から [1.2.1](https://docs.unity3d.com/Packages/com.unity.web.stripping-tool@1.2//changelog/CHANGELOG.html) へ。