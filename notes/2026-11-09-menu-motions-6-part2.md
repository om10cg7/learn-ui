# メニューの開閉アニメーション6種 Part 2（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のリール「Menu Part 2 — menu open & close animations for your app」（2026-11-02投稿）
  - https://www.instagram.com/reel/DfPXXuZD-1K/
  - 内容は動画解析で確認。ダーク背景に6パネルのグリッド、各パネルがメニューの開閉をループ実演（紫アクセント）
  - このチャット（Threads要約）経由で受領し、仕分けルール（url_repo_router）で learn-ui 行きと判定して作成
- 関連：同じ作者のシリーズ notes/2026-11-08-glass-menus-6-me20.md、メニューの見た目側 notes/2026-10-29-mobile-menu-styles-8.md

## 6種

1. **Push Back** — ページ全体が縮んで右へ寄り、脇からサイドメニューが現れる
2. **Kebab Popover** — 「…」がポップオーバーに広がり、Edit／Share／Delete が出る
3. **Gooey Menu** — ハンバーガーアイコンが粘るように分裂して丸ボタン群になり、ぱっと戻る
4. **Fold Down** — Categories のドロップダウンが紙をめくるように行ごとに展開
5. **Button to Panel** — 「+ New」ボタン自体が Create パネル（Note／Photo／Event）に成長する
6. **Command Palette** — 検索バーが降りてきて、入力（"set"）に合わせて結果が stagger で並ぶ

## 学び・所感

- 軸は「開く対象の大きさ」：2 はその場の小さなポップオーバー、4 はリストの展開、5 はボタン→パネルの変形、1 は画面遷移級、6 はアプリ全体を覆うパレット。開く範囲が大きいほど「戻る」操作の明示が重要になる
- 5 Button to Panel は、同作者の他シリーズでも繰り返し出る「要素がそのまま変形する」型。ボタンとパネルが地続きなので、開いた後の文脈（何を作る画面か）を失わない
- 3 Gooey は実務では重い演出だが、ブランド系・遊びのあるアプリではアイコン自体が記憶に残る。速度と粘りの調整が肝
