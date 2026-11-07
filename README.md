# behavioraleconlab-legal

「行動経済学図鑑 / Behavioral Economics Lab」のサポートサイト（GitHub Pages）。

- `/` — サポートトップ（FAQ 付き）
- `/privacy/` — プライバシーポリシー（日英）
- `/terms/` — 利用規約（日英）

公開URL: https://non-migi.github.io/behavioraleconlab-legal/
（アプリの設定画面は `/privacy/` と `/terms/` を開く。`Features/Settings/SettingsView.swift`）


## メモ

構成と文面は姉妹アプリの `statzukan-legal` を元にしている。違いは次のとおり。

- **1.0 は広告なし**（AdMob・同意管理・ATT なし）。プライバシーポリシーに「広告について」の章はなく、「広告は表示しない・広告識別子は使わない」とだけ書いてある。
  広告を入れるときは `statzukan-legal` / `gametheorylab-legal` の「広告について」の章を戻し、`PrivacyInfo.xcprivacy` と ASC の申告も揃えること。
- 実験の答え（予想・選択・引っかかったか）は端末内だけで使うが、Aptabase へはイベントの中身として一部が行く。2章の表の「例」にそう書いてある。
  Aptabase に送るイベントを増やしたら、表の「例」も合わせて直す（アプリ側は `BehavioralEcon/Core/Services/AnalyticsManager.swift`）。
- フィードバックは統計用語図鑑と同じ Google フォーム（アプリ名の欄で区別）。
