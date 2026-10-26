# UI勉強ノート 2026-10-26（OTP認証UIのリデザイン編）

code.xr（Arastoo）のInstagramリール「OTP Verification, but Version 7」から、ワンタイムパスコード入力画面のマイクロインタラクション設計をメモする。今回の投稿者は uiux.build ではなく code.xr（React/CSS のフロントエンド系クリエイター）。

## 出典

- code.xr のリール（UIデモ動画）
  - https://www.instagram.com/reel/DbavLeDTP5H/
  - 実装は React + CSS。キャプションの特徴リスト：Premium OTP UI、Smooth Micro Interactions、Advanced Success Animation、Auto Focus Navigation。「OTP」とコメントでソースコード配布。

## 画面の流れ（UI認識）

1. ダークテーマのモバイル画面。「Let's verify your number」と、電話番号宛に送られた4桁コードの入力を促す。
2. 4つの入力ボックスに数字（4、5…）が入っていく。入力すると次のボックスへ自動でフォーカスが移る（Auto Focus Navigation）。
3. 入力完了で数字たちがグリッド状にアニメーションし、緑のチェックマーク＋パーティクル（粒子）エフェクトへ遷移。
4. 「Verified Successfully — Your number has been verified. Verified and Secure.」の成功表示。
5. 画面下にはコードエディタ（React/JavaScript）が映り、実装物であることを示す構成。

## 学び

- OTP入力の要点は地味だが効く：自動フォーカス移動、ペースト対応を思わせる滑らかさなど、入力の摩擦を減らすマイクロインタラクションの積み重ね。
- 「成功アニメーション」は気持ちよさ（satisfying）を設計対象にしている好例で、認証のような義務的な手続きでも完了の瞬間に報酬感を作れる。ボタン状態設計編の PROCESSING／成功状態と地続き。
- 一方でコメント欄には実務的な批判もあった：「失敗時はどう見えるのか」「UXの改善になっているのか」。成功状態だけでなくエラー状態（誤入力・期限切れ・再送）まで設計して初めて認証UIとして完成する、という視点もセットで記録する。
- バージョン7まで作り直し続ける反復自体も題材：同じ小さな画面を磨き続ける練習法（リソース編の「毎日1つ模写」に通じる）。
