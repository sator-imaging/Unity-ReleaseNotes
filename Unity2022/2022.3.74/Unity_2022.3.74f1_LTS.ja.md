# Unity 2022.3.74f1 LTS
公開日時: Wed, 11 Mar 2026 10:15:36 GMT
https://unity.com/releases/editor/whats-new/2022.3.74f1

# 2022.3.74f1 の既知の問題



* iOS/tvOs：iOS/tvOs:UISceneの要件により、2022.3.72f1以降iOS/tvOS 13が新しい最小値であるにもかかわらず、ターゲットとなるiOS/tvOsの最小バージョンが12と表示される。UISceneをサポートしていないiOS12デバイスでのクラッシュを避けるため、手動で13に上げてください。
* メタル：  コマンドバッファのタイムアウトエラー後にゲームがフリーズする
([uum-125778](https://issuetracker.unity3d.com/issues/metal-game-freezes-after-command-buffer-timeout-error-1))
* Metal：プレイモードのエディターの最小プロジェクトで macOS が吃音する。
([uum-85256](https://issuetracker.unity3d.com/issues/macos-stutters-in-a-minimal-project))
* ビデオ：2022.3.X 用の修正: VideoPlayer が特定の Android デバイスで、Video を複数回有効/無効にすると、フリーズまたは停止する。
(UUM-112470)
* Windows：Windows: "バックグラウンドで実行 "が有効で、アクティブなウィンドウが切り替わると、 Player がハングする。
([UUM-130495](https://issuetracker.unity3d.com/issues/player-hangs-when-the-run-in-background-is-enabled-and-active-window-is-switched))



# 2022.3.74f1 リリースノート

## 機能

* エディター：洞察力とエンジン診断を追加（デフォルトではオフ）。


