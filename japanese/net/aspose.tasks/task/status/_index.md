---
title: "Task.Status"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Task プロパティ。タスクのステータスを取得します"
type: docs
weight: 1160
url: /ja/net/aspose.tasks/task/status/
---
## Task.Status property

タスクのステータスを取得します。

```csharp
public TaskStatus Status { get; }
```

## 例

タスクのステータス取得方法を示します。

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// ステータス計算はステータス日付を使用するため、プロジェクトのステータス日付を設定する必要があります。
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### 関連項目

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


