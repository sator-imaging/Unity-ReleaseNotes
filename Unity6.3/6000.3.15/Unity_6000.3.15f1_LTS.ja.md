# Unity 6000.3.15f1 LTS
公開日時： Fri, 08 May 2026 05:39:58 GMT
https://unity.com/releases/editor/whats-new/6000.3.15f1

# 6000.3.15f1 の既知の問題

- `6000.0.61f1`: SDF16 または SDF32 でフォントアトラスを生成すると tlsf_free でクラッシュする。
    ([uum-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true)とUseTextureでAddComputePassを使用するとD3D12SwapChain::Presentでクラッシュする。
    ([uum-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.5.0a4,6000.0.66f1,6000.3.4f1,6000.4.0b4`: ShaderVariantCollection.variantCountとShaderVariantCollection.shaderCountがBuildsで0を返す
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- `メタル`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

DX12グラフィックスAPIがグラフィックスAPIリストの最初にあるのに使用されない
    ([uum-141555](https://issuetracker.unity3d.com/issues/dx12-graphics-api-is-not-used-when-it-is-first-in-the-graphics-api-list))

サブシーンが開いているプレファブモードで子 GameObject を無効にすると、プレファブ内の他の GameObject にマテリアルが移動する
    ([uum-139663](https://issuetracker.unity3d.com/issues/materials-move-to-other-gameobjects-in-a-prefab-when-disabling-a-child-gameobject-in-prefab-mode-with-an-open-subscene))



# 6000.3.15f1 リリースノート

## 改良点

- `ビルドシステム`: 同梱の 7-Zip をバージョン 26.01 に更新。

- `iOS`: iOS`:(codeに頼らずに)メタルリンクの表示を有効にするプレイヤー設定トグルを追加した。

- `iOS`: シリアス/クリティカルな熱状態の時、CAディスプレイリンクに切り替える。



## API の変更

- `物理`: 追加: `Collision` タイプに `angularVelocity` プロパティを追加。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 追加: `ContactPairHeader` タイプに `bodyAngularVelocity` プロパティを追加しました。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 追加: `ContactPairHeader` タイプに `bodyLinearVelocity` プロパティを追加しました。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 追加: `Collision` タイプに `linearVelocity` プロパティを追加しました。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 追加: `ContactPairHeader` タイプに `otherBodyAngularVelocity` プロパティを追加しました。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 追加: `ContactPairHeader` タイプに `otherBodyLinearVelocity` プロパティを追加しました。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 追加: `Collision` タイプに `thisAngularVelocity` プロパティを追加しました。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 追加: `Collision` タイプに `thisArticulationBody` プロパティを追加しました。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 追加: `Collision` タイプに `thisBody` プロパティを追加しました。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 追加: `Collision` タイプに `thisGameObject` プロパティを追加しました。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 追加: `Collision` タイプに `thisLinearVelocity` プロパティを追加しました。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 追加: `Collision` タイプに `thisRigidbody` プロパティを追加しました。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `物理`: 追加: `Collision` タイプに `thisTransform` プロパティを追加しました。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))



## 修正

- `2D`: 特定のプロジェクトを開いた時に ShaderPropertySheet::FindPropertyIndex でクラッシュする問題を修正。
    ([uum-110537](https://issuetracker.unity3d.com/issues/crash-on-shaderpropertysheet-findpropertyindex-when-opening-a-specific-project))

- `2D`: URP 2D を使用している場合に、プレビュー・カメラでライティングとシャドウが欠落していたのを修正。
    (UUM-139229)

- `アクセシビリティ`: アクセシビリティ・ノードが、最大ID値をラップした後に重複したIDで作成されるのを修正。
    ([UUM-137871](https://issuetracker.unity3d.com/issues/accessibilityhierarchy-throws-an-exception-when-node-id-reaches-int-dot-maxvalue))

- `適応パフォーマンス`: ゼロサイズのレンダーテクスチャでのエラーを避けるため、アダプティブ・パフォーマンスの再計算されたディスクリプタのサイズを1にクランプ。
    ([uum-138049](https://issuetracker.unity3d.com/issues/urp-rendergraph-throws-rendertexturedesc-height-must-be-greater-than-zero-when-camera-pixel-height-becomes-0-due-to-small-window-resolution-and-fractional-viewport-rect))

- `AI`: NavAgent.Moveで移動したときに、NavMeshAgentがボックスの障害物の角に引っかかるのを修正。
    ([uum-136684](https://issuetracker.unity3d.com/issues/navmeshagent-gets-stuck-on-the-corner-of-a-box-shape-navmeshobstacle-when-it-is-moved-with-navagent-dot-move))

- `Android`: コントローラーが軸イベントではなくボタンイベントとしてL2/R2を報告する場合、Android上でSwitch Proゲームパッドのトリガーが機能しないのを修正しました。
    (UUM-139567)

- `アニメーション`: Animatorウィンドウで短いループアニメーションのトランジションを選択する際にArgumentOutOfRangeExceptionが発生する問題を修正。
    ([UUM-139812](https://issuetracker.unity3d.com/issues/argumentoutofrangeexception-is-thrown-when-selecting-a-transition-to-an-animation-shorter-than-3-frames-with-loop-time-enabled))

- `DX12`: 大きなシーンでの D3D12 フェンスの遅いメモリリークを修正しました。
    (UUM-140429)

- `DX12`: 負のインデックスを持つ配列にアクセスしないように。
    (UUM-134479)

- `エディター`: UI Builder のタイプピッカーに `None` を追加。
    ([UUM-137289](https://issuetracker.unity3d.com/issues/none-data-source-type-option-is-missing-when-opening-select-type-dot-dot-dot-in-ui-builder-bindings))

- `エディタ`: のような特殊文字を含むクエリでもクリップボードへのコピーが機能するようになりました。
    ([uum-137347](https://issuetracker.unity3d.com/issues/save-to-clipboard-for-search-query-that-contains-a-function-block-throws-a-formatexception-error))

- `エディター`: ネストされたタグが ATG で動作しない問題を修正。
    (UUM-139569)

- `エディター`: TextCoreでUnderlineを使用したときに範囲外の例外が発生する問題を修正。
    ([UUM-137906](https://issuetracker.unity3d.com/issues/ui-builder-windows-text-rendering-breaks-when-using-rich-text-combined-with-an-underlined-emoji))

- `エディター`: LinuxEditorでアンカー・プリセットのUIがShift/Alt修飾キーに反応しない問題を修正。
    ([uum-137598](https://issuetracker.unity3d.com/issues/linux-shift-slash-alt-modifier-keys-are-not-recognized-in-anchor-presets-when-adjusting-rect-transform))

- `エディター`: 列挙値のマルチエディットを修正。
    ([uum-138913](https://issuetracker.unity3d.com/issues/cant-change-the-shape-of-multiple-lights-at-the-same-time-using-lighting-search))

- `Editor`: Adaptive Performance 設定のプロバイダ名リストが中央からずれていたのを修正。
    ([uum-136419](https://issuetracker.unity3d.com/issues/the-provider-name-text-is-off-centered-in-the-adaptive-performance-settings))

- `エディター`: ドメインのリロード時にレイアウトと置換テーブルがリークする問題を修正。
    ([uum-138000](https://issuetracker.unity3d.com/issues/editor-memory-leak-in-visualelement-when-recompiling-in-a-blank-urp-project))

- `エディター`: ウィンドウの切り替え時にビューが正しくリフォーカスされない問題を修正。
    ([uum-139948](https://issuetracker.unity3d.com/issues/cannot-interact-with-gameobjects-in-the-hierarchy-window-by-using-shortcuts-or-edit-menu-when-selecting-a-gameobject-in-the-hierarchy-with-a-select-window-opened))

- `エディター`: DrawText`が指定した色で描画されない問題を修正。
    ([uum-137907](https://issuetracker.unity3d.com/issues/color-parameter-is-ignored-when-creating-dynamic-text-in-a-ui-document-with-drawtext))

- `Editor`: ウイルス対策ソフトウェアが署名されていないバイナリを不審なものとしてフラグを立てることによる潜在的な問題を防ぐため、IL2CPP 関連のファイルに署名。
    (UUM-137463)

- `エディター`: 元に戻す(Undo)がすべてのライトタイプでサポートされました。
    ([UUM-136891](https://issuetracker.unity3d.com/issues/light-type-slash-mode-changes-are-not-undone-with-ctrl-plus-z-shortcut-when-edited-from-lighting-search-window))

- `Editor`: OpenGL ES を搭載した Mali GPU でステンシルのみのフォーマットを使用した場合のクラッシュを回避。
    ([uum-111344](https://issuetracker.unity3d.com/issues/android-crash-on-startup-when-depth-stencil-format-is-set-to-s8-uint))

- `EmbeddedLinux`: コールバックのネストされたウィンドウの非同期操作を修正しました。
    (UUM-138651)

- `エンジン診断`: CrashReportingSettings.captureEditorExceptions が有効な場合に、エディターの例外がエンジン診断に報告されない問題を修正しました。
    ([UUM-136672](https://issuetracker.unity3d.com/issues/diagnostics-does-not-report-editor-exceptions-when-using-crashreportingsettings-dot-captureeditorexceptions))

- `GI`: シーンにUVレイアウトの面積がゼロのメッシュが含まれる場合に、xAtlasでライトマップのパッキングが失敗するバグを修正しました。
    ([uum-139715](https://issuetracker.unity3d.com/issues/crash-on-xatlas-internal-pack-atlas-findchartlocation-bruteforce-when-generating-the-lighting))

- `GI`: xAtlasパッカーを使用する際、参照されていない頂点位置を持つメッシュがベイク中にクラッシュすることがあったバグを修正しました。
    ([uum-138494](https://issuetracker.unity3d.com/issues/crash-with-multiple-stacktraces-when-building-lighting-in-a-specific-scene))

- `GI`: UnifiedRT TraceRay シェーダーにおける FXC の警告を抑制しました。
    ([uum-139001](https://issuetracker.unity3d.com/issues/switching-platforms-will-trigger-shader-related-warnings-tracetransparentrays))

- `GI`: UnifiedRT: Playerのビルドで `RayTracingRenderPipelineResources` がパブリックでなければならない問題を修正しました。
    ([uum-137604](https://issuetracker.unity3d.com/issues/unifiedraytracing-raytracingrenderpipelineresources-being-internal-prevents-loading-raytracingresources-in-the-player))

- `Graphics`: Terrain がアクティブなプロジェクトで Load RenderDoc をクリックするとクラッシュする問題を修正。
    ([uum-99314](https://issuetracker.unity3d.com/issues/crash-on-d3d12descriptorcache-deallocate-or-vkgetinstanceprocaddr-when-loading-renderdoc-in-a-specific-scene))

- `Graphics`: DX12、Metal、およびレガシー Vulkan デバイスで ScalableBufferManager を使用した場合に、MSAA CameraDepthTexture のリサイズに一貫性がない問題を修正しました。 スタンドアロンまたは Android プレーヤーをビルドする際に、ベクター型シェーダーの暗黙の切り捨て警告が投げられる問題を修正しました。
    ([uum-100367](https://issuetracker.unity3d.com/issues/android-ios-macos-inconsistent-cameradepthtexture-behavior-when-using-scalablebuffermanager-across-devices))

- `Graphics`: 複数のピクセル密度を持つマルチモニター設定において、Virtual Texturing Profiler モジュールのヘルプボタンのスケーリングを修正しました。
    ([uum-137763](https://issuetracker.unity3d.com/issues/virtual-texturing-documentation-button-is-oversized-and-not-consistent-with-other-editor-documentation-buttons-when-virtual-texturing-module-is-selected-in-the-profiler-window))

- `Graphics`: Vulkan 使用時の Pixel 10 のインスタンス化を修正。
    (UUM-139629)

- `Graphics`: Direct3D で `R16G16B16` フォーマットのテクスチャをインポートする際の問題を修正。
    ([UUM-104117](https://issuetracker.unity3d.com/issues/texture-displays-visual-artifacts-and-has-a-broken-aspect-ratio-when-it-is-imported-in-rgb-48-bit-format))

- `Graphics`: ユニフォームバッファバインディングに無効なバインディングスロットが渡された場合の OpenGLES のクラッシュを修正しました。
    (UUM-138897)

- `Graphics`: Streaming Controllerコンポーネントのドキュメントへのリンクを修正しました。
    ([UUM-139928](https://issuetracker.unity3d.com/issues/missing-documentation-page-opens-when-clicking-open-reference-button-on-streaming-controller-component))

- `Graphics`: Virtual Texturing Profiler モジュールのドキュメントへのリンクを修正。
    ([uum-137763](https://issuetracker.unity3d.com/issues/virtual-texturing-documentation-button-is-oversized-and-not-consistent-with-other-editor-documentation-buttons-when-virtual-texturing-module-is-selected-in-the-profiler-window))

- `Graphics`: サポートされていないグラフィックスAPIを使用した場合に、GraphicsStateCollection.Warmupがレガシーシェーダーバリアントのロードにフォールバックすることに関する、リリースビルドでの繰り返しのログメッセージを削除しました。
    (UUM-138841)

- `Graphics`: \(UUM-138841) `Graphics`: `RenderTexture` への深度解決またはコンピュートシェーダの書き込み後に、不正確な `DontCare` ロードアクションが適用され、アーティファクトが表示される問題を修正しました。
    (UUM-46565)

- `HDRP`: HDRP SSGIがスクリーンの片側から反対側に色をにじませるバグを修正しました。
    ([UUM-139120](https://issuetracker.unity3d.com/issues/lighting-leaks-from-right-and-top-edges-to-left-and-bottom-edges-when-screen-space-global-illumination-uses-ray-tracing-in-hdrp))

- `HDRP`: レンダリングデバッガーで、*Freeze Camera For Culling*ドロップダウンがオプションとして*None*しか表示されていなかった問題を修正しました。
    ([uum-137626](https://issuetracker.unity3d.com/issues/none-is-only-present-when-using-hdrp-rendering-debuggers-freeze-camera-for-culling-dropdown))

- `HDRP`: 歪曲のためのカラーピラミッド後の _ColorPyramidUvScaleAndLimitCurrentFrame の null limit.xy 値を修正。
    ([uum-130925](https://issuetracker.unity3d.com/issues/hdrp-liquid-sample-custom-injection-pass-breaks-transparency-and-refraction-when-set-to-before-post-process))

- `iOS`: GameCenterから実績を複数回ロードするとクラッシュする問題を修正。
    (UUM-138417)

- `カーネル`: ジョブシステムがファイナライザからアクセスされた場合のシャットダウン中のクラッシュを修正しました。
    ([UUM-128777](https://issuetracker.unity3d.com/issues/crash-on-jobqueue-hasjobgroupidcompleted-when-closing-the-editor-while-in-play-mode-on-a-specific-project))

- `Linux`: Linux Arm64 Server 用の Arm64 sysroot をインストールしない Linux 自動ツールチェーンインストーラを修正しました。
    (UUM-136647)

- `Networking`: Linuxプレーヤのビルドで、ある.NETネットワーキングAPIを使おうとすると例外がスローされる（特に `WebRequest`）欠落していたMono設定ファイルを追加しました。
    ([uum-135731](https://issuetracker.unity3d.com/issues/webrequest-dot-create-function-fails-with-uri-prefix-is-not-recognized-errors-when-the-project-is-built-for-linux-standalone-or-windows-dedicated-server))

- `ネットワーキング`: MbedTLSをバージョン3.6.6に更新し、幾つかの(マイナーでおそらく爆発不可能な)セキュリティ脆弱性に対処した。
    (UUM-140908)

- `パッケージ`: RagdollWindow にリサイズ時の ScrollView サポートを追加。
    ([UUM-139914](https://issuetracker.unity3d.com/issues/the-ragdoll-builder-window-has-no-scrollbar-making-elements-unreachable-unless-the-window-is-resized))

- `パッケージマネージャー`: パッケージキャッシュの場所を変更するとエディターログに "TLS Allocator ALLOC_TEMP_MAIN has unfreed allocations" エラーが繰り返し表示される問題を修正。
    ([uum-131286](https://issuetracker.unity3d.com/issues/tls-allocator-alloc-temp-tls-underlying-allocator-alloc-temp-main-has-unfreed-allocations-dot-dot-dot-error-when-changing-the-packages-cache-location-folder))

- `物理`: MeshCollider コンポーネントが一様でないスケールを受け取ると、それを正しく処理できない問題を修正しました。
    ([uum-139681](https://issuetracker.unity3d.com/issues/mesh-collider-does-not-skew-slash-shear-correctly-when-nested-inside-another-gameobject))

- `物理`: ボディと `Collider` コンポーネントが異なる GameObject 上にある場合、`ArticulationBody` コンポーネントと衝突すると `Collision.transform` が正しくない `Transform` を返す問題を修正しました。
    ([uum-140799](https://issuetracker.unity3d.com/issues/unable-to-access-linear-slash-angular-velocity-inside-collision-in-order-to-use-relativevelocity))

- `プラグイン`: \DLSSのジッターとちらつきの問題を修正しました。
    ([uum-134012](https://issuetracker.unity3d.com/issues/game-view-jitters-on-high-frame-rates-when-dlss-is-enabled-and-the-mode-is-set-to-ultra-performance))

- `Profiler`: FrameTimingManager.GetLatestTimings`APIを更新し、Playerの一時停止が解除されたときに、フォーカスされた次のフレームにバックグラウンドの時間が含まれないようにしました。
    ([uum-132089](https://issuetracker.unity3d.com/issues/frametimingmanager-dot-getlatesttimings-adds-background-time-to-the-next-focused-frame-when-the-player-is-unfocused))

- `QNX`: コールバックでネストされたウィンドウの非同期操作を修正。
    (UUM-138651)

- `シーン/ゲームビュー`: プレイモード中に PlayModeWindow.SetViewType を使用するとエディターがクラッシュするバグを修正。
    ([UUM-139011](https://issuetracker.unity3d.com/issues/crash-on-repaintcontroller-renderplaymodeviewcameras-when-entering-play-mode-and-playmodewindow-dot-setviewtype-being-called-at-end-of-frame))

- `スクリプト`: 新しい空の参照エントリをアセンブリ定義アセットインスペクタに追加し、適用をクリックすると、エントリが空のままではなく、リストの最後のエントリと誤って重複する。
    (UUM-119332)

- `Shadergraph`: enum`キーワード入力に、プロジェクトのシェーダービルド設定を上書きする設定を追加しました。また、`enum`に`none`エントリを追加する設定を追加。
    (UUM-135644)

- `テキスト`: シャドウおよびアウトラインと組み合わせたときにカラーグラデーションが機能するように。
    ([UUM-140065](https://issuetracker.unity3d.com/issues/ui-toolkit-color-gradient-not-applying-to-label-text-when-outline-width-is-set-to-more-than-0))

- `テキスト`: supタグとsubタグの折り返しでNullReferenceExceptionが発生する問題を修正。
    ([uum-139927](https://issuetracker.unity3d.com/issues/nullreferenceexception-is-thrown-when-resizing-a-text-element-in-the-ui-builder-when-it-contains-sup-or-sub-elements-and-wrap-mode-is-enabled))

- `uGUI`: OnValidateイベントでスクリプトを使用して入力フィールドのフォーカスを変更するとNullReferenceExceptionが発生する問題を修正しました。
    ([uum-132637](https://issuetracker.unity3d.com/issues/nullreferenceexception-error-is-thrown-when-changing-input-field-focus-via-script-with-custom-validation))

- `uGUI`: Tabキーでフォーカスを移動したとき、InputFieldがハングル文字の最後の文字を取得できない問題を修正しました。
    ([uum-126213](https://issuetracker.unity3d.com/issues/inputfield-fails-to-get-the-last-character-of-a-hangul-ime-korean-character-text-when-focus-is-shifted-with-the-tab-key))

- `UIツールキット`: NULL可能な参照型が有効な時にプロパティバッグを生成するコードでコンパイルエラーが発生する問題を修正。
    ([uum-126159](https://issuetracker.unity3d.com/issues/createproperty-on-nullable-generic-types-causes-compilation-error-when-using-a-non-nullable-type))

- `UIツールキット`: テクスチャとしてインポートした際のSVGプレビューのアルファを修正。
    ([uum-137765](https://issuetracker.unity3d.com/issues/project-window-preview-icon-is-fully-black-when-a-black-svg-shape-is-imported-and-set-as-a-texture2d))

- `UIツールキット`: テキストシャドウのぼかし半径と別のプロパティを編集した後、Ctrl+S/Cmd+Sで保存すると、IndexOutOfRangeExceptionとぼかし半径の値が元に戻る問題を修正。
    ([uum-139822](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-is-thrown-and-blur-radius-value-reverts-when-saving-after-modifying-blur-radius-and-another-property-in-ui-builder))

- `UIツールキット`: ToSourceバインディングモードを使用したバインディングが、UIの変更後にUIを更新してしまう問題を修正しました。
    ([uum-120902](https://issuetracker.unity3d.com/issues/uitk-textfield-value-is-overwritten-incorrectly-by-the-converter-result-when-binding-mode-is-set-to-to-source))

- `UIツールキット`: ランタイムバインディングシステムを通してUnityEngine.Objectにバインドされたプロパティが、ソースにNULLをセットし返せない問題を修正しました。
    ([uum-134627](https://issuetracker.unity3d.com/issues/ui-toolkit-throws-warning-and-fails-to-clear-references-when-fields-are-not-typed-as-unityengine-dot-object))

- `UIツールキット`: StyleSheet`の色をエクスポートする際に、十分な精度が得られない問題を修正しました。
    ([uum-127703](https://issuetracker.unity3d.com/issues/ui-builder-background-color-picker-alpha-values-are-set-to-even-numbers-when-saving-alpha-value-as-an-odd-number))

- `UIツールキット`: パックされたスプライトがダイナミックアトラスに入ることがある問題を修正。
    ([uum-137771](https://issuetracker.unity3d.com/issues/9-sliced-sprite-assigned-as-background-in-a-ui-toolkit-visual-element-is-rendered-blurry))

- `UIツールキット`: UI Builder Hierarchyで検索しているときにUI Builderで要素を追加できない問題を修正。
    ([uum-138485](https://issuetracker.unity3d.com/issues/unable-to-add-elements-in-ui-builder-when-searching-in-ui-builder-hierarchy))

- `UIツールキット`: SVGImporterとFilterFunctionDefinitionのドキュメントヘルプリンクを修正。
    ([uum-139170](https://issuetracker.unity3d.com/issues/clicking-in-inspector-for-svg-importer-opens-missing-documentation-page-instead-of-relevant-manual))

- `UIツールキット`: インポートされたベクター画像アセットInspectorヘッダーのドキュメントリンクが欠落していたのを修正。
    ([uum-139560](https://issuetracker.unity3d.com/issues/vector-image-asset-documentation-link-is-missing))

- `UIツールキット`: HelpURL]` のネストしたマニュアルトピックが "page missing" ドキュメントページに解決されるのを修正。
    ([uum-140384](https://issuetracker.unity3d.com/issues/sorry-dot-dot-dot-that-page-seems-to-be-missing-is-shown-on-the-browser-when-clicking-the-help-icon-on-a-panel-renderer-component))

- `UIツールキット`: 検索結果の要素を操作した際に、検索モードが終了するように修正。
    ([uum-138487](https://issuetracker.unity3d.com/issues/search-mode-is-exited-when-any-resulting-element-is-manipulated-with))

- `UIツールキット`: 古いデータの削除時にTryRemoveItemの無効な操作例外が発生する問題を修正。
    ([uum-137639](https://issuetracker.unity3d.com/issues/an-invalidoperationexception-error-is-thrown-when-tryremoveitem-is-used-with-rebuildtree-set-to-false))

- `URP`: Adaptive Performanceが実行時にデカールの描画距離をオーバーライドできることを明確にするドキュメントを追加。
    ([uum-138945](https://issuetracker.unity3d.com/issues/urp-decals-become-invisible-when-over-1000-units-away-from-the-camera))

- `URP`: Shader Graphで書かれたカスタムUITKシェーダーにステレオインスタンシングのサポートを追加。
    ([uum-131994](https://issuetracker.unity3d.com/issues/spi-xr-custom-ui-toolkit-ui-shader-graph-materials-only-render-in-one-eye-when-using-single-pass-instanced-rendering))

- `URP`: URP DepthBlit サンプルを修正し、必要でない時に手動で深度を解決しないようにしました。
    ([uum-134993](https://issuetracker.unity3d.com/issues/non-multisampled-texture-binding-errors-are-logged-when-running-the-depthblit-urp-scene-with-msaa-enabled-on-vulkan))

- `Video`: Windows ベースのプラットフォームで Segmented MP4 ファイルを開く際に、このメディアタイプがサポートされていないため、Console の警告を追加。
    ([uum-132004](https://issuetracker.unity3d.com/issues/video-player-does-not-throw-an-error-when-playing-a-video-with-unsupported-encoding-settings))

- `WebGL`: R16UNorm`、`R16SNorm`、`RG16UNorm`、`RG16SNorm`、`RGBA16UNorm`、`RGBA16SNorm` が誤ってフィルタ可能として宣言されていた問題を修正しました。
    ([uum-139873](https://issuetracker.unity3d.com/issues/r16unorm-texture-usage-fails-for-webgpu))

- `WebGL`: フルスクリーン状態を切り替えた時の WebGL コンソールの警告を修正しました。
    ([uum-139208](https://issuetracker.unity3d.com/issues/webgl-console-warnings-switching-fullscreen))

- `WebGL`: \WebGPU]CoreCopyシェーダによるMSAAテクスチャのRenderGraphエラーを修正。
    ([uum-133838](https://issuetracker.unity3d.com/issues/webgpu-errors-when-corecopy-shader-is-used-to-copy-an-msaa-texture))

- `WebGL`: \WebGPU] モバイルデバイスで WebCam ビデオが正しく表示されるようにしました。
    ([uum-139017](https://issuetracker.unity3d.com/issues/ios-web-webgpu-webcamtextures-camera-orientation-is-fixed-relative-to-the-phones-right-edge))

- `XR`: URPでマルチパスXRレンダリングモードを使用する際、内蔵シェーダー定数unity_StereoEyeIndexが適切に設定されず、Skybox/Panoramicなどのシェーダーに影響を与え、3D Layoutオプションを使用しても立体視表示に失敗する問題を修正しました。
    ([uum-120719](https://issuetracker.unity3d.com/issues/stereoscopic-skybox-renders-as-monoscopic-when-using-multi-pass-render-mode-in-xr-plugin-while-using-urp))




## 6000.3.15f1 におけるパッケージの変更

## 更新されたパッケージ

- `com.unity.netcode`: [1.10.0](https://docs.unity3d.com/Packages/com.unity.netcode@1.10//changelog/CHANGELOG.html) から [1.13.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html) へ。

- `com.unity.services.user-reporting`: [2.0.14](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html)から[2.0.15](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html)

- `com.unity.xr.core-utils`: [2.5.3](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html)から[2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.6//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: [2.11.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.11//changelog/CHANGELOG.html)から[2.11.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.11//changelog/CHANGELOG.html)

- `com.unity.polyspatial`: [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.1//changelog/CHANGELOG.html) から [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial@3.1//changelog/CHANGELOG.html) へ。

- `com.unity.polyspatial.visionos`: [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.1//changelog/CHANGELOG.html) から [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.visionos@3.1//changelog/CHANGELOG.html)

- `com.unity.polyspatial.xr`: [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.1//changelog/CHANGELOG.html) から [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.xr@3.1//changelog/CHANGELOG.html) に変更。

- `com.unity.polyspatial.extensions`: [3.1.4](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.1//changelog/CHANGELOG.html) から [3.1.5](https://docs.unity3d.com/Packages/com.unity.polyspatial.extensions@3.1//changelog/CHANGELOG.html) に変更。

- `com.unity.xr.visionos`: [3.1.4](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.1//changelog/CHANGELOG.html) から [3.1.5](https://docs.unity3d.com/Packages/com.unity.xr.visionos@3.1//changelog/CHANGELOG.html) に変更。

- `com.unity.asset-manager-for-unity`: [1.10.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.10//changelog/CHANGELOG.html) から [1.11.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.11//changelog/CHANGELOG.html) へ。

- `com.unity.web.stripping-tool`: [1.2.1](https://docs.unity3d.com/Packages/com.unity.web.stripping-tool@1.2//changelog/CHANGELOG.html) から [1.3.0](https://docs.unity3d.com/Packages/com.unity.web.stripping-tool@1.3//changelog/CHANGELOG.html) へ。

**パッケージ追加**。

- [com.unity.platformtoolkit.steam@1.0.2](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.steam@1.0//changelog/CHANGELOG.html)

- [com.unity.platformtoolkit.playgamesservices@1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.playgamesservices@1.0//changelog/CHANGELOG.html)

- [com.unity.platformtoolkit.gdk@1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gdk@1.0//changelog/CHANGELOG.html)

- [com.unity.platformtoolkit.gamekit@1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit.gamekit@1.0//changelog/CHANGELOG.html)

- [com.unity.platformtoolkit@1.0.1](https://docs.unity3d.com/Packages/com.unity.platformtoolkit@1.0//changelog/CHANGELOG.html)