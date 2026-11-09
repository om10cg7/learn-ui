# 「AI OS / Simpl iOS Design」v2.0 コンセプト（Slava Kornilov）

- 出典：Instagram @slava7118（Slava Design Kornilov）のカルーセル（2026-11-08投稿、キャプションは「Code」のみ）
  - https://www.instagram.com/p/Dffr1tuEa1B/
  - 内容は動画解析＋サムネイル目視で確認。全7スライドの動画カルーセル
  - このチャット（振り分け）経由で受領し、仕分けルール（url_repo_router）で learn-ui 行きと判定して作成。AIアプリ生成の話だが、実在ツールの紹介ではなく UI デザインコンセプトのショーケースであるため learn-ui に分類
- 関連：コンセプト系 notes/2026-10-26-modern-app-ui-showcase.md、notes/2026-10-29-florist-app-concept.md

## 内容

「AI の全サービスを管理する、効率化された iOS 体験」というコンセプトデザイン集。核は**プロンプトでアプリを作り、コードではなくキャンバスとしてデザインを編集する**という提案。

スライド構成:

1. カラフルなアプリ UI のグリッド（アラーム、天気、メンバーシップ、分析、月、ウォッチ、リング）
2. アラームアプリの作成フロー（プロンプト入力 → 画面エディタ → カスタムアイコン設計）
3. 分析ダッシュボード群（天気 29° New York、風速、積み上げメトリクス）
4. Moon アプリ（満月の可視化、距離・月齢・高度）
5. ウェアラブル分析（Watch: Balance／Sleep Quality／Mood／Skin Damage、Ring: 露出、自然光 vs 人工光）
6. Membership／Data／Menu ハブ（タスクリスト、メール要約、放射状アイコンメニュー）

合間に挟まるタイトルカードの主張:

- Design, Prompt, Ship
- Edit design like a canvas, not code
- Instantly preview and test
- Export or publish to the App Store
- Iterate with AI in real time
- Apps, as you imagine them

## 学び・所感

- 見せ方の核は「OS 全体を1つのデザイン言語で統一したモック群」。Metrics カード（Balance 85、Sleep 25% など）のグラデーションとドット数字フォントが全アプリ共通で、天気・月・健康が同じ世界に見える
- Alarm 画面の大きな 09:50 と縦バー群、「Create a new application of the alarm clock」という生成入口の置き方など、「アプリを使う」と「アプリを作る」を同じ画面系に同居させる発想がコンセプトの要
- 実在プロダクトではなくコンセプトなので、学ぶ対象は機能ではなく「AI 生成を前提にした UI の見せ方・世界観の作り方」
