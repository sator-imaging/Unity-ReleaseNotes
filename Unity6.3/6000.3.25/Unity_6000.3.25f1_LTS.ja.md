# Unity 6000.3.25f1 LTS
公開日時：2026年9月24日(木) 12:52:52 GMT  
https://unity.com/releases/editor/whats-new/6000.3.25f1

# 6000.3.25f1 の既知の問題

- `6000.2.0b2`: [Vulkan] vkAcquireNextImageKHR が VK_TIMEOUT を返した際、vk::OnscreenSwapChain::AcquireNextImage で SIGSEGV が発生し、クラッシュする
    ([UUM-153744](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153744))

- `6000.3.0a1,6000.0.51f1`: 2D レンダラーでブルームが有効な場合、画面が真っ暗になる
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

- `6000.3.13f1`: グラフィックスジョブが有効な状態で、非同期シェーダーコンパイルが別のシェーダーに対するバリアント要求をキューに保持している間に、あるシェーダーが破棄されると、プレイモードの終了時にデッドロックが発生する
    ([UUM-152966](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152966))

bee_backendが複数実行されている際に、mono_log_write_logfileの呼び出しでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))



# 6000.3.25f1 リリースノート

## 改善点

- `ビルドシステム`: バンドルされている 7-Zip をバージョン 26.03 に更新しました。



## 変更点

- `Android`: エディタに同梱されている Gradle のバージョンを 9.1.0 から 9.3.1 に更新しました。



## 修正

