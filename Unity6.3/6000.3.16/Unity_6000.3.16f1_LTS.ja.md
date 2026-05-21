# Unity 6000.3.16f1 LTS
公開日時: Wed, 20 May 2026 14:16:31 GMT
https://unity.com/releases/editor/whats-new/6000.3.16f1

# 6000.3.16f1 の既知の問題

- `6000.0.61f1`: SDF16 または SDF32 で Font Atlas を生成すると tlsf_free でクラッシュする。
    ([uum-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true)とUseTextureでAddComputePassを使用するとD3D12SwapChain::Presentでクラッシュする。
    ([uum-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.4.0a2,6000.3.0b6`: ATG経由でレンダリングされた<link>タグを持つUITKラベルをホバーすると、TextLib::FindIntersectingLinkでエディタがクラッシュする。
    ([uum-142829](https://issuetracker.unity3d.com/issues/editor-crashes-in-textlib-findintersectinglink-when-hovering-uitk-labels-with-tags-rendered-via-atg))

- `メタル`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- テキスト (TextMeshPro)：TMPro Font Asset CreatorでマルチスレッドのFont Atlasを生成するとUNITY_FT_Load_Glyphでクラッシュする
    ([uum-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

複数のbee_backendを実行している場合にmono_log_write_logfileでクラッシュする
    ([uum-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

DX12 Graphics API がグラフィック API リストの最初にあるのに使用されない
    ([uum-141555](https://issuetracker.unity3d.com/issues/dx12-graphics-api-is-not-used-when-it-is-first-in-the-graphics-api-list))

サブシーンが開いているプレファブモードで子 GameObject を無効にすると、プレファブ内の他の GameObject にマテリアルが移動する
    ([uum-139663](https://issuetracker.unity3d.com/issues/materials-move-to-other-gameobjects-in-a-prefab-when-disabling-a-child-gameobject-in-prefab-mode-with-an-open-subscene))



# 6000.3.16f1 リリースノート

## 改良点

- `Graphics`: GfxDeviceGLES::DrawBuffersBatchModeにNULLインデックスバッファに対するガードを追加。
    (UUM-135891)



## APIの変更

- `UIツールキット`: 追加: `CallbackOptions` 引数を持つ `CallbackEventHandler.RegisterCallbacks` メソッドのオーバーライドを追加した。

- `UIツールキット`: 追加: `CallbackEventHandler.UnregisterAllRemovableCallbacks` メソッドを追加した。

- `UIツールキット`: 追加: `CallbackOptions` 列挙型を追加した。



## 変更点

- `Android`: JDK を 17.0.18+8 に更新。
    (UUM-141159)



## 修正

- `2D`: Hidden/Light2D のシェーダーの警告を修正。
    ([uum-134522](https://issuetracker.unity3d.com/issues/shader-warning-in-hidden-slash-light2d-implicit-truncation-of-vector-type-is-thrown-when-building-universal-2d-template))

- `2D`: 編集モードのシーンビューでタイルパレットオーバーレイが開いている時に、プレイモードでタイルを選択すると例外が発生するのを修正。
    ([uum-137165](https://issuetracker.unity3d.com/issues/invalidoperationexception-and-nullreferenceexception-errors-are-thrown-when-clicking-inside-a-tile-palette-with-the-tile-palette-overlay-and-tile-palette-edit-enabled))

- `2D`: スプライトエディタ(Sprite Editor)ウィンドウで、インポートされたテクスチャがソーステクスチャより小さい場合にプレビュートグルを使用すると例外が発生するのを修正しました。
    ([uum-134129](https://issuetracker.unity3d.com/issues/sprite-editor-argumentexception-error-when-scene-view-preview-option-is-used-on-psb-format-files))

- `2D`: スプライトエディタウィンドウのプレビュートグルを使用してプレイモードに入った後、スプライトレンダラーのスプライト参照が元に戻らない問題を修正しました。スプライトエディターウィンドウのプレビュートグルは、編集モードでのみ使用できるようになりました。
    ([uum-134128](https://issuetracker.unity3d.com/issues/sprite-does-not-revert-to-original-texture-when-entering-play-mode-with-scene-view-preview-enabled-in-the-sprite-editor-window))

- `2D`: ユーザーがタイルパレット用のスプライトアセットをドラッグ＆ドロップし、タイルアセットを作成する操作をキャンセルすると、タイルパレットに空のグリッドが表示される問題を修正しました。
    ([uum-132388](https://issuetracker.unity3d.com/issues/tile-palette-texture-drag-area-label-drag-tile-sprite-or-texture-sprite-type-asset-slash-s-here-dot-disappears-when-the-asset-save-pop-up-is-closed-slash-canceled))

- `2D`: 2Dシャドウのボリューム強度に関する問題を修正しました。
    ([uum-136056](https://issuetracker.unity3d.com/issues/shadows-from-light2d-do-not-change-when-volumetric-shadow-strength-is-toggled-off))

- `2D`: Tilemapのタイル・アンカーがデフォルトのセル・センターと異なる場合に、コライダー・タイプのグリッドを持つタイルが正しく並ばない問題を修正しました。
    (UUM-136995)

- `Android`: フルスクリーンのユースケースをカバーするために、RunInBackgroundのテストを追加。

- `Android`: アプリが中断されたときに MediaPlayer が一時停止する問題を修正。
    (UUM-140840)

- `Android`: SeekTimeOnResumeVideo テストの不安定性を修正。
    (UUM-140837)

- `Android`: Unity as a Library ︙(UAAL)シナリオでApplication.UnloadまたはReload中に送信されたUnitySendMessageコールがAndroid上でドロップされる問題を修正しました。
    (UUM-141440)

- `Android`: Run without focus "を有効(enabled)に切り替えると、Unityから起動されたAndroidアクティビティを含む、別のアクティビティが起動されたときにUnityアクティビティが実行され続けるようになりました。
    ([UUM-120304](https://issuetracker.unity3d.com/issues/android-unityplayer-gets-paused-when-another-activity-is-launched-even-with-run-without-focus-enabled))

- `アニメーション`: 何も選択されていない時に表示される "Animation Clip is Read-Only" メッセージを修正。
    ([uum-139142](https://issuetracker.unity3d.com/issues/animation-clip-is-read-only-is-shown-in-the-animation-window-when-nothing-is-selected))

- `オーディオ`: AudioTrack を含むタイムラインが AssetBundle からロードされ、オーディオクリップが FMOD チャンネルの割り当てに失敗した場合、プレイモードに入るとクラッシュする問題を修正。
    ([uum-136551](https://issuetracker.unity3d.com/issues/crash-on-soundchannelinstance-setdelay-when-loading-an-assetbundle-containing-a-timeline-with-an-audioclip-at-scene-startup))

- `ビルドパイプライン`: ビルドパイプライン：Rider IDE で実行中にソースジェネレータが実行されていないことを確認。
    (UUM-133605)

- `ビルド・パイプライン`: ILPP.Trigger の待機ロジックを修正し、unity ログの "The pipe is being closed" 例外を防止。
    (UUM-136791)

- `ビルドシステム`: 特定のビルドパスを使用すると、ビルド中にノードGUIDの重複エラーが発生する問題を修正しました。
    ([UUM-128491](https://issuetracker.unity3d.com/issues/build-fails-with-duplicate-node-guids-error-when-using-specific-build-path))

- `ドキュメント`: ユーザーマニュアルへのFlare Layerヘルプリンクを修正しました。
    ([uum-134470](https://issuetracker.unity3d.com/issues/the-help-icon-of-flare-layer-component-refers-to-a-missing-unity-documentation-page-when-clicked))

- `DX12`: 特定のハードウェアで、D3D12がプロジェクトのグラフィックスAPIリストに含まれていなくても、起動時にD3D12の初期化コードが実行されるクラッシュを修正しました。
    ([uum-137629](https://issuetracker.unity3d.com/issues/unity-player-loads-d3d12-dll-even-when-direct3d12-is-removed-from-project-settings))

- `エディタ`: リモートビルドが指定されているにもかかわらず、ローカルで無効なアーキテクチャの場合、Build and Runボタンがグレーアウトする不具合を修正しました。
    ([uum-138399](https://issuetracker.unity3d.com/issues/build-and-run-button-greyed-out-for-locally-invalid-architecture-despite-remote-build-is-specified))

- `Editor`: macOS上で-projectPathコマンドライン引数を指定してエディターを起動するとUnity Hubが開いてしまうバグを修正しました。
    ([uum-136928](https://issuetracker.unity3d.com/issues/unity-hub-opens-when-launching-the-editor-with-projectpath-argument))

- `エディター`: BoxColliderと凸MeshColliderが中心で重なっている時にcomputePenetrationを呼び出すとクラッシュする問題を修正しました。
    ([uum-100359](https://issuetracker.unity3d.com/issues/meshcollider-does-not-detect-collisions-with-capsules-and-charactercontroller-when-using-physics-dot-computepenetration))

- `Editor`: Forward+ が有効で、Keep Lighting Variants が無効の状態で Custom Lighting ShaderGraph マテリアルをレンダリングするとクラッシュする問題を修正。
    ([uum-137255](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-rendering-custom-lighting-shadergraph-material-while-forward-plus-is-enabled-and-keep-lighting-variants-is-disabled))

- `エディター`: UnityEngine.Object` 型を受け付けるフィールド(Preloaded Assets リストのエントリなど)でオブジェクトピッカーを開くと `ArgumentException` 例外が発生する問題を修正しました。
    ([uum-135060](https://issuetracker.unity3d.com/issues/argumentexception-no-valid-types-in-required-type-list-error-is-thrown-when-opening-an-object-picker-menu-in-the-preloaded-assets-in-player-settings))

- `エディター`: CapsuleCollider と convex MeshCollider 間の ComputePenetration 呼び出しの信頼性が向上しました。ComputePenetration は距離がゼロの時に真を返します。
    ([uum-100359](https://issuetracker.unity3d.com/issues/meshcollider-does-not-detect-collisions-with-capsules-and-charactercontroller-when-using-physics-dot-computepenetration))

- `エディター`: CharacterControllerと凸MeshCollider間のComputePenetration呼び出しの信頼性を向上。距離がゼロの場合、ComputePenetrationはtrueを返します。
    ([uum-100359](https://issuetracker.unity3d.com/issues/meshcollider-does-not-detect-collisions-with-capsules-and-charactercontroller-when-using-physics-dot-computepenetration))

- `エディタ`: メモリーレスのRenderGraphレンダーターゲットをFrameDebuggerで表示できるようになりました。
    ([uum-133585](https://issuetracker.unity3d.com/issues/draw-gbuffer-pass-appears-black-in-frame-debugger-when-deferred-or-deferred-plus-is-enabled))

- `Editor`: 全てのNativeプラグインのユースケースをサポートするために、Vulkanエディター用のパッケージエンタイトルメントをより早くセットアップしました。
    ([uum-135157](https://issuetracker.unity3d.com/issues/vulkan-native-graphics-plugins-load-after-graphics-device-initialization-in-editor-when-placed-in-packages))

- `Graphics`: V-Sync が有効な場合に Windows 上で発生する Vulkan フレームタイムのスタッタリングを修正しました。
    (UUM-140217)

- `iOS`: バックバッファへのレンダリングでフレームキャプチャが動作しないのを修正。
    ([UUM-141280](https://issuetracker.unity3d.com/issues/ios-frame-debugger-rendering-output-doesnt-work-with-ios-builds))

- `iOS`: UISceneライフサイクルイベントのさらなる改善 - ユニバーサルなディープリンク処理。
    (UUM-140746)

- `ネットワーキング`: パッケージマネージャからアセットストアからアセットをダウンロードしようとするとTLSハンドシェイクエラーになるMbedTLSのリグレッションを修正しました。他の HTTPS エンドポイントもこのリグレッションの影響を受ける可能性がありました。
    (UUM-141298)

- `ネットワーキング`: 複数の自動プロキシをサポートすることで UUM-135025 を修正しました。
    ([uum-135025](https://issuetracker.unity3d.com/issues/unitywebrequest-returns-curl-error-5-instead-of-timing-out-when-the-windows-proxy-auto-config-script-returns-multiple-proxies))

- `物理 2D`: ([uum-139048](https://issuetracker.unity3d.com/issues/physicscomposer-dot-createchaingeometry-is-returning-stale-vertex-geometry))

- `物理 2D`: (uum-139044]())：3頂点ChainGeometry(triangle)の作成が許可されていなかった問題を修正しました。
    ([uum-139044](https://issuetracker.unity3d.com/issues/chaingeometry-does-not-allow-3-vertex-buffers-even-when-using-isloop-equals-true))

- `物理 2D`: ([uum-139044]()) `Physics 2D`: 非推奨の "ContactFilter2D.NoFilter\(˶‾᷄ -̫ ᷅˵) "インスタンスメソッドが、呼び出された `ContactFilter2D` のインスタンスを正しく修正するようになりました。しかし、このメソッドはまだ非推奨です。
    ([uum-139052](https://issuetracker.unity3d.com/issues/deprecated-contactfilter2d-dot-nofilter-method-should-assign-the-filter-to-the-instance))

- `プラグイン`: Linux 用のネイティブプラグインが CPU アーキテクチャを指定できない問題を修正しました。
    ([uum-131765](https://issuetracker.unity3d.com/issues/native-plugins-experience-name-conflicts-when-built-for-both-x86-linux-and-arm64-linux))

- `プロファイラ`: Profiler Hierarchy Calls テーブルの None テキストのレンダリングを修正しました。
    ([uum-114430](https://issuetracker.unity3d.com/issues/module-details-pane-window-and-text-is-too-dark-when-editor-theme-is-set-to-light))

- `スクリプト`: コンテナの整数オーバーフローのクラッシュを修正。
    ([uum-134628](https://issuetracker.unity3d.com/issues/crash-on-memcpy-when-opening-a-scene-with-specific-assets))

- `シェーダー`: プレイヤービルドで `ShaderCount` と `variantCount` にアクセスすると `ShaderVariantCollection` が 0 を返すのを修正。
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- `テキスト`: NoBR` タグを `SpriteAsset` と一緒に使用した場合の問題を修正しました。
    (UUM-139609)

- `UIツールキット`: Painter2D.fillGradientを使用してVisualElementでPlayerを構築したりシーンを切り替えたりするときに記録されるエラー "Attempted to release an invalid texture \(index=-1). "を修正しました。
    ([uum-140738](https://issuetracker.unity3d.com/issues/ui-builder-window-throws-an-attempted-to-release-an-invalid-texture-index-equals-1-dot-error-when-building-a-project-after-changing-gradient-settings-of-a-visualelement))

- `UI ツールキット`: UI Builder で、テンプレートに同名の要素がある場合に発生する無効なキャスト例外を修正しました。
    ([uum-140739](https://issuetracker.unity3d.com/issues/invalid-cast-exception-in-ui-builder-when-template-has-element-with-same-name))

- `UIツールキット`: RenderSpriteToTexture2Dが利用可能な場合、ローカルパッケージシェーダーを使用するように修正。
    ([uum-140566](https://issuetracker.unity3d.com/issues/svg-shaders-get-stripped-when-building-player))

- `UIツールキット`: UI Toolkit シェーダで BaseColor のような接続されていないスロット値が変更された場合に、シェーダグラフのメインプレビューが更新されない問題を修正しました。
    ([uum-138534](https://issuetracker.unity3d.com/issues/shader-graph-main-preview-color-is-not-updated-when-modifying-the-base-color-node-in-ui-shader-graph))

- `アンドゥシステム`: オブジェクトトラッキングを通知する前に、REDOでNULLコンポーネントをクリアするようにしました。
    ([uum-135948](https://issuetracker.unity3d.com/issues/crash-on-objecttotypedispatchdatahandle-when-redoing-canvas-creation-in-a-specific-project))

- `URP`: スクリプタブル・レンダラー機能を追加または削除した際に、プロジェクト・ウィンドウの変更が更新されない問題を修正しました。
    ([uum-139513](https://issuetracker.unity3d.com/issues/urp-asset-sub-assets-show-changes-in-sub-assets-only-after-reimporting-the-urp-asset-manually))

- `URP`: カメラが中間テクスチャにレンダリングする際、ポストプロセスパスのビューポートのスケーリングが後続のカスタムパスの存在を考慮していなかった問題を修正しました。
    ([uum-109492](https://issuetracker.unity3d.com/issues/urp-camera-output-texture-has-wrong-scale-when-using-bilinear-upscale-filter-and-when-renderfeature-requires-intermediate-texture))

- `VFX Graph`: VisualEffectAsset の依存関係の予期せぬ巨大なリストを修正。
    ([uum-140725](https://issuetracker.unity3d.com/issues/editorutility-dot-collectdependencies-returns-non-dependent-assets-when-checking-visual-effects-assets))




## 6000.3.16f1 におけるパッケージの変更

## 更新されたパッケージ

- `com.unity.collections`: [2.6.5](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) から [2.6.6](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) へ。

- `com.unity.entities`: [1.4.5](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) から [1.4.6](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html)

- `com.unity.physics`: [1.4.5](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) から [1.4.6](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: [1.4.18](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) から [1.4.19](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) へ。

- `com.unity.2d.animation`: [13.0.4](https://docs.unity3d.com/Packages/com.unity.2d.animation@13.0//changelog/CHANGELOG.html) から [13.0.5](https://docs.unity3d.com/Packages/com.unity.2d.animation@13.0//changelog/CHANGELOG.html)

- `com.unity.2d.common`: [12.0.2](https://docs.unity3d.com/Packages/com.unity.2d.common@12.0//changelog/CHANGELOG.html) から [12.0.3](https://docs.unity3d.com/Packages/com.unity.2d.common@12.0//changelog/CHANGELOG.html) に変更。

- `com.unity.2d.psdimporter`: [12.0.1](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@12.0//changelog/CHANGELOG.html) から [12.0.2](https://docs.unity3d.com/Packages/com.unity.2d.psdimporter@12.0//changelog/CHANGELOG.html) に変更。

- `com.unity.2d.tilemap.extras`: [6.0.1](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@6.0//changelog/CHANGELOG.html) から [6.0.2](https://docs.unity3d.com/Packages/com.unity.2d.tilemap.extras@6.0//changelog/CHANGELOG.html) に変更。

- `com.unity.2d.aseprite`: [3.0.1](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@3.0//changelog/CHANGELOG.html) から [3.0.2](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@3.0//changelog/CHANGELOG.html) に変更。

- `com.unity.2d.tooling`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.2d.tooling@1.0//changelog/CHANGELOG.html) から [1.0.3](https://docs.unity3d.com/Packages/com.unity.2d.tooling@1.0//changelog/CHANGELOG.html) に変更。

- `com.unity.ide.rider`: [3.0.39](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html) -> [3.0.40](https://docs.unity3d.com/Packages/com.unity.ide.rider@3.0//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.3.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) から [1.3.4](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) に変更。

- `com.unity.services.cloud-build`: [2.0.7](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.0//changelog/CHANGELOG.html) から [2.0.8](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.0//changelog/CHANGELOG.html) に変更。

- `com.unity.transport`: [2.7.2](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html) から [2.7.3](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html) に変更。

- `com.unity.netcode.gameobjects`: [2.11.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.11//changelog/CHANGELOG.html) から [2.11.2](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.11//changelog/CHANGELOG.html) へ。

- `com.unity.toolchain.win-x86_64-linux`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.toolchain.win-x86_64-linux@1.0//changelog/CHANGELOG.html) から [1.1.0](https://docs.unity3d.com/Packages/com.unity.toolchain.win-x86_64-linux@1.1//changelog/CHANGELOG.html) へ。

- `com.unity.toolchain.win-arm64-linux`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.toolchain.win-arm64-linux@1.0//changelog/CHANGELOG.html)から[1.1.0](https://docs.unity3d.com/Packages/com.unity.toolchain.win-arm64-linux@1.1//changelog/CHANGELOG.html)

- `com.unity.toolchain.macos-x86_64-linux`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-x86_64-linux@1.0//changelog/CHANGELOG.html)から[1.1.0](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-x86_64-linux@1.1//changelog/CHANGELOG.html)

- `com.unity.toolchain.macos-arm64-linux`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-arm64-linux@1.0//changelog/CHANGELOG.html)から[1.1.0](https://docs.unity3d.com/Packages/com.unity.toolchain.macos-arm64-linux@1.1//changelog/CHANGELOG.html)

- `com.unity.toolchain.linux-x86_64-linux`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.toolchain.linux-x86_64-linux@1.0//changelog/CHANGELOG.html)から[1.1.0](https://docs.unity3d.com/Packages/com.unity.toolchain.linux-x86_64-linux@1.1//changelog/CHANGELOG.html)

- `com.unity.sysroot.base`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.sysroot.base@1.0//changelog/CHANGELOG.html) から [1.1.0](https://docs.unity3d.com/Packages/com.unity.sysroot.base@1.1//changelog/CHANGELOG.html) に変更。

- `com.unity.sdk.linux-x86_64`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.sdk.linux-x86_64@1.0//changelog/CHANGELOG.html) から [1.1.0](https://docs.unity3d.com/Packages/com.unity.sdk.linux-x86_64@1.1//changelog/CHANGELOG.html) に変更。

- `com.unity.sdk.linux-arm64`: [1.0.2](https://docs.unity3d.com/Packages/com.unity.sdk.linux-arm64@1.0//changelog/CHANGELOG.html)から[1.1.0](https://docs.unity3d.com/Packages/com.unity.sdk.linux-arm64@1.1//changelog/CHANGELOG.html)