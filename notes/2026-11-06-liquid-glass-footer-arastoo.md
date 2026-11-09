# リキッドグラスのフッターUI（Arastoo）

- 出典：Instagram @arastoo のリール「Glassy Liquid Footer」（2026-11-05投稿）
  - https://www.instagram.com/reel/DfXHLZVz0JI/
  - 内容は動画解析で確認。ソースコード全文は「Code」コメントで配布の形式
- 関連：図鑑のリキッドグラス／グラスモーフィズム系カード、notes/2026-10-26-glass-button-figma.md

## 中身

- 架空ブランド「Vertix」（タグラインは "One good money idea, every Friday."）のサイトフッターのデモ
- 半透明＋ぼかしで背後の室内が見えるグラス面の上に、液体状の blob がアニメーションで流れる
- 青いグロー、ホバーのアニメーション、Product／Company／Resources／Legal のナビ、SNSアイコン、ダークモード切替つき
- 実装は React + framer-motion + lucide-react（画面下のコードエディタで一部表示）

## 学び

- リキッドグラスの適用先としてボタンやカードではなく「フッター」という大きな面に使っているのが目新しい。面が広い分、背後の透けと blob の動きが主役になる
- グラス系は要素が増えると煩くなりがちだが、フッターは情報量が定型（ナビ＋SNS＋切替）なので質感の実験場として相性がいい
