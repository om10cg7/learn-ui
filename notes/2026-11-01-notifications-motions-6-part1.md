# 通知（トースト・アラート）の演出6種 Part 1（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のリール「Notifications Part 1 — toast & alert animations for your app」（お知らせの演出 その1、2026-11-01投稿）
  - https://www.instagram.com/reel/DfMymirDBxv/
  - 内容は動画解析とサムネイル（全パネルの英字説明）で確認。各パネルのラベルと説明はサムネイル表記ママ
  - このチャット（振り分け）経由で受領し、仕分けルール（url_repo_router）で learn-ui 行きと判定して作成

## 6種

1. **Island Expand** — 黒いピル（粒）がバネで開いて、アバターと再生中の波形を持つカードになる（Mika のボイスメッセージ 0:12）。「A black pill springs open into a card with an avatar and a live waveform.」
2. **Stacked Toasts** — 新しいトーストが上から滑り込み、古いものは後ろで縮む。タップで扇状に広がる。「New toasts slide in on top, older ones shrink behind. Tap to fan out.」
3. **Swipe to Dismiss** — トーストがポップアップし、横にドラッグして少し傾けて放り投げるように消す（配達完了の通知）。「A toast pops up. Drag it sideways and fling it off with a slight tilt.」
4. **Countdown Ring** — 右から滑り込み、×印の周りのリングがカウントダウンしてから消える（「Team sync in 5 min」）。「Slides in from the right. A ring around the × counts down, then fades.」
5. **Bell Badge** — ベルが揺れ、「3」のバッジがポップし、プレビューの吹き出しが育つ（新規フォロワー）。「The bell swings, a "3" badge pops, and a preview bubble grows out.」
6. **Copied HUD** — 「Copy link」をタップするとガラス質の HUD がポップし、手前のコピーアイコンが滑り出る。「Tap "Copy link": a glass HUD pops and the front copy icon slides out.」

## 学び・所感

- 6種は「出方」ではなく通知のライフサイクルの局面ごとに分かれている：出現の変形（1）、複数同時の捌き方（2）、消し方のジェスチャ（3）、自動消滅の残り時間の見せ方（4）、未読の集約（5）、操作完了のフィードバック（6）。通知UIの設計チェックリストとして使える
- 2 Stacked Toasts は「古いものを後ろで縮める」ことで件数を保ったまま場所を空ける解法。タップで fan out する展開も含め、積み重ねの圧縮と展開がセットになっている
- 4 Countdown Ring は自動で消える通知に「あと何秒か」を付けたもの。消える前に読ませる・留める判断をユーザーに渡す設計で、×の周りのリングという置き場所も小さい
- 6 Copied HUD は通知ではなく操作フィードバック側で、「コピーできた」という1回きりの確認をガラス HUD で返す。トーストと HUD の使い分けの例として置かれている
- 1 Island Expand は Dynamic Island 系の「常駐ピルが文脈で開く」形。ボイスメッセージの波形まで中に入れており、通知と再生中インジケータの合体になっている
