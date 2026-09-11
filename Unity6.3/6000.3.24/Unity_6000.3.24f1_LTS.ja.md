# Unity 6000.3.24f1 LTS
公開日時：2026年9月10日（木）14:47:57 GMT  
https://unity.com/releases/editor/whats-new/6000.3.24f1

# 6000.3.24f1 の既知の問題

- `6000.3.0a1`: 2D レンダラーでブルームが有効な場合、画面が真っ暗になる
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

- `6000.6.0a3、6000.5.0b8、6000.3.16f1`: D3D12において、ShaderWarmup.WarmupShaderFromCollection() の直後にシェーダーをアンロードすると、use-after-free によりプレイヤーがクラッシュする
    ([UUM-149781](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149781))

- テキスト (TextMeshPro): TMPro Font Asset Creator でマルチスレッドのフォントアトラスを生成する際、UNITY_FT_Load_Glyph の処理中にクラッシュする
 ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

bee_backend が複数実行されている際に mono_log_write_logfile でクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

Font Atlasの生成時に、複数のスタックトレースが発生してクラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.3.24f1 リリースノート

## 改善点

- `シェーダー`: 「マテリアルセット」\[Type\] API を使用してリスト外のプロパティを更新すると、マテリアルが「変更済み」状態になるようになりました。



## 修正

- `AI`: バウンズが極端に大きくなるオブジェクトを含むナビメッシュをベイクした際に発生していたエディタのクラッシュを修正しました。
    ([UUM-134462](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134462))

- `Android`: AndroidのバージョンラベルをGoogleの命名規則に合わせて修正しました。
    (UUM-150412)

- `Android`: 「Run Without Focus」が設定されている場合、AndroidでWebCamTextureが復元されない問題を修正しました。
    (UUM-149681)

- `Audio`: スクリプト対応プロセッサがテアダウン中にリアルタイムコールバックからパイプを読み込むと、Playモード終了時にエラーが記録される問題を修正しました。
    ([UUM-141072](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141072))

- `Audio`: 読み込み中のストリーミングクリップを含む AudioRandomContainer を一時停止した際に発生していたクラッシュを修正しました。
    (UUM-148440)

- `Audio`: オーディオ設定のリセット後に、一部のオーディオクリップで LoadState が無効になる問題を修正しました。
    ([UUM-147700](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147700))

- `コードエディタ`: [環境設定] > [外部ツール] 内の「引数をリセット」ボタンについて、フォーカスが移動した後にのみ更新されるのではなく、即座に「外部スクリプトエディタの引数」フィールドが更新されるように修正しました。
    (UUM-150210)

- `エディタ`: Unity シーンのアンロードによって MeshCollider コンポーネントが削除される際に発生していたハングを修正しました。
    ([UUM-149370](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149370))

- `エディタ`: TextMeshPro フォントアセットをインスペクトした際に発生していたエディタのクラッシュを修正しました。
    ([UUM-145753](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145753))

- `エディタ`: パーティクルシステムに 8 キーを超えるカーブが設定された際に発生していたエディタのクラッシュを修正しました。
    ([UUM-144792](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144792))

- `エディタ`: オーバーレイのコンテナの `rootVisualElement` にアクセスすると、再帰呼び出しが発生し、エディタがクラッシュする問題を修正しました。
    ([UUM-149209](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149209))

- `エディタ`: INspectorの「コンポーネントの追加」→「新しいスクリプト」ビューで**Enter**キーを押してもスクリプトが作成されない問題を修正しました。
    ([UUM-149682](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149682))

- `エディタ`: フローティングのビデオクリップインスペクタのプレビューエラーおよび表示上の警告を修正しました。
    ([UUM-147192](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147192))

