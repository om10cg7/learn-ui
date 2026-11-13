# スクロールパターン9種 Part 1（David Mráz / @davidm_ai）

- 出典：Instagram @davidm_ai（David Mráz）のリール「Scroll Patterns Overview - PT. 1」（2026-11-12投稿）
  - https://www.instagram.com/reel/DforJnyAYzs/
  - 内容は動画解析とサムネイル（インフォグラフィック全体）で確認。HTML & CSS 前提の3×3グリッド教材で、各パターンに小さなアニメーション見本と一言の定義が付く
  - 作者のシリーズは「Vocabulary for Agentic Coding（エージェントに指示するための語彙）」が看板で、iOS フィードバックパターン9種（notes/2026-11-08-ios-feedback-patterns-9.md）と同じ構図。キャプションも「正確なスクロールパターンを知ることでエージェント型コーディングが上手くなる」
  - 詳細リンクは「Code」コメントで配布（Pass メンバー向け）
  - このチャット（振り分け）経由で受領し、仕分けルール（url_repo_router）で learn-ui 行きと判定して作成

## 内容（サムネイルの一言定義を転記）

1. **Sticky positioning** — Headers pin, then hand off（ヘッダーが留まり、やがて受け渡す）
2. **Scroll snap** — Panels lock into place（パネルが位置に吸着する）
3. **Scroll triggered** — Fades in on enter（入ってきたらフェードイン）
4. **Infinite scroll** — More loads near the end（末尾近くで次が読み込まれる）
5. **Scroll driven** — Progress follows scroll（進捗がスクロールに追従する）
6. **Zoom on scroll** — Image grows as it passes（通過しながら画像が大きくなる）
7. **Parallax** — Background moves slower（背景が遅れて動く）
8. **Horizontal scroll** — Vertical → sideways track（縦スクロールを横移動に変換）
9. **Scrollytelling** — Steps play, scene stays put（場面は留まり、ステップが進む）

## 学び・所感

- 似た言葉の切り分けが核。Scroll triggered は「到達をきっかけに再生」、Scroll driven は「スクロール量そのものが進捗」、Scrollytelling は「固定した場面の上で段階的に語る」と、発火条件と時間の扱いが違う。名前を混同するとエージェントへの指示も実装もずれる
- Sticky の定義が「pin, then hand off」なのが良い。留まることより「次の要素へ受け渡す（積み重なる見出しの交代）」まで含めて1パターンとして扱っている
- 9種は「要素の固定（Sticky／Snap）」「出現の演出（Triggered／Driven／Zoom／Parallax）」「読み進め方そのもの（Infinite／Horizontal／Scrollytelling）」の3群に分けると覚えやすい
- 同作者のページネーション8種と同じく、図鑑には名前カタログとしてカードを追加した（カテゴリは動き・UX原則）
