# Unity 6000.3.14f1 LTS
公開日時: Wed, 22 Apr 2026 12:21:09 GMT
https://unity.com/releases/editor/whats-new/6000.3.14f1

# 6000.3.14f1 の既知の問題点

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true)とUseTextureでAddComputePassを使用するとD3D12SwapChain::Presentでクラッシュする。
    ([uum-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.2.0a10`: プロジェクトを初めて開いたときに TexturesD3D12::CreateTextureInternal() でクラッシュする。
    ([uum-135024](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-opening-a-project-for-the-first-time))

- `6000.3.0a3`: Umbra::QueryExt::queryStaticShadowCasters で、Near Clipping Planes の最小値でカスタム Reflection Probe をベイクするとクラッシュする。
    ([uum-137250](https://issuetracker.unity3d.com/issues/crash-on-umbra-queryext-querystaticshadowcasters-when-baking-a-custom-reflection-probe-with-the-minimum-near-clipping-planes-value))

- `6000.3.0a5`: カメラから1000ユニット以上離れるとURPデカールが見えなくなる
    ([uum-138945](https://issuetracker.unity3d.com/issues/urp-decals-become-invisible-when-over-1000-units-away-from-the-camera))

- `6000.5.0a4,6000.0.66f1,6000.3.4f1,6000.4.0b4`: ShaderVariantCollection.variantCountとShaderVariantCollection.shaderCountがBuildsで0を返します。
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- `6000.5.0a8,6000.6.0a1,6000.4.0b12,6000.3.12f1`: 照明生成時に xatlas::internal::pack::Atlas::findChartLocation_bruteForce でクラッシュする。
    ([uum-139715](https://issuetracker.unity3d.com/issues/crash-on-xatlas-internal-pack-atlas-findchartlocation-bruteforce-when-generating-the-lighting))

- `6000.5.0a8,6000.6.0a1,6000.4.0b12,6000.3.12f1`: 特定のシーンで照明をビルドすると複数のスタックトレースでクラッシュする
    ([uum-138494](https://issuetracker.unity3d.com/issues/crash-with-multiple-stacktraces-when-building-lighting-in-a-specific-scene))

- `6000.6.0a1,6000.3.11f1`: UIドキュメントでDrawText()を使用して動的テキストを作成すると、Colorパラメータが無視される
    ([uum-137907](https://issuetracker.unity3d.com/issues/color-parameter-is-ignored-when-creating-dynamic-text-in-a-ui-document-with-drawtext))

- `6000.6.0a1,6000.5.0a9,6000.3.12f1,6000.4.0f1`: プラットフォームを切り替えるとシェーダ関連の警告が発生する (TraceTransparentRays)
    ([uum-139001](https://issuetracker.unity3d.com/issues/switching-platforms-will-trigger-shader-related-warnings-tracetransparentrays))

- `メタル`: コマンドバッファのタイムアウトエラーの後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

List<T>構造体でネストされた[SerializeReference]フィールドを使用すると "core::base_hash_set "でクラッシュする
    ([uum-139722](https://issuetracker.unity3d.com/issues/crash-on-core-base-hash-set-when-using-nested-serializereference-fields-in-list-structures))

空白のURPプロジェクトで再コンパイルする際のVisualElementのエディタ・メモリ・リーク
    ([uum-138000](https://issuetracker.unity3d.com/issues/editor-memory-leak-in-visualelement-when-recompiling-in-a-blank-urp-project))

サブシーンが開いているプレファブモードで子 GameObject を無効にすると、プレファブ内の他の GameObject にマテリアルが移動する。
    ([uum-139663](https://issuetracker.unity3d.com/issues/materials-move-to-other-gameobjects-in-a-prefab-when-disabling-a-child-gameobject-in-prefab-mode-with-an-open-subscene))



# 6000.3.14f1 リリースノート

## 機能

- `UIツールキット`: UIツールキット：一般的な問題や非推奨のパターンを修正するための自動UXMLアップグレードを適用するためのUXMLアップグレードフレームワークを導入しました。



## 改善点

- `UIツールキット`: UIビルダーに要素のUXML属性をアルファベット順にエクスポートするオプションを追加。

- `UIツールキット`: デフォルト・メッシュでエッジ・アンチエイリアスが適用される領域を減らすことで、GPUパフォーマンスを改善。

- `UIツールキット`: VisualElement.UpdateWorldTransformInverse のパフォーマンスを改善。

- `XR`: Meta Quest Build Profileのカスタム品質設定のデフォルト設定を更新しました。



## API の変更

- `エディタ`: 変更: ENABLE_UNITY_COLLECTIONS_CHECKS が定義されていない場合に、JobHandle.GetHashCode と Equals と ==/!= 演算子を公開。

- `UIツールキット`: 追加: VisualElementのインラインスタイルをクリアするAPIを追加しました。



## 変更点

- `オーディオ`: メモリーリークを回避するため、Chromium ベースのウェブブラウザーで Compressed In Memory 設定のデフォルトを Decompress On Load に変更。
    ([uum-136929](https://issuetracker.unity3d.com/issues/detached-audio-source-is-not-released-from-browser-memory-when-audio-stops-playing-in-webgl-player))



## 修正

- `2D`: 2D レンダラーで Unity Recorder を使用するためのサポートを追加。
    (UUM-136415)

- `2D`: スプライトスキンがカリングされた時のスプライトのちらつき/描画コールの変動。
    ([UUM-132924](https://issuetracker.unity3d.com/issues/draw-call-count-fluctuates-and-frame-debugger-output-flickers-when-viewing-a-psd-based-sprite-skin-with-always-update-disabled-in-game-view))

- `アクセシビリティ`: アクセシビリティAPIを使用する際にクラッシュする可能性を修正。
    (UUM-132644)

- `アクセシビリティ`: Windows 10 で UI Automation が無効なポインタにアクセスすることで発生するプレーヤーのクラッシュを修正しました。
    ([UUM-126552](https://issuetracker.unity3d.com/issues/application-crash-when-setting-assistivesupport-dot-activehierarchy-with-narrator-enabled-on-windows-10))

- `アクセシビリティ`: Windows10で失敗していた `AssistiveSupport` のプレイモードテストを修正し、再度有効にしました。
    (UUM-111323)

- `アダプティブ・パフォーマンス`: Adaptive Performance プロファイラー・モジュールのスケーラー・データの UI 構造を修正。
    (UUM-138268)

- `適応パフォーマンス`: パフォーマンスのためのアダプティブ・パフォーマンス・ロギングをリファクタリング。機能的な変更はありません。
    (UUM-138191)

- `AI`: 半径が小さく、目的地が遠いエージェントのデバッグビジュアライゼーションの描画クラッシュを修正。
    ([UUM-133552](https://issuetracker.unity3d.com/issues/crash-on-memcpy-repmovs-when-selecting-navmesh-agent-objects-while-in-play-mode-in-a-specific-scene))

- `Android`: AndroidのPlayer SettingsでDepth/Stencil bufferを無効にしてURPを使用するとクラッシュする問題を修正しました。
    ([uum-109005](https://issuetracker.unity3d.com/issues/android-player-crashes-on-vk-renderpasses-getpackedrenderpass-when-using-vulkan-graphics-api-in-a-specific-project))

- `Android`: Pixel 10 で、discard や clip を使用するシェーダーでアーティファクトが発生する問題を修正しました。
    (UUM-139019)

- `アニメーション`: 一部のParticleSystemプロパティがAnimationClipに追加され、AnimationWindowでサンプリングされた際にエラーや警告を引き起こす問題を修正しました。
    ([UUM-134950](https://issuetracker.unity3d.com/issues/unsupported-type-minmaxcurve-error-and-could-not-register-property-modification-for-animation-binding-dot-dot-dot-warnings-are-thrown-after-moving-playhead-when-particle-system-property-is-added-to-animation-window))

- `オーディオ`: スクリプト可能なジェネレーターでIRealtime.ProcessからPipe.GetAvailableDataを呼び出すと例外がスローされるのを修正しました。
    ([uum-133969](https://issuetracker.unity3d.com/issues/pipes-are-not-working-for-nested-generators))

- `オーディオ`: 非ChromiumウェブブラウザでCompressed In Memory設定を使用した場合のメモリリークを修正しました。
    ([uum-136929](https://issuetracker.unity3d.com/issues/detached-audio-source-is-not-released-from-browser-memory-when-audio-stops-playing-in-webgl-player))

- `DX12`: 保留中のコマンドバッファが多すぎる場合に定期的なフルフラッシュを実行するようにしました。
    ([uum-138597](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-selecting-gameobjects-in-the-scene-view-while-using-dx12))

- `DX12`: (Alt-Tabで) "Exclusive Fullscreen "ウィンドウを最小化する時、レンダリングを一時停止することで致命的なクラッシュを減らしました。他のモードとグラフィックAPIは影響を受けません。より良い安定性のために、"FullScreenWindow"⇄(borderless) mode⇄(https://devblogs.microsoft.com/directx/demystifying-full-screen-optimizations/) の使用を検討してください。
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))

- `エディタ`: 適応パフォーマンス設定にリセットボタンを追加。
    ([uum-135693](https://issuetracker.unity3d.com/issues/adaptive-performance-settings-on-the-custom-build-profile-cant-be-reset))

- `エディター`: ドッキングされたBuild Profilesウィンドウでプレビューをクリックすると`NullReferenceException`が発生する問題を修正。
    ([uum-134827](https://issuetracker.unity3d.com/issues/nullreferenceexception-error-is-thrown-when-clicking-to-preview-the-splash-image-in-build-profiles-window))

- `Editor`: Graphics Settingsでデフォルトのボリュームプロファイルを変更する際にスローされる例外を修正。
    (UUM-136748)

- `Editor`: EditorSettings.asset`のアップグレードに失敗したり、手動で元に戻したり変更した場合に、Enter Play ModeのDomain Reloadが無効でもDomain Reloadが発生する問題を修正しました。
    ([uum-138521](https://issuetracker.unity3d.com/issues/enterplaymodeoptions-doesnt-take-effect-if-user-manually-modifies-m-enterplaymodeoptionsenabled-to-0))

- `エディター`: アニメーションウィンドウでHDRカラーが正しく記録されていなかった問題を修正。
    ([uum-83771](https://issuetracker.unity3d.com/issues/hdr-colors-are-recorded-in-gamma-compressed-values-instead-of-linear-values-when-using-the-animation-window))

- `Editor`: AssetBundle から VFX アセットをロードする際、Type Trees が無効で開発用プレーヤがビルドされているとクラッシュする問題を修正しました。
    ([uum-137538](https://issuetracker.unity3d.com/issues/crash-on-cachedreader-outofboundserror-when-loading-vfx-object-from-an-asset-bundle-with-disabletypetree))

- `エディター`: エディターでコンテンツファイルをロードしたりアンロードしたりする際のデッドロックの競合状態を修正しました。
    (UUM-137677)

- `エディター`: ボリュームプロファイルの一貫性のないハッシュコード生成を修正。
    ([UUM-130711](https://issuetracker.unity3d.com/issues/switching-graphics-default-or-devlook-profile-to-nightskyrenderingsettings-profile-throws-keynotfoundexception-error-in-the-console-window))

- `Editor`: InvalidOperationExceptionを修正：エディターでビットマップテキストを使用する際に発生する `InvalidOperationException: EnsureRunningOnMainThread` を修正しました。
    ([uum-137062](https://issuetracker.unity3d.com/issues/invalidoperationexception-ensurerunningonmainthread-can-only-be-called-from-the-main-thread-is-randomly-thrown-in-the-console-when-working-in-a-urp-project-on-a-non-4k-screen-with-the-editor-default-text-rendering-mode-set-to-bitmap))

- `エディター`: グラフィックデバイスの初期化でネイティブプラグインを再び参照できるように、スタートアップ時間の最適化を元に戻しました。
    ([uum-134389](https://issuetracker.unity3d.com/issues/package-manager-vulkan-native-rendering-plugin-can-no-longer-intercept-vulkan-initialization-as-it-is-loaded-later-when-added-via-package-manager))

- `エディター`: 特定の ScriptableObject アセット名によって、Build Profiles ウィンドウを開いたときに警告が発生することがなくなりました。
    ([uum-135389](https://issuetracker.unity3d.com/issues/scriptableobject-asset-is-accessed-during-the-lookup-of-build-profiles-when-opening-the-build-profiles-window))

- `エディター`: vsync がオンでない場合に、cpuactetime から waitfromlastpresentation 時間を抽象化。
    (UUM-131842)

- `Editor`: \不正なGTKの使い方がコンソールでエラーを発生させるケースを修正。
    (UUM-138332)

- `GI`: シャドウキャスティング混合ライトとベイクドライトマップまたはライトプローブの両方を含むシーンが1つもない場合に、シャドウマスクまたは減算シェーダのバリアントが誤って取り除かれるバグを修正しました。
    ([uum-127288](https://issuetracker.unity3d.com/issues/baked-shadows-are-missing-when-loading-a-scene-additively-and-lighting-was-baked-in-2022-dot-3))

- `グラフィック`: LJT-01-003脆弱性の悪用によるサービス拒否を防ぐために、"ImageConversion "クラスによって使用されるJPEGデコーダーに予防策を追加しました。Unityは、1000回のプログレッシブスキャンをデコードした後、JPEGファイルのデコードを自動的に中断するようになりました。
    (UUM-129186)

- `Graphics`: (UUM-1291) `Graphics`: UAV上でシェーダー型ロード/ストアを行う際に、指定されたハード ウェア上でのフォーマットサポートをチェックするための SystemInfo.SupportsTypedUAVShaderLoadStoreOnGraphicsFormat(￤)を追加。DX11 と DX12 に適用可能。
    (UUM-101875)

- `Graphics`: Vulkan スワップチェーンが次の画像を取得する際にクラッシュする問題を修正。
    ([UUM-138508](https://issuetracker.unity3d.com/issues/crash-in-vk-onscreenswapchain-acquirenextimage))

- `Graphics`: Adreno デバイスで GPU スキニングを使用するとクラッシュする問題を修正しました。
    ([uum-93243](https://issuetracker.unity3d.com/issues/crash-on-apigles-clearbuffersubdata-when-running-the-player-a-second-time-on-meta-quest-2))

- `Graphics`: Vulkan Editorのスレッドセーフティエラーチェックの誤りを修正。
    ([uum-90240](https://issuetracker.unity3d.com/issues/databuffer-getcurrentresourcewriteable-error-is-thrown-in-custom-srp-when-using-vulkan-graphics-api))

- `Graphics`: Vulkan と GraphicsJobs を使用する際の mip ストリーミングに関する問題を修正しました。
    (UUM-137032)

- `Graphics`: Vulkan使用時の計算スキニングのアーティファクトやクラッシュを修正しました。
    ([UUM-135988](https://issuetracker.unity3d.com/issues/crash-on-vulkan-plus-mali-when-skinned-mesh-renderer-starts-enabled-off-screen-then-enabled-and-moved-on-screen))

- `Graphics`: 一部の Adreno Vulkan ドライバで未使用の頂点属性を持つシェーダを使用するとクラッシュする問題を修正しました。
    (UUM-137056)

- `Graphics`: MetalグラフィックスAPIを使用している場合に、STPアップスケーリングでダイナミック解像度を使用するとグラフィカルが破損する問題を修正しました。
    (UUM-136227)

- `Graphics`: Vulkan使用時に一部のAdreno 7xxドライババージョンで不正なUVを修正しました。
    ([UUM-126477](https://issuetracker.unity3d.com/issues/android-vulkan-the-uv-quad-is-displayed-incorrectly-with-vulkan-on-a-specific-device))

- `Graphics`: OpenGLで1bitアルファのDXT1テクスチャを使用する際にアルファチャンネルが欠落していたのを修正しました。
    ([uum-86650](https://issuetracker.unity3d.com/issues/opengl-alpha-channel-loss-in-dds-textures-when-viewing-them-with-opengl-selected-as-graphics-api))

- `Graphics`: OpenGLを使用して、リードバック矩形よりも幅の広いテクスチャにリードバックを行う場合のReadPixelsを修正しました。
    ([uum-121817](https://issuetracker.unity3d.com/issues/android-texture2d-dot-readpixels-writes-pixels-into-a-texture-incorrectly-when-used-with-opengles3))

- `Graphics`: 一部の古いAndroidデバイスでのアーティファクトを回避するため、可能な限りclear quadの代わりに`glClear`を使用するようにしました。
    ([uum-135708](https://issuetracker.unity3d.com/issues/visual-artifacts-appear-when-using-clip-method-in-custom-shader-and-running-on-gles))

- `HDRP`: DRS を有効にした Custom Pass ボリュームを検査する際の NullReferenceException を修正しました。
    ([uum-136075](https://issuetracker.unity3d.com/issues/errors-thrown-into-the-console-when-adding-certain-custom-passes-to-a-custom-pass-volume-component-if-dynamic-resolution-is-enabled))

- `IL2CPP`: libil2cpp コードの C++ 警告を修正。
    (UUM-138294)

- `IL2CPP`: 無効なコード生成の原因となる C++ ポインタエイリアスの問題を修正。
    ([UUM-132447](https://issuetracker.unity3d.com/issues/ios-stripping-issue-on-xcode-26-when-use-incremental-gc-is-disabled))

- `Linux`: ビルドして実行" で Linux Player が二度起動する問題を修正しました。
    ([uum-138018](https://issuetracker.unity3d.com/issues/build-and-run-on-ubuntu-opens-two-instances-of-the-player-at-once))

- `Linux`: SDK オブジェクトファイルが SSE2 を超える機能を使用した場合に発生する古い CPU でのクラッシュを修正しました。
    ([uum-137227](https://issuetracker.unity3d.com/issues/linux-crash-on-gl-projectpolygon-when-opening-the-editor-using-an-older-cpu))

- `Profiler`: 録画中にProfilerキャプチャをロードすると、ロードされたデータと処理が終了していないフレームが混ざってしまう問題を修正しました。
    ([uum-134269](https://issuetracker.unity3d.com/issues/load-profiler-capture-pop-up-window-appears-again-when-selecting-the-same-profiler-capture-for-the-second-time))

- `Profiler`: ProfilerのスクリーンショットがVulkan上で記録されない問題を修正しました。
    (UUM-126495)

- `シーン/ゲームビュー`: EditorToolContextの動作がシーン内の通常のGameObject選択を妨げていたのを修正。
    ([UUM-135908](https://issuetracker.unity3d.com/issues/unable-to-select-a-gameobject-in-scene-view-when-using-a-custom-editor-tool))

- `スクリプト`: ScriptingCoverage::FilterRecordedMethods にメインスレッドガードを追加し、スクリプトの再読み込み時のスレッドセーフを実現。
    ([uum-137724](https://issuetracker.unity3d.com/issues/crash-on-mono-jit-runtime-invoke-when-disabling-the-debug-mode-with-the-code-coverage-enabled))

- `シリアライズ`: ボックス化された構造体オブジェクトに対して `OnAfterDeserialize` を呼び出したときに、構造体フィールドを変更するとオブジェクトのメモリが破損する問題を修正しました。インターフェイスメソッドの呼び出し先は、ボックス化されたオブジェクトの構造体データを指すようになりました。
    ([uum-119163](https://issuetracker.unity3d.com/issues/crash-on-buffer-add-value-full-when-hovering-over-serializedproperty-dot-boxedvalue-in-debug-mode-after-iserializationcallbackreceiver-dot-onafterdeserialize-modifies-value))

- `SRP Core`: PlayerビルドでSRPシェーダーの `Awake()` や `Start()` 中に `Material.FindPass(...)` が -1 を返す問題を修正しました。
    ([uum-101568](https://issuetracker.unity3d.com/issues/material-dot-findpass-returns-1-in-build-when-shader-pass-is-used))

- `UIツールキット`: 新しい属性 `UxmlCreateInstanceMethod` を追加しました。UxmlElement`を使用する際に、デフォルトのコンストラクタの代わりにインスタンスを作成するメソッドを指定します。

- `UIツールキット`: ビルダー階層に検索機能を追加した。

- `UIツールキット`: ビルダーのスタイルシートに検索機能を追加した。

- `UI ツールキット`: Microsoft Basic Renderer の UITK GPU パフォーマンステストを無効化。
    (UUM-137559)

- `UIツールキット`: Antialiased Arc Encoding" SVGの9スライスを修正。
    ([UUM-133494](https://issuetracker.unity3d.com/issues/svg-with-antialiased-arc-encoding-and-slices-dont-behave-well))

- `UIツールキット`: Macのコーナーで、端に無効なピクセルが表示される問題を修正。
    (UUM-122540)

- `UIツールキット`: SVGグラデーションでのカバレッジ問題を修正。
    ([UUM-115304](https://issuetracker.unity3d.com/issues/gradient-draw-larger-when-a-custom-shader-is-used))

- `UIツールキット`: VectorImageインポートがビューポートを無視する問題を修正。
    ([uum-133924](https://issuetracker.unity3d.com/issues/svgs-imported-as-antialiased-arc-encodings-do-no-honor-the-svg-provided-viewport))

- `UIツールキット`: SVG VectorImageのビューポートオプションが公開されていなかったのを修正。
    ([uum-138244](https://issuetracker.unity3d.com/issues/viewport-options-are-not-exposed-in-the-inspector-when-svg-is-imported-as-ui-toolkit-vector-image))

- `UIツールキット`: 一部のTジャンクションに起因するピクセル欠落を修正。
    ([uum-121344](https://issuetracker.unity3d.com/issues/some-ui-toolkit-pixels-are-transparent-when-not-all-corners-are-rounded))

- `UI Toolkit`: UI Toolkit Test Framework：エディタテストフィクスチャの panelSize を標準化。
    (UUM-133472)

- `URP`: Color Space* が *Gamma* に設定されている場合に、on-tile PostPro が従来の PostPro と異なる結果になる問題を修正。
    (UUM-135686)

- `VFX Graph`: PrepareVFXRenderNodes でクラッシュしやすい競合状態を防止。
    (UUM-136687)

- `WebGL`: プロジェクトの最大メモリが2GBを超える場合のWebGPUエラーを修正。
    (UUM-139633)

- `WebGL`: WebGPUバインディングライブラリを更新し、全般的な改善とメモリの修正を行いました。
    (UUM-139098)

- `XR`: フレームバッファフェッチを使用してMSAAカメラカラーアタッチメントがコピーされた時に、誤ったリゾルブアタッチメントが選択されるのを修正。
    ([UUM-132450](https://issuetracker.unity3d.com/issues/the-view-renders-black-when-using-framebuffer-fetch-with-foveated-rendering-in-a-player-for-meta-quest))




## 6000.3.14f1 におけるパッケージの変更

## 更新されたパッケージ

- `com.unity.editorcoroutines`: [1.0.1](https://docs.unity3d.com/Packages/com.unity.editorcoroutines@1.0//changelog/CHANGELOG.html) から [1.1.0](https://docs.unity3d.com/Packages/com.unity.editorcoroutines@1.1//changelog/CHANGELOG.html) へ。

- `com.unity.recorder`: [5.1.5](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) から [5.1.6](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) に変更。

- `com.unity.services.leaderboards`: [2.3.3](https://docs.unity3d.com/Packages/com.unity.services.leaderboards@2.3//changelog/CHANGELOG.html) から [2.3.4](https://docs.unity3d.com/Packages/com.unity.services.leaderboards@2.3//changelog/CHANGELOG.html) に変更。

- `com.unity.microsoft.gdk`: [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html) から [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.6//changelog/CHANGELOG.html) に変更。

- `com.unity.microsoft.gdk.tools`: [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html) から [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.6//changelog/CHANGELOG.html) に変更。

- `com.unity.microsoft.gdk.discovery`: [1.2.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html) から [1.3.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.3//changelog/CHANGELOG.html) に変更。

- `com.unity.ai.inference`: [2.6.0](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.6//changelog/CHANGELOG.html)から[2.6.1](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.6//changelog/CHANGELOG.html)