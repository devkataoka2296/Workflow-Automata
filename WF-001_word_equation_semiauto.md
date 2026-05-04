---
workflow_id: WF-001
name: Word 数式半自動変換
version: 0.1
status: experimental
---

# WF-001: Word 数式半自動変換

## 目的
数式をWord数式エディタで編集可能な形式（LaTeX）に整形する

---

## 入力
- 数式を含む文章（Word / テキスト）

---

## 出力
- LaTeX形式に整形された数式
- Word貼り付け用文章

---

## 禁止事項（重要）
- 数式の意味を変更しない
- 変数名を変更しない
- 添字・上付き文字を変更しない
- 単位を変更しない
- 式番号を勝手に変更しない

---

## Phase 1: 数式抽出

- 数式部分を抽出する
- テキスト部分と分離する

出力：
- 抽出された数式一覧
- 元文との対応

---

## Phase 2: LaTeX変換

- 各数式をLaTeX形式に変換
- Word数式として貼れる形にする

例：
a/b → \frac{a}{b}

---

## Phase 3: 再構成

- 元文章にLaTeX数式を埋め込む
- 構造を維持する

---

## 完了条件

- すべての数式がLaTeX形式
- Wordで変換可能

---

## 出力形式

Phase:
Extracted equations:
Converted equations:
Reconstructed text:

---

## 次の選択

A. OK（次のPhaseへ）
B. 修正
C. 別workflow
