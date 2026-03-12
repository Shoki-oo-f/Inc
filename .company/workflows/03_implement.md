# 📋 03_implement — 実装フェーズ SOP

> **担当ロール**: Frontend Engineer / Backend Engineer / AI Engineer / DevOps Engineer

---

## 目的

Architect の設計書に基づき、各エンジニアが担当領域のコードを実装する。

---

## 前提条件

- Architect が API 仕様書を作成し、社長の承認を得ていること
- `.company/phase.md` が `03_implement` であること

---

## 手順

### Step 1: 設計書の確認
- 各エンジニアは `docs/api-specs/` の設計書を確認する
- 自身の管轄に関連する仕様を把握する

### Step 2: 実装の順序
推奨される実装順序：

1. **DevOps Engineer**: インフラ環境のセットアップ（Docker, CI/CD等）
2. **Backend Engineer**: API エンドポイント、ビジネスロジック、DB 連携
3. **AI Engineer**: LLM 連携、RAG パイプライン、プロンプト設計
4. **Frontend Engineer**: UI コンポーネント、API 連携、画面遷移

> ただし、並行作業が可能な場合は順不同で進めてよい。

### Step 3: 各エンジニアの作業
- 自身の管轄領域 **のみ** にコードを実装する
- 設計書に記載された仕様に **厳密に** 従う
- セルフテストを実施し、基本的な動作確認を行う

### Step 4: QA 提出
- 実装完了後、QA Engineer にレビューを依頼する
- **直接社長に報告することは禁止**

---

## 完了条件

- [x] 各エンジニアが担当コードを実装済み
- [x] セルフテストが完了している
- [x] QA Engineer にレビュー依頼済み
- [x] `.company/phase.md` を `04_qa_review` に更新

---

## 次のフェーズ

→ **04_qa_review**（QA Engineer が稼働）
