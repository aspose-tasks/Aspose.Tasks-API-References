---
title: "Tsk.WBSLevel"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Tsk. Самый правый уровень WBS задачи"
type: docs
weight: 1140
url: /ru/net/aspose.tasks/tsk/wbslevel/
---
## Tsk.WBSLevel field

Самый правый уровень WBS задачи.

```csharp
public static readonly Key<string, TaskKey> WBSLevel;
```

## Примеры

Показывает, как читать коды WBS задачи.

```csharp
var project = new Project(DataDir + "TaskWBS.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Проанализировать все собранные задачи
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.WBS));
    Console.WriteLine(task.Get(Tsk.WBSLevel));
}
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


