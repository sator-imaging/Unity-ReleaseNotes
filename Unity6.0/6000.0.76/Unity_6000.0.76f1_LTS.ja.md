# Unity 6000.0.76f1 LTS
公開日時: Wed, 27 May 2026 09:43:20 GMT
https://unity.com/releases/editor/whats-new/6000.0.76f1

# 6000.0.76f1 の既知の問題点

- `6000.0.61f1`: SDF16 または SDF32 でフォントアトラスを生成すると tlsf_free でクラッシュする。
    ([uum-141061](https://issuetracker.unity3d.com/issues/crash-on-tlsf-free-when-generating-font-atlas-with-sdf16-or-sdf32))

- `6000.0.6f1`: [RenderGraph][D3D12] EnableAsyncCompute(true)とUseTextureでAddComputePassを使用するとD3D12SwapChain::Presentでクラッシュする。
    ([uum-140183](https://issuetracker.unity3d.com/issues/rendergraph-d3d12-crash-on-d3d12swapchain-present-when-using-addcomputepass-with-enableasynccompute-true-and-usetexture))

- `6000.2.0a8`: スクリプティングドメインのティアダウン後に非同期 HTTP コールバックが実行されると Scripting::LogException でクラッシュする。
    ([uum-141434](https://issuetracker.unity3d.com/issues/crash-on-scripting-logexception-when-async-http-callback-executes-after-scripting-domain-teardown))

- `アセットインポーター`: プレイモードに入ったときに"(Unity) WriteObjectToVector "でエディタがクラッシュする
    ([uum-112617](https://issuetracker.unity3d.com/issues/editor-crashes-on-unity-writeobjecttovector-when-entering-into-the-play-mode))

- `メタル`: コマンドバッファのタイムアウトエラーの後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- テキスト (TextMeshPro)：TMPro Font Asset CreatorでマルチスレッドのFont Atlasを生成するとUNITY_FT_Load_Glyphでクラッシュする
    ([uum-125366](https://issuetracker.unity3d.com/issues/crash-on-unity-ft-load-glyph-when-generating-multi-threaded-font-atlas-in-tmpro-font-asset-creator))

複数のbee_backendを実行している場合にmono_log_write_logfileでクラッシュする
    ([uum-142773](https://issuetracker.unity3d.com/issues/crash-on-mono-log-write-logfile-when-more-than-one-copy-of-bee-backend-is-running))



# 6000.0.76f1 リリースノート

## 改良点

- `Graphics`: GfxDeviceGLES::DrawBuffersBatchModeにNULLインデックスバッファに対するガードを追加。
    (UUM-135891)



## 変更点

- `Android`: JDK を 17.0.18+8 に更新。
    (UUM-141159)



## 修正

- `2D`: ユーザーがタイルパレット用のスプライトアセットをドラッグ＆ドロップし、タイルアセットを作成する操作をキャンセルした場合、タイルパレットに空のグリッドが表示される問題を修正。
    ([uum-132388](https://issuetracker.unity3d.com/issues/tile-palette-texture-drag-area-label-drag-tile-sprite-or-texture-sprite-type-asset-slash-s-here-dot-disappears-when-the-asset-save-pop-up-is-closed-slash-canceled))

- `Android`: フルスクリーンのユースケースをカバーするために、RunInBackgroundのテストを追加しました。

- `Android`: AndroidApplication.onConfigurationChanged が GameActivity の言語/国の変更を正しく反映するようになった。

- `Android`: スワイプ/戻るジェスチャーを離した後、EnhancedTouch.Touch.activeTouches.Countが正しく減少するようになった（GameActivity 4.4.1アップグレードの一部）。
    ([uum-128219](https://issuetracker.unity3d.com/issues/android-enhancedtouch-dot-touch-dot-activetouches-dot-count-does-not-decrease-after-releasing-the-swipe-slash-go-back-gesture))

- `Android`: カーソルロック時のマウス入力を修正しました。
    (UUM-91677)

- `Android`: Unity as a LibraryのApplication.UnloadまたはReload中に送信されるUnitySendMessageコールがAndroidでドロップされるのを修正しました。
    (UUM-141440)

- `Android`: SamsungA53上のValidateAndroidEscapeButtonテストを修正した。
    (UUM-96035)

- `Android`: Run without focus" を有効に切り替えると、Unity から起動された Android のアクティビティを含め、別のアクティビティが起動されても Unity のアクティビティが実行され続けるようになりました。
    ([UUM-120304](https://issuetracker.unity3d.com/issues/android-unityplayer-gets-paused-when-another-activity-is-launched-even-with-run-without-focus-enabled))

- `Android`: GameActivity ライブラリを 3.0.5 から 4.4.2 に更新しました。注意: 4.4.0はAndroid 7以降にしか対応していませんが、4.4.2ではGameActivityが再びAndroid 6に対応するように修正されました。

- `Android`: Android`: タッチパネルでキーボードをスワイプしても入力フィールドに単語が入力されない。
    ([uum-116283](https://issuetracker.unity3d.com/issues/android-ui-toolkit-gameactivity-swipe-typed-word-overrides-a-last-entry-with-an-inputfield-with-a-large-amount-of-characters))

- `アニメーション`: Animatorウィンドウで短いループアニメーションのトランジションを選択する際にArgumentOutOfRangeExceptionが発生するのを修正。
    ([uum-139812](https://issuetracker.unity3d.com/issues/argumentoutofrangeexception-is-thrown-when-selecting-a-transition-to-an-animation-shorter-than-3-frames-with-loop-time-enabled))

- `ビルド・パイプライン`: 初期ハッシュマップサイズを指定する BootConfig キー "remapper-initial-capacity" を使用して PersistentManager.Remapper の容量を予約するサポートを追加しました。
    (UUM-136275)

- `ビルドパイプライン`: ビルドパイプライン：Rider IDE で実行中にソースジェネレータが実行されていないことを確認。
    (UUM-133605)

- `ビルド・パイプライン`: ILPP.Trigger の待機ロジックを修正し、unity ログの "The pipe is being closed" 例外を防止。
    (UUM-136791)

- `ビルドシステム`: 特定のビルドパスを使用すると、ビルド中にノードGUIDの重複エラーが発生する問題を修正しました。
    ([UUM-128491](https://issuetracker.unity3d.com/issues/build-fails-with-duplicate-node-guids-error-when-using-specific-build-path))

- `ドキュメント`: Handles Scripting API ドキュメントへのリンクのタイプミスを修正しました。

- `ドキュメント`: 2DコライダーのリファレンスページのValeエラーを修正。

- `エディター`: enableHeightmapLODFrustumCulling`というオプションを追加。これはデバッグモードのTerrain Inspectorの設定で利用可能で、地形フラストラムベースのLODカリングをオプトアウトすることができます。
    (UUM-141589)

- `Editor`: リモートビルドが指定されているにもかかわらず、ローカルで無効なアーキテ クチャの場合、Build and Run ボタンがグレーアウトする。
    ([UUM-138399](https://issuetracker.unity3d.com/issues/build-and-run-button-greyed-out-for-locally-invalid-architecture-despite-remote-build-is-specified))

- `Editor`: macOS上で-projectPathコマンドライン引数を指定してエディターを起動するとUnity Hubが開いてしまうバグを修正しました。
    ([uum-136928](https://issuetracker.unity3d.com/issues/unity-hub-opens-when-launching-the-editor-with-projectpath-argument))

- `エディター`: ファイル破損や外部ファイルロックのためにCurlファイルキャッシュデータベース \(CurlRequestCache.db) を開くことができない場合、起動時にクラッシュする問題を修正しました。エディタはキャッシュデータベースの削除と再作成を試行し、ディスクファイルが使用できない場合はメモリ内キャッシュにフォールバックするようになりました。
    ([uum-140399](https://issuetracker.unity3d.com/issues/crash-on-getdatabase-when-sqlite-database-for-the-curl-file-cache-fails-to-open-or-create))

- `エディター`: BoxColliderと凸型MeshColliderの中心が重なっている時にcomputePenetrationを呼び出すとクラッシュする問題を修正しました。
    ([uum-100359](https://issuetracker.unity3d.com/issues/meshcollider-does-not-detect-collisions-with-capsules-and-charactercontroller-when-using-physics-dot-computepenetration))

- `Editor`: Fixed TimestepフィールドにInfまたはNaNを入力した時に発生する "Invalid double parameter "エラーを修正。
    ([uum-138227](https://issuetracker.unity3d.com/issues/argumentexception-invalid-double-parameter-dot-error-is-thrown-when-infinity-is-typed-into-the-fixed-timestep-field))

- `エディター`: Player Settings &gt; Preloaded AssetsなどのInspector配列のSizeフィールドに非常に大きな値(例えば24124124)を入力するとエディターがフリーズする不具合を修正しました。
    ([uum-139781](https://issuetracker.unity3d.com/issues/the-editor-freezes-indefinitely-when-entering-24124124-into-the-preloaded-assets-size))

- `エディター`: テクスチャがCubemapとして、またはミップマップなしでインポートされるように設定されている場合、選択されたレベルがこれらのテクスチャに対して効果を持っているにもかかわらず、テクスチャインポーターの「Aniso Level」スライダと対話することができなかった問題を修正しました。
    ([uum-138249](https://issuetracker.unity3d.com/issues/aniso-level-still-applies-when-generate-mipmap-is-disabled-in-texture-import-settings))

- `Editor`: UI Toolkit ￤インスペクタモードを使用している時、インスペクタのPrefab Variantのプロパティのオーバーライドを元に戻した後、OnValidateが呼び出されないのを修正しました。以前は、トグルやドロップダウンのような非テキストフィールドが、Prefabアセットの自動保存を正しく防止していませんでした。
    ([uum-134476](https://issuetracker.unity3d.com/issues/the-onvalidate-method-is-not-invoked-when-reverting-changes-on-a-prefab-variant))

- `エディター`: 色空間の設定を変更したときにプロジェクトウィンドウのパスが壊れていたのを修正しました。
    ([uum-139519](https://issuetracker.unity3d.com/issues/project-window-path-display-breaks-visually-when-player-settings-color-space-is-changed))

- `Editor`: CapsuleColliderと凸MeshCollider間のComputePenetration呼び出しの信頼性を向上。ComputePenetration は距離がゼロの時に真を返します。
    ([uum-100359](https://issuetracker.unity3d.com/issues/meshcollider-does-not-detect-collisions-with-capsules-and-charactercontroller-when-using-physics-dot-computepenetration))

- `エディター`: CharacterControllerと凸MeshCollider間のComputePenetration呼び出しの信頼性を向上。距離がゼロの場合、ComputePenetrationはtrueを返します。
    ([uum-100359](https://issuetracker.unity3d.com/issues/meshcollider-does-not-detect-collisions-with-capsules-and-charactercontroller-when-using-physics-dot-computepenetration))

- `エンジン診断`: プレイヤーループが停止した後、非同期のクラッシュ報告パイプラインが完了できなかったため、シャットダウン中に重複した管理例外カウントが失われる問題を修正しました。
    ([uum-141101](https://issuetracker.unity3d.com/issues/combined-log-and-throw-exceptions-function-does-not-show-up-in-diagnostics-cloud-dashboard-when-called-in-player))

- `エンジン診断`: JNI ネイティブメソッドが早期に登録解除され、nativeOnAndroidAppSetIdResult で java.lang.UnsatisfiedLinkError が発生することによるクラッシュを修正しました。
    (UUM-137662)

- `Graphics`: GPU Occlusion Culling(GPUオクルージョンカリング)中にGPU常駐ドローワーがクアッドトポロジーメッシュを三角形として誤ってレンダリングしていた問題を修正しました。
    ([UUM-132444](https://issuetracker.unity3d.com/issues/automatic-lod-fails-and-gpu-occlusion-culling-incompatibility-occurs-when-using-spline-based-quad-topology-meshes))

- `Graphics`: V-Sync が有効な場合に Windows 上で発生する Vulkan フレームタイムのスタッタリングを修正しました。
    (UUM-140217)

- `IL2CPP`: ランクが18を超える多次元配列でのIL2CPPコード生成の問題を修正しました。
    ([UUM-138552](https://issuetracker.unity3d.com/issues/build-fails-when-building-a-project-containing-an-18-plus-dimension-array-with-il2cpp))

- `iOS`: GameAssembly をビルドする il2cpp コマンドが失敗した場合に Xcode プロジェクトのビルドが失敗するように。
    (UUM-141609)

- `物理`: 投影モードを有効にしたConfigurableJointが、接続されているボディがキネマティックからダイナミックになったためにクラッシュすることがある問題を修正しました。
    ([UUM-135394](https://issuetracker.unity3d.com/issues/crash-on-constraintprojectiontree-projectiontreebuildstep-when-configurablejoint-uses-jointprojectionmode-dot-positionandrotation-and-connected-rigidbody-switches-from-kinematic-to-non-kinematic))

- `物理`: MeshCollider コンポーネントが一様でないスケールを受け取ると、それを正しく処理できない問題を修正しました。
    ([uum-139681](https://issuetracker.unity3d.com/issues/mesh-collider-does-not-skew-slash-shear-correctly-when-nested-inside-another-gameobject))

- `シェーダー`: プロパティを持たないシェーダに対して、シェーダ・インスペクタが空の「プロパティ」フォールドアウトを表示する問題を修正。
    ([uum-127146](https://issuetracker.unity3d.com/issues/planeocclusionshader-properties-foldout-does-not-display-any-content))

- `uGUI`: リッチテキスト編集を許可」が無効の状態でTMP InputFieldの先頭でキャレットを左に移動すると `IndexOutOfRangeException` がスローされるのを修正。
    ([uum-134157](https://issuetracker.unity3d.com/issues/indexoutofrangeexception-thrown-when-moving-caret-left-at-start-of-tmp-input-field-with-rich-text))

- `UIエレメント`: いくつかのUIToolkit<br>の原因となっていた新しいコードを最適化しました。
    .Bindings.PerformanceTestsのリグレッションの原因となっていた新しいコードを最適化しました。
    (UUM-139531)

- `URP`: スクリプタブル・レンダラー機能を追加または削除したときに、プロジェクト・ウィンドウの変更が更新されない問題を修正しました。
    ([UUM-139513](https://issuetracker.unity3d.com/issues/urp-asset-sub-assets-show-changes-in-sub-assets-only-after-reimporting-the-urp-asset-manually))

- `Web`: マルチスレッドのWebビルドでゲームパッドAPIが動作しない問題を修正しました。
    ([uum-136543](https://issuetracker.unity3d.com/issues/gamepad-input-does-not-work-in-a-web-build-when-native-c-slash-c-plus-plus-multithreading-is-enabled))




## 6000.0.76f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.collections`: [2.6.5](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) から [2.6.6](https://docs.unity3d.com/Packages/com.unity.collections@2.6//changelog/CHANGELOG.html) へ。

- `com.unity.entities`: [1.4.5](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html) から [1.4.6](https://docs.unity3d.com/Packages/com.unity.entities@1.4//changelog/CHANGELOG.html)

- `com.unity.physics`: [1.4.5](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html) から [1.4.6](https://docs.unity3d.com/Packages/com.unity.physics@1.4//changelog/CHANGELOG.html)

- `com.unity.entities.graphics`: [1.4.18](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) から [1.4.19](https://docs.unity3d.com/Packages/com.unity.entities.graphics@1.4//changelog/CHANGELOG.html) へ。