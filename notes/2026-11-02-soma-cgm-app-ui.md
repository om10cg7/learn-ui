# 持続血糖モニタリングアプリ「Soma」のUI（rondesignlab）

- 出典：Instagram @rondesignlab のカルーセル（全13枚、2026-10-14投稿）
  - https://www.instagram.com/p/DeeqesTjPuq/?img_index=6
  - 指定6枚目を目視で重点確認（全スライドも目視済み）
  - キャプションのコンセプト：「Your body talks all day. Soma finally translates」
- 関連：notes/2026-11-02-neka-health-app-ui.md（同じスタジオの姉妹作）

## プロダクトの概要

- 腕に貼るパッチ型センサー（SOMA 3 SENSOR）と連動する持続血糖モニタリング（CGM）アプリ
- 血糖のほか、ヘモグロビン、コレステロール、代謝マーカーを1つのセンサーで測る想定
- 糖尿病管理の人にも、代謝の健康を追いたい人にも「検査レポート」ではなく「自分の体の状態」として見せる

## 指定6枚目（センサー詳細画面「CGM Device」）

- 手持ちスマホの傾いたクローズアップ。血糖値ではなく「センサー本体の状態・仕様・接続状態」の画面
- 上部：円形センサーの図解＋ Diam 35 mm、Prot IP68、バッテリー81%、Lev 3.2（略称の意味は読み取り不可）。別アングルの全体像では Mass 4.3 g も確認
- 中央の大きなクリーム色カード：
  - SOMA 3 SENSOR（Gen 3、黄色ドットで「Active」）
  - Expiration 11 / 14 d、Accuracy 98%、Metering 43 times、Signal Strong
  - Expires Jun 8, 09:14／Last sync 11 days ago
- 下部：ヘルプ（?）ボタン、中央に黒いピル型ボタン（スキャン系アイコン）、右端に設定スライダー

## 画面の顔ぶれ（13枚は5画面のバリエーション）

- Statistics：Cholesterol 23/28 days、Energy 74%、Recovery 85%、Hydration 62%、Variability 93、Range 55 mg/dL、Daily Macronutrients
- Metabolic Score：89 mg/dL（▲29 from yesterday）、10:00〜22:00 のグラフ
- CGM Device：センサー詳細（上記）
- GLUCOSE：149 mg/dl（▲6 from 1h ago、Active）、06:00〜22:00 のグラフ
- Glucose Monitoring：Glucose／Hemoglobin／Cholesterol／Metabolic の放射状（ラジアル）メニュー

## デザインの要点

- 配色：臨床的な白×青を捨て、肌色系のベージュ・クリーム・淡黄のグラデーションが基調（キャプションでも明記）
- 大きな数字が主役：血糖値や精度など「1つの数値」を大きく黒字で見せ、変化量（▲29、▲6）は小さく添える
- 角の大きく丸いカードを重ね、左にアイコン＋項目名、右に値。項目と値を点線のリーダー線で結ぶ箇所も
- 人物のシルエットや手持ち端末の写真を背景・前景に使い、医療機器らしさを消している

## 学び

- Neka と同じ設計言語（温色グラデーション＋大きな数字＋状態ラベル）。スタジオの「ヘルスUIの型」が2作で確認できる
- デバイス詳細のような地味な画面でも、スペックを「カード＋状態語」で見せると製品体験の一部になる。ハードの状態表示もUIデザインの対象
- 放射状メニュー（Glucose Monitoring）は測定項目の切り替えを「選ぶ楽しさ」に変える仕掛け
