# Website Fix Plan Builder

Website Improvement Analyzer の診断結果をもとに、改善作業、納品物、見積もり目安、クライアント確認事項へ変換するブラウザツールです。
依存ライブラリなしで、`index.html` を開くだけで使えます。

## Purpose

サイト診断を「改善提案」で終わらせず、小規模事業者向けのサイト改善ミニ支援として実行できる状態にします。

## How To Use

1. Website Improvement Analyzer のMarkdownレポートから、最優先、次に直す点、余裕があれば直す点、提案文を転記する。
2. 改善メニューを選ぶ。
3. 対応範囲、作業条件、クライアント確認事項を入力する。
4. 右側のMarkdown出力を確認する。
5. `Markdown をコピー` を押して、提案書、Client CRM、Work Log Builder、Portfolio Case Builder へ転記する。

## Inputs

- 基本情報
- 診断結果の貼り付け欄
- 改善メニュー
- 対応範囲
- 作業条件
- クライアント確認事項

## Output

- 改善作業リスト
- 納品物一覧
- 作業手順
- 見積もり目安
- クライアント確認事項
- 作業ログ用Markdown
- 実績化メモ

## Design Notes

- HTML単体で動く。
- 外部API、APIキー、ログインは使わない。
- 入力値はブラウザの localStorage に保存する。
- 価格目安と納品物は `docs/website-improvement-fix-playbook.md` の考え方をもとにする。
- サーバー移転、決済機能、予約システム、大規模リニューアル、深いWordPress改修、本格SEO運用、高度な解析、広告運用代行は対象外にする。

## Example

- `examples/sample-fix-plan.md`: サイト改善計画のサンプル。
