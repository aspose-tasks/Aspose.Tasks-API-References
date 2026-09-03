---
title: "Aspose::Tasks::Task::MoveToSibling メソッド"
linktitle: "MoveToSibling"
articleTitle: "MoveToSibling"
second_title: "Aspose.Tasks for C++"
description: "現在のタスクを同じアウトラインレベルで、指定されたタスクの前に移動します。"
type: docs
weight: 1370
url: /ja/cpp/aspose.tasks/task/movetosibling/
---

## MoveToSibling (1 of 2) {#movetosibling_1}

現在のタスクを同じアウトラインレベルで指定されたタスクの前に移動します。ParentProject.CalculationMode が None の場合、このメソッド使用後に Project.Recalculate() を呼び出す必要があります（これにより、すべてのプロジェクトタスク（開始/終了日、早期/遅延日を設定）を再スケジュールし、スラック、作業、コストフィールド、アウトラインレベルなどの依存フィールドを計算します）。ParentProject.CalculationMode が Manual の場合、メソッドはタスク ID、アウトラインレベル、アウトライン番号のみを自動的に計算します。ParentProject.CalculationMode が Automatic の場合、メソッドはプロジェクトのすべてのタスクを自動的に再スケジュールします（開始/終了日、早期/遅延日を設定し、スラック、作業、コストフィールドを計算し、ID とアウトラインレベルを再計算します）。

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(const System::SharedPtr< Task > & beforeTask)
```

| パラメーター | 説明 |
| --- | --- |
| beforeTask | 現在のタスクが挿入される前のタスク。 |

---

## MoveToSibling (2 of 2) {#movetosibling_2}

指定された Id を持つタスクの前に、同じアウトラインレベルで現在のタスクを移動します。ParentProject.CalculationMode が None の場合、ユーザーはこのメソッド使用後に Project.Recalculate() を呼び出す必要があります（これにより、すべてのプロジェクトタスク（開始/終了日、早期/遅延日を設定）のスケジュールが再計算され、スラック、作業、コストフィールド、アウトラインレベルなどの依存フィールドが計算されます）。ParentProject.CalculationMode が Manual の場合、このメソッドはタスク ID、アウトラインレベル、アウトライン番号のみを自動的に計算します。ParentProject.CalculationMode が Automatic の場合、このメソッドはプロジェクトのすべてのタスクを自動的に再スケジュールします（開始/終了日、早期/遅延日を設定し、スラック、作業、コストフィールドを計算し、ID とアウトラインレベルを再計算）。

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(int32_t beforeTaskId)
```

| パラメーター | 説明 |
| --- | --- |
| beforeTaskId | 現在のタスクが挿入されるタスクの前の Id（Tsk::Id）。 |

