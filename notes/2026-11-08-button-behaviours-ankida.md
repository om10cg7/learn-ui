# 同じボタン、2つの振る舞い — decorated vs engineered（Ankida Code）

- 出典：Instagram @ankida_code（Ankida Code、制作スタジオ）のリール「Same button. Two behaviours.」（2026-11-07投稿、14秒）
  - https://www.instagram.com/reel/DfcdCxnjkmr/
  - 内容は動画解析で確認。数値は動画内の表示どおり転記。受注誘導は DM／code.ankida.studio
- キャプションの言葉：「Decoration is how it looks. Engineering is how it feels.」（装飾は"どう見えるか"、エンジニアリングは"どう感じるか"）

## 比較：Sendボタンの4状態

| 状態 | .decorated（見た目だけ） | .engineered（振る舞いまで設計） |
|---|---|---|
| Hover | 色が濃くなるだけ | **-16px 浮き上がり＋ scale 1.05 ＋グロー** |
| Press | 無反応 | **潰れる（scaleX 1.12／scaleY 0.74）→ バネで戻る** |
| Loading | グレーアウト | **ピル形（幅468px）から円形リングスピナーへ、要素を差し替えずモーフ** |
| Success | テキストを「Sent ✓」に差し替え | **リングが420msでチェックマークへ変形アニメーション** |

締めの言葉は「Interfaces that behave beautifully.」（美しく振る舞うインターフェース）。

## 学び・所感

- 「状態遷移を"差し替え"で済ませるか、"変形"でつなぐか」が要点。engineered 側は全状態で要素が同一のまま形を変えるので、ユーザーは「同じボタンが応えてくれている」と感じる
- 数値が具体的でそのまま実装に使える：ホバーの浮き -16px はかなり大きめ（通常のボタンでは過剰気味。主役CTA向けの値として読む）。潰れ比率 scaleY 0.74 は「押した感触」を出すには十分な変形量
- Vamshi のローダー8種（notes/2026-11-08-loader-types-8-vamshi.md）の Button Loader の先の話として読める：ボタン内スピナーにするだけでなく、ボタン自体がモーフしてスピナーになる、がこの投稿の提案
