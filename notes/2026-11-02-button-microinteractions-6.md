# ボタンのマイクロインタラクション6種（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のリール「Button Part 2」（2026-11-01投稿）
  - https://www.instagram.com/reel/DfMXIvrG9Fq/
  - テーマ：「buttons that do something after the tap」タップの「後」に何かが起きるボタン。内容は動画解析に基づく
- 関連：notes/2026-11-02-tab-bar-animations-6.md（同じ作者のタブ編）、InfiWeb Craft の削除ボタンUX

## 6種の演出

1. **Hold to Confirm**：ゴミ箱アイコンを長押しするとリングが満ちて、チェック＋「Deleted」に変わる（削除の確認）
2. **Paper Plane**：タップで紙飛行機が飛び、ラベルが「Sent!」に変わる（送信完了）
3. **Confetti Burst**：「Celebrate」をタップすると紙吹雪が弾ける（お祝い）
4. **Copy Feedback**：コピーアイコンをタップするとリンクがコピーされ「Copied!」ツールチップ（フィードバック）
5. **Shine Sweep**：「Upgrade to Pro」に斜めの光沢が流れる（アップグレード誘導）
6. **Slide to Confirm**：スライダーを最後まで引くと「Confirmed」（確定操作）

## 学び

- 共通の型は「操作 → 状態変化の見える化」。結果がボタン自体の変化で返ってくるので、トーストや画面遷移なしに完了が伝わる
- 取り消しにくい操作には「長押し（1）」「スライド（6）」という摩擦のある確定方式を使うのが実務的。誤タップ防止と演出を兼ねる
- 5の Shine は唯一「押す前」の演出（注目を集める側）。演出は押す前＝誘導、押した後＝フィードバック、と役割で分けられる
