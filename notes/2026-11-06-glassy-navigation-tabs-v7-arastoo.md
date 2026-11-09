# グラス質感のナビゲーションタブ V7（Arastoo）

- 出典：Instagram @arastoo のリール「Glassy Navigation Tabs V7」（2026-11-06投稿）
  - https://www.instagram.com/reel/DfZr3GkTD8a/
  - 内容は動画解析で確認。ソースコード全文は「Code」コメントで配布の形式
- 関連：notes/2026-11-06-liquid-glass-footer-arastoo.md（同じ作者）、図鑑のタブバーアニメーション／リキッドグラス系カード

## 中身

- 暗いリビング（大型TV）の画面を背景に、半透明のピル型ナビゲーションバーを表示するデモ
- 1段目：Home／Discover／Library／Messages／Profile、2段目：User／Overview／Projects／Alerts／Settings。カーソルが通ると紫のグローでハイライト
- 下にはモバイル風の小型バーも併置（Home／検索／お気に入り／プロフィール／カート＋通知バッジ）
- 実装は React + TypeScript + Tailwind CSS + lucide-react（画面下のコードエディタで一部表示）

## 学び

- フッター回に続いて「グラス×定型ナビ」の作例。タブバー系の既存ノート（ui_motion_prompts のスライディングピル等）がモバイル前提なのに対し、こちらはTV画面のような大画面・ポインタ操作前提のタブ
- V7 と版を重ねている点からも、同じ部品を質感違いで量産するポートフォリオ型の発信スタイル
