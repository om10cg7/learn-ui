# Glassy Dashboard V7（Arastoo / code.xr）

- 出典：Instagram @code.xr（Arastoo）のリール「Glassy Dashboard V7 — Premium Glassmorphism UI」（2026-10-30投稿）
  - https://www.instagram.com/reel/DfHrMboTVDZ/
  - 内容は動画解析で確認。動画内タイトルは「Glassy Dashboard V7 + Crm」
  - 同じ Glassy V7 シリーズの既存ノート：notes/2026-11-08-glassy-sidebar-v7-arastoo.md（サイドバー版）。同作者のダッシュボード系は notes/2026-11-09-dashboard-v25-arastoo.md も参照
  - このチャット（振り分け）経由で受領し、仕分けルール（url_repo_router）で learn-ui 行きと判定して作成

## 内容

紫×白のグラスモーフィズム・ダッシュボード（CRM 寄り）。半透明のガラスカードを、ぼかした暖色のリビングルーム写真の上に重ねる見せ方。技術は React.js／CSS／JavaScript とされ、ソースは「Code」コメントでリンク配布。

動画で切り替わる指標・画面（解析より）:

- Revenue $99,560、Total sales 34、Users 45,500、Orders 98 などの StatCard 群
- Customer intelligence のグラフ
- Performance analytics

画面下にはコードエディタが常時表示され、StatCard コンポーネントが framer-motion と lucide-react を import している（Dashboard V25 と同じ見せ方・同じ部品名）。

## 学び・所感

- V25 との違いは「背景に写真を敷いてガラスの透けを見せる」点。グラスモーフィズムは背景がないと質感が伝わらないので、無地背景の V25 よりこの V7 のほうが様式の要点（背景の透け・ぼけ）が分かりやすい
- シリーズ内では SideBar V7 と対になるダッシュボード本体側。新しい用語・技法の追加はないため、図鑑カードは追加せずノートのみ
- コメント欄には「プレビューできないのに有料なら詐欺では」という懐疑も混じっている（解析より）。「Code」コメント配布系の常として、入手可否は未確認のまま記録する
