# Island Carousel — CSS scroll-snap の実演（David Mráz）

- 出典：Instagram @davidm_ai（David Mráz）のリール（2026-10-30投稿）
  - https://www.instagram.com/reel/DfIk43eADPr/
  - 内容は動画解析で確認。自作の Atheros AI Builder（builder.atheros.ai）のコンポーネント紹介。コードは「Code」コメントで配布（キャプションでは Pass+ 会員向け、動画内では24時間無料の表記）
- 関連：同じ作者の notes/2026-11-08-ios-feedback-patterns-9.md

## 中身

- ダークなピル型カルーセル「Island Carousel」が画面上部中央に浮く構成（Dynamic Island 風）。左右矢印でも、スワイプ／スクロールでも送れる
- 中のカードは4種のウィジェット：音楽プレイヤー（「Midnight Drive」Neon Coast）、Focus タイマー（12:45）、Activity（428 kcal、Move／Exercise／Stand リング）、天気（Bergen 18°C、曇り時々晴れ）
- 実装の核は CSS scroll-snap で、動画内でコードも提示：
  - `.track` に `scroll-snap-type: x mandatory`
  - `.card` に `scroll-snap-align: center`
  - 矢印ボタン側は JavaScript でスクロール位置を制御

## 学び・所感

- カルーセルの「吸着」は JS で頑張らず CSS の scroll-snap に任せるのが最小構成。mandatory＋center の2プロパティが要点
- 「ピルの中に複数ウィジェットを横並びにしてスナップで切り替える」という形は、モバイルのウィジェットスタックや Dynamic Island 的な常駐UIの応用として読める
- ui_motion_prompts のカルーセル演出6種（notes/2026-11-08-carousel-motions-6-part1.md）が「見た目の演出」カタログなのに対し、こちらはその実装側（scroll-snap）の話として対になる
