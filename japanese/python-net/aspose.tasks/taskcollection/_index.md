---
title: "TaskCollection"
second_title: "Aspose.Tasks for Python via .NET API リファレンス"
description: 
type: docs
weight: 1140
url: /ja/python-net/aspose.tasks/taskcollection/
---

## TaskCollection class

[Task](/tasks/python-net/aspose.tasks/task/) オブジェクトのコレクションを表します。

TaskCollection 型は次のメンバーを公開します:
## プロパティ
| 名前 | 説明 |
| :- | :- |
| parent_project | TaskCollection オブジェクトの親プロジェクトを取得します。 |
## メソッド
| 名前 | 説明 |
| :- | :- |
| add() | 指定されたタスクを [TaskCollection](/tasks/python-net/aspose.tasks/taskcollection/) クラスのインスタンスに追加します。<br/>            ParentProject.CalculationMode が None の場合、このメソッド使用後に Project.Recalculate() を呼び出す必要があります（これにより、すべてのプロジェクトタスク（開始/終了日、早期/遅延日を設定）を再スケジュールし、スラック、作業およびコストフィールド、ID、アウトラインレベルなどの依存フィールドを計算します）。<br/>            ParentProject.CalculationMode が Manual の場合、メソッドはタスク ID、アウトラインレベル、アウトライン番号のみを自動的に計算します。<br/>            ParentProject.CalculationMode が Automatic の場合、メソッドはプロジェクトのすべてのタスクを自動的に再スケジュールします<br/>            （開始/終了日、早期/遅延日を設定し、スラック、作業およびコストフィールドを計算し、ID とアウトラインレベルを再計算します）。 |
| add(task_name) | 子タスクコレクションに新しいタスクを追加します。 |
| add(task_name, before_task_id) |  |
| add(parameters) | 指定された ID のタスクの前に、同じアウトラインレベルで新しいタスクを挿入します。 |
| to_list() | TaskCollection オブジェクトを [Task](/tasks/python-net/aspose.tasks/task/) オブジェクトのリストに変換します。 |
| get_by_uid(uid) | このコレクションの親タスクが祖先である、指定された Uid を持つタスクを返します。 |
| get_by_id(id) | このコレクションの親タスクが祖先である、指定された Id を持つタスクを返します。 |

### 関連項目

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

