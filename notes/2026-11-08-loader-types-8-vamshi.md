# ローダーの種類8種（Vamshi）

- 出典：Instagram @vamshi.work（Vamshi | AI for Designers）のリール「Not every loading state needs a spinner! — 8 types of loaders every UX designer should know」（2026-11-05投稿、いいね1.3万超）
  - https://www.instagram.com/reel/DfXCN_Gqd1a/
  - 内容は動画解析で確認。本人が画面下半分に映って指折り数え、上半分に各ローダーの実演アニメーションを出す分割画面形式
- 関連：同じ作者の notes/2026-11-08-bottom-nav-styles-8-vamshi.md、notes/2026-11-05-designer-websites-54-vamshi.md

## 8種

1. **Spinner Loader** — 円形の回転スピナー（基本形）
2. **Skeleton Loader** — コンテンツの形をしたプレースホルダー
3. **Progress Bar** — 進捗バー（作例はファイルアップロード50％表示）
4. **Pulsing Loader** — 3つのドットが脈打つ
5. **Button Loader** — ボタン内蔵型（「Saving...」の状態表示）
6. **Full-Screen Loader** — 画面全体を覆い中央にスピナー
7. **Pull-to-Refresh Loader** — 引っ張って更新
8. **Infinite Scroll Loader** — 無限スクロールの末尾で追加読み込み

## 学び・所感

- 主張はタイトル通り「全部スピナーにしない」。8種は「待ち時間の性質」で選ぶのが筋：
  - 進捗が分かる処理（アップロード等）→ 3 Progress Bar
  - レイアウトが決まっている読み込み → 2 Skeleton（体感待ち時間を縮める）
  - 押したボタンへの反応 → 5 Button Loader（画面遷移せず、その場で処理中を示す）
  - 区切りがない一覧の継続読み込み → 8 Infinite Scroll
  - 短い・進捗不明の待ち → 1 Spinner か 4 Pulsing
- 6 Full-Screen は「他に何もできない」状態専用で、乱用すると離脱要因になる、という位置づけで見ると使い分けが整理できる
- David Mráz の iOS フィードバック9種（notes/2026-11-08-ios-feedback-patterns-9.md）と合わせると、「処理中フィードバック」の語彙が揃う
