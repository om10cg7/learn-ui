# ダイアログの演出6種 Part 1（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のリール「Dialog Part 1 — six ways a confirm dialog can enter and leave」（2026-11-09投稿）
  - https://www.instagram.com/reel/DfikgDPgqpF/
  - 内容は動画解析で確認。ファイル削除の確認ダイアログを題材に、出現（と退場）の演出6種を2×3グリッドで実演。背後のアプリ UI では Trip notes.pdf／Budget plan.xlsx／Beach photo.jpg の3ファイルが切り替わる。各パネルのラベルは解析で読み取れた正式名
  - このチャット（振り分け）経由で受領し、仕分けルール（url_repo_router）で learn-ui 行きと判定して作成
- 関連：同じ作者のシリーズ notes/2026-11-09-datepicker-motions-6-part1.md、notes/2026-11-09-menu-motions-6-part2.md

## 6種

1. **Scale Pop** — 72%から拡大してポップに出現する（定番のスケールイン）
2. **Spring Drop** — 上からバネの効いた落下で入ってくる
3. **Hinge Swing** — 上端を蝶番（ヒンジ）にして、ぶら下がるようにスイングして開く
4. **Line Unfold** — まず線が開き、そこから面が満ちてダイアログになる
5. **Soft Focus** — ぼけ（ブラー）からピントが合って現れる
6. **Wobble In** — ゼリーのように揺れながら入ってくる

## 学び・所感

- 確認ダイアログは「注意を引く」ことが仕事なので、動きの強さの配分が他パーツと逆になる。1 Scale Pop と 5 Soft Focus は邪魔をしない穏当枠、2 Spring Drop と 6 Wobble In は遊びが強く、削除のような重い確認には 6 は軽すぎる、という使い分けが実務判断になる
- 3 Hinge Swing は「上から吊られた看板」の連想で、画面端に起点がある分、どこから来たかが分かりやすい。4 Line Unfold はボタンや行から線が伸びる形にすると、起点（どの操作への確認か）との接続が作れる
- シリーズ共通の型として、題材が「削除確認」という具体的な場面に固定されているのがよい。汎用の出現演出集より、文脈込みで転用しやすい
