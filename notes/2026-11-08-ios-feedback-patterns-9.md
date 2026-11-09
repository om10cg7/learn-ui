# iOSフィードバックパターン9種 Pt.1（David Mráz）

- 出典：Instagram @davidm_ai のリール「iOS Feedback Patterns - Vocabulary for Agentic Coding」（2026-11-06投稿）
  - https://www.instagram.com/reel/DfauQgWgCoz/
  - 内容は動画解析で確認。3×3グリッドのインフォグラフィックをカーソルで順に示す形式

## 9種

| パターン | 内容 |
|----------|------|
| Dynamic Island | カメラ周りの領域が伸縮して状態を見せる |
| Live Activity | ロック画面等にリアルタイムの進捗を出す |
| HUD | 画面上に一時的に重なる表示（音量など） |
| Action sheet | 下から出る選択肢シート |
| Swipe actions | リスト項目のスワイプで出るアクション |
| Haptic feedback | 振動による触覚フィードバック |
| Jiggle mode | アイコンが揺れる編集モード |
| Symbol effect | SF Symbols のアニメーション |
| Shake to undo | 端末を振って取り消し |

## 学び

- 副題が「Vocabulary for Agentic Coding」＝AIエージェントに指示するための語彙、という位置づけ。usutaku の「AIに伝わるUI用語」と同じ発想で、対象が iOS 固有のフィードバック表現に絞られている
- 前の投稿（インジケーター9種）が「バーの名前」だったのに対し、こちらは「反応の名前」。視覚以外の Haptic や Shake to undo まで含むのが iOS らしい
