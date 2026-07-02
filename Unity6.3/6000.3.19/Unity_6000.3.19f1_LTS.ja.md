# Unity 6000.3.19f1 LTS
公開日時：2026年7月1日（水）05:37:48 GMT  
https://unity.com/releases/editor/whats-new/6000.3.19f1

# 6000.3.19f1 の既知の問題

- `6000.0.11f1`: 特定のアセットを含むプロジェクトを閉じる際に ProfilerMutexLock でクラッシュする
    ([UUM-144371](https://issuetracker.unity3d.com/issues/crash-on-profilermutexlock-when-closing-a-project-with-specific-assets))

- `6000.0.67f1`: [iOS] iOSのコントロールセンターにアクセスした際に音声が途切れる
    ([UUM-145522](https://issuetracker.unity3d.com/issues/ios-audio-is-cut-out-when-accessing-ios-control-center))

- `アセットインポーター`: プレイモードに入ると、「(Unity) WriteObjectToVector」の処理中にエディターがクラッシュする
    ([UUM-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `Metal`: コマンドバッファのタイムアウトエラー発生後にゲームがフリーズする
    ([UUM-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- テキスト (TextMeshPro): TMPro Font Asset Creatorでマルチスレッドのフォントアトラスを生成する際、UNITY_FT_Load_Glyphでクラッシュする
    ([UUM-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

エディタで各種操作を行う際に mdb_cursor_sibling でクラッシュする
    ([UUM-141720](https://issuetracker.unity3d.com/issues/crash-on-mdb-cursor-sibling-when-performing-various-actions-in-the-editor))

bee_backendが複数実行されている際にmono_log_write_logfileでクラッシュする
    ([UUM-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))

フォントアトラスの生成時に複数のスタックトレースが発生し、クラッシュする
    ([UUM-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))



# 6000.3.19f1 リリースノート

## 改善点

- `エディタ`: LMDB の MDB_BAD_RSLOT ランタイムエラーに対する診断チェックを改善しました。
    ([UUM-110320](https://issuetracker.unity3d.com/issues/crash-on-sourceassetdbreadtxn-sourceassetdbreadtxn-when-idling-on-a-specific-project))



## 修正

- `2D`: `TileChangeData` の `Tile` ゲッタープロパティを使用する際に発生していた `InvalidCastException` を修正しました。
    ([UUM-142760](https://issuetracker.unity3d.com/issues/invalidcastexception-is-thrown-when-hovering-over-a-tilemap-with-a-saved-random-brush-pick-containing-empty-cells))

- `アクセシビリティ`: デスクトッププラットフォームでアプリケーションウィンドウを移動またはサイズ変更した際に、アクセシビリティフレームがリセットされる問題を修正しました。
    ([UUM-126569](https://issuetracker.unity3d.com/issues/accessibility-frames-reset-when-the-application-window-is-moved-or-resized-on-desktop-platforms))

- `Android`: GameActivity ベースのアプリケーションがバックグラウンド中に強制終了される問題を修正しました。
    ([UUM-143555](https://issuetracker.unity3d.com/issues/android-gameactivity-app-fails-to-relaunch-after-it-was-closed-when-a-foreground-service-started-while-app-was-backgrounded))

- `Android`: ターゲットアーキテクチャごとに分割されたAPKがすべて同じバージョンコードを受け取ってしまう問題を修正しました。
    ([UUM-144372](https://issuetracker.unity3d.com/issues/arm64-and-armv7-apks-return-the-same-version-code-when-split-apks-by-target-architecture-is-enabled))

- `Audio`: iOSのSafariで、アプリがバックグラウンドに移行した後、再開された際に、AudioSourceのループ再生が誤った再生位置から再開される問題を修正しました。
    ([UUM-144080](https://issuetracker.unity3d.com/issues/looping-audiosource-resumes-from-the-wrong-playback-position-when-the-app-is-backgrounded-and-resumed-on-ios-safari))

- `ドキュメント`: UI Toolkit ドキュメントの余白に関する問題を修正しました。

- `エディタ`: モデルインポーターがプロジェクト全体でテクスチャを検索しないようにするオプションを追加しました。
    (UUM-137345)

- `エディタ`: エディタの再起動を促すプロンプトが表示された際の、グラフィックス API の自動切り替えロジックの動作を変更しました。
    ([UUM-140948](https://issuetracker.unity3d.com/issues/auto-graphics-api-chackbox-will-not-stay-disabled-if-the-api-change-is-canceled))

- `エディタ`: ビルドプロファイルを複製した際、追加済みだがまだ編集されていない「プレイヤー設定」のオーバーライドが失われる問題を修正しました。
    (UUM-141702)

- `エディタ`: テンプレートシーンを変更した際に、シーンテンプレートのインスペクタにある依存関係リストが更新されない問題を修正しました。
    ([UUM-143123](https://issuetracker.unity3d.com/issues/selecting-dependencies-type-in-scene-template-inspector-throws-objectdisposedexception-and-nullreferenceexception-errors-in-the-console-when-sorting-dependencies))

- `エディタ`: ATGでFontAssetを「静的」から「動的」に切り替えた際に発生していたクラッシュを修正しました。
    ([UUM-144549](https://issuetracker.unity3d.com/issues/windows-editor-freezes-and-consumes-all-available-disk-space-when-changing-a-referenced-font-assets-atlas-population-mode-from-static-to-dynamic))

- `エディタ`: Linux版エディタで、マウスの前進ボタンおよび後退ボタンの入力が機能しない問題を修正しました。
    ([UUM-143528](https://issuetracker.unity3d.com/issues/input-system-does-not-register-the-backbutton-or-forwardbutton-when-using-the-linux-editor))

- `エディタ`: FBX モデルプレハブインスタンス上で、ネストされたシリアライズ済み配列を持つコンポーネントを使用する際、インスペクタのスクロール領域が伸びてしまう問題を修正しました。
    ([UUM-135480](https://issuetracker.unity3d.com/issues/inspector-scroll-area-stretches-when-using-components-with-nested-serialized-arrays-on-fbx-model-prefab-instances))

- `エディタ`: `RedrawFromNative` 実行中に新しいウィンドウを開いたり閉じたりすると、InspectorWindow で例外が発生する問題を修正しました。
    ([UUM-141990](https://issuetracker.unity3d.com/issues/invalidoperationexception-is-thrown-when-clicking-ctrl-plus-z-after-opening-gradient-editor))

- `エディタ`: グラフィック設定でのリセットに関する問題を修正しました。
    ([UUM-139127](https://issuetracker.unity3d.com/issues/resetting-graphics-settings-in-project-settings-window-throws-gpuresidentdrawer-batchrenderergroup-variants-must-be-keep-all-warnings-in-the-console-window))

- `エディタ`: Wacom デバイスを使用中に、ドロップダウンメニューの選択を終了した際にインスペクタがスクロールモードに入る問題を修正しました。
    ([UUM-138133](https://issuetracker.unity3d.com/issues/inspector-enters-scroll-mode-when-exiting-dropdown-menu-selection-and-using-wacom-device))

- `Editor`: Perforce 内の追跡対象外のフォルダに対して、VCCache が無限の再クエリループに陥る問題を修正しました。
    ([UUM-143313](https://issuetracker.unity3d.com/issues/cpu-usage-spikes-when-perforce-version-control-is-set-up-and-ai-assistant-is-installed))

- `Editor`: ベクトルのハッシュコード計算を改善しました。
    ([UUM-143005](https://issuetracker.unity3d.com/issues/hdrp-bloom-renders-with-a-purple-blue-or-green-anomaly-in-the-game-view-when-toggling- カメラのアナモルフィック設定が 1 に設定され、アスペクト比が 16 で割り切れる値であり、グラフィックス API が DX11 または DX12 に設定されている場合の、ブルーム・アナモルフィック・ボリューム設定))

- `エディター`: 「リセット」を使用すると、ライトマップモードとフォグモードが正しく元に戻るようになりました。
    ([UUM-139005](https://issuetracker.unity3d.com/issues/dropdown-values-are-not-reverted-when-selecting-reset-in-graphics-project-settings))

- `エディタ`: 「ドメインのリロード」が有効な状態でプレイモードに入ると、マルチプレイヤープレイモードの `enterPlayModeFromMppm` アナリティクスイベントが送信されない。
    (UUM-144601)

- `エディタ`: プレハブが予約済みフィールドを使用している場合に発生するクラッシュを防止した。
    ([UUM-144557](https://issuetracker.unity3d.com/issues/crash-on-saveprefabasset-when-selecting-a-specific-prefab))

- `エディタ`: 「Tier Settings Editor」ウィンドウで、サイズ変更時に長いテキストが正しく処理されるようになりました。
    ([UUM-138911](https://issuetracker.unity3d.com/issues/tier-settings-editor-window-does-not-handle-long-text-properly-on-resize))

- `エディタ`: キャンバスレンダラーのアイコンを更新しました。
    ([UUM-142443](https://issuetracker.unity3d.com/issues/canvas-renderer-component-uses-a-low-resolution-icon))

- `Graphics`: IDATチャンクが破損しているPNGファイルを読み込もうとした際に、「ImageConversion.LoadImage」でメモリリークが発生する問題を修正しました。
    ([UUM-143641](https://issuetracker.unity3d.com/issues/alloc-temp-main-leaks-a-persistent-4096-byte-allocation-when-imageconversion-dot-loadimage-fails-to-decode-a-png-with-valid-headers-but-corrupted-idat-chunk-data))

- `Graphics`: マテリアルで GPU インスタンス化が有効になっているにもかかわらず、関連するシェーダーにインスタンス化されたシェーダーバリアントが存在しない場合に、モーションベクトルが破損するのを防ぐ。
    ([UUM-130621](https://issuetracker.unity3d.com/issues/gameobject-shows-visual-corruption-due-to-incorrect-previous-transform-matrix-while-using-active-spacewarp))

- `HDRP`: SSGI コンピュートシェーダーのディスパッチにおけるパラメータ型の不一致を修正し、アダプティブ・プローブ・ボリュームを併用したスクリーン空間グローバルイルミネーション（SSGI）使用時の照明色の不正確さを解消しました。
    ([UUM-143777](https://issuetracker.unity3d.com/issues/lighting-sometimes-produces-incorrect-colors-when-baking-lightmaps-with-screen-space-global-illumination-and-adaptive-probe-volumes))

- `Linux`: イベントのショートカットパスを回避するため、AltGr によるテキスト合成を防ぐ入力テキストチェックを追加しました。
    ([UUM-142414](https://issuetracker.unity3d.com/issues/linux-character-at-is-not-inputted-when-pressing-altgr-plus-q-with-a-german-keyboard-layout))

- `Linux`: LinuxエディタからWindowsプレーヤーをビルドしたり、Visual Studioソリューションを作成したりする際のバグを修正しました。
    ([UUM-140187](https://issuetracker.unity3d.com/issues/linuxeditor-building-for-windows-throws-agilitysdk-dll-could-not-be-retrieved-when-create-visual-studio-solution-was-enabled-before-switching-build-platform-to-windows))

- `Networking`: CVE-2026-27135 を緩和する更新された nghttp2 を利用する libcurl artifactory をバージョンアップしました。
    (UUM-140912)

- `Particles`: 背景に対してレンダリングする場合や SSAO を適用した場合に、Deferred および Deferred+ モードで URP Particle Lit および Simple Lit シェーダーが正しく照明されるよう修正しました。
    (UUM-140364)

- `Physics`: 無効化された Rigidbody コンポーネントのインスタンスが、内部アクターを無期限に存続させ続けることによって引き起こされていたクラッシュを修正しました。
    ([UUM-143658](https://issuetracker.unity3d.com/issues/crash-on-physicscommands-physx-bodysetpose-when-entering-play-mode-in-a-specific-project))

- `Physics`: マルチボックス・プルーニング・ブロードフェーズを使用していない物理シーンで `Physics.RebuildBroadphaseRegions 内で発生していたクラッシュを修正しました。このクラッシュは、マルチボックス・プルーニング・ブロードフェーズを使用していない物理シーンでこのメソッドが呼び出された場合に発生する可能性がありました。
    ([UUM-144472](https://issuetracker.unity3d.com/issues/physics-dot-rebuildbroadphaseregions-does-not-repopulate-them-with-pre-existing-shapes))

- `Physics`: `Physics.RebuildBroadphaseRegions` を呼び出した際、既存の Collider コンポーネントが新しく生成されたブロードフェーズ領域から除外されてしまう問題を修正しました。
    ([UUM-144472](https://issuetracker.unity3d.com/issues/physics-dot-rebuildbroadphaseregions-does-not-repopulate-them-with-pre-existing-shapes))

- `Physics 2D`: PhysicsMask、ContactFilter、QueryFilter、PhysicsUserData、PolygonGeometry、PhysicsRotate、およびPhysicsLayerについて、既存のUI-Toolkitプロパティドロワーに加え、IMGUIプロパティドロワーを追加しました。
    ([UUM-142727](https://issuetracker.unity3d.com/issues/no-gui-implemented-is-displayed-when-using-physicsmask-with-a-customeditor))

- `Physics 2D`: 「PhysicsBody.collisionThreshold」が無視されていた問題を修正し、PhysicsBodyがチェーンセグメントを含むすべての形状タイプに対して連続衝突を行うタイミングを制御できるようにしました。
    ([UUM-144698](https://issuetracker.unity3d.com/issues/physicsbody-dot-collisionthreshold-not-correctly-controlling-ccd))

- `Profiler`: ProfilerSymbolsDelayedDeletion::AddCloneObject でのクラッシュを修正しました。
    ([UUM-144194](https://issuetracker.unity3d.com/issues/crash-on-profilersymbolsdelayeddeletion-addcloneobject-when-deserializing-an-object-instantiate-marker-with-a-dangling-slash-corrupt-name-string))

- `Profiler`: 「ビルドして実行」または「Profiler への自動接続」設定を使用しているプレイヤーにおける、プロファイラーのスクリーンショット取得レートおよびタイミングに関する問題を修正しました。
    (UUM-144511)

- `Profiler`: PersistentManager.Remapper のメモリ追跡を改善しました。
    (UUM-141167)

- `Scene/Game View`: マルチモニター使用時に、GameView のスケールスライダーが正しく動作しないことがある問題を修正しました。
    ([UUM-135174](https://issuetracker.unity3d.com/issues/game-view-scale-drops-lower-than-is-possible-to-choose-manually-when-a-domain-reload-occurs))

- `Shadergraph`: グラデーションの変更を元に戻したりやり直したりすると、グラデーションピッカーウィンドウが閉じてしまう問題を修正しました。
    ([UUM-141977](https://issuetracker.unity3d.com/issues/hdr-gradient-editor-window-closes-when-undoing-changes-in-sample-gradient-node-with-ctrl-plus-z))

- `Shadergraph`: Escキーを押してもノード検索ウィンドウが閉じない問題を修正しました。
    ([UUM-143233](https://issuetracker.unity3d.com/issues/shader-graphs-create-node-menu-cannot-be-closed-with-esc-button))

- `Shaders`: レンダリングオブジェクトを使用してシェーダーを上書きする際、元のマテリアルのプロパティが保持されるようになりました。
    ([UUM-100850](https://issuetracker.unity3d.com/issues/material-properties-are-not-preserved-when-overriding-shader-using-render-objects))

- `テキスト`: macOSのエディタテキストフィールドでCJK文字が表示されない問題を修正しました。
    ([UUM-144095](https://issuetracker.unity3d.com/issues/characters-are-invisible-in-the-textfield-when-certain-japanese-characters-are-used))

- `UI`: コンテンツが収まっているにもかかわらず、ScrollView が空白領域までドラッグスクロールしてしまう問題を修正しました。
    ([UUM-142498](https://issuetracker.unity3d.com/issues/blank-area-appears-at-the- Wacomタブレットペンでインスペクタやビルド設定ウィンドウの上部をタッチして下方向にドラッグした際に発生する問題))

- `UI Toolkit`: Painter2D によって FillGradient.radius が無視される問題を修正しました。
    ([UUM-138358](https://issuetracker.unity3d.com/issues/[放射状グラデーションの「fillgradient.dot.radius」プロパティを変更しても半径が変わらない問題](https://issuetracker.unity3d.com/issues/))

- `UI Toolkit`: アンチエイリアス処理された円弧エンコーディングにおけるSVGの軽微なテッセレーションの問題を修正しました。
    ([UUM-144586](https://issuetracker.unity3d.com/issues/svg-icon-has-tessellation-issues-in-antialiased-arc-encodings-ok-with-basic-triangulation))

- `UI Toolkit`: 複数のインスペクタウィンドウで、Grid Layout Group コンポーネントを持つ異なるオブジェクトが表示されている場合、プレイモードに入った後に MissingReferenceException エラーが発生する問題を修正しました。
    ([UUM-145062](https://issuetracker.unity3d.com/issues/missingreferenceexception-errors-are-thrown-after-entering-play-mode-when-multiple-inspector-windows-are-displaying-different-objects-with-grid-layout-group-component))

- `UI Toolkit`: VectorImage としてインポートされた SVG のプロジェクトブラウザのアイコンを修正しました。
    ([UUM-141655](https://issuetracker.unity3d.com/issues/svgs-imported-as-vector-image-dont-show-a-static-preview-in-the-project-browser))

- `UI Toolkit`: 「アンチエイリアス付き円弧エンコーディング」としてインポートされた場合、SVGの放射状フォーカスが機能しない問題を修正しました。
    ([UUM-138043](https://issuetracker.unity3d.com/issues/svg-radial-gradient-focus-isnt-working-with-antialiased-arc-encodings))

- `UI Toolkit`: 既存のコンテキストモードの直後に元に戻す/やり直しを実行した際に発生していた、UI Builderのnull参照例外を修正しました。
    ([UUM-142693](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-and-nullreferenceexception-are-thrown-and-element-disappears-from-ui-builder-when-undoing-rename-of-element-in-open-instance-in-context-menu))

- `Undo System`: EraseUndos における境界チェックを更新しました。
    (UUM-142925)

- `VFX Graph`: 静止状態のパーティクルに対する「Collision with Signed Distance Field」ブロックの安定性を向上させました。
    ([UUM-99382](https://issuetracker.unity3d.com/issues/vfx-graph-position-jitter-in-reststate-with-collision-sdf))

- `Windows`: スタンドアロン版のPlayerビルドでInput Managerを使用する際、Windowsのペン入力からマウスポインタイベント（`Input.GetMouseButtonDown`）が生成されない問題を修正しました。
    ([UUM-140737](https://issuetracker.unity3d.com/issues/windows-pen-input-does-not-generate-mouse-pointer-events-when-using-input-manager))

- `Windows`: Windowsのタッチスクリーンデバイスでピンチジェスチャーを実行した後、UIツールキットのボタンがタッチ操作に反応しなくなる問題を修正しました。
    ([UUM-138595](https://issuetracker.unity3d.com/issues/ui-toolkit-buttons-stop-responding-to-single-taps-Windowsタッチデバイスで新しい入力システムを使用してマルチタッチジェスチャーを実行した際))

- `Windows`: WindowsのIL2CPPビルドがLNK1104エラーで失敗する問題を修正しました。
    ([UUM-139929](https://issuetracker.unity3d.com/issues/build-fails-with-a-link-error-when-building-for-windows-x64-with-il2cpp-and-having-visual-studio-2026および2022がインストールされている場合))

- `XR`: VrsResources.DisposeResources\(\) に存在していたメモリリークを修正しました。
    (UUM-143173)




## 6000.3.19f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.netcode`: [1.13.2](https://docs.unity3d.com/Packages/com.unity.netcode@1.13//changelog/CHANGELOG.html) から [1.14.0](https://docs.unity3d.com/Packages/com.unity.netcode@1.14//changelog/CHANGELOG.html)

- `com.unity.probuilder`: [6.0.9](https://docs.unity3d.com/Packages/com.unity.probuilder@6.0//changelog/CHANGELOG.html) から [6.1.2](https://docs.unity3d.com/Packages/com.unity.probuilder@6.1//changelog/CHANGELOG.html) へ

- `com.unity.services.authentication`: [3.6.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.6//changelog/CHANGELOG.html) から [3.7.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.7//changelog/CHANGELOG.html) へ

- `com.unity.splines`: [2.8.4](https://docs.unity3d.com/Packages/com.unity.splines@2.8//changelog/CHANGELOG.html) から [2.9.0](https://docs.unity3d.com/Packages/com.unity.splines@2.9//changelog/CHANGELOG.html)

- `com.unity.netcode.gameobjects`: [2.12.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.12//changelog/CHANGELOG.html) から [2.13.0](https://docs.unity3d.com/Packages/com.unity.netcode.gameobjects@2.13//changelog/CHANGELOG.html)

- `com.unity.multiplayer.tools`: [2.2.8](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) から [2.2.9](https://docs.unity3d.com/Packages/com.unity.multiplayer.tools@2.2//changelog/CHANGELOG.html) へ