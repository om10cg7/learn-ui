# AIに伝わるUIの名前30（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のカルーセル「Vague prompt, vague UI. Say the name instead.」（AI に伝わる UI の名前 その1、2026-11-12投稿、全7枚）
  - https://www.instagram.com/p/DfqSzJdHdb9/
  - 内容は解析と表紙で確認。30の名前とカテゴリ分けは解析で読み取れたもの。表紙の例は Mesh Gradient／Glassmorphism／Bento Grid／Gradient Text／Neo-Brutalism／Confetti Burst の6つ
  - このチャット（振り分け）経由で受領し、仕分けルール（url_repo_router）で learn-ui 行きと判定して作成

## 主張

- 「曖昧なプロンプトからは曖昧な UI しか出ない。代わりに名前で言え」— AI は確立した UI 用語を学習しているので、見た目をくどくど説明するより、用語名をそのまま渡すほうが正確に伝わる
- 締めのスライドは「Every name here is a prompt（ここにある名前は全部プロンプト）」で、例は「Make a bento grid with glassmorphism cards」— 名前同士を組み合わせて使う

## 30の名前（5カテゴリ×6）

- **Backgrounds（背景）** — Mesh Gradient、Aurora Background、Noise Texture、Dot Grid、Spotlight Effect、Animated Gradient
- **Textures（質感）** — Glassmorphism、Neumorphism、Claymorphism、Skeuomorphism、Neo-Brutalism、Aurora Glass
- **Layouts（レイアウト）** — Hero Section、Bento Grid、Masonry、Split Screen、Sidebar、Full-width Banner
- **Text Effects（文字効果）** — Gradient Text、Shimmer Text、Typewriter、Text Scramble、Marker Highlight、Blur Reveal
- **Motion（動き）** — Sliding Pill、Skeleton Loading、Pull to Refresh、Swipe to Delete、Odometer Roll、Confetti Burst

## 学び・所感

- この図鑑（learn-ui）自体が「UI/UX 用語を集める」営みで、その用語がそのまま AI への指示語になるという話。用語を覚える理由が「人との共通言語」から「AI へのプロンプト精度」に広がった、という位置づけの投稿
- Motion の6つ（Sliding Pill／Pull to Refresh／Swipe to Delete／Odometer Roll 等）は、この作者の6種カタログシリーズで個別に扱ってきた演出と一致する。カタログで「動き」として学んだものが、ここでは「名前」として再提示されている
- 注意点として、名前が通じるのは「AI がその用語の典型像を持っている」場合だけ。組み合わせ（Bento Grid × Glassmorphism の例）や、どの部分に効かせるかの指定は依然として書き手の仕事
- 全プロンプト（名前ごとの使い方）は bio リンクで配布