- `エディタ`: `Vector4` インスペクタで、「W」コンポーネントのラベルが「...」に切り詰められて表示される問題を修正しました。
    ([UUM-143161](https://issuetracker.unity3d.com/issues/shadergraph-graph-inspector-vector4-w-label-is-always-truncated-to-dot-dot-dot))

- `エディタ`: 新規作成したプロジェクトの「最近開いたシーン」ドロップダウンに表示されていた「パスが見つからないか、破損しています\(\)」というメッセージを削除しました。 \(\[UUM-113848\]\(https://jira.unity3d.com/browse/UUM-113848\)\)。
    ([UUM-113848](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-113848))

- `エディタ`: 検索 : 編集モードのプロファイラ記録を有効にした状態でスクリプトを作成した際、「SearchImporter.IndexingRequest」に対して「Non-matching Profiler.EndSample」エラーが発生する問題を修正しました。
    ([UUM-143780](https://issuetracker.unity3d.com/issues/non-matching-profiler-dot-endsample-error-is-thrown-for-searchimporter-dot-indexingrequest-when-creating-a-script-with-edit-mode-profiler-recording-enabled))

- `EmbeddedLinux`: 最初のタッチ入力が失われる問題を修正しました。
    (UUM-150086)

- `Graphics`: 大規模なシーンでオクルージョンカリングをベイクした際に発生するクラッシュを修正しました。
    ([UUM-143361](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143361))

- `Graphics`: Blit Type が「Auto」に設定されている際に、Midgard Mali GPU でデバイスがフリーズする問題を修正しました。
    (UUM-149414)

- `Graphics`: Vulkan Player が 'PlayerSettings.vulkanNumSwapchainBuffers' の値を反映せず、代わりに 3 つのスワップチェーンバッファを固定数として使用していた問題を修正しました。
    (UUM-148724)

- `Graphics`: OpenGL ES 使用時に、マテリアルごとの定数バッファに関連するメモリエラーによって引き起こされるクラッシュを修正しました。
    (UUM-150590)

- `Graphics`: 画質設定 — デフォルトのプラットフォームには省略記号（…）を追加し、名前が非常に長い画質レベルには画質レベルヘッダーを追加しました。
    ([UUM-148889](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148889))

- `HDRP`: 「ライトマップのバイキュービックサンプリング」が有効になっている際の、誤ったシェーダーの削除を修正しました。
    ([UUM-134794](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134794))

- `IMGUI`: プロパティの矩形がGUI座標で負の値にある場合、プロパティフィールドの子フィールドが描画されない問題を修正しました。
    ([UUM-149255](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149255))

- `iOS`: マウスが接続されている状態で、ScrollViewがマウスホイールの入力に応答しない問題を修正しました。
    ([UUM-141279](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141279))

- `Linux`: 最初のタッチ入力が無視される問題を修正しました。
    (UUM-150086)

- `Linux`: glibc のバージョンを 2.34 に引き下げました。
    (UUM-150342)

- `Physics`: PhysX 4 SDK 内の問題（CharacterController が一度に 100 個以上のシェイプと衝突できない）を修正しました。
    ([UUM-132204](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-132204))

- `Physics`: Colliderを破棄する際のIgnoreCollisionのクリーンアップパフォーマンスを改善しました。
    ([UUM-115186](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-115186))

- `Physics 2D`: Collider2D を含む子 GameObject をアクティブ化した際に、Rigidbody2D をウェイクアップするようになりました。
    ([UUM-149852](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149852))

- `QNX`: 最初のタッチ入力が失われる問題を修正しました。
    (UUM-150086)

- `uGUI`: **Atlas Population Mode** が **Static** に設定され、**Multi Atlas Textures** が有効になっている TMP フォントアセットを、マテリアルプレビューが表示されている状態でインスペクトした際に発生する可能性のあるクラッシュを修正しました。
    ([UUM-145753](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145753))

- `uGUI`: 「オーバーフロー」が「省略記号」に設定されている大きなテキスト（TMP）GameObject がある場合に、`IndexOutOfRangeException` が発生する問題を修正しました。
    ([UUM-134477](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-インデックスが配列の範囲外であったため、大きなText \(TMP\) GameObjectのオーバーフローフィールドが「Ellipsis」に設定されている場合にエラーが発生する))

- `uGUI`: TMP_FontAsset.fontWeight 内の未使用の代入値によるコンパイラ警告を抑制します。
    (UUM-137669)

- `UI Toolkit`: 品質設定で「異方性テクスチャ」が「強制オン」に設定されている場合、ミラーまたはラップのアドレスモードを使用するグラデーションに発生していた白い線のアーティファクトを修正し、グラデーションの開始点より前の領域のレンダリング不具合を修正しました。
    ([UUM-139509](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-139509))

- `URP`: 一部のAndroidデバイスでVulkanを使用する際、深度法線を使用するとアーティファクトが発生する問題を修正しました。
    ([UUM-133583](https://issuetracker.unity3d.com/issues/android-vulkan-visual-artifacts-when-using-depth-normals-with-vulkan-api))

- `バージョン管理`: エディタの起動時に、バージョン管理エラー「UpdateSettings: Unknown version control plugin: XYZ」を引き起こすレースコンディションを修正しました。
    ([UUM-149884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149884))

- `VFX グラフ`: NaN によってグラフが永続的に「ダーティ」状態のままになる問題を修正しました。
    ([UUM-139398](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-139398))

- `VFX Graph`: URP におけるフラスタムカリングを修正しました。
    ([UUM-138375](https://issuetracker.unity3d.com/issues/vfx-graph-particles-are-not-culled-when-using-urp-and-frustum-culling-is-enabled-on-vfx-mesh-output))

- `VFX Graph`: 前の接線と次の接線が互いに打ち消し合う場合に、ストリップ内でNaNが発生するのを防止しました。
    ([UUM-141608](https://issuetracker.unity3d.com/issues/nan-normals-produced-when-using-custom-y-mode-in-an-orient-node-of-a-vfx-graph))

- `Video`: NVIDIAの「Fast」垂直同期が有効な場合、Direct3DでStop\(\)後に動画の再生が再開できない問題を修正した（デコードデバイスが失われ、復旧されなかったため）。
    ([UUM-135548](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-135548))

- `Video`: WebM Vorbis オーディオトラックが 0 Hz および 0 チャンネルと報告される問題を修正しました。
    (UUM-144045)

- `XR`: XR プラットフォームで、特に Deferred または Forward+ レンダリングパスで動的解像度を使用している際に発生する可能性のある、ブロック状またはずれた照明アーティファクトを修正しました。
    (UUM-143709)

- `XR`: 深度テクスチャの送信が有効になっている状態で、実行時に MSAA レベルを変更すると XR グラフィックスがフリーズする問題を修正しました。




## 6000.3.24f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.netcode`: [1.14.1](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html) から [1.14.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html)

- `com.unity.charactercontroller`: [1.4.1](https://docs.unity3d.com/Packages/com.unity.charactercontroller@1.4//changelog/CHANGELOG.html) から [1.4.5](https://docs.unity3d.com/Packages/com.unity.charactercontroller@1.4//changelog/CHANGELOG.html) に変更

- `com.unity.services.wire`: [1.4.4](https://docs.unity3d.com/Packages/com.unity.services.wire@1.4//changelog/CHANGELOG.html) から [1.5.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.5//changelog/CHANGELOG.html)

- `com.unity.terrain-tools`: [5.3.2](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html) から [5.3.3](https://docs.unity3d.com/Packages/com.unity.terrain-tools@5.3//changelog/CHANGELOG.html) へ

- `com.unity.netcode.gameobjects`: [2.13.1](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html) から [2.13.2](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html) へ

- `com.unity.multiplayer.tools`: [2.2.10](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) から [2.2.11](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) へ

- `com.unity.services.multiplayer`: [2.3.0](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.3//changelog/CHANGELOG.html) から [2.3.1](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.3//changelog/CHANGELOG.html) へ