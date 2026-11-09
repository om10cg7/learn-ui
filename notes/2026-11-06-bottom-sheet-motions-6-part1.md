# ボトムシートの演出6種 Part 1（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のリール「Bottom Sheet Part 1」（2026-11-04投稿）
  - https://www.instagram.com/reel/DfWBEVCggI9/
  - 内容は動画解析で確認。同作者のタブバー／ボタン／通知に続くモーション見本帳シリーズ。プロンプトはプロフィールリンクで配布
- 関連：notes/2026-11-04-ui-components-navigation-8.md（Bottom sheet の「いつ使うか」）

## 6種

| # | 名称 | 動き |
|---|------|------|
| 1 | Snap Points | ドラッグで覗き見（peek）・半分・全高の定位置にスナップする |
| 2 | Drag to Close | 下へ引っ張ると閉じる |
| 3 | Rubber Band | 上限を超えて引くとゴムのような抵抗がかかる |
| 4 | Mini Player | 小さなプレイヤーが展開してフルプレイヤーのシートになる |
| 5 | Keyboard Lift | コメント欄タップでキーボードが上がり、シートも一緒に持ち上がる |
| 6 | Floating Card | カードがバネでカスケード状にせり上がる |

## 学び

- タブバー回が「見た目の演出」中心だったのに対し、こちらはドラッグやスナップなど「操作への応答」のパターン集。特に Rubber Band のような「限界を超えたら抵抗で知らせる」フィードバックは、物理感のあるUIの基本形
- 実務との対応：Snap Points は地図アプリ、Mini Player は音楽アプリ、Keyboard Lift はコメント入力の定番
