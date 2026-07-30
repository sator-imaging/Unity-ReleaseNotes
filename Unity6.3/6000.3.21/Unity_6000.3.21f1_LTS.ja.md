# Unity 6000.3.21f1 LTS
公開日時：2026年7月29日（水）07:10:05 GMT  
https://unity.com/releases/editor/whats-new/6000.3.21f1

# 6000.3.21f1 の既知の問題

- `6000.0.67f1`: [iOS] iOSのコントロールセンターにアクセスすると音声が途切れる
    ([UUM-145522](https://issuetracker.unity3d.com/issues/ios-audio-is-cut-out-when-accessing-ios-control-center))

- `6000.0.72f1`: DirectX12使用中にフルスクリーンウィンドウモードでアプリのフォーカスを素早く切り替えると、「UnityMain」でプレイヤーがクラッシュする
    ([UUM-148214](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-148214))

- `アセットインポーター`: プレイモードに入ると、「(Unity) WriteObjectToVector」でエディタがクラッシュする
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

bee_backendが複数実行されている際にmono_log_write_logfileでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

フォントアトラスの生成時に複数のスタックトレースが発生し、クラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.3.21f1 リリースノート

## 改善点

- `アクセシビリティ`: Android での `AccessibilityState.Expanded` のサポートを追加しました。

- `アセットパイプライン`: 以下の説明に詳細を追加しました。



## 修正

- `2D`: 「2D パッケージをインストール」ボタンが、本来無効になるべきでない状況で無効になっていた問題を修正しました。
    ([UUM-143583](https://issuetracker.unity3d.com/issues/install-2d-sprite-package-button-in-sprite-renderer-is-disabled-when-no-sprite-is-assigned-contradicting-its-own-help-text))

- `アクセシビリティ`: Android における `AccessibilityRole.Toggle` ノードで状態のアナウンスが二重に再生される問題を修正しました。
    ([UUM-146950](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146950))

- `アクセシビリティ`: UI Automation クライアントにおいて、セカンダリウィンドウに対してもメインアプリケーションウィンドウが提供されてしまう問題を修正しました。

- `アクセシビリティ`: Android において、スクリーンリーダーが `AccessibilityRole.Dropdown` ノードから移動する際に動作が遅くなる問題を修正しました。
    ([UUM-146949](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146949))

- `アクセシビリティ`: UI Automation クライアント（例：スクリーンリーダー）がアプリケーションとやり取りした後、Windows プレーヤーがシャットダウン時にクラッシュする問題を修正しました。
    (UUM-146676)

- `Android`: ```Screen.brightness``` に負の値を指定した場合、デバイスの推奨画面輝度が復元されるようになりました。
    ([UUM-145925](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145925))

- `Android`: AGP 9 のより厳格な R8 キープルールの適用要件を緩和しました。
    ([UUM-147136](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147136))

- `Animation`: Animator.ResetControllerState\(true\) が、float 型以外のパラメータをリセットしていなかった。
    ([UUM-146636](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146636))

- `Animation`: Animatorのトランジションのコピー＆ペースト時に、中断パラメータが貼り付けられない問題を修正しました。
    ([UUM-143599](https://issuetracker.unity3d.com/issues/interruption-source-ordered-interruption-and-can-transition-to-self-fields-are-not-pasted-to-transition-settings-when-pasting-transition-parameters))

- `Animation`: クラッシュの可能性を防ぐため、Animation Playable Outputのバインドおよびアンバインドの検証処理を再実装しました。
    ([UUM-146750](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146750))

- `アセットパイプライン`: 参照されているテクスチャが削除された後、同じ GUID で復元された際に、アセットのプレビューが白いままである問題を修正しました。
    ([UUM-138622](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-138622))

- `アセットパイプライン`: プロセス外のインポーターで `CreateAsset` が呼び出された際に、クラッシュしなくなりました。
    ([UUM-141087](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141087))

- `Audio`: オーディオミキサーでスナップショットを削除した際に発生していたエラーを修正しました。
    ([UUM-119443](https://issuetracker.unity3d.com/issues/error-is-thrown-when-deleting-snapshot-with-another-snapshot-present-in-audio-mixer-window))

- `Audio`: Burst でのコンパイルは成功し、インスペクタに関連するコードも表示されていたにもかかわらず、要求された際に `RootOutputInstance.IRealtime` が Burst を通じて正しく実行されない問題を修正しました。
    ([UUM-145622](https://issuetracker.unity3d.com/issues/scriptable-audio-processor-rootoutput-isnt-bursted-at-runtime))

- `エディター`: URP および HDRP で XR レンダリングに対応しているカメラを正射影モードに設定した際に、警告メッセージが表示されるようになりました。
    ([UUM-63527](https://issuetracker.unity3d.com/issues/カメラの投影モードが正射影に設定されていると、反射の形状が変化し、パフォーマンスに影響が出る))

- `エディタ`: 起動時のクラッシュを防ぐため、色空間の同期をアセットDBの初期リフレッシュ後まで延期しました。
    ([UUM-141297](https://issuetracker.unity3d.com/issues/an-refreshinternalv2-is-called-before-initialrefresh-error-is-thrown-when-opening-a-project-where-a-build-profile-with-player-settings-added-is-selected))

- `エディター`: SpriteRendererのマテリアルがインデックス化されていることを確認してください。
    (UUM-144279)

- `エディタ`: `[SerializeReference]` フィールドを使用している異なる MonoBehaviour スクリプトを持つ GameObject を複数選択した際に、`SerializableManagedRef::CallMethod` で発生していたクラッシュを修正しました。
    ([UUM-142019](https://issuetracker.unity3d.com/issues/crash-on-serializablemanagedref-callmethod-when-performing-various-unity-operations))

- `エディタ`: `AsyncInstantiateOperation` 内で破棄されなかった `CancellationTokenSource` オブジェクトによって引き起こされていたメモリリークを修正しました。
    ([UUM-147016](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147016))

- `Editor`: スプライト・アセットのインスペクター・ウィンドウの位置がずれる問題を修正しました。
    ([UUM-145514](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145514))

- `エディタ`: Handles.APIドキュメント「Handles.SnapValue」に記載されている通り、`SnapValue`および`Snapping.Snap`メソッドが正の値でのみスナップされるように修正しました。
    ([UUM-143716](https://issuetracker.unity3d.com/issues/handles-handles-dot-snapvalue-is-not-snapping-properly-with-negative-values))

- `Editor`: WindowsのDPIスケールとUnityのUIスケーリングの特定の組み合わせで、WinEditorに黒いバーのアーティファクトが表示される問題を修正しました。
    ([UUM-146885](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146885))

- `エディター`: AssetImporter プロセスによって開かれた EditorWindows が、タスクバーで孤立してしまう問題を修正しました。
    ([UUM-145778](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145778))

- `エディタ`: MS Windows 環境で、ローカルパッケージの解決に失敗した際にエディタがクラッシュする問題を修正しました。
    ([UUM-146678](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146678))

- `エディタ`: OpenGLESがアクティブなグラフィックスAPIである場合、エディタ内でMSAAテクスチャがレンダリングされない問題を修正しました。
    ([UUM-143867](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-143867))

- `エディタ`: 「適応型パフォーマンス」設定の「フレームレートスケーラー」における間隔の不具合を修正しました。
    ([UUM-141453](https://issuetracker.unity3d.com/issues/adaptive-performance-settings-framerate-field-doesnt-display-the-supported-without-vsync-warning-when-the-field-is-collapsed-in-build-profiles))

- `エディタ`: テキストが不規則にはみ出す問題を修正しました。
    (UUM-145644)

- `エディタ`: ATGで使用されるスプライトアセットに関する様々な問題を修正しました。
    ([UUM-145506](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145506))

- `GI`: マテリアルが null のシャドウキャスターを抽出する際に発生していたクラッシュを修正しました。
    ([UUM-132304](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-132304))

- `Graphics`: インジェクションされた RenderObjects パスで動的解像度が有効になっている場合、XR でのレンダリングの問題を修正しました。
    ([UUM-142592](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-142592))

- `Graphics`: ウォームアップ済みの GraphicsStateCollection バリアントに対して、処理負荷の高いバリアントごとの操作をスキップするようにしました。
    (UUM-139193)

- `HDRP`: `ClearBuffer2D` シェーダーを更新し、マルチビューに対応させました。
    ([UUM-137877](https://issuetracker.unity3d.com/issues/hdrp-xr-dx12-ssr-pbr-accumulation-algorithm-artifacts-are-present-in-one-eye-when-using-spi-openxr-rendering-mode))

- `iOS`: 深度カメラを 2 回目に作成した際に発生していたクラッシュを修正しました。
    ([UUM-141173](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-141173))

- `iOS`: アプリがバックグラウンドに移行した際に、iOSで誤って表示されていた「Touch was already deallocated」というエラーを修正しました。
    ([UUM-145381](https://issuetracker.unity3d.com/issues/ios-when-application-is-sent-to-background-with-active-touch-error-message-is-printed))

- `Networking`: libcurl ライブラリを 8.20 に更新しました。

- `Package Manager`: Unity アカウント名に引用符が含まれている場合、無効なパッケージが生成される問題を修正しました。
    ([UUM-133956](https://issuetracker.unity3d.com/issues/package-manager-create-package-creates-invalid-json-when-unity-account-name-includes-quotes))

- `パッケージマネージャー`: ページの更新時に、ユーザーのライセンス権限も更新されるように修正しました。
    (UUM-147523)

- `パッケージマネージャー`: プレイモードシナリオの追加エディターを有効にした際に、パッケージマネージャー関連のエラーが発生する問題を修正しました。
    ([UUM-147009](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147009))

- `パッケージマネージャー`: ライセンス権限に問題があるパッケージが、パッケージマネージャーウィンドウで「未インストール」として正しく表示されるようになりました。
    (UUM-134515)

- `Physics`: リンク深度の制限（64）が正しく適用されていなかったために発生していた、ArticulationBody コンポーネントの階層構造に関連するクラッシュを修正しました。
    ([UUM-145530](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145530))

- `Physics`: 接触距離が正しく処理されていなかったため、ConfigurableJointの設定が距離制約の最大値に達するとジッターが発生する問題を修正しました。
    ([UUM-146852](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146852))

- `Physics`: Rigidbody コンポーネントのシリアライズに関する問題を修正しました。2022LTS のシーンに保存されたプレハブのオーバーライド（\(for drag/angular drag\)）が、アップグレード後に保持されなくなっていた問題を修正しました。
    ([UUM-147601](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147601))

- `Profiler`: メモリプロファイラが ALLOC_TEMP_JOB_ASYNC の使用量を過小評価していたため、未使用のブロックが「未追跡」として表示される問題。
    ([UUM-145712](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-145712))

- `シーン/ゲームビュー`: シーンビューに SRP ボリュームのギズモが表示されない問題を修正しました。
    ([UUM-146740](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146740))

- `UI Toolkit`: メソッド `VectorUtils.BuildVectorImage(SceneInfo, Rect)` を公開しました。
    ([UUM-146278](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146278))

- `UI Toolkit`: UI Builderのバインディングウィンドウで、一部の型コンバータが無視されてしまう問題を修正しました。
    ([UUM-147357](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147357))

- `UI Toolkit`: フィルタリングされた要素で不透明度が反映されない問題を修正しました。
    ([UUM-147157](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147157))

- `UI Toolkit`: インスペクターにプレハブのオーバーライドマーカーが表示されない問題、およびインスペクターのスクロール領域の修正後に不要な水平スクロールバーが表示される問題を修正しました。
    ([UUM-147367](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147367))

- `UI Toolkit`: 9スライスとスライススケールを適用した大きなスプライトを使用する際のレンダリングの問題を修正しました。
    ([UUM-147415](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-147415))

- `UI Toolkit`: 参照先のアセットの Addressables コンテンツがアンロードおよびリロードされた後、-unity-material \(および background-image や -unity-font などのその他のアセットベースのスタイルプロパティ\) でスタイル設定された VisualElements が、デフォルトのシェーダー \(純白\) でレンダリングされる問題を修正しました。
    ([UUM-144652](https://issuetracker.unity3d.com/issues/ui-toolkit-uss-materials-in-assetbundles-break-due-to-instanceid-referencing-a-material-that-no-longer-exists-when-a-scene-is-loaded-through-addressables-for-the-second-time))

- `Universal Windows Platform`: UWP上で、マウスの動きによってスクロール操作が再トリガーされる問題を修正しました。
    ([UUM-144660](https://issuetracker.unity3d.com/issues/uwp-mouse-movement-re-triggers-stale-slash-scroll-value-after-the-scroll-wheel-is-used-once))

- `Video`: AudioSampleProvider.sampleFramesAvailable コールバックが、API Only モードで VideoPlayer を使用し、Unity Audio を無効にしている場合、macOS 上で決して発火しない問題を修正しました。
    ([UUM-143660](https://issuetracker.unity3d.com/issues/audiosampleprovider-dot-sampleframesavailable-callback-never-fires-when-using-macos))

- `Web`: サーバーが「Content-Length」ヘッダーを設定していない場合、UnityWebRequest でのレスポンスボディのストリーミングに関する問題を修正しました。
    ([UUM-146537](https://issuetracker.unity.com/api/v1.0/redirects/guid/UUM-146537))




## 6000.3.21f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.collections`: [2.6.6](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) から [2.6.8] へ(https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html)

- `com.unity.entities`: [1.4.6](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) から [1.4.8](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) へ

- `com.unity.physics`: [1.4.6](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) から [1.4.7](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: [1.4.19](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) から [1.4.21](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) へ

- `com.unity.burst`: [1.8.29](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) から [1.8.30](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html)

- `com.unity.formats.alembic`: [2.4.5](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) から [2.4.7](https://docs.unity3d.com/Packages/com.unity.formats.alembic@2.4//changelog/CHANGELOG.html) へ

- `com.unity.inputsystem`: [1.19.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.19//changelog/CHANGELOG.html) から [1.20.0](https://docs.unity3d.com/Packages/com.unity.inputsystem@1.20//changelog/CHANGELOG.html)

- `com.unity.services.authentication`: [3.7.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html) から [3.7.3](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html) へ

- `com.unity.services.cloudcode`: [2.10.3](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.10//changelog/CHANGELOG.html) から [2.10.4](https://docs.unity3d.com/Packages/com.unity.services.cloudcode@2.10//changelog/CHANGELOG.html) へ

- `com.unity.services.economy`: [3.5.3](https://docs.unity3d.com/Packages/com.unity.services.economy@3.5//changelog/CHANGELOG.html) から [3.5.4](https://docs.unity3d.com/Packages/com.unity.services.economy@3.5//changelog/CHANGELOG.html) へ

- `com.unity.visualscripting`: [1.9.11](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html) から [1.9.12](https://docs.unity3d.com/Packages/com.unity.visualscripting@1.9//changelog/CHANGELOG.html)

- `com.unity.transport`: [2.7.3](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html) から [2.7.4](https://docs.unity3d.com/Packages/com.unity.transport@2.7//changelog/CHANGELOG.html)

- `com.unity.ai.navigation`: [2.0.13](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) から [2.0.14](https://docs.unity3d.com/Packages/com.unity.ai.navigation@2.0//changelog/CHANGELOG.html) へ

- `com.unity.microsoft.gdk`: [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.6//changelog/CHANGELOG.html) から [1.7.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk@1.7//changelog/CHANGELOG.html)

- `com.unity.microsoft.gdk.tools`: [1.6.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.6//changelog/CHANGELOG.html) から [1.7.0](https://docs.unity3d.com/Packages/com.unity.microsoft.gdk.tools@1.7//changelog/CHANGELOG.html) へ