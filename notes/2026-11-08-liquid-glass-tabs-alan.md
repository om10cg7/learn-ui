# リキッドグラスのタブ：CSS 8行＋1つのレンズ（Alan Builds）

- 出典：Instagram @alan.build（Alan Builds）のリール「Liquid glass tabs: 8 lines of CSS + 1 lens」（2026-11-06投稿）
  - https://www.instagram.com/reel/DfbdNyjDw30/
  - 内容は動画解析で確認。コード全文は「REPO」コメントで配布の形式
- 関連：同じ作者のボタン版レシピは notes/2026-10-26-glass-button-figma.md の追記（2026-11-01投稿「Liquid glass is just six CSS properties stacked」）。タブ版の本投稿とは別物

## 手順（動画の実演順）

題材はリンク4つ（Home／Code／Design／AI）＋白いピル1つのナビゲーション。

1. **素の状態**：ピルはタブ間で「ジャンプ」する（transition なし）
2. **cubic-bezier の transition を1行**：ピルが滑って移動するようになる
3. **レンズ追加**：`backdrop-filter` に SVG の displacement map（変位マップ）を入れた「lens」を適用し、ピルの背後が**屈折**して見える（ぼかしではなく本物の屈折、というのが作者の主張）。あわせて border で縁（rim）、box-shadow でハイライトを付ける
4. 合計 **CSS 8行** で完成。「どのナビにも貼れる」とのこと

## 学び・所感

- リキッドグラス再現の肝は blur ではなく **displacement（変位）による屈折** という指摘が核心。backdrop-filter: blur() のグラスモーフィズムとは別物で、SVG フィルタを backdrop-filter に噛ませるのが実装上のポイント
- 動きの部分は「ピル＋cubic-bezier 1行」という最小構成で、Vamshi のボトムナビ集の Pill highlight（notes/2026-11-08-bottom-nav-styles-8-vamshi.md）の実装レシピとして読める
- 注意：backdrop-filter への SVG フィルタ参照はブラウザ差がある（特に Firefox の対応状況）。コード全文は未取得なので、実際のプロパティ列は REPO 配布待ち
