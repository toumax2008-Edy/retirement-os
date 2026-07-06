# Client CRM

応募した案件、受注案件、クライアント情報を管理するための単体ブラウザツールです。
依存ライブラリなしで、`index.html` を開くだけで使えます。

## Purpose

応募した案件を忘れず、次にやることを明確にするための簡易 CRM です。
Opportunity Scorecard、Proposal Draft Builder、Portfolio Case Builder の間に入り、応募から実績化までの流れを管理します。

## How To Use

1. `index.html` をブラウザで開く。
2. クライアント名、案件名、案件種別、応募日、ステータス、報酬、次にやること、メモを入力する。
3. `案件を追加` を押す。
4. 一覧のステータスを必要に応じて変更する。
5. 右側の Markdown をコピーして、日報、Notion、GitHub Issue などに貼る。

## Managed Fields

- クライアント名
- 案件名
- 案件種別
- 応募日
- ステータス: 応募中 / 面談 / 契約 / 作業中 / 納品 / 継続 / 終了
- 報酬
- 次にやること
- メモ

## Output

- 案件一覧の Markdown
- ステータス別の件数
- 次にやることの一覧

## Design Notes

- HTML 単体で動かす。
- 外部 API や認証は使わない。
- データはブラウザの localStorage に保存する。外部送信はしない。
- 項目追加は JavaScript の `fields` と `sampleDeals` を拡張する。
- 実名、メールアドレス、契約条件などは公開前に伏せる。

## Examples

- `examples/sample-client-crm.md`: サンプル案件一覧の Markdown 出力。

## Future Improvements

- CSV export/import。
- ステータス別フィルター。
- 次回連絡日の追加。
- Portfolio Case Builder へ渡す実績候補の出力。

