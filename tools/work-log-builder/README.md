# Work Log Builder

日々の作業内容を記録し、あとからポートフォリオ化・改善・振り返りに使うための単体ブラウザツールです。
依存ライブラリなしで、`index.html` を開くだけで使えます。

## Purpose

毎日の作業を短く残し、あとから「実績化できる作業」「改善すべき作業」「次に進める作業」を見返せるようにします。
Client CRM と Portfolio Case Builder の間に入り、作業ログから実績紹介文へつなげます。

## How To Use

1. `index.html` をブラウザで開く。
2. 作業日、カテゴリ、作業内容、時間、成果、気づき、次にやること、実績化候補を入力する。
3. `ログを追加` を押す。
4. 一覧と実績化候補だけの抽出を確認する。
5. `Markdown をコピー` を押して、日報、Notion、GitHub Issue などへ貼る。

## Fields

- 作業日
- 作業カテゴリ: 案件 / 自作ツール / 学習 / 実験 / 営業
- 作業内容
- かかった時間
- 得られた成果
- 気づき
- 次にやること
- 実績化候補: はい / いいえ

## Output

- 作業ログ一覧の Markdown
- 実績化候補だけの Markdown
- カテゴリ別件数

## Design Notes

- HTML 単体で動かす。
- 外部 API や認証は使わない。
- データはブラウザの localStorage に保存する。外部送信はしない。
- 項目追加は JavaScript の `fields` と `sampleLogs` を拡張する。
- 実績化候補は Portfolio Case Builder に移す前提で短く書く。

## Examples

- `examples/sample-work-log.md`: サンプル作業ログの Markdown 出力。

## Future Improvements

- CSV export/import。
- 月別・カテゴリ別フィルター。
- 作業時間の合計表示。
- Portfolio Case Builder へ貼りやすい詳細出力。
- Client CRM の案件名を選べるようにする。
