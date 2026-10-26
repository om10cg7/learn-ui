# UI勉強ノート 2026-10-26（ダッシュボードUI編）

uiux.build の作品投稿「FlowFin — Financial Dashboard UI/UX」の画面を読み解くメモ。画像を実際に確認してUI要素を認識した。

## 出典

- uiux.build の単独画像投稿（財務管理ダッシュボードのデザイン作品）
  - https://www.instagram.com/p/DeYjte4NqnX/
  - 目的：請求書管理、支払い状況、収益分析をシンプルに見せるSaaSダッシュボード

## 画面構成（UI認識）

全体は「上部ヘッダー＋左サイドバー＋メインエリア」の典型的なダッシュボードレイアウト。基調色は白と薄いラベンダーグレーで、紫（インディゴ）がアクセント。

### ヘッダー
- 左：FlowFin のロゴ
- 中央：タブ型ナビ（Overview が選択中で下線、Invoices / Payments / Customers / Reports / Settings）
- 右：検索ボックス「Search anything...」、通知ベル（赤ドット付き）、設定ギア、ユーザー（Darpan Ganotra / Admin）のアバターとドロップダウン

### 左サイドバー
- メニュー：Dashboard（選択中は紫のピル型ハイライト）、Invoices、Payments、Customers、Reports、Analytics、Integrations、Settings。アイコン＋ラベルの統一リスト
- 下部：「Upgrade to Pro」カード（Upgrade Now ボタン）と「Need help? support@flowfin.com」の導線を固定配置

### メインエリア
1. **タイトル行**：「Financial Overview」＋説明文、右上に期間セレクタ（Oct 1, 2025 – Oct 31, 2025）
2. **KPIカード ×4**（カード内にミニグラフ付き）
   - Outstanding Invoices $48,750.00（先月比の変化率＋棒スパークライン。カードだけ濃い紫で強調）
   - Upcoming Payments $32,680.00（+8.2%）
   - Average Payment Time 12 days（-3 days、折れ線スパークライン）
   - Available Balance $1,24,860.00（+15.4%、波形ライン）
3. **フィルタバー**：Customers / Payment Status / Date Range のドロップダウンと、請求書検索フィールド
4. **Invoices パネル**（濃紺の大きなパネルで画面の主役に）
   - 左：一覧リスト（12件）。行ごとに顧客イニシャルのアバター、請求書番号・日付、顧客名、金額、ステータスバッジ
   - ステータスの色分けバッジ（ピル型）：Pending＝黄、Paid＝緑、Overdue＝赤
   - 中央：選択中 INV-1042（Acme Corp）の詳細。発行日・期限・合計、明細テーブル（UI/UX Design $6,000 / Frontend Development $4,500 / Project Management $1,950）、Notes、小計・税・合計
   - 右：Payment Status、Download Invoice / Send Reminder ボタン、Client Details（担当者・メール・電話）
   - 右上：主アクション「+ Create Invoice」ボタンとケバブメニュー
5. **下段カード ×2**
   - Revenue Analytics：Total Revenue $1,28,450 / Total Expenses $62,320 / Net Profit $66,130（増減率付き）＋月別（Jan–Dec）の Revenue vs Expenses 棒グラフ、「This year」切替
   - Payment Breakdown：ドーナツチャート（中央に合計 $1,24,860）＋凡例 Credit Card 48% / Bank Transfer 32% / Digital Wallet 20%

## 学び（UIパターンとして）

- **マスター・ディテール型レイアウト**：左で一覧を選ぶと中央・右に詳細とアクションが出る。大量の請求書を扱う業務UIの王道。
- **色の役割分担**：通常面は白、重要パネルは濃紺、選択・主要ボタンは紫、状態は黄/緑/赤。色に意味を持たせると一目で状況が分かる（図鑑の「ダークUI」「ピル（チップ）」の実例）。
- **KPIカードには必ず文脈を付ける**：大きい数字＋前月比の変化率＋スパークラインの3点セットで「良いのか悪いのか」まで伝わる。
- **ベントーグリッド的な配置**：大きさの異なるカードを並べて、情報の優先順位（KPI→一覧/詳細→分析）を視線の流れに合わせている。
- 細かい点：金額が $1,24,860 のようにインド式桁区切り（ラーク方式）になっている。国・地域で数字の書式も変わるという実例。
