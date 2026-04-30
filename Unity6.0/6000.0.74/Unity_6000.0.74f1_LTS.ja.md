# Unity 6000.0.74f1 LTS
公開日時: Wed, 29 Apr 2026 10:05:57 GMT
https://unity.com/releases/editor/whats-new/6000.0.74f1

# 6000.0.74f1 の既知の問題

- `6000.0.61f1`: SDF16 または SDF32 でフォントアトラスを生成すると tlsf_free でクラッシュする。
    ([uum-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true)とUseTextureでAddComputePassを使用するとD3D12SwapChain::Presentでクラッシュする。
    ([uum-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.5.0a4,6000.0.66f1,6000.3.4f1,6000.4.0b4`: ShaderVariantCollection.variantCountとShaderVariantCollection.shaderCountがBuildsで0を返す
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- `IL2CPP`: [iOS] [Android] IL2CPPのビルド中に外部ライブラリのジェネリックに失敗する
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- `メタル`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

List<T>構造体でネストされた[SerializeReference]フィールドを使用すると "core::base_hash_set "でクラッシュする
    ([uum-139722](https://issuetracker.unity3d.com/issues/crash-on-core-base-hash-set-when-using-nested-serializereference-fields-in-list-structures))

DX12使用時にシーンビューでGameObjectを選択するとCheckDeviceStatusでクラッシュする。
    ([uum-138597](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-selecting-gameobjects-in-the-scene-view-while-using-dx12))

空白のURPプロジェクトで再コンパイルする際のVisualElementにおけるエディタのメモリリーク
    ([uum-138000](https://issuetracker.unity3d.com/issues/editor-memory-leak-in-visualelement-when-recompiling-in-a-blank-urp-project))



# 6000.0.74f1 リリースノート

## 変更点

- `オーディオ`: メモリリークを回避するため、Chromium ベースのウェブブラウザで Compressed In Memory 設定のデフォルトを Decompress On Load に変更。
    ([uum-136929](https://issuetracker.unity3d.com/issues/detached-audio-source-is-not-released-from-browser-memory-when-audio-stops-playing-in-webgl-player))



## 修正

- `2D`: 2D レンダラーで Unity Recorder を使用するためのサポートを追加。
    (UUM-136415)

- `Android`: Android の Player Settings で Depth/Stencil buffer を無効にして URP を使用するとクラッシュする問題を修正。
    ([UUM-109005](https://issuetracker.unity3d.com/issues/android-player-crashes-on-vk-renderpasses-getpackedrenderpass-when-using-vulkan-graphics-api-in-a-specific-project))

- `Android`: Pixel 10 で、discard や clip を使用するシェーダーでアーティファクトが発生する問題を修正しました。
    (UUM-139019)

- オーディオ非 Chromium ウェブブラウザで Compressed In Memory 設定を使用した際のメモリリークを修正しました。
    ([UUM-136929](https://issuetracker.unity3d.com/issues/detached-audio-source-is-not-released-from-browser-memory-when-audio-stops-playing-in-webgl-player))

- `エディター`: ゲームのフレームレートがビデオのフレームレートよりかなり低い状態でビデオファイルを再生すると、無限フレームスキップループが発生するのを修正しました。
    ([uum-131279](https://issuetracker.unity3d.com/issues/video-framerate-is-not-restored-when-trying-to-raise-it-after-lowering-it-to-10-fps))

- `エディター`: EditorSettings.asset`のアップグレードに失敗したり、手動で元に戻したり変更した場合に、Enter Play ModeのDomain Reloadを無効にしてもDomain Reloadが発生する問題を修正しました。
    ([uum-138521](https://issuetracker.unity3d.com/issues/enterplaymodeoptions-doesnt-take-effect-if-user-manually-modifies-m-enterplaymodeoptionsenabled-to-0))

- `エディター`: EditorSettings.asset`のアップグレードに失敗したり、手動で元に戻したり修正した場合、Enter Play ModeのDomain Reloadが無効でもDomain Reloadが発生する問題を修正しました。
    ([uum-138521](https://issuetracker.unity3d.com/issues/enterplaymodeoptions-doesnt-take-effect-if-user-manually-modifies-m-enterplaymodeoptionsenabled-to-0))

- `エディター`: TextCoreでUnderlineを使用した場合に発生する範囲外の例外を修正しました。
    ([uum-137906](https://issuetracker.unity3d.com/issues/ui-builder-windows-text-rendering-breaks-when-using-rich-text-combined-with-an-underlined-emoji))

- `エディター`: 全てのNativeプラグインのユースケースをサポートするために、Vulkanエディター用のパッケージエンタイトルメントを早めにセットアップしました。
    ([uum-135157](https://issuetracker.unity3d.com/issues/vulkan-native-graphics-plugins-load-after-graphics-device-initialization-in-editor-when-placed-in-packages))

- `エディター`: ウイルス対策ソフトウェアが署名されていないバイナリを不審なものとしてフラグを立てることによる潜在的な問題を防ぐために、IL2CPP 関連のファイルに署名するようにしました。
    (UUM-137463)

- `エディター`: OpenGL ES で Mali GPU 上でステンシルオンリーフォーマットを使用した場合のクラッシュを回避。
    ([UUM-111344](https://issuetracker.unity3d.com/issues/android-crash-on-startup-when-depth-stencil-format-is-set-to-s8-uint))

- `GI`: 一つのシーンにシャドウキャスティング混合ライトとベイクドライトマップまたはライトプローブの両方が含まれていない場合に、シャドウマスクまたは減算シェーダのバリアントが誤って取り除かれるバグを修正しました。
    ([uum-127288](https://issuetracker.unity3d.com/issues/baked-shadows-are-missing-when-loading-a-scene-additively-and-lighting-was-baked-in-2022-dot-3))

- `グラフィック`: LJT-01-003脆弱性の悪用によるサービス拒否を防ぐために、"ImageConversion "クラスによって使用されるJPEGデコーダーに予防策を追加しました。Unityは、1000回のプログレッシブスキャンをデコードした後、JPEGファイルのデコードを自動的に中断するようになりました。
    (UUM-129186)

- `グラフィック`: Vulkan swapchain が次の画像を取得する際にクラッシュする問題を修正しました。
    ([UUM-138508](https://issuetracker.unity3d.com/issues/crash-in-vk-onscreenswapchain-acquirenextimage))

- `Graphics`: Vulkan Editorのスレッドセーフティエラーチェックの誤りを修正しました。
    ([uum-90240](https://issuetracker.unity3d.com/issues/databuffer-getcurrentresourcewriteable-error-is-thrown-in-custom-srp-when-using-vulkan-graphics-api))

- `Graphics`: DX12、Metal、およびレガシーVulkanデバイスでScalableBufferManagerを使用した場合に、MSAA CameraDepthTextureのリサイズに一貫性がない問題を修正しました。 スタンドアロンまたはAndroidプレーヤーをビルドした場合に、ベクトル型シェーダーの暗黙の切り捨て警告が投げられる問題を修正しました。
    ([uum-100367](https://issuetracker.unity3d.com/issues/android-ios-macos-inconsistent-cameradepthtexture-behavior-when-using-scalablebuffermanager-across-devices))

- `Graphics`: Vulkanを使用する際の計算スキニングのアーティファクトやクラッシュを修正しました。
    ([uum-135988](https://issuetracker.unity3d.com/issues/crash-on-vulkan-plus-mali-when-skinned-mesh-renderer-starts-enabled-off-screen-then-enabled-and-moved-on-screen))

- `Graphics`: Vulkan 使用時の Pixel 10 でのインスタンス化を修正。
    (UUM-139629)

- `Graphics`: OpenGLで1bitアルファのDXT1テクスチャを使用する際にアルファチャンネルが欠落していたのを修正。
    ([UUM-86650](https://issuetracker.unity3d.com/issues/opengl-alpha-channel-loss-in-dds-textures-when-viewing-them-with-opengl-selected-as-graphics-api))

- `Graphics`: OpenGLを使用して、リードバック矩形よりも幅の広いテクスチャにリードバックを行う場合のReadPixelsを修正しました。
    ([uum-121817](https://issuetracker.unity3d.com/issues/android-texture2d-dot-readpixels-writes-pixels-into-a-texture-incorrectly-when-used-with-opengles3))

- `Graphics`: サポートされていないグラフィックスAPIを使用している場合に、GraphicsStateCollection.Warmupがレガシーシェーダーのバリアント読み込みにフォールバックすることに関する、リリースビルドでの繰り返しのログメッセージを削除。
    (UUM-138841)

- `Graphics`: 一部の古い Android デバイスでのアーティファクトを避けるため、可能な限り clear quad の代わりに glClear を使用。
    ([UUM-135708](https://issuetracker.unity3d.com/issues/visual-artifacts-appear-when-using-clip-method-in-custom-shader-and-running-on-gles))

- `HDRP`: カスタムレンダーパスを追加した後のDLSS &amp; FSR2のブラックスクリーンを修正。
    ([uum-113720](https://issuetracker.unity3d.com/issues/shadowmappass-breaks-the-game-view-when-dlss-is-enabled))

- `HDRP`: 歪みのためのカラーピラミッド後の_ColorPyramidUvScaleAndLimitCurrentFrameのnull limit.xy値を修正。
    ([uum-130925](https://issuetracker.unity3d.com/issues/hdrp-liquid-sample-custom-injection-pass-breaks-transparency-and-refraction-when-set-to-before-post-process))

- `パッケージ`: RagdollWindowにリサイズ時のScrollViewサポートを追加。
    ([uum-139914](https://issuetracker.unity3d.com/issues/the-ragdoll-builder-window-has-no-scrollbar-making-elements-unreachable-unless-the-window-is-resized))

- `パッケージマネージャー`: パッケージキャッシュの場所を変更するとエディターログに "TLS Allocator ALLOC_TEMP_MAIN has unfreed allocations" エラーが繰り返し表示される問題を修正。
    ([uum-131286](https://issuetracker.unity3d.com/issues/tls-allocator-alloc-temp-tls-underlying-allocator-alloc-temp-main-has-unfreed-allocations-dot-dot-dot-error-when-changing-the-packages-cache-location-folder))

- `Particles`: ネストしたサブエミッターを持つ TrailModule::Update でのクラッシュを防止。
    ([uum-131142](https://issuetracker.unity3d.com/issues/crash-on-trailmodule-update-when-loading-particle-systems-with-trails-module-enabled-from-assetbundles))

- `Particles`: Birthスポーン条件でネストしたサブエミッターを使用した際のクラッシュを防止。
    ([uum-115382](https://issuetracker.unity3d.com/issues/unity-player-crashes-on-unityplayer-unitymain-and-an-access-violation-reading-location-error-in-particlesystem-emit-occurs-when-running-player-with-debugallocator-and-using-particle-systems-with-a-complex-hierarchical-structure))

- `シーン/ゲームビュー`: プレイモード中にPlayModeWindow.SetViewTypeを使用するとエディターがクラッシュするバグを修正。
    ([uum-139011](https://issuetracker.unity3d.com/issues/crash-on-repaintcontroller-renderplaymodeviewcameras-when-entering-play-mode-and-playmodewindow-dot-setviewtype-being-called-at-end-of-frame))

- `スクリプト`: ScriptingCoverage::FilterRecordedMethods にメインスレッドガードを追加し、スクリプトの再読み込み時のスレッドセーフを実現。
    ([uum-137724](https://issuetracker.unity3d.com/issues/crash-on-mono-jit-runtime-invoke-when-disabling-the-debug-mode-with-the-code-coverage-enabled))

- `URP`: URP DepthBlitのサンプルを修正し、必要でない場合に手動で深度を解決しないようにした。
    ([uum-134993](https://issuetracker.unity3d.com/issues/non-multisampled-texture-binding-errors-are-logged-when-running-the-depthblit-urp-scene-with-msaa-enabled-on-vulkan))

- `WebGL`: WebGPUとWebGLで地形詳細メッシュを使用する際に発生するレンダリングエラーを修正しました。
    ([uum-91734](https://issuetracker.unity3d.com/issues/webgl-player-fails-to-render-scene-when-terrain-with-detail-mesh-is-added-and-webgpu-graphics-api-is-used))

- `WebGL`: R16UNorm`、`R16SNorm`、`RG16UNorm`、`RG16SNorm`、`RGBA16UNorm`、`RGBA16SNorm` が誤ってフィルタ可能として宣言されていた問題を修正しました。
    ([uum-139873](https://issuetracker.unity3d.com/issues/r16unorm-texture-usage-fails-for-webgpu))

- `WebGL`: フルスクリーン状態を切り替えた時の WebGL コンソールの警告を修正しました。
    ([uum-139208](https://issuetracker.unity3d.com/issues/webgl-console-warnings-switching-fullscreen))




## 6000.0.74f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.editorcoroutines`: [1.0.0](https://docs.unity3d.com/Packages/com.unity.editorcoroutines@1.0//changelog/CHANGELOG.html) から [1.1.0](https://docs.unity3d.com/Packages/com.unity.editorcoroutines@1.1//changelog/CHANGELOG.html) へ。

- `com.unity.xr.arcore`: [6.0.6](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.0//changelog/CHANGELOG.html)から[6.0.7](https://docs.unity3d.com/Packages/com.unity.xr.arcore@6.0//changelog/CHANGELOG.html)

- `com.unity.xr.arfoundation`: [6.0.6](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.0//changelog/CHANGELOG.html)から[6.0.7](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.0//changelog/CHANGELOG.html)

- `com.unity.xr.arkit`: [6.0.6](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.0//changelog/CHANGELOG.html)から[6.0.7](https://docs.unity3d.com/Packages/com.unity.xr.arkit@6.0//changelog/CHANGELOG.html)

- `com.unity.xr.core-utils`: [2.5.3](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.5//changelog/CHANGELOG.html)から[2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.core-utils@2.6//changelog/CHANGELOG.html)

- `com.unity.dt.app-ui`: [1.3.5](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.3//changelog/CHANGELOG.html)から[1.3.6](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@1.3//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk`: [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html) から [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.6//changelog/CHANGELOG.html) に変更。

- `com.unity.microsoft.gdk.tools`: [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html) から [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.6//changelog/CHANGELOG.html) へ。

- `com.unity.microsoft.gdk.discovery`: [1.2.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html) から [1.3.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.3//changelog/CHANGELOG.html) に変更。

- `com.unity.ai.inference`: [2.5.0](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.5//changelog/CHANGELOG.html)から[2.6.1](https://docs.unity3d.com/Packages/com.unity.ai.inference@2.6//changelog/CHANGELOG.html)