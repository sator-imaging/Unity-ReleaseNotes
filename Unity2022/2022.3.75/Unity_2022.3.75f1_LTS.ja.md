# Unity 2022.3.75f1 LTS
公開日時: Wed, 08 Apr 2026 06:21:50 GMT
https://unity.com/releases/editor/whats-new/2022.3.75f1

# 2022.3.75f1 の既知の問題

- `メタル`: コマンドバッファのタイムアウトエラーの後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))



# 2022.3.75f1 リリースノート

## 機能

- `バージョン管理`: プロジェクトブラウザとインスペクタから、フォルダーの "ソースコントロールに追加 "と "変更を元に戻す "アクションを追加。

- `バージョン管理`: ブランチを視覚化し、ナビゲートするための新しいブランチエクスプローラーを追加。

- `バージョン管理`: ウィンドウの再読み込みやセッションをまたがるすべてのスプリッターの位置の永続性を追加。

- `バージョン管理`: マージビューでシェルブを部分的に適用できるようにした。

- `バージョン管理`: F2キーボードショートカットでブランチやラベルの名前を変更できるようにした。



## 変更点

- `バージョン管理`: ステータスバーにチェンジセットとラベルのアイコンを追加。

- `バージョン管理`: Unity Hub からプロジェクトを開くときにワークスペースの作成を遅延。

- `バージョン管理`: より一貫したキーボードワークフローのために、ダイアログ間のテキストフィールドのフォーカス動作を改善。

- `バージョン管理`: 変更待ちビューの空の状態を改善。

- `バージョン管理`: プロジェクトを誤って別の組織に接続しないようにした。

- `バージョン管理`: 新規プロジェクトの初期化を更新し、完全な初期チェックを行うようにした。

- `バージョン管理`: macOS の非表示ショートカットを Cmd+Shift+H に更新。



## 修正

- `DX12`: 以前コンピュートシェーダーの SRV としてバインドされていたレンダーターゲットへの描画を再開した後、リソースバリアが欠落していたのを修正。
    (UUM-127520)

