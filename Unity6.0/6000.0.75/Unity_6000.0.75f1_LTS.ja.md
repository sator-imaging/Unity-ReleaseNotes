# Unity 6000.0.75f1 LTS
公開日時：Wed, 13 May 2026 14:51:23 GMT
https://unity.com/releases/editor/whats-new/6000.0.75f1

# 6000.0.75f1 の既知の問題

- `6000.0.61f1`: SDF16 または SDF32 でフォントアトラスを生成すると tlsf_free でクラッシュする。
    ([uum-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true)とUseTextureでAddComputePassを使用するとD3D12SwapChain::Presentでクラッシュする。
    ([uum-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `メタル`: コマンドバッファタイムアウトエラーの後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))



# 6000.0.75f1 リリースノート

## 改良点

- `AI`: NavMeshHit 構造体および関連する概念の API ドキュメントに情報が不足していました。
    (UUM-140847)

- `ビルドシステム`: 同梱の 7-Zip をバージョン 26.01 に更新。

- `エディター`: Canvasコンポーネントで、OverlayモードでNormalまたはTangentが有効な場合の警告を削除。
    ([uum-137367](https://issuetracker.unity3d.com/issues/additional-shader-channel-keeps-reverting-when-saving-prefab))



## API の変更

- `エディタ`: 追加: 新しいパブリック DeeplinkHandlerAttribute を追加しました。



## 修正

- `2D`: Hidden/Light2D のシェーダーの警告を修正。
    ([uum-134522](https://issuetracker.unity3d.com/issues/shader-warning-in-hidden-slash-light2d-implicit-truncation-of-vector-type-is-thrown-when-building-universal-2d-template))

- `2D`: 2Dシャドウのボリューム強度に関する問題を修正。
    ([uum-136056](https://issuetracker.unity3d.com/issues/shadows-from-light2d-do-not-change-when-volumetric-shadow-strength-is-toggled-off))

- `2D`: Tilemapのタイル・アンカーがデフォルトのセル・センターと異なる場合に、コライダー・タイプのグリッドを持つタイルが正しく並ばない問題を修正しました。
    (UUM-136995)

- `2D`: URP 2D を使用しているときに、プレビュー・カメラに欠けていたライティングとシャドウを修正しました。
    (UUM-139229)

- `アクセシビリティ`: ノードIDが`int.MaxValue`に達した時に`AccessibilityHierarchy`が例外をスローし、最大ID値にラップした後に重複したIDでアクセシビリティノードが作成されるのを修正。
    ([uum-137871](https://issuetracker.unity3d.com/issues/accessibilityhierarchy-throws-an-exception-when-node-id-reaches-int-dot-maxvalue))

- `Android`: コントローラーが軸イベントではなくボタンイベントとしてL2/R2を報告する場合、Android上でSwitch Proゲームパッドのトリガーが機能しないのを修正しました。
    (UUM-139567)

- `オーディオ`: AudioTrack を含むタイムラインが AssetBundle からロードされ、オーディオクリップが FMOD チャンネルの割り当てに失敗した場合、Play Mode に入るとクラッシュする問題を修正。
    ([UUM-136551](https://issuetracker.unity3d.com/issues/crash-on-soundchannelinstance-setdelay-when-loading-an-assetbundle-containing-a-timeline-with-an-audioclip-at-scene-startup))

- `ビルドシステム`: プリビルド・コールバック中にアセンブリを含むフォルダが削除されると、起動時にプレーヤーがクラッシュする問題を修正しました。
    ([uum-137492](https://issuetracker.unity3d.com/issues/player-crashes-upon-launch-when-a-folder-is-deleted-as-a-prebuild-step))

- `DX12`: 大きなシーンでの D3D12 フェンスの遅いメモリリークを修正。
    (UUM-140429)

- エディター(Editor`): 2D: スプライトアトラス V2 パッキングが有効な状態で、"SpriteAtlasManager.atlasRequested "による Addressables SpriteAtlas ローディングを使用した場合に、エディターのプレイモードで SpriteSkin を持つスプライトが不可視になるケースを修正しました。
    (UUM-137123)

- `エディター`: レイアウトと置換テーブルがドメインのリロードの間にリークするのを修正。
    ([UUM-138000](https://issuetracker.unity3d.com/issues/editor-memory-leak-in-visualelement-when-recompiling-in-a-blank-urp-project))

- `Graphics`: 複数のピクセル密度を持つマルチモニター環境で Virtual Texturing Profiler モジュールのヘルプボタンのスケーリングを修正。
    ([uum-137763](https://issuetracker.unity3d.com/issues/virtual-texturing-documentation-button-is-oversized-and-not-consistent-with-other-editor-documentation-buttons-when-virtual-texturing-module-is-selected-in-the-profiler-window))

- `Graphics`: ユニフォームバッファバインディングに無効なバインディングスロットが渡された場合の OpenGLES のクラッシュを修正しました。
    (UUM-138897)

- `Graphics`: Streaming Controllerコンポーネントのドキュメントへのリンクを修正しました。
    ([UUM-139928](https://issuetracker.unity3d.com/issues/missing-documentation-page-opens-when-clicking-open-reference-button-on-streaming-controller-component))

- `Graphics`: Virtual Texturing Profiler モジュールのドキュメントへのリンクを修正。
    ([uum-137763](https://issuetracker.unity3d.com/issues/virtual-texturing-documentation-button-is-oversized-and-not-consistent-with-other-editor-documentation-buttons-when-virtual-texturing-module-is-selected-in-the-profiler-window))

- `Graphics`: \RenderTexture`に深度解決またはコンピュートシェーダが書き込まれた後に、不正確な`DontCare`ロードアクションが適用され、アーティファクトが表示される問題を修正しました。
    (UUM-46565)

- `HDRP`: HDRP SSGIがスクリーンの片側から反対側に色をにじませるバグを修正しました。
    ([UUM-139120](https://issuetracker.unity3d.com/issues/lighting-leaks-from-right-and-top-edges-to-left-and-bottom-edges-when-screen-space-global-illumination-uses-ray-tracing-in-hdrp))

- `iOS`: GameCenterから実績を複数回ロードするとクラッシュするバグを修正。
    (UUM-138417)

- `iOS`: UISceneのライフサイクルイベントのさらなる改善 - ユニバーサルなディープリンクの処理、Awake(≖)で見逃さないようにAbsoluteURLのセットを早めに移動。
    (UUM-140746)

- `カーネル`: ジョブシステムがファイナライザからアクセスされた場合のシャットダウン中のクラッシュを修正しました。
    ([UUM-128777](https://issuetracker.unity3d.com/issues/crash-on-jobqueue-hasjobgroupidcompleted-when-closing-the-editor-while-in-play-mode-on-a-specific-project))

- `ネットワーキング`: LinuxプレーヤのビルドでMonoの設定ファイルが欠落していて、特定の.NETネットワーキングAPIを使おうとすると例外が発生する問題を修正しました。
    ([uum-135731](https://issuetracker.unity3d.com/issues/webrequest-dot-create-function-fails-with-uri-prefix-is-not-recognized-errors-when-the-project-is-built-for-linux-standalone-or-windows-dedicated-server))

- `ネットワーキング`: パッケージマネージャからアセットストアからアセットをダウンロードしようとするとTLSハンドシェイクエラーになるMbedTLSのリグレッションを修正しました。潜在的に他の HTTPS エンドポイントもこのリグレッションの影響を受ける可能性がありました。
    (UUM-141298)

- `ネットワーキング`: MbedTLSをバージョン3.6.6に更新して、いくつかの(マイナーでおそらく爆発不可能な) セキュリティ脆弱性に対処しました。
    (UUM-140908)

- `物理`: Incremental Static Broadphase" の値が物理 sdk に送られない問題を修正。
    (UUM-141093)

- `スクリプト`: コンテナの整数オーバーフローのクラッシュを修正しました。
    ([UUM-134628](https://issuetracker.unity3d.com/issues/crash-on-memcpy-when-opening-a-scene-with-specific-assets))

- `シェーダー`: プレイヤービルドで `ShaderCount` と `variantCount` にアクセスすると `ShaderVariantCollection` が 0 を返すのを修正。
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- `uGUI`: OnValidate イベントでスクリプトを使用して入力フィールドのフォーカスを変更すると nullReferenceException が発生する問題を修正しました。
    ([uum-132637](https://issuetracker.unity3d.com/issues/nullreferenceexception-error-is-thrown-when-changing-input-field-focus-via-script-with-custom-validation))

- `uGUI`: Tabキーでフォーカスを移動したとき、InputFieldがハングル文字の最後の文字を取得できない問題を修正しました。
    ([uum-126213](https://issuetracker.unity3d.com/issues/inputfield-fails-to-get-the-last-character-of-a-hangul-ime-korean-character-text-when-focus-is-shifted-with-the-tab-key))

- `ビデオ`: WindowsベースのプラットフォームでSegmented MP4ファイルを開く際に、このメディアタイプがサポートされていないためConsoleの警告を表示するようにした。
    ([uum-132004](https://issuetracker.unity3d.com/issues/video-player-does-not-throw-an-error-when-playing-a-video-with-unsupported-encoding-settings))

- `WebGL`: \WebGPU] モバイルデバイスでWebCamの映像が正しく表示されるようにしました。
    ([uum-139017](https://issuetracker.unity3d.com/issues/ios-web-webgpu-webcamtextures-camera-orientation-is-fixed-relative-to-the-phones-right-edge))

- `XR`: レンズフレアの位置がビュー間で同じになり、視覚的なアーティファクトが発生するバグを修正。
    ([uum-108851](https://issuetracker.unity3d.com/issues/lens-flare-vfx-is-duplicated-when-observed-through-a-vr-headset))

- `XR`: URPでマルチパスXRレンダリングモードを使用する際、内蔵シェーダー定数unity_StereoEyeIndexが適切に設定されず、Skybox/Panoramicのようなシェーダーに影響し、3D Layoutオプションを使用しても立体視表示に失敗する不具合を修正しました。
    ([uum-120719](https://issuetracker.unity3d.com/issues/stereoscopic-skybox-renders-as-monoscopic-when-using-multi-pass-render-mode-in-xr-plugin-while-using-urp))




## 6000.0.75f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.netcode`: [1.11.0](https://docs.unity3d.com/Packages/com.unity.netcode@1.11//changelog/CHANGELOG.html) から [1.13.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html) へ。

- `com.unity.performance.profile-analyzer`: [1.3.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) から [1.3.4](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) に変更。

- `com.unity.services.user-reporting`: [2.0.14](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html) から [2.0.15](https://docs.unity3d.com/Packages/com.unity.services.user-reporting@2.0//changelog/CHANGELOG.html) へ。

- `com.unity.asset-manager-for-unity`: [1.10.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.10//changelog/CHANGELOG.html) から [1.11.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.11//changelog/CHANGELOG.html) に変更。