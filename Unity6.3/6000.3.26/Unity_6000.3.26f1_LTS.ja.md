# Unity 6000.3.26f1 LTS
公開日時：2026年10月8日（木）13:38:24 GMT  
https://unity.com/releases/editor/whats-new/6000.3.26f1

# 6000.3.26f1 の既知の問題

- `6000.3.0a1,6000.0.51f1`: 2D レンダラーでブルームが有効な場合、画面が真っ黒になる
    ([UUM-150232](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150232))

- `6000.3.14f1`: [マルチプレイヤープレイモード] 追加のエディタインスタンスとVulkanグラフィックスAPIを使用してプレイモードに入ると、プレイモードのシナリオが「展開中」の状態のままになる
    ([UUM-154645](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-154645))

- `7000.0.0a5`: List<T> を継承するシリアライズ型を使用して Addressables コンテンツをビルドする際、mono_class_get_name の呼び出しでクラッシュする
    ([UUM-155711](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-155711))

- `7000.0.0a5`: Unity 6 から 7000.0.0a5 以降へプロジェクトをアップグレードする際、Scripting::LogExceptionFromManaged でクラッシュし、「BadImageFormatException: Bad IL format.」という致命的なエラーが発生する
    ([UUM-156142](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-156142))

bee_backend が複数実行されている際に mono_log_write_logfile の処理中にクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))



# 6000.3.26f1 リリースノート

## 新機能

- `エディタ`: Simulation Pro クライアント向けに、Linux ヘッドレスシミュレーションのビルドターゲットを再追加



## 変更点

- `Android`: Android Gradle Plugin (AGP) のバージョンを 9.0.0 から 9.1.1 に更新しました。



## 修正

- `2D`: グリッド選択のスケール/回転を編集する際の TilemapRenderer のちらつきを修正しました
    ([UUM-146002](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146002))

- `2D`: 2D Renderer が誤ったビューポートサイズを使用してアップスケーリングを行う問題を修正
    ([UUM-151621](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151621))

- `2D`: `SetTiles` がタイルのトランスフォームまたは色のみを変更した場合に、`Tilemap.tilemapPositionsChanged` および `tilemapTileChanged` コールバックが呼び出されない問題を修正しました。
    (UUM-146094)

- `2D`: タイルに法線マップがない場合、`TilemapRenderer`が他のタイルから法線マップを継承してしまう問題を修正しました。
    ([UUM-145359](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145359))

- `2D`: 2Dレンダラーの「Render Scale」設定によって、カメラソートレイヤーのテクスチャ解像度が影響を受けていた問題を修正しました。
    ([UUM-151723](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151723))

- `2D`: 「タイルパレットを開く」ボタンと「タイルマップフォーカス」ドロップダウンが、シーンビューのオーバーレイの全幅に表示されない問題を修正しました。
    ([UUM-151417](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151417))

- `Android`: ターゲット API レベル 37 が選択された際に表示される「ハッシュ文字列 android-37 を持つターゲットが見つかりませんでした」というエラーを修正しました。
    ([UUM-150216](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150216))

- `アセットバンドル`: 別のアセットバンドル内のプレハブの子オブジェクトへの参照を経由してアクセスしたアセットバンドルからプレハブをインスタンス化した際に、プレイヤーがクラッシュする問題を修正しました。
    (UUM-141605)

- `ビルドパイプライン`: `-activeBuildProfile` オプションで開始された連続したコマンドラインビルドにおいて、直前にアクティブだったプラットフォーム用のスクリプトがコンパイルされてしまう問題を修正しました。
    (UUM-150775)

- `エディタ`: Vulkanのプリトランスフォームによって投影行列が回転する可能性がある場合、その行列を最適化しないようにしました
    ([UUM-150650](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150650))

- `エディタ`: Linux版エディタで、「ヘルプ」および「ウィンドウ」メニューがメインメニューバーの末尾に配置されていなかったバグを修正しました。
    (UUM-113169)

- `エディタ`: Direct3D12 で非同期シェーダーコンパイルがまだ進行中の状態でプレイモードを終了した際に発生していたデッドロックを修正しました。
    ([UUM-152966](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-152966))

- `エディタ`: プレイモードに入る際のアカウントドロップダウンの表示を修正しました
    ([UUM-150759](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150759))

