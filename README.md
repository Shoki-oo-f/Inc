# 🏢 Elpis Innovations — Antigravity Edition

**Google Antigravity 環境で動作する、仮想開発組織フレームワーク**

単一の AI モデルが複数の専門的なロール（役職）を自律的に切り替えながら、高品質なソフトウェア開発を遂行します。

---

## ✨ 特徴

- 🧠 **遅延読み込み（Lazy Loading）** — 必要なロールのみを都度読み込み、コンテキスト汚染を防止
- 🚧 **承認ゲート** — 各フェーズ完了時に社長（ユーザー）の承認を必須化
- 🛡️ **QA ピアレビュー** — 実装後は必ず QA Engineer のテストを通過
- 📋 **ADR 記録** — 技術決定の背景を永続化し、後から追跡可能に
- 📂 **管轄分離** — 各ロールは自身の管轄領域のみ編集可能

---

## 👥 役職一覧

| 役職 | ミッション | 管轄領域 |
|---|---|---|
| 👩‍💼 **Secretary** | 社長窓口、要件ヒアリング・整理 | `.company/board.md` |
| 👔 **CEO** | プロジェクト指揮、フェーズ管理 | `.company/board.md`, `.company/phase.md` |
| 📅 **PM** | 要件ヒアリング、PRD 作成 | `docs/prd/` |
| 📐 **Architect** | 技術選定、API/DB 設計 | `docs/api-specs/`, `.company/adr/` |
| 🎨 **Frontend** | UI/UX 実装 | `src/frontend/` |
| ⚙️ **Backend** | ビジネスロジック、API 実装 | `src/backend/` |
| 🤖 **AI Engineer** | 自社AI独自開発（LLM連携は最終手段） | `src/ai/`, `docs/prompts/` |
| 🚀 **DevOps** | インフラ、CI/CD | `infra/`, `.github/` |
| 🛡️ **QA Engineer** | テスト、コードレビュー | `tests/` |

---

## 🔄 開発ワークフロー

```
01_planning ──→ 02_design ──→ 03_implement ──→ 04_qa_review
   (PM)        (Architect)    (Engineers)      (QA Engineer)
     ↓              ↓              ↓                ↓
  PRD作成 →     設計・ADR →     コード実装 →    テスト・レビュー
  社長承認       社長承認        QA提出          社長報告
```

---

## 📂 ディレクトリ構成

```
├── GEMINI.md                    ← エントリーポイント（ルートプロンプト）
├── .company/                    ← 仮想会社の脳・記憶領域
│   ├── rules.md                 ← 全社絶対ルール
│   ├── phase.md                 ← フェーズ管理
│   ├── board.md                 ← カンバンボード
│   ├── adr/                     ← アーキテクチャ決定記録
│   ├── roles/                   ← 役職定義（遅延読み込み対象）
│   └── workflows/               ← 各フェーズの SOP
├── docs/                        ← PRD・API 仕様書・プロンプト設計書
├── src/                         ← ソースコード（frontend / backend / ai）
├── infra/                       ← インフラ構成コード
└── tests/                       ← テストコード
```

---

## 🚀 使い方

1. Antigravity 環境で `Elpis/` をワークスペースとして開く
2. `GEMINI.md` がルートプロンプトとして読み込まれる
3. 秘書があなたの要望をヒアリングします
4. 自律的にロールを切り替えながら開発が進行します

---

## 📜 全社絶対ルール

1. **管轄絶対** — 自身の管轄外のファイルは編集禁止
2. **ピアレビュー厳守** — 実装後は必ず QA を通す
3. **ADR 記録** — 重要な技術決定は理由と共に記録
4. **遅延読み込み** — 必要なロールファイルのみ読み込む
5. **承認ゲート** — フェーズ遷移時に社長承認が必須
6. **ドキュメント駆動** — 部署間の情報共有は `docs/` を介して行う

---

## 📝 ライセンス

MIT
