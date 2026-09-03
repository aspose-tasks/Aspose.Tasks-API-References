---
title: "Aspose::Tasks::TaskCollection::Add メソッド"
linktitle: "追加"
articleTitle: "追加"
second_title: "Aspose.Tasks for C++"
description: "最後のタスクと同じアウトラインレベルで、プロジェクトのタスクコレクションに新しいタスクを追加します。"
type: docs
weight: 10
url: /ja/cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

最後のタスクと同じアウトラインレベルで、プロジェクトのタスクコレクションに新しいタスクを追加します。

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

指定された ID のタスクの前に、新しいタスクを同じアウトラインレベルで挿入します。

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| パラメーター | 説明 |
| --- | --- |
| パラメーター | 定期タスク作成のために指定されたパラメーターです。 |

---

## Add (3 of 5) {#add_3}

指定されたタスクを TaskCollection クラスのインスタンスに追加します。ParentProject.CalculationMode が None の場合、ユーザーはこのメソッド使用後に Project.Recalculate() を呼び出す必要があります（これにより、すべてのプロジェクトタスク（開始/終了日、早期/遅延日を設定）を再スケジュールし、スラック、作業量、コストフィールド、ID、アウトラインレベルなどの依存フィールドを計算します）。ParentProject.CalculationMode が Manual の場合、このメソッドはタスク ID、アウトラインレベル、アウトライン番号のみを自動的に計算します。ParentProject.CalculationMode が Automatic の場合、このメソッドはプロジェクトのすべてのタスクを自動的に再スケジュールします（開始/終了日、早期/遅延日を設定し、スラック、作業量、コストフィールドを計算し、ID とアウトラインレベルを再計算します）。

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| パラメーター | 説明 |
| --- | --- |
| 項目 | このタスクコレクションに追加すべき指定されたタスクです。 |

---

## Add (4 of 5) {#add_4}

子タスクコレクションに新しいタスクを追加します。

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| パラメーター | 説明 |
| --- | --- |
| taskName | 指定されたタスク名です。 |

---

## Add (5 of 5) {#add_5}

子タスクコレクションに新しい繰り返しタスクを追加します。

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| パラメーター | 説明 |
| --- | --- |
| taskName | 指定されたタスク名です。 |
| beforeTaskId | 新しいタスクが挿入されるタスクの前の指定された ID です。 |

