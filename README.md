# Retirement OS

Antigravity のナレッジベースとは分離した、引退OS専用の開発ルートです。
案件選別・受託実績・自社事業化の実験環境として、小さな道具を作りながら育てます。
このリポジトリの目的は、仕事の判断を記録し、再利用できる制作資産へ変えることです。

## Folder Structure

```text
retirement-os/
├── index.html    # GitHub Pages 用の全体入口
├── tools/        # 実務で使える小型ツール
├── automation/   # 定期処理、API連携、ローカル自動化スクリプト
├── docs/         # 運用ルール、ロードマップ、公開前の整理
├── experiments/  # 試作品、検証コード、短期テスト
├── templates/    # 提案書、案件レビュー、README などの再利用テンプレート
├── archive/      # 完了・停止・旧版になった資産
└── README.md     # この開発ルートの運用ルール
```

## Naming Rules

- フォルダ名とファイル名は原則 `kebab-case` を使う。
- 日付を入れる場合は `YYYY-MM-DD-topic` にする。
- ツールは `tools/tool-name/README.md` を必ず持つ。
- 実験は `experiments/YYYY-MM-DD-topic/` に置き、採用したら `tools/` または `automation/` へ移す。
- 個人情報、認証情報、契約情報、支払い情報は保存しない。必要な場合は `.env.example` だけ置く。

## GitHub Workflow

- `main` は動く状態を保つ。
- 作業単位は小さくし、1ツールまたは1改善ごとにコミットする。
- コミットメッセージは `type: summary` 形式にする。
  - `docs: update root readme`
  - `feat: add opportunity scorecard`
  - `fix: adjust export markdown`
- ライセンスは MIT License とする。
- 外部公開、契約、支払い、認証を伴う変更は、実行前に必ずユーザー確認を残す。
- 公開前に README、使い方、入力例、注意点を確認する。

## Launcher

- index.html: GitHub Pages 用の全体入口。既存ツールへアクセスできます。

## Tools

- `tools/opportunity-scorecard/`: 案件や企画を採点し、応募 / 保留 / 見送りを判断する。
- `tools/website-improvement-analyzer/`: 企業サイト、LP、ECサイトの改善点を診断し、提案書のたたき台を作る。
- `tools/website-fix-plan-builder/`: サイト診断結果を改善作業、納品物、見積もり目安、確認事項へ変換する。
- `tools/proposal-draft-builder/`: 応募と判断した案件の応募文下書きを作る。
- `tools/client-crm/`: 応募・受注案件と次アクションを管理する。
- `tools/work-log-builder/`: 日々の作業ログを記録し、実績化候補を抽出する。
- `tools/portfolio-case-builder/`: 完了した案件や制作物を実績紹介文に変換する。

## Documents

- `docs/roadmap.md`: 今後の開発順序。
- `docs/operation-rules.md`: 長期運用の基本ルール。
- `docs/showcase.md`: 外部に見せる成果物の紹介。
- `templates/job-review-template.md`: 案件判断を残すための型。

## Asset Addition Rules

- 追加する資産は、次のどれに該当するかを README に明記する。
  - 受託で使える
  - ポートフォリオで見せられる
  - 自社事業に転用できる
- ツールは、できるだけ単体で動く形から始める。
- 外部 API や有料サービスへの依存は、必要性が明確になってから追加する。
- 長期運用する資産は、最低限 `目的`, `使い方`, `入力`, `出力`, `今後の改善` を記録する。
- 古くなったものは削除せず、理由を書いて `archive/` に移す。
