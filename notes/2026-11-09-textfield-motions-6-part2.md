# 入力欄（テキストフィールド）の演出6種 Part 2（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のリール「Text Field Part 2 — more text field animations for your app」（2026-11-05投稿）
  - https://www.instagram.com/reel/DfYRPKEDSDJ/
  - 内容は動画解析で確認。無料プロンプトは ui-motion-prompts.pages.dev（プロフィールリンク）
- 関連：Part 1 は notes/2026-11-08-textfield-motions-6-part1.md（Floating Label／Live Validation 等の基本形）。Part 2 は用途特化型の回

## 6種

1. **OTP Code** — 6つのボックスが順に埋まり（作例：4 8 2 9 1 3）、最後に「Verified」状態になる認証コード欄
2. **Card Number** — 打つそばから数字が4桁ずつグルーピングされ、有効期限欄がスライドインしてくるカード番号欄
3. **Password Strength** — 新パスワード欄。「Sunset42!」の入力に連れて強度メーターが満ち、弱→強で色が変わる
4. **Auto Grow** — メモ欄が改行に合わせてバネ感のある動きで縦に伸びる
5. **Tag Input** — 打った語（design／motion／ui／prompts）がチップ化され、個別に削除できるタグ欄
6. **Ghost Complete** — メールアドレスの候補がグレーで薄く先行表示され、タップで確定（白）になるゴースト補完

## 学び・所感

- Part 1 が「汎用フィールドの状態演出」だったのに対し、Part 2 は「入力形式ごとに決まった作法がある欄」の集まり。OTP・カード・パスワード強度はいずれも"入力しやすさ"の型が確立している領域
- 2 Card Number の自動グルーピングは、視認性だけでなく入力ミス（桁数違い）の検知にも効く実務パターン。有効期限欄のスライドインは「次に何を入れるか」を逐次見せる段階開示
- 3 の強度メーターは Part 1 の Live Validation の親戚で、「送信後エラー」ではなく「打っている最中のフィードバック」という同じ原則
- 6 Ghost Complete は補完候補の確定を「タップ」に割り当てているのが要点で、Tab確定のキーボード前提にしないモバイル向けの作法
