# メニュー開閉モーション6種 Part 4（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のリール「Menu Part 4 — six ways to open a menu, drawn in pencil」（2026-11-09投稿）
  - https://www.instagram.com/reel/DfjNoNsDHNZ/
  - 内容は動画解析で確認。鉛筆描き風（線画・モノクロ）の画面で、HOME／EXPLORE／LIBRARY の遷移を6パネルでループ実演。各パネルのラベルは解析で読み取れた正式名
  - このチャット（振り分け）経由で受領し、仕分けルール（url_repo_router）で learn-ui 行きと判定して作成
- 関連：同作者の Part 2 notes/2026-11-09-menu-motions-6-part2.md。鉛筆描き風の再演は同作者の「ボタンの演出 Part 4」と同系統

## 6種

1. **PUSH BACK** — 画面全体が奥へ引けて、メニューが現れる
2. **KEBAB POPOVER** — ケバブボタン（縦3点）からポップオーバーが開く
3. **GOOEY MENU** — 粘液のようにつながって広がるグーイーな開き方
4. **FOLD DOWN** — 上から折りたたみがほどけるように下りてくる
5. **BUTTON TO PANEL** — ボタン自体がパネルへ変形する
6. **COMMAND PALETTE** — コマンドパレット型（検索付きのオーバーレイ）

## 学び・所感

- Part 2 が「開閉の動き」のバリエーションだったのに対し、Part 4 は動きと「メニューの形式」そのもの（ポップオーバー／パレット／変形）が混ざっている。6 のコマンドパレットはモーションというより UI パターン寄り
- 1 PUSH BACK は奥行きで階層を伝える型で、ドロワーと違い「下の画面がまだそこにある」感が残る。5 BUTTON TO PANEL は起点と結果が同一オブジェクトなので、どこから開いたか迷わない
- 鉛筆描き風の線画で見せると、色や質感に惑わされず動きの骨格だけを比較できる。シリーズの Part 4 がこの様式なのは「人気パターンの様式替え再演」という位置づけ
