# Lightroomシネマティック・カラーグレーディング手順（CINEPHOR1A）

- 出典：Instagram @cinephor1a のカルーセル「THE ART OF COLOR GRADING IN ADOBE LIGHTROOM」（全9枚、2026-10-30投稿）
  - https://www.instagram.com/p/DfISpc-ku62/?img_index=7
  - 題材：霧の森で白いドレスの女性と黒馬のポートレート。撮影設定は 85mm／ISO 500／F2.8／1/250s
  - 指定の img_index=7（表紙を1枚目と数えて8枚目）＝カラーグレーディング画面を目視で重点確認。全スライドの設定値を目視転記
- 関連：notes/2026-10-29（mikita.yo のLightroomマスキング）

## 手順と設定値

### 1. Radial Gradient（霧を足す）
背景に柔らかい霧を加えて被写体のシルエットを作る。
Contrast +17／Highlights +15／Shadows +21／Blacks +11／Texture -22／Clarity -19／Dehaze -10

### 2. Subject Mask（被写体マスク）
被写体を背景から分離してすっきり見せる。
Exposure -0.20／Contrast -12／Highlights +27／Shadows +16／Whites +11／Texture +29／Clarity +14

### 3. Radial Gradient（ビネット）
全体に暗いトーンとバランスを与える。
Exposure -0.25／Contrast +13／Highlights +48／Shadows -12／Whites -33／Texture -15

### 4. Background Mask（背景マスク）
背景を分離してミニマルに。
Contrast -15／Highlights +26／Shadows +25／Blacks +09／Texture -18／Clarity -15／Dehaze -12

### 5. カラーグレーディング＋HSL（指定スライド）
- トーンカーブはS字。カラーホイール2つの数値は読み取り不可
- HSL：
  - オレンジ：Hue +8／Saturation -6／Luminance +13
  - イエロー：Hue +20／Saturation +24／Luminance +15
  - グリーン：Hue 0／Saturation -100／Luminance -50
  - ブルー：Hue 0／Saturation -100／Luminance -31

## 学び

- シネマティック化の核心はHSLで、緑と青の彩度を -100 まで落として森と空の色を消し、暖色（オレンジ／イエロー）だけを残して肌と光を際立たせる
- 霧は Dehaze マイナス＋テクスチャ／クラリティ低下で「足す」もの。被写体側は逆に Texture +29／Clarity +14 で締める対比が効いている
- マスクを「霧用グラデーション／被写体／ビネット／背景」の4層に分ける構成で、部分ごとに正反対の調整をかけている
