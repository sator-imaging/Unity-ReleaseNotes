# Unity 6000.0.78f1 LTS
公開日時：2026年6月25日（木）09:24:01 GMT  
https://unity.com/releases/editor/whats-new/6000.0.78f1

# 6000.0.78f1 の既知の問題

- `6000.0.11f1`: 特定のアセットを含むプロジェクトを閉じる際に、ProfilerMutexLock でクラッシュする
    ([UUM-144371](https://issuetracker.unity3d.com/issues/crash-on-profilermutexlock-when-closing-a-project-with-specific-assets))

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true) および UseTexture を指定して AddComputePass を使用する際、D3D12SwapChain::Present でクラッシュする
    ([UUM-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `アセットインポーター`: プレイモードに入ると、「(Unity) WriteObjectToVector」の処理中にエディターがクラッシュする
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: コマンドバッファのタイムアウトエラー発生後にゲームがフリーズする
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- テキスト (TextMeshPro): TMPro Font Asset Creator でマルチスレッドのフォントアトラスを生成する際、UNITY_FT_Load_Glyph の実行中にクラッシュする
 ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

bee_backendが複数実行されている際に、mono_log_write_logfileでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

Font Atlasの生成時に、複数のスタックトレースが発生してクラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.0.78f1 リリースノート

## 新機能

- `ドキュメント`: UDP ドキュメントパイプラインに、エンジンドキュメント内の外部参照リンクを解決するステップを追加しました。



## 修正

- `2D`: 編集モードでシーンビューにタイルパレットのオーバーレイが開いている状態で、プレイモード中にタイルを選択した際に発生していた例外を修正しました。
    ([UUM-137165](https://issuetracker.unity3d.com/issues/invalidoperationexception-and-nullreferenceexception-errors-are-thrown-when-clicking-inside-a-tile-palette-with-the-tile-palette-overlay-and-tile-palette-edit-enabled))

- `2D`: 特定のプロジェクトを開いた際に、ShaderPropertySheet::FindPropertyIndex で発生していたクラッシュを修正しました。
    ([UUM-110537](https://issuetracker.unity3d.com/issues/crash-on-shaderpropertysheet-findpropertyindex-when-opening-a-specific-project))

- `2D`: Light2D および Shadow Caster 2D コンポーネントが、インスペクタで誤ったアイコンを表示する問題を修正しました。
    ([UUM-132563](https://issuetracker.unity3d.com/issues/not-clear-abbreviation-ld-on-the-2d-light-overlay))

- `Android`: GameActivity ベースのアプリケーションがバックグラウンド中に強制終了される問題を修正しました。
    ([UUM-143555](https://issuetracker.unity3d.com/issues/android-gameactivity-app-fails-to-relaunch-after-it-was-closed-when-a-foreground-service-started-while-app-was-backgrounded))

- `DX12`: セカンダリ画面ではなくプライマリ画面でレンダリングが行われてしまう問題を修正しました。
    ([UUM-102150](https://issuetracker.unity3d.com/issues/uitoolkit-dx3d12-enabling-a-panel-by-changing-style-dot-display-from-none-to-flex-in-lateupdate-for-1-frame-it-will-render-on-the-wrong-display))

- `DX12`: シェーダーの非同期コンパイル中に、Meta pass CommandBuffer.DrawMesh\(\)が無視される問題を修正しました。
    (UUM-139294)

- `エディター`: 「プロジェクトが Unity Cloud に接続されていない場合、Unity Services が無効化されず、ビルド時間が長くなる」というバグを修正しました。
    (UUM-143898)

- `エディター`: Linux エディターで、マウスの前進ボタンと後退ボタンの入力が機能しない問題を修正しました。
    ([UUM-143528](https://issuetracker.unity3d.com/issues/input-system-does-not-register-the-backbutton-or-forwardbutton-when-using-the-linux-editor))

- `エディタ`: Canvas Renderer のアイコンを更新しました。
    ([UUM-142443](https://issuetracker.unity3d.com/issues/canvas-renderer-component-uses-a-low-resolution-icon))

- `Graphics`: ボーンが欠落している `SkinnedMeshRenderer` コンポーネントが、特定のレンダリングパスで依然としてレンダリングされてしまう問題を修正しました。
    (UUM-135684)

- `Graphics`: まだ読み込まれていない親を設定しても、マテリアルプロパティが失われなくなりました。
    ([UUM-113050](https://issuetracker.unity3d.com/issues/material-properties-are-lost-when-setting-a-parent-that-hasnt-been-loaded-yet))

- `Graphics`: レンダリングコマンドをレンダリングスレッドに渡す際に使用されるメモリ量を削減し、関連する診断機能を改善しました。
    (UUM-127793)

- `Graphics`: マテリアルで GPU インスタンス化が有効になっているにもかかわらず、関連するシェーダーにインスタンス化されたシェーダーバリアントが存在しない場合に、モーションベクトルが破損するのを防止しました。
    ([UUM-130621](https://issuetracker.unity3d.com/issues/gameobject-shows-visual-corruption-due-to-incorrect-previous-transform-matrix-while-using-active-spacewarp))

- `IL2CPP`: メソッド、ファイル、行番号を表示するオプションを選択した際、コールスタックに誤ったメソッドが表示されることがある問題を修正しました。
    ([UUM-138416](https://issuetracker.unity3d.com/issues/build-stack-trace-contains-invalid-lines-when-building-with-il2cpp-using-scripts-with-delegates-containing-generic-types-in-the-signature))

- `Linux`: イベントのショートカットパスを回避するために、AltGr によるテキスト合成を防ぐ入力テキストチェックを追加しました。
    ([UUM-142414](https://issuetracker.unity3d.com/issues/linux-character-at-is-not-inputted-when-pressing-altgr-plus-q-with-a-german-keyboard-layout))

- `Particles`: 背景に対してレンダリングする場合や SSAO を適用している場合、Deferred および Deferred+ モードで URP Particle Lit および Simple Lit シェーダーが正しく照らされるように修正しました。
    (UUM-140364)

- `Scene Manager`: 複数のシーンが読み込まれた状態でプレイモードを終了する際、ユーザースクリプトが `EditorSceneManager.sceneClosed` をサブスクライブし、ハンドラ内で開いているシーンを列挙するとクラッシュする問題を修正しました。
    ([UUM-131346](https://issuetracker.unity3d.com/issues/crash-on-scene-custom-getpathinternal-when-exiting-play-mode-while-listening-to-editorscenemanager-dot-sceneclosed-and-printing-open-scenes))

- `シーン/ゲームビュー`: マルチモニター使用時に、ゲームビューのスケールスライダーが正しく動作しないことがある問題を修正しました。
    ([UUM-135174](https://issuetracker.unity3d.com/issues/game-view-scale-drops-lower-than-is-possible-to-choose-manually-when-a-domain-reload-occurs))

- `Shadergraph`: グラデーションの変更を元に戻したりやり直したりすると、グラデーションピッカーウィンドウが閉じてしまう問題を修正しました。
    ([UUM-141977](https://issuetracker.unity3d.com/issues/hdr-gradient-editor-window-closes-when-undoing-changes-in-sample-gradient-node-with-ctrl-plus-z))

- `Shaders`: レンダリングオブジェクトを使用してシェーダーを上書きする際、元のマテリアルのプロパティが保持されるようになりました。
    ([UUM-100850](https://issuetracker.unity3d.com/issues/material-properties-are-not-preserved-when-overriding-shader-using-render-objects))

- `バージョン管理`: UnityYAMLMerge では、マージ後に空の配列に値が設定されると、無効なプレハブ YAML が生成されることがありました。場合によっては、これによりプレハブの解析に失敗し、使用できなくなることがありました。
    ([UUM-131530](https://issuetracker.unity3d.com/issues/prefabs-are-corrupted-due-to-inline-styled-yaml-when-unityyamlmerge-is-used-to-merge-prefabs))

- `WebGL`: WebGPU でカメラが存在しないシーンにおいて、ワインディング順が正しくない問題を修正しました。
    ([UUM-133894](https://issuetracker.unity3d.com/issues/invalid-front-face-configuration-when-building-with-graphicsapi-set-to-webgpu))




## 6000.0.78f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.formats.alembic`: [2.4.4](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) から [2.4.5](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) へ

- `com.unity.performance.profile-analyzer`: [1.3.4](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) から [1.4.0](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.4//changelog/CHANGELOG.html) へ

- `com.unity.purchasing`: [4.14.2](https://docs.unity3d.com/Packages/com.unity.purchasing@4.14//changelog/CHANGELOG.html) から [4.15.1](https://docs.unity3d.com/Packages/com.unity.purchasing@4.15//changelog/CHANGELOG.html)

- `com.unity.formats.fbx`: [5.1.4](https://docs.unity3d.com/Packages/com.unity.formats.fbx@5.1//changelog/CHANGELOG.html) から [5.1.6](https://docs.unity3d.com/Packages/com.unity.formats.fbx@5.1//changelog/CHANGELOG.html) へ

- `com.unity.ai.navigation`: [2.0.12](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) から [2.0.13](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) へ