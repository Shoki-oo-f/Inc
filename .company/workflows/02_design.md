# 📋 02_design — 設計フェーズ SOP

> **担当ロール**: Architect（アーキテクト）

---

## 目的

PRD を元に技術選定を行い、ADR に記録し、API 仕様書・システム設計書を作成して承認を得る。

---

## 前提条件

- PM が PRD を作成し、社長の承認を得ていること
- `.company/phase.md` が `02_design` であること

---

## 手順

### Step 1: PRD の分析
- `docs/prd/` の PRD を精読する
- 技術的要件、非機能要件を抽出する

### Step 2: 技術選定
- フレームワーク、言語、DB、インフラ等を選定する
- 選定の理由（代替案との比較含む）を ADR として記録する

### Step 3: ADR の記録
- `.company/adr/` に技術決定記録を作成する
- ADR テンプレート（`.company/rules.md` 参照）に従う

### Step 4: 設計書の作成
- `docs/api-specs/` に API 仕様書を作成する
- システム構成図、データモデル、認証方式を含める

### Step 5: 承認ゲート 🚧
- 設計書を社長に提示する
- **社長の承認が必須** — 承認なしに次フェーズへ進むことは禁止

---

## 完了条件

- [x] ADR が `.company/adr/` に記録されている
- [x] API 仕様書が `docs/api-specs/` に保存されている
- [x] 社長が設計を承認した
- [x] `.company/phase.md` を `03_implement` に更新

---

## 次のフェーズ

→ **03_implement**（Engineers が稼働）