- `エディタ`: Intel 32ビットアーキテクチャのWindowsビルドプロファイルに戻した際、アクティブなビルドターゲットがIntel 32ビット \(StandaloneWindows\) ではなく、Intel 64ビット \(StandaloneWindows64\) のまま残ってしまう問題を修正しました。
    ([UUM-143128](https://issuetracker.unity3d.com/issues/windows-platform-architecture-switching-from-intel-32-bit-to-intel-64-bit-in-backend-when-switching-active-build-profile-back-to-windows-from-any-other-platform))

- `エディタ`: 「シーンが変更されました」ダイアログが表示されている状態で Cmd+Q を複数回押すとエディタがクラッシュする問題を修正しました。<br>
    未保存の変更がある状態でプレイモードのエディタを終了した際に、「シーンが変更されました」ダイアログが2つ表示される問題を修正しました。<br>
    EditorApplication.quitting をサブスクライブしているスクリプトがエディタウィンドウを変更した際、エディタの終了時にクラッシュする問題を修正しました。<br>
    エディタのダイアログで、Escキーを押しても「キャンセル」が選択されない問題を修正しました。
    ([UUM-149668](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149668))

- `GI`: シーンに VFXRenderer が含まれている場合に APV ベイクが失敗するバグを修正しました。
    ([UUM-150965](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150965))

- `Graphics`: GPU Resident Drawer が有効な状態で Unity がシェーダージョブを処理する際、主に macOS 上でメモリリークの警告が発生する可能性があった問題を修正しました。
    ([UUM-140185](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140185))

- `IMGUI`: プロジェクトウィンドウでアセットの名前を変更する場合など、表示領域の幅を超える長さのテキストを入力する際、カーソルが見えるようにテキストフィールドがスクロールしない問題を修正しました。
    ([UUM-149213](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-149213))

- `iOS`: 同じパラメータを持つ TMP 入力フィールド間を切り替えた際に、キーボードが閉じることがある問題を修正しました。
    (UUM-149104)

- `macOS`: macOS エディタのウィンドウがフォーカス外の状態にある際、内部のティック要求が無視され、その結果、非同期およびコルーチンベースの実行がフォーカス時よりも遅くなっていた問題を修正しました。
    (UUM-151097)

- N/A \(内部\): Android 向け Unity Render Service の線形レンダリングを修正しました
    (UUM-129914)

- `Networking`: 同一ホストへの高速な同時リクエストによって新しいクッキーが設定された後、低速なリクエストが完了した際に、UnityWebRequestのクッキーが古い値に戻ってしまうことがある問題を修正しました。
    ([UUM-150958](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150958))

- `Networking`: UnityWebRequest: 進行中のリクエストが、応答しない、または応答が遅いDNSサーバーに対してDNS解決を行っている最中に、スタンドアロンプレイヤーを終了するとフリーズする問題を修正しました。
    ([UUM-151643](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151643))

- `Player`: 実行時に Shader.globalMaximumLOD を変更した後、GameObject が正しい影を落とすようになりました。
    ([UUM-150226](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150226))

- `Profiler`: 空のスタンドアロン・プロファイラーの記録を保存する際に発生していたNullReferenceExceptionを修正しました。
    ([UUM-150588](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150588))

- `Profiler`: GraphicsStateCollection 割り当てに関連付けられた「Unrooted Allocations」のラベル表示を修正しました。
    ([UUM-139555](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-139555))

- `Profiler`: Profiler の [接続の問題のトラブルシューティング] ボタンが、接続のトラブルシューティングとは無関係なドキュメントページにリンクしていた問題を修正しました。
    ([UUM-153354](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-153354))

- `Shaders`: シェーダーのグローバルプロパティ API に範囲外の値が渡されたことにより発生していたクラッシュを修正しました。
    ([UUM-150856](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150856))

- `Terrain`: ハイトマップの解像度がデバイスの最大レンダリングテクスチャサイズを超えるTerrainを読み込んだ際に発生するクラッシュを修正しました。例えば、4096に制限されているデバイスで4097のハイトマップを読み込んだ場合などです。
    ([UUM-150551](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150551))

- `Text`: 複数段落からなる自動サイズ調整テキストが、画面に収まるように縮小されるのではなく、最初の行が省略されて折りたたまれてしまう問題を修正しました。
    (UUM-150602)

- `uGUI`: WorldDocumentRaycaster.camera 内の不要なキーワード「new」によるコンパイラ警告を修正しました。
    ([UUM-151722](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-151722))

- `UI Toolkit`: 別の祖先要素が GroupTransform の使用ヒントを使用している場合、ある祖先要素のスケールが 0 からアニメーションで拡大された後、DynamicTransform の使用ヒントを持つ VisualElement が、マウスオーバーするまで非表示のままになる問題を修正しました。
    ([UUM-140869](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-140869))

- `UI Toolkit`: SVG グラデーションの xlink:href 継承に関する問題を修正しました。
    ([UUM-150193](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150193))

- `UI Toolkit`: ネストされた svg タグによる SVG インポートエラーを修正しました。
    ([UUM-150948](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-150948))

- `URP`: シーンを再読み込みすると、特定の `Blitter` 関数が動作しなくなるバグを修正しました。
    (UUM-153092)

- `URP`: UV4入力のセマンティックの違いによるShaderGraphのコンパイル失敗を修正しました。
    ([UUM-143884](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143884))

- `URP`: 半精度 \(mobile\) プラットフォームにおいて、ボックス投影リフレクションプローブに継ぎ目が現れるバグを修正しましたプラットフォームにおいて、ボックス投影リフレクションプローブに継ぎ目が表示されるバグを修正しました。
    ([UUM-141981](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141981))

- `URP`: UberPost \(ポストプロセッシング\) が最終パスである場合、不要なカラーロードを回避することで、タイルベースのプラットフォームにおける URP プロジェクトの GPU パフォーマンスを改善しました。
    (UUM-140408)

- `Web`: 出力アセットのサイズが 2 GB を超える場合の Web プラットフォーム向けビルドの問題、および出力アセットのサイズが 4 GB を超える場合のビルドエラーメッセージを修正しました \(非対応\)。
    ([UUM-112909](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-112909))




## 6000.3.26f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.netcode`: [1.14.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html) から [1.14.3](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html) へ

- `com.unity.mobile.notifications`: [2.4.3](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.4//changelog/CHANGELOG.html) から [2.5.0](https://docs.unity3d.com/Packages/com.unity.mobile.notifications@2.5//changelog/CHANGELOG.html) へ

- `com.unity.services.authentication`: [3.7.4](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html) から [3.8.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.8//changelog/CHANGELOG.html) へ

- `com.unity.services.cloud-build`: [2.0.8](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.0//changelog/CHANGELOG.html) から [2.1.0](https://docs.unity3d.com/Packages/com.unity.services.cloud-build@2.1//changelog/CHANGELOG.html) へ

- `com.unity.services.friends`: [1.1.1](https://docs.unity3d.com/Packages/com.unity.services.friends@1.1//changelog/CHANGELOG.html) から [1.3.0](https://docs.unity3d.com/Packages/com.unity.services.friends@1.3//changelog/CHANGELOG.html)

- `com.unity.services.wire`: [1.5.1](https://docs.unity3d.com/Packages/com.unity.services.wire@1.5//changelog/CHANGELOG.html) から [1.6.0](https://docs.unity3d.com/Packages/com.unity.services.wire@1.6//changelog/CHANGELOG.html) へ

- `com.unity.netcode.gameobjects`: [2.13.2](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html) から [2.13.3](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html) へ

- `com.unity.multiplayer.tools`: [2.2.11](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) から [2.2.12](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) へ

- `com.unity.ai.navigation`: [2.0.14](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) から [2.0.15](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html)

- `com.unity.dt.app-ui`: [2.1.1](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@2.1//changelog/CHANGELOG.html) から [2.2.4](https://docs.unity3d.com/Packages/com.unity.dt.app-ui@2.2//changelog/CHANGELOG.html) へ

- `com.unity.services.multiplayer`: [2.3.1](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.3//changelog/CHANGELOG.html) から [2.3.3](https://docs.unity3d.com/Packages/com.unity.services.multiplayer@2.3//changelog/CHANGELOG.html) へ

- `com.unity.asset-manager-for-unity`: [1.11.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.11//changelog/CHANGELOG.html) から [1.12.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.12//changelog/CHANGELOG.html) へ