# Unity 6000.0.77f1 LTS
公開日時: 2026年6月10日(水) 09:18:20 GMT  
https://unity.com/releases/editor/whats-new/6000.0.77f1

# 6000.0.77f1 の既知の問題

- `6000.0.61f1`: SDF16 または SDF32 を使用してフォントアトラスを生成する際、tlsf_free でクラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true) および UseTexture を指定して AddComputePass を使用する際、D3D12SwapChain::Present でクラッシュする
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `アセットインポーター`: プレイモードに入ると、「(Unity) WriteObjectToVector」でエディターがクラッシュする
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- テキスト (TextMeshPro): TMPro Font Asset Creator でマルチスレッドのフォントアトラスを生成する際、UNITY_FT_Load_Glyph でクラッシュする
    ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

bee_backendが複数実行されている際にmono_log_write_logfileでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

特定のアセットを含むプロジェクトを閉じる際に ProfilerMutexLock でクラッシュする
    ([UUM-144371](https://issuetracker.unity3d.com/issues/crash-on-profilermutexlock-when-closing-a-project-with-specific-assets))



# 6000.0.77f1 リリースノート

## 修正内容

- `2D`: Lens Flare コンポーネントを追加した際のエラーを修正し、正投影カメラのサポートを追加しました。
    ([UUM-141781](https://issuetracker.unity3d.com/issues/render-graph-execution-and-argumentexception-errors-are-spammed-when-adding-lens-flare-srp-component-in-a-2d-urp-project))

- `2D`: シェーダーグラフマテリアルを使用しているスプライトのスケールが負の値の場合のピック操作を修正しました。
    ([UUM-141627](https://issuetracker.unity3d.com/issues/sprite-shader-graph-material-を-負の-スケール-を持つ-オブジェクトに-適用した際、シーンビューで-sprite-renderer-が-選択できない-問題))

- `Android`: `RunWithoutFocus` を有効にした状態で Android アプリをバックグラウンドに移行した際の Vulkan クラッシュを修正しました。
    (UUM-141888)

- `アニメーション`: レガシーアニメーションシステムにおける精度の不一致により、高フレームレート時にアニメーションイベントがスキップされる問題を修正しました。
    ([UUM-138951](https://issuetracker.unity3d.com/issues/the-animation-event-is-not-triggered-when-the-frame-rate-is-set-to-120-on-the-s26-ultra))

- `Animation`: プレイモードへの移行または終了時に、選択対象に未解決の GameObject 参照が残ってしまう問題を修正しました。
    (UUM-142098)

- `Audio`: すべての AudioListener コンポーネントが無効化されているか、その GameObject が無効化されている場合でも、Player ビルドでオーディオの再生が継続されるようになりました。
    ([UUM-127556](https://issuetracker.unity3d.com/issues/audiolisteners-still-listen-to-audio-when-their-components-are-disabled-in-player))

- `Audio`: プレイモード中に `AudioListener` で `OnAudioFilterRead` エフェクトを有効にしても、`MonoBehaviour` が無効な状態で開始された場合、音が出ない問題を修正しました。
    ([UUM-116871](https://issuetracker.unity3d.com/issues/onaudiofilterread-does-not-affect-signal-on-audiolistener-after-enable))

- `エディタ`: 「ビルドプロファイル」ウィンドウを開いた際、Player Settingsアセットがインポートされていないとクラッシュする問題を修正しました。
    ([UUM-116727](https://issuetracker.unity3d.com/issues/crash-on-std-1-tree-const-iterator-when-opening-the-build-profiles-window-in-a-specific-project))

- `エディタ`: エディタの言語を日本語に変更した際に、Macエディタで発生する極めて稀なクラッシュを修正しました。
    ([UUM-141719](https://issuetracker.unity3d.com/issues/crash-on-platform-strlen-when-the-editors-language-is-changed-to-japanese))

- `エディター`: プレイモード中にプレハブをインポートした際、MonoBehaviour/ScriptableObjectのフィールドに保存された参照が失われることがある問題を修正しました。
    ([UUM-139664](https://issuetracker.unity3d.com/issues/the-reference-to-a-prefab-variant-is-lost-on-instantiation-when-it-is-serialized-in-a-parents-component))

- `エディタ`: -nographics スイッチを使用してバッチモードで、カスタム DefaultCursor が設定されたプロジェクトを開いた際に LinuxEditor がクラッシュする問題を修正しました。
    ([UUM-142569](https://issuetracker.unity3d.com/issues/linuxeditor-crash-on-xaddextension-when-opening-the-unity-editor-on-linux-with-batchmode-and-nographics-on-a-project-with-a-custom-default-cursor))

- `エディタ`: TextCore のスプライトアセットにおける Unicode 処理を修正しました。
    ([UUM-141521](https://issuetracker.unity3d.com/issues/ui-toolkit-doesnt-render-the-assigned-sprites-when-using-unicode-characters-assigned-to-a-sprite))

- `エディタ`: テリレイン: 選択したテリレインのハイトマップを編集する際に発生していたパフォーマンスの低下を修正しました。
    ([UUM-141526](https://issuetracker.unity3d.com/issues/the-editor-start-performing-very-poorly-when-editing-the-terrain-heightmap-with-terraindata))

- `エディタ`: \[Android\] 「属性の競合」エラーウィンドウ内の、存在しない「Gradle トラブルシューティング」ページへのリンクを、Unity 6.0 用の正常に機能する「Gradle for Android」リンクに置き換えました。
    ([UUM-142945](https://issuetracker.unity3d.com/issues/colliding-attributes-error-opens-a-missing-page-when-pressing-the-troubleshoot-button))

- `Graphics`: フレームクリーンアップマップを修正し、無効なテクスチャIDやメモリを割り当てられていないテクスチャIDを削除せずに除去するようにしました。
    (UUM-129828)

- `License`: ライセンスクライアントの再接続に関する問題を修正しました。
    ([UUM-142572](https://issuetracker.unity3d.com/issues/floating-license-is-lost-for-concurrent-jobs))

- `Linux`: Linux上で2 GiBを超えるPOSIXファイルの読み込みが失敗する問題を修正しました。
    ([UUM-140520](https://issuetracker.unity3d.com/issues/couldnt-open-file-for-reading-error-occurs-when-running-binary2text-on-a-file-larger-than-2-gib))

- `Networking`: 複数の自動プロキシをサポートすることで、UUM-135025 を修正しました。
    ([UUM-135025](https://issuetracker.unity3d.com/issues/unitywebrequest-returns-curl-error-5-instead-of-timing-out-when-the-windows-proxy-auto-config-script-returns-multiple-proxies))

- `Physics`: クロスの相互衝突を処理する際、NvClothの内部処理による過剰なメモリ割り当てが原因で発生していたメモリ破損を修正しました。
    ([UUM-64185](https://issuetracker.unity3d.com/issues/crash-on-collideparticles-when-entering-play-mode))

- `Physics`: カプセルコライダーのデバッグ表示を修正し、スケーリングが適用された際にもカプセルのキャップが曲率を維持するようにしました。
    ([UUM-142483](https://issuetracker.unity3d.com/issues/colliders-are-rendered-deformed-when-viewed-through-physics-debugger-in-scene-view))

- `Physics`: NvClothソルバーカーネル内で、SIMD演算がNaN値を生成するいくつかのケースを修正しました。
    ([UUM-64185](https://issuetracker.unity3d.com/issues/crash-on-collideparticles-when-entering-play-mode))

- `Prefabs`: 破損した `PrefabInstance` をクリーンアップする際、追加されたオブジェクトが削除されなくなりました。
    ([UUM-142338](https://issuetracker.unity3d.com/issues/crash-on-mergeobjectcollection-when-repeatedly-selecting-a-prefab-asset-in-the-project-browser))

- `Shaders`: マテリアルバリアントに対して `Material.GetTexturePropertyNameIDs` が空を返す問題を修正しました。
    ([UUM-85842](https://issuetracker.unity3d.com/issues/an-empty-list-is-incorrectly-returned-for-material-variant-when-using-material-dot-gettexturepropertynameids))

- `Shaders`: シェーダーインスペクターの「コンパイルしてコードを表示」ドロップダウンが、要素が重ならないよう幅広くなりました。
    ([UUM-143195](https://issuetracker.unity3d.com/issues/shader-inspector-compile-and-show-code-popup-clips-menu-item-text-and-overlaps-the-show-button-with-the-variants-included-label))

- `Shaders`: 「コンパイルとコード表示」ドロップダウンは、大規模なシェーダーで使用してもエディタがフリーズしなくなりました。これは、Variant Included のカウントを算出するために、すべてのシェーダーステージのすべてのキーワードを反復処理することを回避したためです。
    ([UUM-141740](https://issuetracker.unity3d.com/issues/compile-and-show-code-dropdown-freezes-the-editor-for-a-long-time))

- `TextMeshPro`: TMP シェーダーが、シェーダーで設定されたカラーモードに合わせるのではなく、常に HDR カラーピッカーを使用してしまう問題を修正しました。
    ([UUM-141742](https://issuetracker.unity3d.com/issues/the-eyedropper-tool-selects-an-incorrect-value-when-sampling-a-tmp-text-objects-face-or-outline-color-from-the-game-view))

- `URP`: フレームデバッガーのメモリ使用量が過剰になる不具合を修正しました。
    ([UUM-139160](https://issuetracker.unity3d.com/issues/frame-debugger-excessive-memory-usage-regression))

- `URP`: 「テクスチャ」フォルダを展開した際に、フレームデバッガーでテクスチャプレビューアイコンが表示されない問題を修正しました。
    ([UUM-134917](https://issuetracker.unity3d.com/issues/texture-preview-icons-are-missing-in-frame-debugger-when-expanding-textures-foldout))

- `Video`: Async Scheduler のアルゴリズムの問題によって引き起こされていたリグレッションを修正しました。
    ([UUM-140747](https://issuetracker.unity3d.com/issues/audiosampleprovider-buffer-overflow-warnings-are-thrown-when-any-video-is-played-in-play-mode))




## 6000.0.77f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.collections`: [2.6.6](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) から [2.6.7](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) へ

- `com.unity.entities`: [1.4.6](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) から [1.4.7](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) へ

- `com.unity.netcode`: [1.13.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html) から [1.13.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: [1.4.19](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) から [1.4.20](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) へ

- `com.unity.services.wire`: [1.4.2](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html) から [1.4.4](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html) へ

- `com.unity.test-framework.performance`: [3.4.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.4//changelog/CHANGELOG.html) から [3.5.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.5//changelog/CHANGELOG.html) へ

- `com.unity.xr.interaction.toolkit`: [3.0.10](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@3.0//changelog/CHANGELOG.html) から [3.0.11](https://docs.unity3d.com/Packages/com.unity.xr.interaction.toolkit@3.0//changelog/CHANGELOG.html) へ

- `com.unity.addressables.android`: [1.0.10](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.0//changelog/CHANGELOG.html) から [1.1.0](https://docs.unity3d.com/Packages/com.unity.addressables.android@1.1//changelog/CHANGELOG.html) へ