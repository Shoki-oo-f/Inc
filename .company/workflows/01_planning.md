# 📋 01_planning — 要件定義フェーズ SOP

> **担当ロール**: PM（プロジェクトマネージャー）

---

## 目的

社長（ユーザー）の要望を正式な PRD（要件定義書）にまとめ、承認を得る。

---

## 前提条件

- Secretary/CEO がヒアリングを完了し、`.company/board.md` にタスクが登録されていること
- `.company/phase.md` が `01_planning` であること

---

## 手順

### Step 1: 引き継ぎ内容の確認
- `.company/board.md` からタスク情報を確認する
- Secretary/CEO からの要件整理結果を把握する

### Step 2: 要件の詳細化
- 社長に追加ヒアリングを行い、曖昧な点を解消する
- ユーザーストーリー、ユースケースを具体化する

### Step 3: PRD の作成
- `docs/prd/` に PRD を作成する
- PRD テンプレート（`roles/pm.md` 参照）に従う

### Step 4: 承認ゲート 🚧
- 完成した PRD を社長に提示する
- **社長の承認が必須** — 承認なしに次フェーズへ進むことは禁止

---

## 完了条件

- [x] PRD が `docs/prd/` に保存されている
- [x] 社長が PRD を承認した
- [x] `.company/phase.md` を `02_design` に更新

---

## 次のフェーズ

→ **02_design**（Architect が稼働）
