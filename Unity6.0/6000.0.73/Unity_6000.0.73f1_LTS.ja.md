# Unity 6000.0.73f1 LTS
公開日時：Wed, 15 Apr 2026 08:22:53 GMT
https://unity.com/releases/editor/whats-new/6000.0.73f1

# 6000.0.73f1 の既知の問題

- `6000.5.0a4,6000.0.66f1,6000.3.4f1,6000.4.0b4`: ShaderVariantCollection.variantCountとShaderVariantCollection.shaderCountがBuildsで0を返します。
    ([uum-137398](https://issuetracker.unity3d.com/issues/shadervariantcollection-dot-variantcount-and-shadervariantcollection-dot-shadercount-returns-0-in-builds))

- `IL2CPP`: [iOS] [Android] IL2CPPのビルド中に外部ライブラリのジェネリックに失敗する
    ([uum-125284](https://issuetracker.unity3d.com/issues/ios-android-external-library-generics-fail-during-il2cpp-build))

- `メタル`: コマンドバッファのタイムアウトエラー後にゲームがフリーズする
    ([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))

- `Metal`: プレイモードのエディタで最小プロジェクトで macOS が吃音になる
    ([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))

List<T>構造体でネストされた[SerializeReference]フィールドを使用すると "core::base_hash_set "でクラッシュする
    ([uum-139722](https://issuetracker.unity3d.com/issues/crash-on-core-base-hash-set-when-using-nested-serializereference-fields-in-list-structures))

DX12使用時にシーンビューでGameObjectを選択するとCheckDeviceStatusでクラッシュする。
    ([uum-138597](https://issuetracker.unity3d.com/issues/crash-on-checkdevicestatus-when-selecting-gameobjects-in-the-scene-view-while-using-dx12))

ConfigurableJoint が JointProjectionMode.PositionAndRotation を使用し、接続された Rigidbody がキネマティックから非キネマティックに切り替わるとき、ConstraintProjectionTree::projectionTreeBuildStep でクラッシュする。
    ([uum-135394](https://issuetracker.unity3d.com/issues/crash-on-constraintprojectiontree-projectiontreebuildstep-when-configurablejoint-uses-jointprojectionmode-dot-positionandrotation-and-connected-rigidbody-switches-from-kinematic-to-non-kinematic))

空白のURPプロジェクトで再コンパイルすると、VisualElementのエディタ・メモリ・リークが発生する
    ([uum-138000](https://issuetracker.unity3d.com/issues/editor-memory-leak-in-visualelement-when-recompiling-in-a-blank-urp-project))



# 6000.0.73f1 リリースノート

## API の変更

- `エディタ`: ENABLE_UNITY_COLLECTIONS_CHECKS が定義されていない場合に JobHandle.GetHashCode と Equals および ==/!= 演算子を Expose するように変更。



## 修正

- `2D`: パレット名やブラシ名が長いとタイルパレットの他のUI要素が隠れてしまう問題を修正。
    ([uum-130336](https://issuetracker.unity3d.com/issues/long-tile-palette-name-breaks-window-ui))

- `2D`: 異なる長さの名前を持つ他のパレットやブラシに切り替えると、パレットやブラシのドロップダウンのサイズが変わってしまう問題を修正しました。
    ([uum-132618](https://issuetracker.unity3d.com/issues/tile-palette-dropdown-expands-when-palette-name-is-longer-in-tile-palette-window))

- `2D`: スプライトスキンがカリングされた時にスプライトのちらつきと描画コールが変動する問題を修正。
    ([uum-132924](https://issuetracker.unity3d.com/issues/draw-call-count-fluctuates-and-frame-debugger-output-flickers-when-viewing-a-psd-based-sprite-skin-with-always-update-disabled-in-game-view))

- `2D`: セパレーターを使ってタイルパレットビューを折りたたみ、ブラシビューボタンを使ってウィンドウを拡大した後、タイルパレットウィンドウが極端に拡大される問題を修正。
    ([uum-132739](https://issuetracker.unity3d.com/issues/tile-palette-viewport-becomes-extremely-zoomed-in-after-disabling-a-previously-adjusted-brush-inspector-tab))

- `2D`: ターゲット(Target)、パレット(Palette)、ブラシ(Brush)ドロップダウンの長いターゲット名、パレット名、ブラシ名を切り捨てました。

- `AI`: 半径が小さく、目的地が遠いエージェントのデバッグビジュアライゼーションの描画クラッシュを修正。
    ([uum-133552](https://issuetracker.unity3d.com/issues/crash-on-memcpy-repmovs-when-selecting-navmesh-agent-objects-while-in-play-mode-in-a-specific-scene))

- `DX12`: レンダリングを一時停止することで、プレイヤーで(Alt-Tabで)「Exclusive Fullscreen」ウィンドウを最小化する時の重大なクラッシュを減らしました。他のモードとグラフィックAPIは影響を受けません。より良い安定性のために、"FullScreenWindow"⇄(borderless) mode⇄(https://devblogs.microsoft.com/directx/demystifying-full-screen-optimizations/) の使用を検討してください。
    ([uum-134743](https://issuetracker.unity3d.com/issues/player-crash-when-switching-focus-in-exclusive-fullscreen-mode-with-directx-12))

- `Editor`: パブリッシング設定/WebAssembly言語機能のメモリ設定を0以下にならないようにクランプした。
    ([uum-134687](https://issuetracker.unity3d.com/issues/memory-related-fields-in-the-webassembly-language-features-can-be-set-to-the-negative-numbers))

- `エディター`: Win64プラグインの古いメタファイルをアップグレードするとプラグインが無効になる問題を修正。
    ([uum-137610](https://issuetracker.unity3d.com/issues/win64-cpu-is-set-to-none-when-applying-changes-to-plugin-where-the-meta-has-the-serializedversion-2))

- `エディター`: ビルドプロファイルウィンドウの適切な動作を保証するために、buildprofilecontext.assetがロードできない場合に再作成するようにしました。
    ([uum-136377](https://issuetracker.unity3d.com/issues/nullreferenceexception-and-empty-build-profiles-window-when-buildprofilecontext-dot-asset-contains-invalid-script-reference))

- `エディター`: 特定の ScriptableObject アセット名が、ビルド・プロファイル・ウィンドウを開く際に警告を発生させることがなくなりました。
    ([uum-135389](https://issuetracker.unity3d.com/issues/scriptableobject-asset-is-accessed-during-the-lookup-of-build-profiles-when-opening-the-build-profiles-window))

- `Graphics`: UAV上でシェーダー型ロード/ストアを行う際に、指定されたハードウェア上の フォーマットサポートをチェックするための SystemInfo.SupportsTypedUAVShaderLoadStoreOnGraphicsFormat( \) を追加。DX11 と DX12 に適用可能。
    (UUM-101875)

- `Graphics`: Adreno デバイス上で GPU スキニングを使用した際のクラッシュを修正。
    ([UUM-93243](https://issuetracker.unity3d.com/issues/crash-on-apigles-clearbuffersubdata-when-running-the-player-a-second-time-on-meta-quest-2))

- `Graphics`: 一部の Adreno Vulkan ドライバで未使用の頂点属性を持つシェーダを使用するとクラッシュする問題を修正しました。
    (UUM-137056)

- `Graphics`: Android でコマンドプールがメモリ不足になった時に発生するクラッシュを修正しました。
    ([UUM-125566](https://issuetracker.unity3d.com/issues/vulkan-the-memory-allocation-increases-rapidly-when-there-are-multiple-three-or-more-real-time-reflection-probes-in-the-scene))

- `Graphics`: DirectX11でレンダーテクスチャの代わりにcamera.SetTargetBuffers(￤)で設定した時、GrabPassがrectサイズを正しく設定しないのを修正。
    ([uum-135889](https://issuetracker.unity3d.com/issues/grabpass-does-not-correctly-set-the-rect-size-when-set-up-with-a-camera-dot-settargetbuffers-instead-of-a-render-texture-in-directx11))

- `Graphics`: Metal グラフィックス API を使用している場合に、STP アップスケーリングでダイナミック解像度を使用するとグラフィカルが破損する問題を修正しました。
    (UUM-136227)

- `Graphics`: Vulkan使用時に一部のAdreno 7xxドライババージョンで不正なUVを修正しました。
    ([UUM-126477](https://issuetracker.unity3d.com/issues/android-vulkan-the-uv-quad-is-displayed-incorrectly-with-vulkan-on-a-specific-device))

- `IL2CPP`: libil2cpp コードの C++ 警告を修正。
    (UUM-138294)

- `Physics`: RigidbodyにForceMode.Accelerationによる加速度が適用され、回転が拘束されている場合に発生するNaN値を修正しました。この問題は、Physics.Simulate を手動で呼び出した場合によく発生します。
    (UUM-103515)

- `シェーダー`: シェーダーを保存する際にクラッシュすることがあったのを修正しました。
    ([UUM-133627](https://issuetracker.unity3d.com/issues/crash-on-enumeratedisabledkeywordsinvariantsarray-or-unity-xxh32-when-rapidly-saving-shadergraph-or-vfxgraph-changes))

- `テキスト`: UITKにhideSoftkeyboardオプションを追加し、物理キーボードとタッチスクリーンキーボードを同時にアクティブにするオプションを追加。
    (UUM-122340)

- `テキスト`: 物理キーボードの言語切り替えが正しく動作しない問題を修正。
    ([UUM-130105](https://issuetracker.unity3d.com/issues/android-legacy-tmp-and-ui-toolkit-input-field-language-toggle-to-some-non-latin-alphabet-languages-does-not-work-with-external-keyboard))

- `UI Toolkit`: Microsoft Basic Renderer の UITK GPU パフォーマンステストを無効にしました。
    (UUM-137559)

- `UIツールキット`: 開始色が透明な場合にボーダー色の遷移が機能しない問題を修正。
    ([UUM-136876](https://issuetracker.unity3d.com/issues/border-is-not-rendered-when-transition-duration-is-set-and-border-color-is-transparent))

- `XR`: テクスチャ圧縮ターゲティングを有効にして Meta Quest アプリケーションをビルドして実行する際の問題を修正しました。
    ([uum-131974](https://issuetracker.unity3d.com/issues/meta-quest-player-stuck-at-splashscreen-when-build-app-bundle-and-split-application-binary-are-enabled-with-multiple-texture-compression-formats))




## 6000.0.73f1 におけるパッケージの変更点

## 更新されたパッケージ

- `com.unity.burst`: [1.8.28](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) から [1.8.29](https://docs.unity3d.com/Packages/com.unity.burst@1.8//changelog/CHANGELOG.html) へ。

- `com.unity.recorder`: [5.1.5](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) から [5.1.6](https://docs.unity3d.com/Packages/com.unity.recorder@5.1//changelog/CHANGELOG.html) へ。

- `com.unity.services.authentication`: [3.6.0](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.6//changelog/CHANGELOG.html) から [3.6.1](https://docs.unity3d.com/Packages/com.unity.services.authentication@3.6//changelog/CHANGELOG.html) に変更。

- `com.unity.test-framework.performance`: [3.3.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.3//changelog/CHANGELOG.html)から[3.4.0](https://docs.unity3d.com/Packages/com.unity.test-framework.performance@3.4//changelog/CHANGELOG.html)

- `com.unity.timeline`: [1.8.10](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)から[1.8.12](https://docs.unity3d.com/Packages/com.unity.timeline@1.8//changelog/CHANGELOG.html)