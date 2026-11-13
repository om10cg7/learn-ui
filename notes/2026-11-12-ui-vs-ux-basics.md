# UIとUXの違いを比喩で掴む（@uiuxaadi の教材を @flutterdeviser.agency が共有）

- 出典：Instagram @flutterdeviser.agency のカルーセル「UI VS UX」（2026-11-12投稿、全9枚）
  - https://www.instagram.com/p/DfoxdH-Epd5/
  - 教材のクレジットは表紙に「CREDIT TO @UIUXAADI」とあり、元の制作者は @uiuxaadi（パレット教材で既存ノートあり）。キャプションでも @uiuxaadi を冒頭に掲げている
  - 内容はキャプション、解析、表紙画像の目視で確認
  - このチャット（振り分け）経由で受領し、仕分けルール（url_repo_router）で learn-ui 行きと判定して作成

## 内容

表紙（目視で確認）:

- **UI = High-Fidelity（見える仕上げ）**: Layout／Colors／Typography／Iconography／Spacing／Design Systems／Visual Branding
- **UX = Low-Fidelity（見えない下ごしらえ）**: UX Research／UX Strategy／User Stories／User Personas／Layouts & IA／User Flows／User Testing
- 中央の帯は両者をつなぐ **Design Psychology**: Hick's Law／Gestalt Principles／Color Psychology／Fitt's Law／Jakob's Law／Cognitive Load

残りは比喩で同じ対比を繰り返す構成（解析より）:

- 氷山: UI は水上の小さな一角、UX は水面下の本体（インタラクション設計・テスト・フィードバックを含む）。この比喩は2枚ある
- **サラダとフォーク（指定スライド img_index=2 はこの枚）**: サラダ＝UX（食べる体験の中身）、フォーク＝UI（それを掴むための道具）
- 骨格と赤いドレス: UX は骨組み（構造）、UI は見た目
- 家: UX は間取り（キッチンをどこに置くか＝設計図）、UI は色
- ベビーモバイル: 親から見える可愛い動物が UI、赤ちゃん側から見える裏側が UX（視点で見えるものが違う）
- ハリネズミのマグ: 見た目は良い（UI）が飲みにくい（悪い UX）

最終スライドは投稿アカウントの Flutter 電子書籍「The Ultimate 2300+ Page Guide to Mastering Flutter」（2300ページ超、₹149／$4.99、投稿表記ママ）の宣伝。キャプションでは Figma のワークシートを「uiux」コメントで配布している。

## 学び・所感

- 新しい技法ではないが、「UI は Hi-Fi の仕上げ、UX は Lo-Fi の思考」という表紙の切り分けは、図鑑の基礎定義として置く価値がある。中央に心理学の法則（ヒック／フィッツ／ヤコブ等）を挟み、両者が別物ではなく積み重なっている構図も良い
- 比喩の中で実務に効くのは氷山とベビーモバイル。前者は「見える部分は一部」という分量感、後者は「作り手と使い手で見えている面が違う」という視点の非対称を1枚で伝える
- UXリサーチのマップ6種（別ノート）が「UX 側の具体的な道具」なのに対し、こちらは「UI/UX という言葉の地図」。基礎編として図鑑カードも追加した
