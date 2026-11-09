# 折れ線グラフの切り替え演出6種 Part 1（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のリール「Line Chart Part 1 — one chart, six ways to switch the range」（2026-11-05投稿）
  - https://www.instagram.com/reel/DfW4CtNlJYq/
  - 内容は動画解析で確認。各チャート下の期間切替（W／M／6M／Y）を切り替えたときの線の動きを、2×3グリッドで同時デモ。データ形状は U字の落ち込み→右肩上がり→山型→波型 をループ
- 関連：同じ作者のシリーズ notes/2026-11-08-carousel-motions-6-part1.md、notes/2026-11-08-progress-steps-motions-6-part1.md など

## 6種

1. **LINE MORPH** — 線そのものが形を変形して次のデータへ移る
2. **DRAW ON** — 線が最初から描き直される
3. **DOT HOP** — データ点のドットが跳ねながら移動
4. **STAGGER WAVE** — 波のように遅延しながら（stagger）形が変わる
5. **STEM RISE** — ステム（点から伸びる茎）がせり上がる
6. **SCRUB LINE** — 掃引する縦線（スクラブ）が通って切り替わる

## 学び・所感

- データ可視化では「値が変わった」ことより「どう変わったか」をアニメーションで見せるのが要点。1 LINE MORPH は連続性が保たれるので、期間切替の比較（前期間との形の違い）が一番読み取りやすい
- 2 DRAW ON は毎回ゼロから描くので「再読み込み」感が出る。初回表示や画面遷移時向きで、頻繁な切替には重い
- 3・4 は遊びの要素が強く、金融系の固いダッシュボードよりコンシューマー向け（家計・健康アプリ等）向き
- 期間切替 W／M／6M／Y のような頻繁な操作では、短く・連続性のある 1 か 4 が無難、という判断軸になる
