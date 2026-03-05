# Unity 2022.3.73f1 LTS
公開日時: Wed, 04 Mar 2026 13:54:00 GMT
https://unity.com/releases/editor/whats-new/2022.3.73f1

# 2022.3.73f1 の既知の問題

- `メタル`: コマンドバッファのタイムアウトエラーの後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

- `Video`: 2022.3.Xの修正: 特定のAndroidデバイスで、Videoを何度も有効/無効にすると、VideoPlayerがフリーズまたは停止する。
    (UUM-112470)

- `Windows`: バックグラウンドで実行 "が有効で、アクティブなウィンドウが切り替わると、プレーヤーがハングする。
    ([UUM-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))



# 2022.3.73f1 リリースノート

## 変更点

- `グラフィック`: テクスチャのインポートは https://docs.unity3d.com/Documentation/Manual/ImportingTextures.html でサポートされているフォーマットに厳密に従うようになりました。画像ファイルの拡張子を変更することでこれを回避することはもはやできません。もし画像ファイルのフォーマットが必要であれば、機能要求を出してください。



## 修正

- `アセットバンドル`: AssetBundleUnloadOperation` のアロケーションが予想以上に長く持続し、次の `GC.collect()` までクリアされない問題を修正した。
    (UUM-132703)

- `Editor`: EditorUtility.CompressTexture/EditorUtility.CompressCubemapTextureが符号付きEACフォーマットへの圧縮を処理の遅すぎる時点で中断し、テクスチャが壊れた状態になる問題を修正しました。符号付きEACフォーマットは圧縮のためにサポートされていないことに注意してください。

- `Editor`: EditorUtility.CompressTexture/EditorUtility.CompressCubemapTextureで、NPOTミップマップされたテクスチャをサポートされていないターゲットフォーマットに圧縮しようとする可能性があった問題を修正しました。この件に関する追加の詳細が API ドキュメントに追加されました。
    ([uum-129605](https://issuetracker.unity3d.com/issues/corrupted-mipmaps-are-generated-when-using-editorutility-dot-compresstexture-with-npot-textures))

- `iOS`: キーボードの UI をリキッドグラスによりフィットするように調整。
    (UUM-133464)

- `パッケージマネージャー`: upm パッケージを使用した URL のディープリンクで、発見可能であれば選択されたパッケージを表示。また、バージョンが指定されている場合や、パッケージが検出できない場合には、追加ポップアップを表示。
    (PAK-8687)




## 2022.3.73f1 におけるパッケージの変更

## 更新されたパッケージ

- `com.unity.inputsystem`: [1.18.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.18//changelog/CHANGELOG.html) から [1.19.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.19//changelog/CHANGELOG.html) へ。

- `com.unity.services.analytics`: [6.2.1](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) から [6.2.2](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: [1.1.10](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) から [1.1.11](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) に変更。

- `com.unity.microsoft.gdk`: [1.5.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html) から [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.5//changelog/CHANGELOG.html) に変更。

- `com.unity.microsoft.gdk.tools`: [1.5.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html) から [1.5.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.5//changelog/CHANGELOG.html) に変更。

- `com.unity.microsoft.gdk.discovery`: [1.2.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html) から [1.2.1](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.discovery@1.2//changelog/CHANGELOG.html) に変更。