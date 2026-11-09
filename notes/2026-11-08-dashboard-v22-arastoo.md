# グラス質感のダッシュボード V22（Arastoo）

- 出典：Instagram @arastoo のリール「Dashboard V22」（2026-11-07投稿）
  - https://www.instagram.com/reel/DfcQ2TrTbGV/
  - 内容は動画解析で確認。ソースコードは「Code」コメントで配布の形式（コメント欄では「サイトのコードは有料では」との指摘も出ていた）
- 関連：notes/2026-11-06-liquid-glass-footer-arastoo.md、notes/2026-11-06-glassy-navigation-tabs-v7-arastoo.md（同じ作者）

## 中身

- ライトグリーン×白の分析ダッシュボードUI。ローディング画面から本画面へ遷移
- 要素：メンバーアバター、統計カウンター（00.2h、49、53 など）、通知、最近の動画
- 遷移先：ユーザープロフィール（Hannah Brooke：プロジェクト数、フォロワー、集中時間）、「Saved for later」のカード一覧
- 実装は React + framer-motion + lucide-react（画面下のコードエディタに StatCard コンポーネントの定義が表示）

## 追記：別バージョン V24（2026-11-08）

- 別投稿 https://www.instagram.com/reel/DfeTS2Jzcgx/（2026-11-08）。キャプションの題名は「Glassy Dashboard V22」だが、動画内のタイトルは「Glassy Dashboard V24」で食い違っている
- 中身は別物：挨拶「Good afternoon, Code XR」から始まる分析ダッシュボードで、左サイドバー（Dashboard／Analytics／Team／Schedule／Projects／Activity／Settings／Notifications／Help）、統計カード（完了率94%、進行中プロジェクト128、メンバー49人、収益$42,500、稼働率99.96%）、Analytics 画面の収益チャートまで見せる
- 同じ StatCard コンポーネントの型を使い回し、数値とレイアウトを差し替えた量産バリエーション

## 学び

- 同じ作者の3作目で、グラス適用先がフッター→タブ→ダッシュボード全体へ拡大
- コメント欄の反応が割れているのが教材として面白い：見た目（グラスモーフィズムと青白の配色は高級感がある）への称賛と、「アニメーションが重く実務では使いにくい」「データは動的なのか静的モックか」という実用面の批判。ダッシュボードは日常的に使う道具なので、質感の演出と効率のトレードオフが最も問われる部品、という指摘として記録する