- `Graphics`: (UUM-127520): builtinRP blit copyがfloat4カラーを出力するようにした(fxed4はメタル上 でhalf4に変換されるため、u16やf32データではデータが切り捨てられる)。
    ([uum-128591](https://issuetracker.unity3d.com/issues/terrain-heightmap-loses-precision-on-android-and-ios-when-the-heightmap-texture-is-blitted-to-a-rendertexture-using-the-default-blit-shader))

- `IL2CPP`: ラムダ式の無効な MethodsToPreserve エントリを修正。
    ([uum-124814](https://issuetracker.unity3d.com/issues/unity-cil-linker-fails-on-player-build-when-persistent-listeners-have-and-in-their-xml-attribute-names))

- `入力`: IOHIDDevice_GetUsage の無効なロングバッファポインタを修正しました。
    ([uum-135043](https://issuetracker.unity3d.com/issues/silicon-crash-on-os-unfair-recursive-lock-lock-with-options-when-opening-a-project-while-the-razer-synapse-app-is-open))

- `iOS`: iOS/tvOS の minspec を 12.0 から 13.0 にバンプ。
    (UUM-136440)

- `iOS`: アプリが既に実行されている状態でカスタムURLスキームまたはユニバーサルリンク経由でアプリが開かれた場合、またはコールドスタートからディープリンク経由でアプリが起動された一部のケースで、Application.deepLinkActivatedが呼び出されない問題を修正しました。
    ([uum-135497](https://issuetracker.unity3d.com/issues/ios-application-dot-deeplinkactivated-does-not-get-invoked-while-app-is-running-when-uiapplicationscenemanifest-is-added-in-info-dot-plist))

- `物理`: MeshCollider`で`Use Fast Midphase`クッキングオプションを使用してレイキャストする際にスタックオーバーフローを防止しました。
    ([uum-110564](https://issuetracker.unity3d.com/issues/silent-crash-when-raycasting-on-a-specific-dense-mesh))

- `バージョン管理`: サイドバーの「保留中の変更」を右クリックした時のレイアウト例外を修正。

- `バージョン管理`: ブランチ差分から履歴を開く際に NullReferenceException が発生する問題を修正。

- `バージョン管理`: チェンジセットごとの diff パネルで NullReferenceException が発生する可能性があったのを修正。

- `バージョン管理`: チェックインダイアログの進行状況ラベルを修正し、ローカライズした。

- `バージョン管理`: Explore Repositories ウィンドウのぼやけたアイコンを修正。

- `バージョン管理`: バージョン管理ウィンドウのボタンの大文字と小文字をUnityの標準に合わせて修正。

- `バージョン管理`: Unity 6.4以降で非推奨のinstanceID APIの使い方を修正。

- `バージョン管理`: ブランチビューからのチェンジセットごとの差分の問題を修正。

- `バージョン管理`: テーブルが空の時にブランチのコンテキストメニューが開かない問題を修正。

- `バージョン管理`: チェックインダイアログでコメント欄がオートフォーカスされないのを修正。

- `バージョン管理`: テーブルが空の時にラベルのコンテキストメニューが開かないのを修正。

- `バージョン管理`: 現在の選択範囲がチェンジセットやラベルの場合に、新規ブランチボタンが失敗するのを修正。

- `バージョン管理`: 再生モードを終了した後、ステータスバーが灰色になるのを修正。

- `バージョン管理`: ワークスペースの作成中にUnityのバージョン管理ウィンドウがマウスの移動を必要とせずに更新されるように修正。

- `バージョン管理`: Unity バージョン管理ウィンドウの検証メッセージの配置を修正。

- `ビデオ`: Vulkan Graphics API を使用した特定のモバイルデバイスで Video の再生に失敗する問題を修正しました。
    ([uum-133914](https://issuetracker.unity3d.com/issues/video-player-renders-no-video-on-specific-devices-when-using-vulkan))




## 2022.3.75f1 におけるパッケージの変更

## 更新されたパッケージ

- `com.unity.2d.aseprite`: [1.1.10](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html) から [1.1.11](https://docs.unity3d.com/Packages/com.unity.2d.aseprite@1.1//changelog/CHANGELOG.html) に変更

- `com.unity.addressables`: [1.28.2](https://docs.unity3d.com/Packages/com.unity.addressables@1.28//changelog/CHANGELOG.html) から [1.29.0](https://docs.unity3d.com/Packages/com.unity.addressables@1.29//changelog/CHANGELOG.html)

- `com.unity.ads`: [4.16.4](https://docs.unity3d.com/Packages/com.unity.ads@4.16//changelog/CHANGELOG.html) から [4.17.0](https://docs.unity3d.com/Packages/com.unity.ads@4.17//changelog/CHANGELOG.html)

- `com.unity.burst`: [1.8.28](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) から [1.8.29](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.collab-proxy`: [2.11.3](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.11//changelog/CHANGELOG.html) から [2.12.4](https://docs.unity3d.com/Packages/com.unity.collab-proxy@2.12//changelog/CHANGELOG.html)

- `com.unity.performance.profile-analyzer`: [1.3.1](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) から [1.3.3](https://docs.unity3d.com/Packages/com.unity.performance.profile-analyzer@1.3//changelog/CHANGELOG.html) に変更。

- `com.unity.postprocessing`: [3.5.0](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html) から [3.5.4](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5//changelog/CHANGELOG.html)

- `com.unity.scriptablebuildpipeline`: [1.23.3](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html) から [1.23.4](https://docs.unity3d.com/Packages/com.unity.scriptablebuildpipeline@1.23//changelog/CHANGELOG.html) に変更。

- `com.unity.services.analytics`: [6.2.2](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.2//changelog/CHANGELOG.html) から [6.3.0](https://docs.unity3d.com/Packages/com.unity.services.analytics@6.3//changelog/CHANGELOG.html) に変更。

- `com.unity.services.vivox`: [16.9.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.9//changelog/CHANGELOG.html)から[16.10.0](https://docs.unity3d.com/Packages/com.unity.services.vivox@16.10//changelog/CHANGELOG.html)

- `com.unity.timeline`: [1.8.10](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html) から [1.8.12](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)

- `com.unity.memoryprofiler`: [1.1.11](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html) から [1.1.12](https://docs.unity3d.com/Packages/com.unity.memoryprofiler@1.1//changelog/CHANGELOG.html)

- `com.unity.asset-manager-for-unity`: [1.9.1](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.9//changelog/CHANGELOG.html) から [1.10.0](https://docs.unity3d.com/Packages/com.unity.asset-manager-for-unity@1.10//changelog/CHANGELOG.html) へ。

- `com.unity.cloud.draco`: [5.4.2](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html) -> [5.4.3](https://docs.unity3d.com/Packages/com.unity.cloud.draco@5.4//changelog/CHANGELOG.html)

- `com.unity.cloud.ktx`: [3.6.2](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html) から [3.6.3](https://docs.unity3d.com/Packages/com.unity.cloud.ktx@3.6//changelog/CHANGELOG.html) に変更。