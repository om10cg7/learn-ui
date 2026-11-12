# パスワード強度メーターの演出6種 Part 1（ui_motion_prompts）

- 出典：Instagram @ui_motion_prompts のリール「Password Strength Part 1 — one meter, six ways to show a stronger password」（パスワードの強さの演出 その1、2026-11-11投稿）
  - https://www.instagram.com/reel/DfmigE5Cf0F/
  - 内容は動画解析で確認。全パネル共通で、文字が増えるにつれて Weak（赤）→ Fair（橙）→ Good（青）→ Strong（緑）と状態が進み、「Add more characters」「Add a number」「Add a symbol」「Great password!」の助言ラベルが添えられる。各パネルのラベルは解析で読み取れた正式名
  - このチャット（振り分け）経由で受領し、仕分けルール（url_repo_router）で learn-ui 行きと判定して作成

## 6種

1. **Flow Fill** — 液体が滑らかに流れ込んで満たしていく
2. **Block Drop** — セグメントが潰れながら落ちて積まれる
3. **Spark Feed** — 火花が弧を描いて落ちて点火する
4. **Chain Light** — セグメントが順に点灯して連なっていく
5. **Flap Label** — 強さラベル自体がパタパタ板（スプリットフラップ）で切り替わる
6. **Liquid Link** — 充填がにじむように進み、最後にパチンとつながる

## 学び・所感

- 強度メーターの本体は「何が足りないか」の助言（数字を足せ、記号を足せ）で、バーの演出はその理解を助ける副次要素。6 種とも色の段階（赤→橙→青→緑）とラベルが共通なので、演出が派手でも情報の読み取りはぶれていない
- 5 Flap Label はバーではなく文字側を動かす唯一のパターン。Split Flap は Number Counter Part 1（notes/2026-11-10-number-counter-motions-6-part1.md）でも使われていた機械式メタファーの再登場
- 1 Flow Fill と 6 Liquid Link は液体メタファーで、強くなるほど「満ちる」感が出る。逆に 3 Spark Feed の火花は強さよりも派手さが前に出やすく、セキュリティ文脈の落ち着きとは相性が分かれる
