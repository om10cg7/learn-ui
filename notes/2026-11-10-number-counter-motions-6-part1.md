# 数字カウンターの演出6種 Part 1（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のリール「Number Counter Part 1 — one number, six ways to change it」（数字が変わる演出 その1、2026-11-10投稿）
  - https://www.instagram.com/reel/Dfld7zxgt1K/
  - 内容は動画解析で確認。歩数カウンター（9,105 → 7,348 など）の数字が6パネルでそれぞれ違う変わり方をする。各パネルのラベルは解析で読み取れた正式名
  - このチャット（振り分け）経由で受領し、仕分けルール（url_repo_router）で learn-ui 行きと判定して作成

## 6種

1. **Odometer Roll** — 桁ごとに縦にロールして次の数字へ（機械式オドメーター）
2. **Split Flap** — パタパタ板（空港の案内板）がめくれるように変わる
3. **Blur Slide** — ブラー（残像）を伴ってスライドしながら切り替わる
4. **Spring Stagger** — 桁ごとにタイミングをずらし、バネの弾みで変わる
5. **Decode Lock** — ランダムな文字が左から順に確定していくデコード式
6. **Smooth Count** — 値を補間して滑らかにカウントアップ／ダウン

## 学び・所感

- 数字の変化は「前の値→新しい値」の差分が大きいほど演出の効き目が出る題材。1 Odometer と 2 Split Flap は機械式のメタファーで、桁の繰り上がりまで見せられるのが強み
- 5 Decode Lock はゲームや SF 系の世界観向けで、歩数のような日常データには大げさ。6 Smooth Count は最も控えめで、ダッシュボードの指標更新のような「頻繁に変わる数字」に向く
- 4 Spring Stagger の「桁ごとの時間差」は、同作者のシリーズで繰り返し出てくる stagger の応用。数字は桁という自然な分割単位があるので、ずらす設計がしやすい