- `Android`: 入力中にカーソルがテキストの末尾に戻ってしまう問題を修正しました。
    ([UUM-121294](https://issuetracker.unity3d.com/issues/android-ios-the-input-field-caret-moves-back-to-the-end-of-the-text-when-typing))

- `Android`: 仮想キーボードとUGUIテキストフィールド間の双方向同期に関する不具合を修正しました。
    (UUM-133870)

- `Android`: `editText`の`setText`呼び出しにより、`EditText`の選択範囲に関係なく、IMEの内部カーソルがテキストの末尾にリセットされる問題を修正しました。
    (UUM-142513)

- `Android`: `TouchScreenKeyboard.selection.length`が常に`0`を返す問題を修正しました。
    ([UUM-125821](https://issuetracker.unity3d.com/issues/android-touchscreenkeyboard-dot-selection-dot-length-always-returns-0-when-any-length-text-is-selected))

- `Android`: Android API レベル 32 未満の場合、SystemInfo.processorModel および SystemInfo.processorManufacturer は、警告文字列ではなく「不明」を返すようになりました。これにより、他のプラットフォームでの動作と一致するようになりました。
    (UUM-150389)

- `Audio`: 再生モードでのオーディオミキサーのフェーダーのクリック音を修正しました。
    ([UUM-150250](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150250))

- `Audio`: 一定時間の無音後に出力を再開しようとした際、オーディオ出力デバイスの再初期化に失敗しても、エディタがエラーをログに記録しなくなりました。出力は停止状態のままとなり、警告がログに記録され、次にオーディオが使用される際に再開が再試行されます。また、出力を再開できなかった場合にエディタの終了時に発生する可能性があったクラッシュも修正しました。
    (UUM-115959)

- `ビルドシステム`: ビルド中にシステムクロックが巻き戻された場合、ビルドが成功した後に IL2CPP Analytics ツールが JsonException を発生させて終了する問題を修正しました。
    ([UUM-150019](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150019))

- `エディタ`: ソースメッシュが 8 ビット UNorm などの非浮動小数点型の頂点フォーマットを使用している場合、メッシュパーティクルが誤った UV \(およびその他の頂点チャンネル\) でレンダリングされる問題を修正しました。
    ([UUM-141864](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141864))

- `エディタ`: インスペクタのマテリアルにある「GPUインスタンス化」および「両面グローバルイルミネーション」フィールドの「元に戻す/やり直し」機能を修正しました。
    ([UUM-143569](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143569))

- `IMGUI`: `OnGUI`中にGUISkinスタイルが割り当てられた際のGC割り当てを削減しました。
    ([UUM-134155](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134155))

- `Linux`: シーンの読み込み中にダイアログが開いた際、エディタがスプラッシュ画面でフリーズする問題を修正しました。
    ([UUM-151324](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151324))

- `パーティクル`: 一部のデバイスで、「カメラフェードオフ」と「ソフトパーティクルオン」を併用するとパーティクルが消えてしまう問題を修正しました。
    ([UUM-146249](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146249))

- `Player`: 開発用プレイヤービルドでデバッグアサートが発生するのを防ぐためのガードを追加しました。
    (UUM-152365)

- `Profiler`: UI Toolkitの「ライブリロード」オプションを切り替えた後、スタンドアロンプロファイラウィンドウのトップメニューからプロファイラデータを保存する際にNullReferenceExceptionが発生する問題を修正しました。
    ([UUM-150706](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150706))

- `Scripting`: コンパイル中のハングを解消しました。
    (UUM-126023)

- `SRP Core`: ネイティブパスがオンタイルピクセル記憶容量の上限を超えていると判断された場合、古いiOSデバイス（Apple GPUファミリー3以下）において、レンダリングパスがマージされず、フレーム全体がレンダリングパスごとに1つのネイティブパスにシリアライズされてしまう問題を修正しました。
    ([UUM-148865](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148865))

- `Text`: ハイフンの直前に空白があるテキストの測定で発生していた無限ループを修正しました。
    ([UUM-144559](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-144559))

- `Text`: ソースフォントのアンロード／リロード後にフォントフェイスが更新されない問題を修正しました。
    (UUM-150877)

- `TextCore`: 「Font Asset Creator」でフォントアセットを生成する際に発生する可能性があったクラッシュを修正しました。
    ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

- `TextCore`: Font Asset Creatorでフォントアセットを生成する際に発生する可能性があったクラッシュを修正しました。
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `TextCore`: Font Asset Creator でフォントアセットを生成する際に、代替のフォントフェイスが使用されてしまう可能性のある問題を修正しました。
    ([UUM-137866](https://issuetracker.unity3d.com/issues/glyph-adjustment-table-is-modified-when-using-an-existing-tmp-font-atlas-to-generate-a-new-tmp-font-atlas-with-the-same-settings))

- `TextCore`: 「Font Asset Creator」でフォントアセットアトラスの生成をキャンセルした際に発生する可能性があったメモリリークの問題を修正しました。
    ([UUM-142952](https://issuetracker.unity3d.com/issues/memory-leak-warnings-are-thrown-when-cancelling-the-creation-of-a-font-asset-using-render-mode-sdf16-or-sdf32))

- `uGUI`: フォントに省略記号（…）のグリフがなく、「Ellipsis overflow」モードが選択されている場合に発生していた、省略記号の改行に関する再帰的な問題を修正しました。
    ([UUM-134066](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-134066))

- `UI Toolkit`: パネルから削除された要素が、次のフォーカス移動が行われるまでメモリに残ってしまう問題を修正しました。
    ([UUM-151139](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151139))

- `UI Toolkit`: UI Builder で「切り取り」操作を行った際、UXML ドキュメントに「未保存の変更があります」と表示される問題を修正しました。
    ([UUM-151306](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151306))

- `URP`: タイルマップのグリッド線が表示されない問題を修正しました。 SRP でのレンダリング後、プレビューカメラのレンダリングターゲットが正しいことを確認してください。
    ([UUM-122618](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-122618))

- `URP`: Deferred+ レンダリングパスにおいて、Shader Graph マテリアルにリフレクションプローブが正しく適用されない問題を修正しました。
    (UUM-151317)

- `URP`: ScriptableRendererData.TryGetRendererFeature が NullReferenceException をスローしていた問題を修正しました。
    ([UUM-150772](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150772))

- `VFX Graph`: 組み込み属性の再分類を禁止しました。
    ([UUM-151058](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151058))

- `VFX Graph`: 特定のボクセル数で `MeshToSDFBaker` を使用する際に発生していた範囲外アクセス問題を修正しました。
    ([UUM-151674](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151674))

- `Video`: 再生モードに入った際に、ループ再生中のクリップで VideoPlayer がフリーズし、再生が停止して回復しなくなる問題を修正しました。
    (UUM-144106)

- `Video`: \[Android\] Vulkan ビデオデコードの回避策が誤って適用されることにより発生していたクラッシュを修正しました。
    ([UUM-145932](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145932))

- `Web`: NameFilesAsHashes の機能を修正しました。
    (UUM-148663)

- `WebGL`: シェーダーがキューブテクスチャを期待しているにもかかわらず、テクスチャが明示的にバインドされていなかった場合に発生するエラーを修正しました。
    ([UUM-150746](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150746))




## 6000.3.25f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.addressables`: [2.9.1](https://docs.unity3d.com/Packages/com.unity.addressables@2.9//changelog/CHANGELOG.html) から [2.10.3](https://docs.unity3d.com/Packages/com.unity.addressables@2.10//changelog/CHANGELOG.html) へ

- `com.unity.scriptablebuildpipeline`: [2.6.1](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html) から [2.6.2](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@2.6//changelog/CHANGELOG.html) へ

- `com.unity.services.wire`: [1.5.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.5//changelog/CHANGELOG.html) から [1.5.1](https://docs.unity3d.com/Packages/com.unity.services.wire@1.5//changelog/CHANGELOG.html) へ

- `com.unity.splines`: [2.9.0](https://docs.unity3d.com/Packages/com.unity.splines@2.9//changelog/CHANGELOG.html) から [2.9.1](https://docs.unity3d.com/Packages/com.unity.splines@2.9//changelog/CHANGELOG.html) へ

- `com.unity.xr.compositionlayers`: [2.5.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.5//changelog/CHANGELOG.html) から [2.6.0](https://docs.unity3d.com/Packages/com.unity.xr.compositionlayers@2.6//changelog/CHANGELOG.html) へ

- `com.unity.profiling.systemmetrics.mali`: [1.1.1](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) から [1.1.4](https://docs.unity3d.com/Packages/com.unity.profiling.systemmetrics.mali@1.1//changelog/CHANGELOG.html) へ