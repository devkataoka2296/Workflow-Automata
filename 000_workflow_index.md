# Workflow Index

## Rule (VERY IMPORTANT)
- You MUST select exactly ONE workflow_id before execution
- You MUST NOT execute anything before selecting a workflow
- You MUST read ONLY the selected workflow file
- You MUST NOT mix workflows
- After execution, ALWAYS ask user A/B/C

---

## WF-01
Name:
Word 数式半自動変換ワークフロー

Use when:
- 数式入りWord文書を扱う
- 数式を数式エディタ形式にしたい
- LaTeX形式や変換しやすい形に整理したい
- Wordを最終編集環境とする

Input:
- Word文書 or テキスト（数式含む）

Output:
- 数式をLaTeX形式に整形した文書
- Wordで変換しやすい構造

File:
workflows/WF-01_word_equation_semiauto.md

---

## WF-99
Name:
ダミーワークフロー（テスト用）

Use when:
- ワークフロー選択の動作確認をしたい
- Coordinatorが正しく分岐できるか確認したい

Input:
- 任意

Output:
- 簡単なテストメッセージ

File:
workflows/WF-99_dummy_test.md

---

## Selection Instruction

When user gives a task:

1. Analyze the task
2. Select exactly one workflow_id
3. State selected workflow
4. Load the workflow file
5. Execute Phase 1 ONLY

---

## Output Format

Selected workflow:
Reason:
Next step:
A. OK
B. Revise
C. Change workflow
