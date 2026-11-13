# ボタンのタップ演出6種 Part 1（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のリール「Button Part 1 — tap animations for your app」（ボタンの演出 その1、2026-10-31投稿）
  - https://www.instagram.com/reel/DfKwGKqDzOT/
  - 内容は動画解析とサムネイル（全パネルの英字説明）で確認。各パネルのラベルと説明はサムネイル表記ママ
  - このチャット（振り分け）経由で受領し、仕分けルール（url_repo_router）で learn-ui 行きと判定して作成

## 6種

1. **Press Down** — 押すとボタンが濃い土台側へ沈み、バネで戻る（「Continue」）。「Button sinks into its darker base on press, then springs back up.」
2. **Ripple** — タップした正確な点からインクの波紋が広がり、内側で消える（「Get started」）。「An ink ripple spreads from the exact tap point and fades inside.」
3. **Glow Pulse** — ネオンのリングが静かに呼吸し、押すと閃いて光のパルスを外へ送る（電源アイコン）。「Neon ring breathes softly, then flashes and sends a pulse of light out.」
4. **Jelly Bounce** — タップで平たく潰れ、ゼリーのように震えて落ち着く。「Squishes flat on tap, then wobbles like jelly until it settles.」
5. **Load & Success** — 円に縮んでスピナーになり、✓がポップしてから幅が戻る（「Submit」）。「Shrinks into a circle with a spinner, then a ✓ pops and it widens back.」
6. **Expand Morph** — 丸い「＋」ボタンがピル形に伸び、「New post」の文字が滑り込む。「Round + button stretches into a pill as "New post" slides in.」

## 学び・所感

- 6種は「押した感触」の種類で分かれている：物理的な沈み（1）、触れた点の可視化（2）、待機中も生きている常時演出（3）、素材感の誇張（4）、処理状態まで含めた状態遷移（5）、形そのものの変形（6）。ただ気持ちいいだけでなく、役割が違う
- 5 Load & Success はボタンの演出というより非同期処理のフィードバック設計そのもの。送信→処理中→成功をボタンの形の変化で完結させ、画面遷移なしに結果まで伝える
- 2 Ripple は Material 系の定番だが、「タップした正確な点から」という出発点の指定が本体。中心から広がる波紋とは意味が違う
- 3 Glow Pulse は押す前の「呼吸」が主役で、CTA に視線を集める常時アニメーション。押した瞬間の閃光とパルスで常時と反応が地続きになっている
- 6 Expand Morph は FAB の展開パターン。アイコンだけの丸からラベル付きピルへ伸ばすことで、押す前に意味を伝え直している
