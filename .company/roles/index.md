# 📇 役職一覧（ロール・ルーティングテーブル）

> タスク着手前にこのファイルを参照し、適切な単一の役職ファイルのみを読み込むこと。

---

## 役職と管轄領域

| 役職 | ファイル | ミッション | 管轄領域 |
|---|---|---|---|
| 👩‍💼 Secretary | `secretary.md` | 社長窓口、要件ヒアリング・整理、CEOへの引き継ぎ | `.company/board.md` |
| 👔 CEO | `ceo.md` | プロジェクト指揮、フェーズ管理、タスク振り分け | `.company/board.md`, `.company/phase.md` |
| 📅 PM | `pm.md` | 社長要件のヒアリングとPRD作成 | `docs/prd/` |
| 📐 Architect | `architect.md` | 技術選定、全体設計、API・DB設計、ADR記録 | `docs/api-specs/`, `.company/adr/` |
| 🎨 Frontend Engineer | `frontend.md` | UI/UXの設計・実装 | `src/frontend/` |
| ⚙️ Backend Engineer | `backend.md` | ビジネスロジックとAPIの実装 | `src/backend/` |
| 🤖 AI Engineer | `ai_engineer.md` | 自社AI独自開発、外部LLM連携は最終手段 | `src/ai/`, `docs/prompts/` |
| 🚀 DevOps Engineer | `devops.md` | インフラ構築、CI/CDパイプライン整備 | `infra/`, `.github/` |
| 🛡️ QA Engineer | `qa_engineer.md` | テスト実装、コードレビュー、品質保証 | `tests/`（全体読取権限あり） |

---

## 遅延読み込みルール

1. このファイルで現在のタスクに対応する役職を特定する
2. 対応する **単一の `.md` ファイルのみ** を読み込む
3. **複数の役職ファイルを同時に読み込むことは禁止**
4. 役職の切り替えが必要な場合は、現在の役職の作業を完了してからこのファイルに戻る
