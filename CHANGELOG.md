# Changelog

このプロジェクトの主な変更を記録します。

## 2026-07-09 - Development #013

### Added

- `tools/website-fix-plan-builder/` を追加。
- Website Improvement Analyzer の診断結果を、改善作業、納品物、作業手順、見積もり目安、クライアント確認事項へ変換するMVPを追加。
- 作業ログ用Markdownと実績化メモの生成に対応。
- README とサンプル改善計画を追加。

### Changed

- Retirement OS Launcher に Website Fix Plan Builder を追加。
- ルート README と showcase に Website Fix Plan Builder を反映。
## 2026-07-09 - Development #010

### Changed

- Website Improvement Analyzer を v1.5 に更新。
- SEO、CTA、スマホ対応、ファーストビュー、信頼材料、表示速度の診断チェックリストを追加。
- チェック結果をMarkdownレポートへ反映。
- 改善優先度を「最優先」「次に直す」「余裕があれば直す」に分けて出力。
- 提案書の短い版と詳しい版を生成できるように改善。
- README、examples、showcase を v1.5 に合わせて更新。
## 2026-07-05

### Added

- 公開前ファイルとして `.gitignore` と `LICENSE` を追加。
- `docs/roadmap.md` と `docs/operation-rules.md` を追加。
- `docs/showcase.md` を追加。
- 案件レビュー用テンプレートを追加。
- Opportunity Scorecard のサンプルレビューを追加。

### Changed

- ルート README を、案件選別・受託実績・自社事業化の実験環境として整理。
- Opportunity Scorecard に評価日、理由メモ、Markdown 出力、応募 / 保留 / 見送り判定を追加。
- Opportunity Scorecard に「作業負荷の低さ」を評価項目として追加。

### Security

- 公開前確認として、個人情報・契約情報・APIキー・メールアドレスに該当しそうな文字列を検索。
- 実データとして公開を止めるべき情報は見つからなかった。

## 2026-07-05 - Development #002

### Added

- `tools/proposal-draft-builder/` を追加。
- 応募文下書きを Markdown 形式で生成する単体 HTML ツールを追加。
- README とサンプル応募文を追加。

### Changed

- ルート README、showcase、roadmap に Proposal Draft Builder を反映。

## 2026-07-05 - Autonomous Development

### Added

- `tools/portfolio-case-builder/` を追加。
- 完了案件や制作物を Markdown の実績紹介文へ変換する単体 HTML ツールを追加。
- README とサンプルケースを追加。

### Changed

- ルート README、showcase、roadmap に Portfolio Case Builder を反映。
- ルート README のツールパス表記を修正。
- showcase の次候補から実装済み項目を整理。
## 2026-07-05 - Development #004

### Added

- `tools/client-crm/` を追加。
- 応募・受注案件を一覧管理する単体 HTML ツールを追加。
- ステータス変更、Markdown 出力、サンプルデータ、localStorage 自動保存を追加。
- README とサンプル Markdown を追加。

### Changed

- ルート README、showcase、roadmap に Client CRM を反映。
- showcase の実装済み候補を整理。
## 2026-07-05 - Development #005

### Added

- `tools/work-log-builder/` を追加。
- 日々の作業ログを記録する単体 HTML ツールを追加。
- ブラウザ内自動保存、一覧表示、Markdown 出力、実績化候補抽出を追加。
- README とサンプル Markdown を追加。

### Changed

- ルート README、showcase、roadmap に Work Log Builder を反映。
- showcase の次候補を未実装テーマに整理。
## 2026-07-06 - Development #006

### Added

- ルート `index.html` を追加。
- 既存5ツールへアクセスできる Retirement OS Launcher を追加。
- GitHub Pages 公開時の全体入口を追加。

### Changed

- ルート README と showcase に Launcher を反映。
## 2026-07-08 - Development #008

### Added

- `tools/website-improvement-analyzer/` を追加。
- v1.0 手動入力版として、Webサイト改善診断レポート生成ツールを追加。
- README とサンプル分析レポートを追加。
- ブラウザ内保存、Markdown出力、ワンクリックコピーを追加。

### Changed

- ルート `index.html` から Website Improvement Analyzer を開けるように更新。
- `docs/showcase.md` に Website Improvement Analyzer を追加。
## 2026-07-08 - Development #009

### Changed

- Website Improvement Analyzer を v1.1 に更新。
- 強みと改善点のバランスを取った出力へ改善。
- 優先順位に理由を付けて出力できるように変更。
- 今すぐ改善できることと中長期で改善することを分けて出力。
- 提案書のたたき台を、営業で渡しやすい自然な文章へ改善。
- README と examples を v1.1 に合わせて更新。
