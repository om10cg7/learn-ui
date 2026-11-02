# AI動画編集Skill：スラッシュコマンドで編集スタイルを適用（david_knowsai）

- 出典：Instagram @david_knowsai のリール（2026-10-28投稿）
  - https://www.instagram.com/reel/DfDlJjAhif-/
  - 未編集のトーキングヘッド素材（take.mov）に、スラッシュコマンドを打つだけで編集済みショート動画のスタイルが適用されるデモ。画面上の表記は「Opus 5.5」
  - キャプション：「Comment "Edit" to get the editing skill」（コメントでSkillを配布する形式）
  - 内容は動画解析に基づく
- 関連：notes/2026-11-02-day-trader-claude-skills.md、2026-10-28 の Claude 動画系Skillまとめ

## コマンド6種 → 生成されるスタイル

1. **/business-short-form-reels**：マルチパネルレイアウトのビジネス系リール
2. **/ranking-format**：ティアリスト（ランキング表）グラフィック付き
3. **/depth-ui-reel**：YouTube Shorts のフィード風UIを模し、再生数が上がっていく演出（〜400,000）
4. **/cutout-grid-reel**：4分割コラージュ（お金のイメージ等）
5. **/explainer-panel-reel**：対比数字（$0 vs $5,000）を出す解説パネル
6. **/personal-short-form-reels**：ロボット掃除機などの商品ショット系

## 学び

- 「編集スタイル＝名前付きコマンド」という Skill 化の発想。Premiere のプリセットではなく、LLMへの指示セットとして編集様式を配布している
- フックは「Write this to get this（これを書けば、これが得られる）」の対比提示。コマンド名そのものが成果物の説明になっている命名が上手い
- 配布方法はコメントキーワード→DM送付のリード獲得型（ai.nxtlvl のデイトレードSkillと同じパターン）
