# Coinly 支出分析ダッシュボードUI（UI認識）

- 出典：Instagram @orbixdashboard（Orbix Studio）のカルーセル（全5枚：全体図＋クローズアップ3枚＋連絡先）
  - https://www.instagram.com/p/DekIudmlPv5/
  - 本人指定の4枚目は斜めアングルのクローズアップ。1〜3枚目も同じ「Analytics」画面の切り取り違い
- 関連：図鑑の「マスター・ディテール」カード、notes/2026-10-26-dashboard-ui.md（FlowFin）

## コンセプト（投稿文より）

「お金がどこへ消えたか」は明細を1行ずつ追えば分かるが面倒。Coinlyは2つの軸を並べて答える：
- カテゴリ（Category）＝習慣：何の種類の支出が一番大きいか
- マーチャント（Merchant）＝場所：実際に誰に払ったか

明細を1件も開かずに、1か月の支出が説明できる、という設計思想。

## 画面構成（全体図の目視確認）

- ヘッダー：ロゴ、「Search or jump to」（⌘K）、「Move Money」、通知、アバター
- サイドバー：左端の細いアイコンレール（名称ラベルは読み取り不可、最下部に設定らしき歯車）
- 見出し：Analytics／「Track your financial performance and insights」、期間「Apr 24, 2026 - May 28, 2026」、「Export Report」
- KPIカード5枚（すべて「Vs last 30 days」付き）：
  1. Total Balance $3,120.00（+4.27%）
  2. Total Income $4,580.00（+2.89%）
  3. Total Expenses $1,995.00（変化率は読み取り不可）
  4. Net Savings $3,750.00（+3.78%）
  5. Transactions 56（+1.94%）
- 中段：左「Balance Overview」（Income=オレンジ／Expense=青の2本折れ線＋下部に棒、ツールチップ例：May 2026 Income $4,120.00／Expense $3,234.00）、右「Spending by category」（円グラフ）
- 下段：左「Top Spending merchants」（横バー）、中央「Income vs Expense」（半円ゲージ）、右「Cash flow Trend」（折れ線）
- 全パネルに共通で「Last 30 days」フィルター表示

## カテゴリ別支出（円グラフ）

- Daily Needs 40%、Savings 20%、Transport 20%、Shopping 10%、Others 10%

## 上位マーチャントの見せ方

ロゴ＋名称（左）、金額＋％（右）、名称の下にマーチャント色のプログレスバー：
- Amazon：$23,628（80%）緑バー
- Starbucks：$18,543（70%）オレンジバー
- Apple Store：$16,543（60%）紫／青バー

## 気づき・注意

- ゲージ中央の「Net Savings $1,750.00」はKPIカードの $3,750.00 と画面上で食い違う（理由は読み取り不可）。実務のモックでは数値の一貫性チェックが大事という教材的なポイント
- FlowFin（請求書管理）と同じく「左レール＋KPI列＋グラフのパネル群」の王道構成だが、こちらは分析対象を「カテゴリ×マーチャント」の二軸に絞って情報設計の意図を明確にしている

## 学び

- ダッシュボードの価値はグラフの多さではなく「どの問い に答えるか」の明確さ。Coinlyは「何に（カテゴリ）×どこで（マーチャント）」の2問に絞っている
- 全パネルに同じ期間フィルター（Last 30 days）を付けることで、パネル同士を比較可能にしている
- マーチャントバーは「ロゴ＋金額＋％＋色バー」の4要素で、ランキングと規模感が一目で伝わる
