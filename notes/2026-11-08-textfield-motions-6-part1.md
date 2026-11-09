# 入力欄（テキストフィールド）の演出6種 Part 1（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のリール「Text Field Part 1 — input field animations for your app」（2026-11-04投稿）
  - https://www.instagram.com/reel/DfVsg-pgkde/
  - 内容は動画解析で確認。無料プロンプトはプロフィールのリンクから、というこの作者の定型形式
- 関連：同じ作者のシリーズ notes/2026-11-06-bottom-sheet-motions-6-part1.md、notes/2026-11-06-accordion-motions-6-part1.md、notes/2026-11-08-carousel-motions-6-part1.md

## 6種（2×3グリッドで同時デモ）

1. **Floating Label** — 入力を始めるとプレースホルダーがラベルとして上に浮く
2. **Underline Grow** — タップ位置からグラデーションの下線が伸びる
3. **Glow Border** — フォーカスで枠が光る
4. **Live Validation** — 入力中に検証：メール形式が不正な間は赤いヒント、正しくなるとチェックマーク
5. **Password Reveal** — 目のアイコンで伏せ字⇔平文を切り替え
6. **Char Counter** — リングで文字数を数え、上限を超えるとピンクに変わる

デモの入力例：mia@email.com／Mia Park／SPRING25（クーポンコード風）／「Coffee first, then code, always!」

## 学び・所感

- 6種のうち装飾寄りは 2・3、機能寄りは 4・5・6。特に 4 Live Validation は「送信してからエラー」ではなく「打っている最中に状態が返る」設計で、UX上の価値が一番大きい
- 6 Char Counter のリング表示は、残数を数字ではなく円の満ち具合で見せるのが要点。上限超過の色変化（ピンク）とセット
- 1 Floating Label は Material Design の定番だが、「ラベルが消えない」ことで何の欄か常時分かる、という実用理由がある
- Ankida の engineered ボタンの話（notes/2026-11-08-button-behaviours-ankida.md）と地続きで、入力欄も「状態変化をアニメーションでつなぐ」ことが共通テーマ
