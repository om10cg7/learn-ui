# ページ送り（カルーセル）の演出6種 Part 1（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のリール「Carousel Part 1 — classic page swipes for your app」（2026-11-05投稿）
  - https://www.instagram.com/reel/DfXFtWEDG5I/
  - 内容は動画解析で確認。無料プロンプトはプロフィールのリンクから、というこの作者の定型形式
- 関連：同じ作者の notes/2026-11-06-bottom-sheet-motions-6-part1.md、notes/2026-11-06-accordion-motions-6-part1.md（いずれも「6種×Part 1」形式のシリーズ）

## 6種（2×3グリッドで同時デモ）

1. **Pill Dots** — ページドットで、アクティブなものだけピル状に伸びる
2. **Snap Peek** — 隣のカードが両端から少しだけのぞく（次があることを示す）
3. **Cover Scale** — 中央のカードが拡大して主役になる
4. **Story Bars** — 上部にストーリーズ式の進行バー
5. **Parallax** — カード内の絵が遅れて動く視差
6. **Page Counter** — 「1/4」のような数字が回転して切り替わるカウンター

デモ素材は4枚のイラスト（紫の山並みと夕景、青い波、緑の庭と花、紫の夜景の街並み）を全パネル共通で巡回させる構成。

## 学び・所感

- 「カルーセルの演出」と一括りにされがちだが、この6種は効く場所が違う：1・4・6 は「現在位置の伝え方」（インジケーター系）、2・3・5 は「送りそのものの感触」（カードの動き系）。実装時は両系から1つずつ選ぶのが自然
- Snap Peek は「続きがある」ことを動きなしで伝える最も安い方法で、初回表示でのスワイプ誘導に効く
- Pill Dots は Vamshi のボトムナビ集（notes/2026-11-08-bottom-nav-styles-8-vamshi.md）の Pill highlight と同じ「ピルで現在地を示す」発想のドット版
