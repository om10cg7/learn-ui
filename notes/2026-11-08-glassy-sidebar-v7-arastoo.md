# グラス質感のフローティングサイドバー V7（Arastoo）

- 出典：Instagram @arastoo（Arastoo、表示名 code.xr 系）のリール「Glassy SideBar V7」（2026-11-08投稿）
  - https://www.instagram.com/reel/Dfe1ilgzcPL/
  - 内容は動画解析で確認。実装は React.js / CSS3 / HTML5、ソースコードは「Code」コメントで配布の形式
- 関連：notes/2026-11-06-glassy-navigation-tabs-v7-arastoo.md（同じ作者・同じ V7 世代だが、こちらは下部ナビタブで別コンポーネント）、notes/2026-11-06-liquid-glass-footer-arastoo.md、notes/2026-11-02-collapsible-sidebar-upgrade.md（@designcodewithav の折りたたみサイドバー、別物）

## 中身

- 半透明グラスモーフィズムの「浮遊型」サイドバー。背景はミニマルなリビング風の壁面で、バー自体がフローティングして見える
- 初期状態は細いガラスのピル（検索アイコン＋「Crema Studio Pro」ラベル）。上部アイコンのクリックで縦方向にスムーズに展開し、フルランチャーになる
- 展開時の構成要素：
  - Home
  - Inbox（通知バッジ 12）
  - Calendar（「Aug 8, 10:30」の予定表示まで一体化）
  - Messages（通知バッジ 3）
  - Projects、Analytics
  - 音楽プレイヤーウィジェット（「Morning Brew - Lo-fi Café」再生中表示）
  - 「Night shift」トグル
  - ユーザープロフィール（Noah Carter）
- ホバーでツールチップが出る（「Home」「Messages 3 new」など、バッジの内訳まで文字で補足）
- さらにクリックすると「Crema studio workspace」ビューに展開し、Favorites と Workspace のセクション一覧になる（2段階展開：ピル → アイコンランチャー → ワークスペース）
- キャプション側の売り文句：紫のグローアクセント、スムーズなホバーアニメーション、レスポンシブ対応

## 学び・所感

- サイドバーを「ナビゲーション」ではなく「ウィジェットを内蔵したランチャー」として設計しているのが要点。カレンダーの次回予定・再生中の曲・通知件数を遷移なしで見せる
- 折りたたみは幅ではなく「段階」で解決：ピル（最小）→ アイコン＋バッジ → ラベル付きワークスペース。情報量を3段階に分けている
- ツールチップに通知の内訳（「3 new」）まで含めるのは、アイコンのみの状態での情報不足を補う実務的な工夫
- 同じ作者の Glassy Navigation Tabs V7／Liquid Glass Footer と並べると、「グラス質感コンポーネント集 V7 世代」としてシリーズ化されていることが分かる
