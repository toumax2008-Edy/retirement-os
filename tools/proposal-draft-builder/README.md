# Proposal Draft Builder

Opportunity Scorecard で「応募」と判断した案件から、応募文の下書きを作るブラウザツールです。
依存ライブラリなしで、`index.html` を開くだけで使えます。

## Purpose

クラウドワークス等の応募文を、毎回ゼロから書かずに素早く下書きするためのツールです。
案件名、募集内容、自分の強み、実績、備考を入力すると、Markdown 形式の応募文を生成します。

## How To Use

1. `index.html` をブラウザで開く。
2. 案件名、募集内容、自分の強み、アピールしたい実績、備考を入力する。
3. 右側の応募文を確認する。
4. `Markdown をコピー` を押して、応募画面へ貼り付ける。
5. 案件ごとに語尾や条件を少し調整して送る。

## Inputs

- 案件名
- 募集内容
- 自分の強み
- アピールしたい実績
- 備考

## Output

- クラウドワークス等で使いやすい Markdown 形式の応募文

## Design Notes

- HTML 単体で動かす。
- 外部 API や認証は使わない。
- 入力項目は JavaScript の `fields` 配列で管理し、後から追加しやすくする。
- 生成文は丁寧すぎず、実務で貼りやすい長さにする。

## Examples

- `examples/sample-proposal.md`: LP 改善案件向けの応募文サンプル。

## Future Improvements

- 文体の切り替え: 丁寧 / 短め / 熱量高め。
- 報酬条件や納期の入力欄追加。
- Opportunity Scorecard の Markdown を貼ると自動で一部入力する機能。
- 複数パターンの応募文生成。
