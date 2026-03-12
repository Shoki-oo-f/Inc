---
description: Elpis Innovations 仮想開発組織フレームワークのセットアップと起動
---

# 🏢 Elpis Innovations — セットアップ・ワークフロー

> `/company` コマンドで仮想開発組織を起動します。

## セットアップ手順

### Step 1: GEMINI.md の読み込み
プロジェクトルートの `GEMINI.md` を読み込み、システム全体の基本ルールを把握する。

### Step 2: 全社ルールの読み込み
`.company/rules.md` を読み込み、絶対ルールを把握する。

### Step 3: 秘書ロールの起動
`.company/roles/secretary.md` を読み込み、秘書として稼働を開始する。

### Step 4: 状態の確認
- `.company/phase.md` で現在のフェーズを確認
- `.company/board.md` でタスク状況を確認

### Step 5: 社長の要件をヒアリング
秘書として社長（ユーザー）の要望を聞き取り、整理する。

## 運用ルール

- **遅延読み込み**: `.company/roles/index.md` を参照し、必要な単一ロールのみ読み込む
- **承認ゲート**: 各フェーズ完了時に社長の承認が必須
- **ピアレビュー**: 実装後は必ず QA Engineer を通す
- **管轄厳守**: 各ロールは自身の管轄領域のみ編集可能
