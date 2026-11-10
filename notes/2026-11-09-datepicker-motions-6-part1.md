# 日付ピッカーの演出6種 Part 1（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のリール「Date Picker Part 1 — same week strip, six ways to pick a day」（2026-11-09投稿）
  - https://www.instagram.com/reel/Dfi5DFtjxMM/
  - 内容は動画解析で確認。2026年11月の週ストリップ（同じ週表示）で、日付を選ぶときの遷移6種を並べ、16日・18日・20日・21日などをタップして繰り返し実演。各パネルのラベルは解析で読み取れた正式名
  - このチャット（振り分け）経由で受領し、仕分けルール（url_repo_router）で learn-ui 行きと判定して作成
- 関連：同じ作者のシリーズ notes/2026-11-09-menu-motions-6-part2.md、notes/2026-11-08-progress-steps-motions-6-part1.md、notes/2026-11-08-textfield-motions-6-part1.md、notes/2026-11-08-rating-motions-6-part2.md

## 6種

1. **Halo Trace** — タップした日を光るリングがなぞって一周し、そのあと色が満ちる
2. **Snap Brackets** — 四隅のブラケットがタップした日へ飛んできて、広がってからパチッと閉じる
3. **Rise & Land** — タップした日が深い影を伴って浮き上がり、スカッシュしながら着地する
4. **Side Wipe** — 色が古い日から抜けて、新しい日へ同じ方向にワイプする
5. **Dot Swell** — 日付の下の小さな点が膨らんで、カプセル全体になる
6. **Twist In** — 新しいカプセルが1/4回転しながらねじれ込む。古い方はねじれて消える

## 学び・所感

- 同じ「週ストリップ」という器で、選択のフィードバックだけを6通り見せる構成。共通するのは「選択マーカー（カプセル）がどう生まれ、どう移動するか」の設計で、色を変えるだけの実装との差はここに出る
- 使い分けの軸：4 Side Wipe と 6 Twist In は旧→新の「移動」を表現するので前後関係が伝わりやすく、1 Halo Trace と 5 Dot Swell はその場の確定感が強い。3 Rise & Land は最も触感寄りで、カジュアルなアプリ向き
- 2 Snap Brackets はカメラのフォーカス枠の連想で「狙って選んだ」感が出る。予約系 UI の確定演出に転用しやすい
