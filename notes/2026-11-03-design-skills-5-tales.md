# AIにデザインセンスを与えるSkill 5選 Part 1（Tales Cavalcanti）

- 出典：Instagram @talescavalcanti.ia のカルーセル「5 skills para dar mais bom gosto à sua IA. Parte 1」（全7枚、2026-11-02投稿）
  - https://www.instagram.com/p/DfP03vpGkoq/?img_index=4
  - 指定の img_index=4 ＝ Hallmark のスライド。全スライド目視で確認（キャプションの列挙順とカルーセル内の並び順は異なる）
  - 共通テーマは「AI slop（AIの安っぽい生成物）を終わらせる」
- 関連：notes/2026-11-03-claude-github-repos-10-anton.md（Impeccable と Hallmark が重複）

## 5選（カルーセル順）

| ツール | 内容 | リンク |
|--------|------|--------|
| shadcn/ui | 公式Skill。shadcn流にコンポーネントを追加・更新 | ui.shadcn.com/docs/skills |
| Hue | あらゆるビジュアルアイデンティティをSkillに変換（内側の細字は読み取り不可） | hueapp.io |
| Hallmark | 21テーマ、ページ構造、58の品質チェック。「The design skill that ends AI slop」。Claude Code／Codex／OpenCode対応、導入は `npx skills add nutlope/hallmark -g` | usehallmark.com |
| Taste Skill | バリエーション・動き・密度を調整し最終チェック。「The anti-slop frontend framework for AI agents」 | tasteskill.dev |
| Impeccable | 構築・批評・改善・アニメーションを1つのSkillで。「The missing design vocabulary for agents」、汎用的なAIインターフェースを検出して除去 | impeccable.style |

## 学び

- 5選すべての売り文句が「汎用的・安っぽいAI出力（AI slop）からの脱却」で統一されている。デザインSkillの競争軸が「作れる」から「センスの言語化と品質チェック」へ移っている
- Hallmark の「58の品質チェック」、Impeccable の「デザイン語彙を与える」という打ち出しは、よそおい図解モーションの「動きの言語化」と同じ方向
- Anton の10選で名前が「Onyx」なのにURLが taste-skill だった件は、この Taste Skill（tasteskill.dev）の存在で裏付けが取れた。Anton 側のカード名が誤っていた可能性が高い
